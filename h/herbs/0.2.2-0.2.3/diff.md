# Comparing `tmp/herbs-0.2.2.tar.gz` & `tmp/herbs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herbs-0.2.2.tar", last modified: Fri Dec 23 15:16:16 2022, max compression
+gzip compressed data, was "herbs-0.2.3.tar", last modified: Mon May  1 14:27:09 2023, max compression
```

## Comparing `herbs-0.2.2.tar` & `herbs-0.2.3.tar`

### file list

```diff
@@ -1,211 +1,210 @@
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.238392 herbs-0.2.2/
--rw-r--r--   0 jingyig    (501) staff       (20)      127 2022-04-03 20:04:52.000000 herbs-0.2.2/AUTHOR.txt
--rw-r--r--   0 jingyig    (501) staff       (20)     1094 2022-06-17 19:22:57.000000 herbs-0.2.2/LICENSE.txt
--rw-r--r--   0 jingyig    (501) staff       (20)      901 2022-10-05 10:21:35.000000 herbs-0.2.2/MANIFEST.in
--rw-r--r--   0 jingyig    (501) staff       (20)     5678 2022-12-23 15:16:16.237954 herbs-0.2.2/PKG-INFO
--rw-r--r--   0 jingyig    (501) staff       (20)     4448 2022-10-05 10:31:51.000000 herbs-0.2.2/README.md
--rw-r--r--   0 jingyig    (501) staff       (20)      725 2022-06-23 13:03:39.000000 herbs-0.2.2/THANKS.txt
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.087529 herbs-0.2.2/herbs/
--rwxr-xr-x   0 jingyig    (501) staff       (20)      293 2022-04-05 08:26:08.000000 herbs-0.2.2/herbs/__init__.py
--rw-r--r--   0 jingyig    (501) staff       (20)      976 2022-11-23 10:05:29.000000 herbs-0.2.2/herbs/about_herbs.py
--rw-r--r--   0 jingyig    (501) staff       (20)    26310 2022-12-18 09:11:04.000000 herbs-0.2.2/herbs/allen_downloader.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    11325 2022-10-13 07:11:17.000000 herbs-0.2.2/herbs/atlas_downloader.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    18106 2022-11-30 20:55:50.000000 herbs-0.2.2/herbs/atlas_loader.py
--rw-r--r--   0 jingyig    (501) staff       (20)    28218 2022-12-18 09:01:36.000000 herbs-0.2.2/herbs/atlas_processor.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    58116 2022-12-23 15:11:33.000000 herbs-0.2.2/herbs/atlas_view.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)     7948 2022-10-26 07:43:32.000000 herbs-0.2.2/herbs/czi_reader.py
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.093480 herbs-0.2.2/herbs/data/
--rwxr-xr-x   0 jingyig    (501) staff       (20)    26573 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/data/atlas_labels.pkl
--rw-r--r--   0 jingyig    (501) staff       (20)   227433 2022-06-07 19:22:38.000000 herbs-0.2.2/herbs/data/query.csv
--rw-r--r--   0 jingyig    (501) staff       (20)   305152 2022-12-23 14:37:10.000000 herbs-0.2.2/herbs/herbsgui.py
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.106274 herbs-0.2.2/herbs/icons/
--rw-r--r--   0 jingyig    (501) staff       (20)      760 2022-04-06 16:43:45.000000 herbs-0.2.2/herbs/icons/backward.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      593 2022-04-06 17:38:39.000000 herbs-0.2.2/herbs/icons/dot.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      611 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/down-arrow.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      867 2022-04-06 16:45:38.000000 herbs-0.2.2/herbs/icons/fast_backward.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      861 2022-04-06 16:33:08.000000 herbs-0.2.2/herbs/icons/fast_forward.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      736 2022-04-06 16:43:00.000000 herbs-0.2.2/herbs/icons/forward.svg
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.113008 herbs-0.2.2/herbs/icons/layers/
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2116 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/layers/add.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2322 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/layers/ai.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2916 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/layers/eye_off.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     3295 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/layers/eye_on.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     3056 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/layers/eye_white.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2193 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/layers/hi.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2107 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/layers/trash.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1869 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/object.svg
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.140540 herbs-0.2.2/herbs/icons/sidebar/
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2116 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/add.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2731 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/atlascontrol.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1704 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/atlascontrol.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1146 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/bnd.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)    14175 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/c_section.png
--rw-r--r--   0 jingyig    (501) staff       (20)     9270 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/c_section2.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2258 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/cell.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)      517 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/check.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1539 2022-06-15 12:52:01.000000 herbs-0.2.2/herbs/icons/sidebar/compare.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      869 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/contour.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)    14191 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/h_section.png
--rw-r--r--   0 jingyig    (501) staff       (20)      691 2022-10-20 11:27:54.000000 herbs-0.2.2/herbs/icons/sidebar/info.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     3336 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/layers.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1728 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/layers.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)      611 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/line.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1323 2022-06-14 18:04:46.000000 herbs-0.2.2/herbs/icons/sidebar/link.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1366 2022-06-14 19:23:53.000000 herbs-0.2.2/herbs/icons/sidebar/link_off.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)      763 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/merge.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)      994 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/object.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2584 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/probe.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1300 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/probe.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      856 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/rotation_horizontal.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      858 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/rotation_vertical.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)    14248 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/s_section.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     3741 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/tool.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1350 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/tool.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2107 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/trash.png
--rw-r--r--   0 jingyig    (501) staff       (20)      614 2022-04-08 19:22:48.000000 herbs-0.2.2/herbs/icons/sidebar/tree_checked.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     3299 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/treeview.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)      697 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/treeview.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     3211 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/treeview2.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1783 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/sidebar/virus.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      653 2022-04-06 08:50:37.000000 herbs-0.2.2/herbs/icons/tdown.svg
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.215606 herbs-0.2.2/herbs/icons/toolbar/
--rw-r--r--   0 jingyig    (501) staff       (20)      669 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/accept.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1974 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/accept2.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     3485 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/aim.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     2108 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/aim_not.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1142 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/anchor.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      777 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/anticlockwise_rotation.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2604 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/atlas_icon.png
--rw-r--r--   0 jingyig    (501) staff       (20)     1371 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/boundary_register.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     2885 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/cancel.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1431 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/cell_select.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      868 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/cell_select_not.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)      517 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/check.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      773 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/clockwise_rotation.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1205 2022-05-15 09:01:01.000000 herbs-0.2.2/herbs/icons/toolbar/closed_path.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1060 2022-05-16 11:52:50.000000 herbs-0.2.2/herbs/icons/toolbar/closed_path2 copy.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1825 2022-05-15 08:57:18.000000 herbs-0.2.2/herbs/icons/toolbar/closed_path2.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2180 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/eraser.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1275 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/eraser.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      984 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/eye.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1343 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/eye_closed.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      865 2022-05-15 07:36:52.000000 herbs-0.2.2/herbs/icons/toolbar/fill.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1215 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/gps.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2172 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/h_flip.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1894 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/handle.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2575 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/image_icon.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2277 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/image_icon.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      788 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/info.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1876 2022-05-15 08:52:11.000000 herbs-0.2.2/herbs/icons/toolbar/inpart.png
--rw-r--r--   0 jingyig    (501) staff       (20)      890 2022-05-16 12:22:33.000000 herbs-0.2.2/herbs/icons/toolbar/inpart.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     5945 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/lasso.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1017 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/lasso.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2913 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/left90.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)      611 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/line.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      613 2022-12-07 09:16:00.000000 herbs-0.2.2/herbs/icons/toolbar/line_sites.svg
--rw-r--r--   0 jingyig    (501) staff       (20)    11865 2022-11-24 11:31:26.000000 herbs-0.2.2/herbs/icons/toolbar/linear_silicon.png
--rw-r--r--   0 jingyig    (501) staff       (20)     5202 2022-11-24 11:30:17.000000 herbs-0.2.2/herbs/icons/toolbar/linear_silicon.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      848 2022-11-11 09:57:28.000000 herbs-0.2.2/herbs/icons/toolbar/list.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)      833 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/location.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1067 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/magic-wand.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2567 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/magic_white.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)      648 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/mask.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1375 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/match.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1151 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/matchbnd.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     2402 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/matching.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)      763 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/merge.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2148 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/move_down.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1963 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/move_left.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2158 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/move_right.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2146 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/move_up.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     5229 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/moving.png
--rw-r--r--   0 jingyig    (501) staff       (20)     7705 2022-11-25 09:08:41.000000 herbs-0.2.2/herbs/icons/toolbar/multi-probe.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1101 2022-11-30 08:26:50.000000 herbs-0.2.2/herbs/icons/toolbar/multi_pencil.svg
--rw-r--r--   0 jingyig    (501) staff       (20)    34495 2022-11-25 11:57:55.000000 herbs-0.2.2/herbs/icons/toolbar/multi_probe.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)      994 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/object.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1893 2022-05-15 07:35:55.000000 herbs-0.2.2/herbs/icons/toolbar/open_path.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1894 2022-05-15 08:49:55.000000 herbs-0.2.2/herbs/icons/toolbar/outpart.png
--rw-r--r--   0 jingyig    (501) staff       (20)     1408 2022-05-16 12:24:00.000000 herbs-0.2.2/herbs/icons/toolbar/outpart.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2319 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/pencil.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1250 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/pencil.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2485 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/plasso.png
--rw-r--r--   0 jingyig    (501) staff       (20)     1601 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/probe.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1721 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/radar.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     4384 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/rotation.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1132 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/rotation_clockwise.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1127 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/rotation_counter_clockwise.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     1816 2022-05-13 08:36:03.000000 herbs-0.2.2/herbs/icons/toolbar/ruler.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      729 2022-12-07 09:15:17.000000 herbs-0.2.2/herbs/icons/toolbar/separate_sites.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      817 2022-11-30 08:25:23.000000 herbs-0.2.2/herbs/icons/toolbar/single_pencil.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      730 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/toa.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     3165 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/toa_delete.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      819 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/toaa.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      740 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/toh.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     3189 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/toh_delete.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      733 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/tohh.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2127 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/trans.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1028 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/trans.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      599 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/triangulation.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2339 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/two_window.png
--rw-r--r--   0 jingyig    (501) staff       (20)     1211 2022-11-21 18:56:10.000000 herbs-0.2.2/herbs/icons/toolbar/unmerge.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2144 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/v_flip.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)     1783 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/virus.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     2367 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/virus_register.svg
--rw-r--r--   0 jingyig    (501) staff       (20)     2332 2022-10-20 11:41:47.000000 herbs-0.2.2/herbs/icons/toolbar/vis2d.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2305 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/window2.png
--rw-r--r--   0 jingyig    (501) staff       (20)    15734 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/window3.png
--rwxr-xr-x   0 jingyig    (501) staff       (20)    16491 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/toolbar/window4.png
--rw-r--r--   0 jingyig    (501) staff       (20)      611 2022-04-06 19:19:18.000000 herbs-0.2.2/herbs/icons/tree_close.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      611 2022-04-06 19:18:02.000000 herbs-0.2.2/herbs/icons/tree_open.svg
--rw-r--r--   0 jingyig    (501) staff       (20)      624 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/icons/up-arrow.svg
--rwxr-xr-x   0 jingyig    (501) staff       (20)    24078 2022-10-26 08:07:28.000000 herbs-0.2.2/herbs/image_curves.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)     8774 2022-10-26 08:22:58.000000 herbs-0.2.2/herbs/image_reader.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    13631 2022-12-21 11:25:29.000000 herbs-0.2.2/herbs/image_stacks.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    27381 2022-11-04 19:05:50.000000 herbs-0.2.2/herbs/image_view.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)        5 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/images_reader.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)     7998 2022-10-14 08:40:46.000000 herbs-0.2.2/herbs/label_tree.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    18954 2022-11-11 18:45:37.000000 herbs-0.2.2/herbs/layers_control.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    26116 2022-12-19 20:36:26.000000 herbs-0.2.2/herbs/main_window.ui
--rw-r--r--   0 jingyig    (501) staff       (20)     7275 2022-05-04 07:10:23.000000 herbs-0.2.2/herbs/movable_points.py
--rw-r--r--   0 jingyig    (501) staff       (20)     3433 2022-11-22 20:22:41.000000 herbs-0.2.2/herbs/obj_items.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    50133 2022-12-15 07:41:25.000000 herbs-0.2.2/herbs/object_control.py
--rw-r--r--   0 jingyig    (501) staff       (20)      393 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/popup_message.py
--rw-r--r--   0 jingyig    (501) staff       (20)    37839 2022-12-21 07:48:11.000000 herbs-0.2.2/herbs/probe_utiles.py
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.236688 herbs-0.2.2/herbs/qss/
--rw-r--r--   0 jingyig    (501) staff       (20)      312 2022-10-28 09:49:15.000000 herbs-0.2.2/herbs/qss/atlas_view_group_box.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      101 2022-10-19 17:23:07.000000 herbs-0.2.2/herbs/qss/box_label.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      446 2022-10-26 08:29:40.000000 herbs-0.2.2/herbs/qss/channel_selector.qss
--rw-r--r--   0 jingyig    (501) staff       (20)     2649 2022-10-26 08:15:37.000000 herbs-0.2.2/herbs/qss/color_combo.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      166 2022-10-11 08:55:16.000000 herbs-0.2.2/herbs/qss/decor_label.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      151 2022-10-04 18:36:02.000000 herbs-0.2.2/herbs/qss/dialogs.qss
--rw-r--r--   0 jingyig    (501) staff       (20)       83 2022-10-28 09:56:10.000000 herbs-0.2.2/herbs/qss/hidden_line_edit.qss
--rw-r--r--   0 jingyig    (501) staff       (20)     2586 2022-10-14 08:39:43.000000 herbs-0.2.2/herbs/qss/label_tree.qss
--rw-r--r--   0 jingyig    (501) staff       (20)     5688 2022-10-04 18:37:15.000000 herbs-0.2.2/herbs/qss/main_window.qss
--rw-r--r--   0 jingyig    (501) staff       (20)     1045 2022-10-11 08:40:10.000000 herbs-0.2.2/herbs/qss/menu_bar.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      612 2022-10-26 08:04:00.000000 herbs-0.2.2/herbs/qss/multi_handle_slider.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      543 2022-11-23 14:00:24.000000 herbs-0.2.2/herbs/qss/obj_ctrl_bottom_button.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      359 2022-10-28 11:23:55.000000 herbs-0.2.2/herbs/qss/object_text_button.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      950 2022-10-12 08:54:29.000000 herbs-0.2.2/herbs/qss/page_control.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      177 2022-10-28 09:53:36.000000 herbs-0.2.2/herbs/qss/rotation_button.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      574 2022-10-28 09:51:11.000000 herbs-0.2.2/herbs/qss/side_bar.qss
--rw-r--r--   0 jingyig    (501) staff       (20)     2631 2022-10-26 08:06:32.000000 herbs-0.2.2/herbs/qss/spinbox.qss
--rw-r--r--   0 jingyig    (501) staff       (20)     4366 2022-10-11 08:53:58.000000 herbs-0.2.2/herbs/qss/tabs.qss
--rw-r--r--   0 jingyig    (501) staff       (20)     1572 2022-10-11 08:38:30.000000 herbs-0.2.2/herbs/qss/tool_bar.qss
--rw-r--r--   0 jingyig    (501) staff       (20)      247 2022-04-03 08:51:58.000000 herbs-0.2.2/herbs/run_herbs.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)     8576 2022-12-21 11:25:29.000000 herbs-0.2.2/herbs/slice_stacks.py
--rw-r--r--   0 jingyig    (501) staff       (20)    30979 2022-11-18 19:33:42.000000 herbs-0.2.2/herbs/temp.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    24452 2022-12-15 10:44:21.000000 herbs-0.2.2/herbs/toolbox.py
--rw-r--r--   0 jingyig    (501) staff       (20)     3362 2022-04-03 06:33:27.000000 herbs-0.2.2/herbs/triangulation_points.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    34823 2022-12-19 20:28:33.000000 herbs-0.2.2/herbs/uuuuuu.py
--rw-r--r--   0 jingyig    (501) staff       (20)       22 2022-06-17 18:03:13.000000 herbs-0.2.2/herbs/version.py
--rw-r--r--   0 jingyig    (501) staff       (20)     5055 2022-10-26 08:30:43.000000 herbs-0.2.2/herbs/widgets_utils.py
--rwxr-xr-x   0 jingyig    (501) staff       (20)    26611 2022-12-17 20:20:14.000000 herbs-0.2.2/herbs/wtiles.py
-drwxr-xr-x   0 jingyig    (501) staff       (20)        0 2022-12-23 15:16:16.091481 herbs-0.2.2/herbs.egg-info/
--rw-r--r--   0 jingyig    (501) staff       (20)     5678 2022-12-23 15:16:15.000000 herbs-0.2.2/herbs.egg-info/PKG-INFO
--rw-r--r--   0 jingyig    (501) staff       (20)     5824 2022-12-23 15:16:16.000000 herbs-0.2.2/herbs.egg-info/SOURCES.txt
--rw-r--r--   0 jingyig    (501) staff       (20)        1 2022-12-23 15:16:15.000000 herbs-0.2.2/herbs.egg-info/dependency_links.txt
--rw-r--r--   0 jingyig    (501) staff       (20)      411 2022-12-23 15:16:15.000000 herbs-0.2.2/herbs.egg-info/requires.txt
--rw-r--r--   0 jingyig    (501) staff       (20)        6 2022-12-23 15:16:15.000000 herbs-0.2.2/herbs.egg-info/top_level.txt
--rw-r--r--   0 jingyig    (501) staff       (20)       86 2022-06-17 19:36:22.000000 herbs-0.2.2/pyproject.toml
--rw-r--r--   0 jingyig    (501) staff       (20)       38 2022-12-23 15:16:16.238498 herbs-0.2.2/setup.cfg
--rwxr-xr-x   0 jingyig    (501) staff       (20)     2854 2022-12-23 15:13:11.000000 herbs-0.2.2/setup.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.991439 herbs-0.2.3/
+-rw-r--r--   0 jingyi     (501) staff       (20)      127 2023-04-25 18:58:14.000000 herbs-0.2.3/AUTHOR.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)     1094 2023-04-25 18:58:15.000000 herbs-0.2.3/LICENSE.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)      901 2023-04-25 18:58:15.000000 herbs-0.2.3/MANIFEST.in
+-rw-r--r--   0 jingyi     (501) staff       (20)     5678 2023-05-01 14:27:09.991178 herbs-0.2.3/PKG-INFO
+-rw-r--r--   0 jingyi     (501) staff       (20)     4448 2023-04-25 18:58:15.000000 herbs-0.2.3/README.md
+-rw-r--r--   0 jingyi     (501) staff       (20)      725 2023-04-25 18:58:15.000000 herbs-0.2.3/THANKS.txt
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.928630 herbs-0.2.3/herbs/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      293 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/__init__.py
+-rw-r--r--   0 jingyi     (501) staff       (20)      976 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/about_herbs.py
+-rw-r--r--   0 jingyi     (501) staff       (20)    26310 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/allen_downloader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    11325 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_downloader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    18106 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_loader.py
+-rw-r--r--   0 jingyi     (501) staff       (20)    28218 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_processor.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    58116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_view.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     7948 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/czi_reader.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.932318 herbs-0.2.3/herbs/data/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    26573 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/data/atlas_labels.pkl
+-rw-r--r--   0 jingyi     (501) staff       (20)   227433 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/data/query.csv
+-rw-r--r--   0 jingyi     (501) staff       (20)   329944 2023-05-01 14:11:36.000000 herbs-0.2.3/herbs/herbsgui.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.937874 herbs-0.2.3/herbs/icons/
+-rw-r--r--   0 jingyi     (501) staff       (20)      760 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/backward.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      593 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/dot.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/down-arrow.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      867 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/fast_backward.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      861 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/fast_forward.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      736 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/forward.svg
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.940994 herbs-0.2.3/herbs/icons/layers/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/add.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2322 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/ai.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2916 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/eye_off.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3295 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/eye_on.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3056 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/eye_white.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2193 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/hi.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2107 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/trash.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1869 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/object.svg
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.952134 herbs-0.2.3/herbs/icons/sidebar/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/add.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2731 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/atlascontrol.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1704 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/atlascontrol.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1146 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/bnd.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    14175 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/c_section.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     9270 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/c_section2.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2258 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/cell.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      517 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/check.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1539 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/compare.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      869 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/contour.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    14191 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/h_section.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      691 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/info.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3336 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/layers.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1728 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/layers.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/line.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1323 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/link.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1366 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/link_off.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      763 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/merge.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      994 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/object.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2584 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/probe.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1300 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/probe.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      856 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/rotation_horizontal.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      858 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/rotation_vertical.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    14248 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/s_section.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3741 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/tool.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1350 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/tool.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2107 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/trash.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      614 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/tree_checked.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3299 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/treeview.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      697 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/treeview.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3211 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/treeview2.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1783 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/virus.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      653 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/tdown.svg
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.984633 herbs-0.2.3/herbs/icons/toolbar/
+-rw-r--r--   0 jingyi     (501) staff       (20)      669 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/accept.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1974 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/accept2.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     3485 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/aim.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2108 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/aim_not.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1142 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/anchor.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      777 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/anticlockwise_rotation.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2604 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/atlas_icon.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1371 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/boundary_register.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2885 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/cancel.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1431 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/cell_select.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      868 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/cell_select_not.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      517 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/check.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      773 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/clockwise_rotation.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1205 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/closed_path.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1060 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/closed_path2 copy.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1825 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/closed_path2.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2180 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eraser.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1275 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eraser.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      984 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eye.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1343 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eye_closed.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      865 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/fill.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1215 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/gps.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2172 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/h_flip.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1894 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/handle.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2575 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/image_icon.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2277 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/image_icon.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      788 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/info.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1876 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/inpart.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      890 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/inpart.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     5945 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/lasso.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1017 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/lasso.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2913 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/left90.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/line.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      613 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/line_sites.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)    11865 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/linear_silicon.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     5202 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/linear_silicon.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      848 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/list.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      833 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/location.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1067 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/magic-wand.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2567 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/magic_white.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      648 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/mask.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1375 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/match.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1151 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/matchbnd.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2402 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/matching.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      763 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/merge.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2148 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_down.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1963 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_left.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2158 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_right.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2146 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_up.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     5229 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/moving.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     7705 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/multi-probe.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1101 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/multi_pencil.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)    34495 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/multi_probe.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      994 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/object.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1893 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/open_path.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1894 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/outpart.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1408 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/outpart.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2319 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/pencil.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1250 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/pencil.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2485 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/plasso.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1601 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/probe.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1721 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/radar.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     4384 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/rotation.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1132 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/rotation_clockwise.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1127 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/rotation_counter_clockwise.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1816 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/ruler.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      729 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/separate_sites.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      817 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/single_pencil.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      730 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toa.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     3165 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toa_delete.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      819 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toaa.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      740 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toh.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     3189 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toh_delete.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      733 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/tohh.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2127 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/trans.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1028 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/trans.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      599 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/triangulation.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2339 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/two_window.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1211 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/unmerge.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2144 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/v_flip.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1783 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/virus.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2367 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/virus_register.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2332 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/vis2d.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2305 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/window2.png
+-rw-r--r--   0 jingyi     (501) staff       (20)    15734 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/window3.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    16491 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/window4.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/tree_close.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/tree_open.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      624 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/up-arrow.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    24078 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_curves.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     8774 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_reader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    13631 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_stacks.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    27381 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_view.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)        5 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/images_reader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     7998 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/label_tree.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    18954 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/layers_control.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    26116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/main_window.ui
+-rw-r--r--   0 jingyi     (501) staff       (20)     7275 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/movable_points.py
+-rw-r--r--   0 jingyi     (501) staff       (20)     3433 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/obj_items.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    52329 2023-05-01 14:09:27.000000 herbs-0.2.3/herbs/object_control.py
+-rw-r--r--   0 jingyi     (501) staff       (20)      393 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/popup_message.py
+-rw-r--r--   0 jingyi     (501) staff       (20)    38740 2023-05-01 05:23:17.000000 herbs-0.2.3/herbs/probe_utiles.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.990847 herbs-0.2.3/herbs/qss/
+-rw-r--r--   0 jingyi     (501) staff       (20)      312 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/atlas_view_group_box.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      101 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/box_label.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      446 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/channel_selector.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     2649 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/color_combo.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      166 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/decor_label.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      151 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/dialogs.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)       83 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/hidden_line_edit.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     2586 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/label_tree.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     5688 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/main_window.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     1045 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/menu_bar.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      612 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/multi_handle_slider.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      543 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/obj_ctrl_bottom_button.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      359 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/object_text_button.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      950 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/page_control.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      177 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/rotation_button.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      574 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/side_bar.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     2631 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/spinbox.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     4366 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/tabs.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     1572 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/tool_bar.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      247 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/run_herbs.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     8576 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/slice_stacks.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    24452 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/toolbox.py
+-rw-r--r--   0 jingyi     (501) staff       (20)     3362 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/triangulation_points.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    36300 2023-05-01 05:19:09.000000 herbs-0.2.3/herbs/uuuuuu.py
+-rw-r--r--   0 jingyi     (501) staff       (20)       22 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/version.py
+-rw-r--r--   0 jingyi     (501) staff       (20)     5055 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/widgets_utils.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    26611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/wtiles.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.930673 herbs-0.2.3/herbs.egg-info/
+-rw-r--r--   0 jingyi     (501) staff       (20)     5678 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/PKG-INFO
+-rw-r--r--   0 jingyi     (501) staff       (20)     5810 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)        1 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)      411 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/requires.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)        6 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/top_level.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)       86 2023-04-25 18:58:15.000000 herbs-0.2.3/pyproject.toml
+-rw-r--r--   0 jingyi     (501) staff       (20)       38 2023-05-01 14:27:09.991508 herbs-0.2.3/setup.cfg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2857 2023-05-01 14:25:34.000000 herbs-0.2.3/setup.py
```

### Comparing `herbs-0.2.2/LICENSE.txt` & `herbs-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/MANIFEST.in` & `herbs-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/PKG-INFO` & `herbs-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herbs
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python-based GUI for Histological E-data Registration in Brain Space
 Home-page: https://github.com/JingyiGF/HERBS
 Author: Jingyi GF
 Author-email: jingyi.g.fuglstad@gmail.com
 Project-URL: Bug Tracker, https://github.com/JingyiGF/HERBS/issues
 Keywords: brain atlas,histological image registration,probe coordinates
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `herbs-0.2.2/README.md` & `herbs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/THANKS.txt` & `herbs-0.2.3/THANKS.txt`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/about_herbs.py` & `herbs-0.2.3/herbs/about_herbs.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/allen_downloader.py` & `herbs-0.2.3/herbs/allen_downloader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/atlas_downloader.py` & `herbs-0.2.3/herbs/atlas_downloader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/atlas_loader.py` & `herbs-0.2.3/herbs/atlas_loader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/atlas_processor.py` & `herbs-0.2.3/herbs/atlas_processor.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/atlas_view.py` & `herbs-0.2.3/herbs/atlas_view.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/czi_reader.py` & `herbs-0.2.3/herbs/czi_reader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/data/atlas_labels.pkl` & `herbs-0.2.3/herbs/data/atlas_labels.pkl`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/data/query.csv` & `herbs-0.2.3/herbs/data/query.csv`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/herbsgui.py` & `herbs-0.2.3/herbs/herbsgui.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,78 +13,122 @@
 import scipy
 import scipy.io
 import scipy.ndimage as ndi
 from scipy.ndimage import map_coordinates
 from natsort import natsorted, ns
 
 import cv2
-opencv_ver = (cv2.__version__).split('.')
+
+opencv_ver = (cv2.__version__).split(".")
 from numba import jit
 import colorsys
 
 
 import PyQt5
 from PyQt5.QtWidgets import *
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtSql import QSqlTableModel
 from PyQt5.QtMultimedia import QSound
+
 # from PyQt5 import uic
 from PyQt5.uic import loadUiType
 import pyqtgraph as pg
-pg.setConfigOption('imageAxisOrder', 'row-major')
-pg.setConfigOption('useNumba', True)
+
+pg.setConfigOption("imageAxisOrder", "row-major")
+pg.setConfigOption("useNumba", True)
 import pyqtgraph.opengl as gl
 from pyqtgraph.Qt import QtCore, QtGui
 from pyqtgraph import metaarray
 
 import warnings
 
 
-from .uuuuuu import get_cell_count, num_side_pnt_changed, rotate, merge_channels_into_single_img, gamma_correction, \
-    create_vis_img, color_vis_img, get_tri_lines, match_sides_points, get_vertex_ind_in_triangle, \
-    warp_triangle, warp_points, get_pnts_triangle_ind, make_label_rgb_img, get_corner_line_from_rect,  \
-    delete_points_inside_eraser, get_bound_color,  \
-    calculate_cells_info, calculate_virus_info, calculate_drawing_info, calculate_contour_line, \
-    check_loading_pickle_file, check_bounding_contains, get_statusbar_style, load_point_data
-from .probe_utiles import line_fit_2d, Probe, MultiProbes, calculate_probe_info, \
-    get_pre_multi_shank_vis_base, get_center_lines
+from .uuuuuu import (
+    get_cell_count,
+    num_side_pnt_changed,
+    rotate,
+    merge_channels_into_single_img,
+    gamma_correction,
+    create_vis_img,
+    color_vis_img,
+    get_tri_lines,
+    match_sides_points,
+    get_vertex_ind_in_triangle,
+    warp_triangle,
+    warp_points,
+    get_pnts_triangle_ind,
+    make_label_rgb_img,
+    get_corner_line_from_rect,
+    delete_points_inside_eraser,
+    get_bound_color,
+    calculate_cells_info,
+    calculate_virus_info,
+    calculate_drawing_info,
+    calculate_contour_line,
+    check_loading_pickle_file,
+    check_bounding_contains,
+    get_statusbar_style,
+    load_point_data,
+)
+from .probe_utiles import (
+    line_fit_2d,
+    Probe,
+    MultiProbes,
+    calculate_probe_info,
+    get_pre_multi_shank_vis_base,
+    get_center_lines,
+)
 from .czi_reader import CZIReader
 from .atlas_downloader import AtlasDownloader
 from .allen_downloader import AllenDownloader
 from .atlas_processor import AtlasProcessor
 from .atlas_loader import AtlasLoader
 from .atlas_view import AtlasView
 
 from .image_reader import ImageReader, ImagesReader, TIFFReader
 from .image_curves import *
 from .image_view import ImageView
 
 from .layers_control import *
 from .object_control import *
 from .toolbox import ToolBox
-from .wtiles import LayerSettingDialog, SliceSettingDialog, LinearSiliconInfoDialog, MultiProbePlanningDialog
-from .obj_items import get_object_vis_color, create_plot_points_in_3d, create_probe_line_in_3d, \
-    create_drawing_in_3d, create_contour_line_in_3d, render_volume, render_small_volume, make_3d_gl_widget
+from .wtiles import (
+    LayerSettingDialog,
+    SliceSettingDialog,
+    LinearSiliconInfoDialog,
+    MultiProbePlanningDialog,
+)
+from .obj_items import (
+    get_object_vis_color,
+    create_plot_points_in_3d,
+    create_probe_line_in_3d,
+    create_drawing_in_3d,
+    create_contour_line_in_3d,
+    render_volume,
+    render_small_volume,
+    make_3d_gl_widget,
+)
 from .about_herbs import AboutHERBSWindow
 
 
 script_dir = dirname(realpath(__file__))
 FORM_Main, _ = loadUiType((join(dirname(__file__), "main_window.ui")))
 
 
 class HERBS(QMainWindow, FORM_Main):
-
     def __init__(self, parent=FORM_Main):
         super(HERBS, self).__init__()
         QMainWindow.__init__(self)
         self.setupUi(self)
-        self.setWindowTitle("HERBS - A toolkit for Histological E-data Registration in Brain Space")
+        self.setWindowTitle(
+            "HERBS - A toolkit for Histological E-data Registration in Brain Space"
+        )
 
-        self.home_path = str(os.path.expanduser('~'))
+        self.home_path = str(os.path.expanduser("~"))
         self.save_path = self.home_path
 
         self.num_windows = 1
         self.volume_atlas_path = None
         self.slice_atlas_path = None
         self.current_atlas_path = None
 
@@ -125,131 +169,142 @@
         self.histo_side_lines = None
         self.histo_tri_data = []
         self.histo_tri_inside_data = []
         self.histo_tri_onside_data = []
 
         self.drawing_allowed = False
 
+        self.working_img_data = {
+            "img-overlay": None,
+            "img-mask": None,
+            "img-probe": [],
+            "img-cells": [],
+            "img-contour": [],
+            "img-virus": None,
+            "img-drawing": [],
+            "img-blob": [],
+            "cell_count": [0 for i in range(5)],
+            "cell_size": [],
+            "cell_symbol": [],
+            "cell_layer_index": [],
+            "lasso_path": [],
+            "ruler_path": [],
+        }
+        self.working_img_type = {
+            "img-overlay": "pixel",
+            "img-mask": "pixel",
+            "img-probe": "vector",
+            "img-cells": "vector",
+            "img-contour": "vector",
+            "img-virus": "pixel",
+            "img-drawing": "vector",
+            "img-blob": "vector",
+            "cell_size": "vector",
+            "cell_symbol": "vector",
+            "cell_layer_index": "vector",
+            "lasso_path": "vector",
+            "ruler_path": "vector",
+        }
+
+        self.working_atlas_data = {
+            "atlas-overlay": None,
+            "atlas-mask": None,
+            "atlas-probe": [],
+            "atlas-cells": [],
+            "atlas-contour": [],
+            "atlas-virus": [],
+            "atlas-drawing": [],
+            "cell_count": [0 for i in range(5)],
+            "cell_size": [],
+            "cell_symbol": [],
+            "cell_layer_index": [],
+            "lasso_path": [],
+            "ruler_path": [],
+        }
+        self.working_atlas_type = {
+            "atlas-overlay": "pixel",
+            "atlas-mask": "pixel",
+            "atlas-probe": "vector",
+            "atlas-cells": "vector",
+            "atlas-contour": "vector",
+            "atlas-virus": "vector",
+            "atlas-drawing": "vector",
+            "cell_size": "vector",
+            "cell_symbol": "vector",
+            "cell_layer_index": "vector",
+            "lasso_path": "vector",
+            "ruler_path": "vector",
+        }
 
-        self.working_img_data = {'img-overlay': None,
-                                 'img-mask': None,
-                                 'img-probe': [],
-                                 'img-cells': [],
-                                 'img-contour': [],
-                                 'img-virus': None,
-                                 'img-drawing': [],
-                                 'img-blob': [],
-                                 'cell_count': [0 for i in range(5)],
-                                 'cell_size': [],
-                                 'cell_symbol': [],
-                                 'cell_layer_index': [],
-                                 'lasso_path': [],
-                                 'ruler_path': []}
-        self.working_img_type = {'img-overlay': 'pixel',
-                                 'img-mask': 'pixel',
-                                 'img-probe': 'vector',
-                                 'img-cells': 'vector',
-                                 'img-contour': 'vector',
-                                 'img-virus': 'pixel',
-                                 'img-drawing': 'vector',
-                                 'img-blob': 'vector',
-                                 'cell_size': 'vector',
-                                 'cell_symbol': 'vector',
-                                 'cell_layer_index': 'vector',
-                                 'lasso_path': 'vector',
-                                 'ruler_path': 'vector'}
-
-        self.working_atlas_data = {'atlas-overlay': None,
-                                   'atlas-mask': None,
-                                   'atlas-probe': [],
-                                   'atlas-cells': [],
-                                   'atlas-contour': [],
-                                   'atlas-virus': [],
-                                   'atlas-drawing': [],
-                                   'cell_count': [0 for i in range(5)],
-                                   'cell_size': [],
-                                   'cell_symbol': [],
-                                   'cell_layer_index': [],
-                                   'lasso_path': [],
-                                   'ruler_path': []}
-        self.working_atlas_type = {'atlas-overlay': 'pixel',
-                                   'atlas-mask': 'pixel',
-                                   'atlas-probe': 'vector',
-                                   'atlas-cells': 'vector',
-                                   'atlas-contour': 'vector',
-                                   'atlas-virus': 'vector',
-                                   'atlas-drawing': 'vector',
-                                   'cell_size': 'vector',
-                                   'cell_symbol': 'vector',
-                                   'cell_layer_index': 'vector',
-                                   'lasso_path': 'vector',
-                                   'ruler_path': 'vector'}
-
-        self.cell_base_symbol = ['+', '+', 'x', 't', 's']
+        self.cell_base_symbol = ["+", "+", "x", "t", "s"]
 
         self.working_atlas_text = []
         self.working_img_text = []
 
         self.a2h_transferred = False
         self.h2a_transferred = False
-        self.project_method = 'pre plan'
+        self.project_method = "pre plan"
         self.register_method = 0
 
         self.action_list = []
         self.layer_action_after_matching = []
 
         self.probe_lines_2d_list = []
 
         self.object_3d_list = []
 
         self.previous_checked_label = []
-        self.atlas_display = 'coronal'
+        self.atlas_display = "coronal"
         self.show_child_mesh = False
         self.warning_status = False
 
         self.current_checked_tool = None
 
         self.drawing_img = None
         self.cell_img = None
         self.probe_img = None
 
         self.overlay_img = None
 
-        self.error_message_color = '#ff6e6e'
-        self.reminder_color = 'gray'
-        self.normal_color = 'white'
+        self.error_message_color = "#ff6e6e"
+        self.reminder_color = "gray"
+        self.normal_color = "white"
 
         self.layer_shift_val = 1
         self.layer_rotate_val = 1
         self.action_id = 0
         self.undo_count = 0
         self.redo_count = -1
 
-        self.current_atlas = 'volume'
+        self.current_atlas = "volume"
 
-        self.display_mode_3d = 'dark'
+        self.display_mode_3d = "dark"
         self.is_planes_on = True
         self.is_axis_on = True
-        self.display_mode_2d = 'dark'
+        self.display_mode_2d = "dark"
         self.is_grids_on = False
-        self.obj_display_mode = 'opaque'
+        self.obj_display_mode = "opaque"
 
         self.kernel = None
 
         # ---------------------
         self.tool_box = ToolBox()
         self.toolbar_wrap_action_dict = {}
         self.pencil_color = (255, 102, 0)
         self.probe_color = (0, 0, 255)
         self.cell_color = (0, 255, 0)
         self.lasso_color = (0, 255, 255)
         self.magic_wand_lut = np.array([[0, 0, 0, 0], [255, 0, 255, 255]])
-        self.magic_wand_lut[1] = np.ravel(self.tool_box.magic_color_btn.color().getRgb()).astype(int)
+        self.magic_wand_lut[1] = np.ravel(
+            self.tool_box.magic_color_btn.color().getRgb()
+        ).astype(int)
         self.contour_color = self.magic_wand_lut[1].copy()
-        self.triangle_color = np.ravel(self.tool_box.triang_color_btn.color().getRgb()).astype(int)
+        self.triangle_color = np.ravel(
+            self.tool_box.triang_color_btn.color().getRgb()
+        ).astype(int)
         self.virus_lut = self.magic_wand_lut.copy()
 
         # ---------------------------- load controls, views, panels
         self.layer_ctrl = LayersControl()
         self.layer_ctrl.sig_opacity_changed.connect(self.layers_opacity_changed)
         self.layer_ctrl.sig_visible_changed.connect(self.layers_visible_changed)
         self.layer_ctrl.sig_layer_deleted.connect(self.layers_exist_changed)
@@ -268,127 +323,202 @@
         self.object_ctrl.merge_virus_btn.clicked.connect(self.merge_virus)
         self.object_ctrl.merge_cell_btn.clicked.connect(self.merge_cells)
         self.object_ctrl.merge_contour_btn.clicked.connect(self.merge_contour)
         self.object_ctrl.merge_drawing_btn.clicked.connect(self.merge_drawings)
         self.object_ctrl.compare_btn.clicked.connect(self.compare_object)
         self.object_ctrl.vis2d_btn.clicked.connect(self.display_object_in_2d_atlas)
 
-
         self.image_view = ImageView()
         self.image_view.sig_image_changed.connect(self.update_histo_tri_onside_data)
         self.image_view.img_stacks.sig_mouse_clicked.connect(self.img_stacks_clicked)
         self.image_view.img_stacks.sig_mouse_hovered.connect(self.img_stacks_hovered)
         self.image_view.img_stacks.sig_key_pressed.connect(self.img_stacks_key_pressed)
-        self.image_view.img_stacks.image_dict['tri_pnts'].mouseDragged.connect(self.hist_window_tri_pnts_moving)
-        self.image_view.img_stacks.image_dict['tri_pnts'].mouseClicked.connect(self.hist_window_tri_pnts_clicked)
-        self.image_view.img_stacks.image_dict['lasso_path'].sigPointsClicked.connect(self.lasso_points_clicked)
-        self.image_view.img_stacks.image_dict['ruler_path'].sigPointsClicked.connect(self.img_ruler_points_clicked)
+        self.image_view.img_stacks.image_dict["tri_pnts"].mouseDragged.connect(
+            self.hist_window_tri_pnts_moving
+        )
+        self.image_view.img_stacks.image_dict["tri_pnts"].mouseClicked.connect(
+            self.hist_window_tri_pnts_clicked
+        )
+        self.image_view.img_stacks.image_dict["lasso_path"].sigPointsClicked.connect(
+            self.lasso_points_clicked
+        )
+        self.image_view.img_stacks.image_dict["ruler_path"].sigPointsClicked.connect(
+            self.img_ruler_points_clicked
+        )
         # self.image_view.img_stacks.image_dict['img-cells'].sigClicked.connect(self.img_cell_pnts_clicked)
         # self.image_view.img_stacks.image_dict['img-probe'].sigClicked.connect(self.img_probe_pnts_clicked)
         # self.image_view.img_stacks.image_dict['img-drawing'].sigClicked.connect(self.img_drawing_pnts_clicked)
 
         self.atlas_view = AtlasView()
         self.atlas_view.show_boundary_btn.clicked.connect(self.vis_atlas_boundary)
         self.atlas_view.section_rabnt1.toggled.connect(self.display_changed)
         self.atlas_view.section_rabnt2.toggled.connect(self.display_changed)
         self.atlas_view.section_rabnt3.toggled.connect(self.display_changed)
         self.atlas_view.label_tree.labels_changed.connect(self.sig_label_changed)
-        self.atlas_view.label_tree.label_color_changed.connect(self.sig_label_color_changed)
+        self.atlas_view.label_tree.label_color_changed.connect(
+            self.sig_label_color_changed
+        )
         self.atlas_view.label_tree.reset_labels.connect(self.sig_reset_labels)
         # hovered
-        self.atlas_view.cimg.sig_mouse_hovered.connect(self.coronal_slice_stacks_hovered)
-        self.atlas_view.simg.sig_mouse_hovered.connect(self.sagital_slice_stacks_hovered)
-        self.atlas_view.himg.sig_mouse_hovered.connect(self.horizontal_slice_stacks_hovered)
+        self.atlas_view.cimg.sig_mouse_hovered.connect(
+            self.coronal_slice_stacks_hovered
+        )
+        self.atlas_view.simg.sig_mouse_hovered.connect(
+            self.sagital_slice_stacks_hovered
+        )
+        self.atlas_view.himg.sig_mouse_hovered.connect(
+            self.horizontal_slice_stacks_hovered
+        )
         # clicked
         self.atlas_view.cimg.sig_mouse_clicked.connect(self.atlas_stacks_clicked)
         self.atlas_view.simg.sig_mouse_clicked.connect(self.atlas_stacks_clicked)
         self.atlas_view.himg.sig_mouse_clicked.connect(self.atlas_stacks_clicked)
         # ruler points
-        self.atlas_view.cimg.image_dict['ruler_path'].sigPointsClicked.connect(self.atlas_ruler_points_clicked)
-        self.atlas_view.simg.image_dict['ruler_path'].sigPointsClicked.connect(self.atlas_ruler_points_clicked)
-        self.atlas_view.himg.image_dict['ruler_path'].sigPointsClicked.connect(self.atlas_ruler_points_clicked)
+        self.atlas_view.cimg.image_dict["ruler_path"].sigPointsClicked.connect(
+            self.atlas_ruler_points_clicked
+        )
+        self.atlas_view.simg.image_dict["ruler_path"].sigPointsClicked.connect(
+            self.atlas_ruler_points_clicked
+        )
+        self.atlas_view.himg.image_dict["ruler_path"].sigPointsClicked.connect(
+            self.atlas_ruler_points_clicked
+        )
         # triangle points moving and clicked
-        self.atlas_view.cimg.image_dict['tri_pnts'].mouseDragged.connect(self.atlas_window_tri_pnts_moving)
-        self.atlas_view.cimg.image_dict['tri_pnts'].mouseClicked.connect(self.atlas_window_tri_pnts_clicked)
-        self.atlas_view.himg.image_dict['tri_pnts'].mouseDragged.connect(self.atlas_window_tri_pnts_moving)
-        self.atlas_view.himg.image_dict['tri_pnts'].mouseClicked.connect(self.atlas_window_tri_pnts_clicked)
-        self.atlas_view.simg.image_dict['tri_pnts'].mouseDragged.connect(self.atlas_window_tri_pnts_moving)
-        self.atlas_view.simg.image_dict['tri_pnts'].mouseClicked.connect(self.atlas_window_tri_pnts_clicked)
+        self.atlas_view.cimg.image_dict["tri_pnts"].mouseDragged.connect(
+            self.atlas_window_tri_pnts_moving
+        )
+        self.atlas_view.cimg.image_dict["tri_pnts"].mouseClicked.connect(
+            self.atlas_window_tri_pnts_clicked
+        )
+        self.atlas_view.himg.image_dict["tri_pnts"].mouseDragged.connect(
+            self.atlas_window_tri_pnts_moving
+        )
+        self.atlas_view.himg.image_dict["tri_pnts"].mouseClicked.connect(
+            self.atlas_window_tri_pnts_clicked
+        )
+        self.atlas_view.simg.image_dict["tri_pnts"].mouseDragged.connect(
+            self.atlas_window_tri_pnts_moving
+        )
+        self.atlas_view.simg.image_dict["tri_pnts"].mouseClicked.connect(
+            self.atlas_window_tri_pnts_clicked
+        )
         # probe clicked
-        self.atlas_view.cimg.image_dict['atlas-probe'].sigClicked.connect(self.atlas_probe_pnts_clicked)
-        self.atlas_view.simg.image_dict['atlas-probe'].sigClicked.connect(self.atlas_probe_pnts_clicked)
-        self.atlas_view.himg.image_dict['atlas-probe'].sigClicked.connect(self.atlas_probe_pnts_clicked)
+        self.atlas_view.cimg.image_dict["atlas-probe"].sigClicked.connect(
+            self.atlas_probe_pnts_clicked
+        )
+        self.atlas_view.simg.image_dict["atlas-probe"].sigClicked.connect(
+            self.atlas_probe_pnts_clicked
+        )
+        self.atlas_view.himg.image_dict["atlas-probe"].sigClicked.connect(
+            self.atlas_probe_pnts_clicked
+        )
         # contour clicked
         # self.atlas_view.cimg.image_dict['atlas-contour'].sigClicked.connect(self.atlas_contour_pnts_clicked)
         # self.atlas_view.simg.image_dict['atlas-contour'].sigClicked.connect(self.atlas_contour_pnts_clicked)
         # self.atlas_view.himg.image_dict['atlas-contour'].sigClicked.connect(self.atlas_contour_pnts_clicked)
         # slice_stack
         self.atlas_view.slice_stack.sig_mouse_clicked.connect(self.atlas_stacks_clicked)
         self.atlas_view.slice_stack.sig_mouse_hovered.connect(self.slice_stack_hovered)
-        self.atlas_view.slice_stack.sig_key_pressed.connect(self.slice_stack_key_pressed)
-        self.atlas_view.slice_stack.image_dict['lasso_path'].sigPointsClicked.connect(
-            self.slice_window_lasso_points_clicked)
-        self.atlas_view.slice_stack.image_dict['ruler_path'].sigPointsClicked.connect(
-            self.atlas_ruler_points_clicked)
+        self.atlas_view.slice_stack.sig_key_pressed.connect(
+            self.slice_stack_key_pressed
+        )
+        self.atlas_view.slice_stack.image_dict["lasso_path"].sigPointsClicked.connect(
+            self.slice_window_lasso_points_clicked
+        )
+        self.atlas_view.slice_stack.image_dict["ruler_path"].sigPointsClicked.connect(
+            self.atlas_ruler_points_clicked
+        )
 
         # set color to mask layer
-        self.image_view.img_stacks.image_dict['img-mask'].setLookupTable(self.magic_wand_lut)
-        self.atlas_view.cimg.image_dict['atlas-mask'].setLookupTable(self.magic_wand_lut)
-        self.atlas_view.himg.image_dict['atlas-mask'].setLookupTable(self.magic_wand_lut)
-        self.atlas_view.simg.image_dict['atlas-mask'].setLookupTable(self.magic_wand_lut)
+        self.image_view.img_stacks.image_dict["img-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.atlas_view.cimg.image_dict["atlas-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.atlas_view.himg.image_dict["atlas-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.atlas_view.simg.image_dict["atlas-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
 
         # --------------------------------------------------------
         #                 connect all menu actions
         # --------------------------------------------------------
         # menubar_style = read_qss_file("qss/menu_bar.qss")
         # self.menuBar.setStyleSheet(menubar_style)
         # file menu related
         self.actionAtlas.triggered.connect(self.load_atlas_clicked)
         self.actionSingle_Image.triggered.connect(self.load_image)
         self.actionSave_Project.triggered.connect(self.save_project_called)
         self.actionCurrent_Layer.triggered.connect(self.save_current_layer)
         self.actionAll_Layer.triggered.connect(self.save_all_layer)
         self.actionSave_Current.triggered.connect(self.save_current_object)
-        self.actionSave_Probes.triggered.connect(lambda: self.save_merged_object('probe'))
-        self.actionSave_Cells.triggered.connect(lambda: self.save_merged_object('cell'))
-        self.actionSave_Virus.triggered.connect(lambda: self.save_merged_object('virus'))
-        self.actionSave_Drawings.triggered.connect(lambda: self.save_merged_object('drawing'))
-        self.actionSave_Contours.triggered.connect(lambda: self.save_merged_object('contour'))
+        self.actionSave_Probes.triggered.connect(
+            lambda: self.save_merged_object("probe")
+        )
+        self.actionSave_Cells.triggered.connect(lambda: self.save_merged_object("cell"))
+        self.actionSave_Virus.triggered.connect(
+            lambda: self.save_merged_object("virus")
+        )
+        self.actionSave_Drawings.triggered.connect(
+            lambda: self.save_merged_object("drawing")
+        )
+        self.actionSave_Contours.triggered.connect(
+            lambda: self.save_merged_object("contour")
+        )
         self.actionLoad_Project.triggered.connect(self.load_project_called)
         self.actionLoad_Objects.triggered.connect(self.load_objects)
         self.actionLoad_Layers.triggered.connect(self.load_layers_called)
         self.actionExternal_Cells.triggered.connect(self.load_external_cells_called)
 
         # edit menu related
         self.actionDistance.triggered.connect(self.shift_setting_changed)
         self.actionAngle.triggered.connect(self.rotate_setting_changed)
-        self.actionUp.triggered.connect(lambda: self.vertical_translation_pressed('up'))
-        self.actionDown.triggered.connect(lambda: self.vertical_translation_pressed('down'))
-        self.actionLeft.triggered.connect(lambda: self.horizontal_translation_pressed('left'))
-        self.actionRight.triggered.connect(lambda: self.horizontal_translation_pressed('right'))
-        self.actionClockwise.triggered.connect(lambda: self.layer_rotation_pressed('clockwise'))
-        self.actionCounter_Clockwise.triggered.connect(lambda: self.layer_rotation_pressed('counter_clock'))
+        self.actionUp.triggered.connect(lambda: self.vertical_translation_pressed("up"))
+        self.actionDown.triggered.connect(
+            lambda: self.vertical_translation_pressed("down")
+        )
+        self.actionLeft.triggered.connect(
+            lambda: self.horizontal_translation_pressed("left")
+        )
+        self.actionRight.triggered.connect(
+            lambda: self.horizontal_translation_pressed("right")
+        )
+        self.actionClockwise.triggered.connect(
+            lambda: self.layer_rotation_pressed("clockwise")
+        )
+        self.actionCounter_Clockwise.triggered.connect(
+            lambda: self.layer_rotation_pressed("counter_clock")
+        )
         self.actionUndo.triggered.connect(self.undo_called)
         self.actionRedo.triggered.connect(self.redo_called)
         self.actionClear.triggered.connect(self.clear_all_layers)
 
         # atlas menu related
         self.actionDownload.triggered.connect(self.download_waxholm_rat_atlas)
-        self.actionDownload_Allen_Mice_Atlas.triggered.connect(self.download_allen_mice_atlas)
+        self.actionDownload_Allen_Mice_Atlas.triggered.connect(
+            self.download_allen_mice_atlas
+        )
         self.actionAtlas_Processor.triggered.connect(self.process_raw_atlas_data)
         self.actionLoad_Image_Atlas.triggered.connect(self.load_atlas_slice)
         self.actionCrop.triggered.connect(self.crop_slice)
         self.actionRegister_Slice_Info.triggered.connect(self.register_slice_info)
         self.actionSave_Slice.triggered.connect(self.save_processed_slice)
         self.actionSwitch_Atlas.triggered.connect(self.switch_atlas)
         self.actionBregma_Picker.setCheckable(True)
         self.actionBregma_Picker.triggered.connect(self.pick_bregma)
         self.actionCreate_Slice_Layer.triggered.connect(self.process_slice)
-        self.actionSave_Triangulation_Points.triggered.connect(self.save_triangulation_points)
-        self.actionLoad_Triangulation_Points.triggered.connect(self.load_triangulation_points)
+        self.actionSave_Triangulation_Points.triggered.connect(
+            self.save_triangulation_points
+        )
+        self.actionLoad_Triangulation_Points.triggered.connect(
+            self.load_triangulation_points
+        )
 
         # view menu related
         self.actionCoronal_Window.triggered.connect(self.show_only_coronal_window)
         self.actionSagital_Window.triggered.connect(self.show_only_sagital_window)
         self.actionHorizontal_Window.triggered.connect(self.show_only_horizontal_window)
         self.action3D_Window.triggered.connect(self.show_only_3d_window)
         self.actionImage_Window.triggered.connect(self.show_only_image_window)
@@ -403,32 +533,39 @@
         self.actionGrids_Off.triggered.connect(self.show_grids)
 
         # image menu related
         self.actionFlip_Horizontal.triggered.connect(self.image_view.image_horizon_flip)
         self.actionFlip_Vertical.triggered.connect(self.image_view.image_vertical_flip)
         self.action180.triggered.connect(self.image_view.image_180_rotate)
         self.action90_Clockwise.triggered.connect(self.image_view.image_90_rotate)
-        self.action90_Counter_Clockwise.triggered.connect(self.image_view.image_90_counter_rotate)
+        self.action90_Counter_Clockwise.triggered.connect(
+            self.image_view.image_90_counter_rotate
+        )
         self.actionProcess_Image.triggered.connect(self.turn_current_to_process)
         self.actionReset_Image.triggered.connect(self.reset_current_image)
-        self.action1_Clockwise.triggered.connect(lambda: self.image_view.image_1_rotate('clockwise'))
-        self.action1_Counter_Clockwise.triggered.connect(lambda: self.image_view.image_1_rotate('counter'))
+        self.action1_Clockwise.triggered.connect(
+            lambda: self.image_view.image_1_rotate("clockwise")
+        )
+        self.action1_Counter_Clockwise.triggered.connect(
+            lambda: self.image_view.image_1_rotate("counter")
+        )
         self.actionCut.triggered.connect(self.cut_image)
         self.actionHide.setCheckable(True)
         self.actionHide.triggered.connect(self.hide_image)
 
         # objects menu related
         self.actionSave_Probe_Setting.triggered.connect(self.save_probe_setting_called)
         self.actionLoad_Probe_Setting.triggered.connect(self.load_probe_setting_called)
-        self.actionMulti_Probe_Planning.triggered.connect(self.multi_probe_setting_called)
+        self.actionMulti_Probe_Planning.triggered.connect(
+            self.multi_probe_setting_called
+        )
 
         # about menu related
         self.actionAbout_HERBS.triggered.connect(self.about_herbs_info)
 
-
         self.init_tool_bar()
         self.init_side_bar()
         # --------------------------------------------------------
         # --------------------------------------------------------
         #
         #                 windows setting up
         #
@@ -473,55 +610,54 @@
         # ------------------ slice view
         self.aslice_view_layout = QGridLayout(self.sliceframe)
         self.aslice_view_layout.setSpacing(0)
         self.aslice_view_layout.setContentsMargins(0, 0, 0, 0)
         self.aslice_view_layout.addWidget(self.atlas_view.slice_stack, 0, 0, 1, 1)
 
         # -------------------- 3D view
-        self.view3d.opts['distance'] = 200  # distance of camera from center
-        self.view3d.opts['elevation'] = 50  # camera's angle of elevation in degrees
-        self.view3d.opts['azimuth'] = 45    # camera's azimuthal angle in degrees
-        self.view3d.opts['fov'] = 60        # horizontal field of view in degrees
+        self.view3d.opts["distance"] = 200  # distance of camera from center
+        self.view3d.opts["elevation"] = 50  # camera's angle of elevation in degrees
+        self.view3d.opts["azimuth"] = 45  # camera's azimuthal angle in degrees
+        self.view3d.opts["fov"] = 60  # horizontal field of view in degrees
         # self.view3d.setBackgroundColor(pg.mkColor(255, 255, 255))
         self.view3d.addItem(self.atlas_view.axis)
         # self.view3d.addItem(self.atlas_view.grid)
 
         self.view3d.addItem(self.atlas_view.mesh)
         self.view3d.addItem(self.atlas_view.ap_plate_mesh)
         self.view3d.addItem(self.atlas_view.dv_plate_mesh)
         self.view3d.addItem(self.atlas_view.ml_plate_mesh)
 
-
         # -------------------- initial window
         self.coronalframe.show()
         self.sagitalframe.hide()
         self.horizontalframe.hide()
         self.sagitalcopyframe.hide()
         self.view3d.hide()
         self.histview.hide()
         self.sliceframe.setVisible(False)
 
         self.sidebar.setCurrentIndex(0)
-        tab1_shortcut = QShortcut(QKeySequence('Ctrl+1'), self)
+        tab1_shortcut = QShortcut(QKeySequence("Ctrl+1"), self)
         tab1_shortcut.activated.connect(lambda: self.sidebar_tab_state(0))
-        tab2_shortcut = QShortcut(QKeySequence('Ctrl+2'), self)
+        tab2_shortcut = QShortcut(QKeySequence("Ctrl+2"), self)
         tab2_shortcut.activated.connect(lambda: self.sidebar_tab_state(1))
-        tab3_shortcut = QShortcut(QKeySequence('Ctrl+3'), self)
+        tab3_shortcut = QShortcut(QKeySequence("Ctrl+3"), self)
         tab3_shortcut.activated.connect(lambda: self.sidebar_tab_state(2))
-        tab4_shortcut = QShortcut(QKeySequence('Ctrl+4'), self)
+        tab4_shortcut = QShortcut(QKeySequence("Ctrl+4"), self)
         tab4_shortcut.activated.connect(lambda: self.sidebar_tab_state(3))
-        tab5_shortcut = QShortcut(QKeySequence('Ctrl+5'), self)
+        tab5_shortcut = QShortcut(QKeySequence("Ctrl+5"), self)
         tab5_shortcut.activated.connect(lambda: self.sidebar_tab_state(4))
 
-        undo_shortcut = QShortcut(QKeySequence('Ctrl+Z'), self)
+        undo_shortcut = QShortcut(QKeySequence("Ctrl+Z"), self)
         undo_shortcut.activated.connect(self.undo_called)
-        redo_shortcut = QShortcut(QKeySequence('Ctrl+Shift+Z'), self)
+        redo_shortcut = QShortcut(QKeySequence("Ctrl+Shift+Z"), self)
         redo_shortcut.activated.connect(self.redo_called)
 
-        self.print_message('Ready', self.normal_color)
+        self.print_message("Ready", self.normal_color)
 
     def sidebar_tab_state(self, tab_num):
         self.sidebar.setCurrentIndex(tab_num)
 
     # ------------------------------------------------------------------
     #
     #               Menubar - View - Window Control
@@ -639,19 +775,19 @@
             self.sagital_copy_layout.removeWidget(self.atlas_view.slut)
             self.sagital_copy_layout.removeWidget(self.atlas_view.spage_ctrl)
             self.sagital_layout.addWidget(self.atlas_view.simg, 0, 0, 1, 1)
             self.sagital_layout.addWidget(self.atlas_view.slut, 0, 1, 1, 1)
             self.sagital_layout.addWidget(self.atlas_view.spage_ctrl, 1, 0, 1, 2)
         self.num_windows = 2
         self.atlas_view.radio_group.setVisible(True)
-        if self.atlas_display == 'coronal':
+        if self.atlas_display == "coronal":
             self.coronalframe.setVisible(True)
             self.sagitalframe.setVisible(False)
             self.horizontalframe.setVisible(False)
-        elif self.atlas_display == 'sagittal':
+        elif self.atlas_display == "sagittal":
             self.coronalframe.setVisible(False)
             self.sagitalframe.setVisible(True)
             self.horizontalframe.setVisible(False)
         else:
             self.coronalframe.setVisible(False)
             self.sagitalframe.setVisible(False)
             self.horizontalframe.setVisible(True)
@@ -680,19 +816,19 @@
             self.sagital_copy_layout.removeWidget(self.atlas_view.slut)
             self.sagital_copy_layout.removeWidget(self.atlas_view.spage_ctrl)
             self.sagital_layout.addWidget(self.atlas_view.simg, 0, 0, 1, 1)
             self.sagital_layout.addWidget(self.atlas_view.slut, 0, 1, 1, 1)
             self.sagital_layout.addWidget(self.atlas_view.spage_ctrl, 1, 0, 1, 2)
         self.num_windows = 3
         self.atlas_view.radio_group.setVisible(True)
-        if self.atlas_display == 'coronal':
+        if self.atlas_display == "coronal":
             self.coronalframe.setVisible(True)
             self.sagitalframe.setVisible(False)
             self.horizontalframe.setVisible(False)
-        elif self.atlas_display == 'sagittal':
+        elif self.atlas_display == "sagittal":
             self.coronalframe.setVisible(False)
             self.sagitalframe.setVisible(True)
             self.horizontalframe.setVisible(False)
         else:
             self.coronalframe.setVisible(False)
             self.sagitalframe.setVisible(False)
             self.horizontalframe.setVisible(True)
@@ -721,76 +857,78 @@
         self.view3d.setVisible(True)
         self.histview.setVisible(False)
         self.sliceframe.setVisible(False)
 
     def show_grids(self):
         if self.is_grids_on:
             self.is_grids_on = False
-            self.actionGrids_Off.setText('Grids: Off')
+            self.actionGrids_Off.setText("Grids: Off")
         else:
             self.is_grids_on = True
-            self.actionGrids_Off.setText('Grids: On')
-        self.atlas_view.cimg.image_dict['grid_lines'].setVisible(self.is_grids_on)
-        self.atlas_view.simg.image_dict['grid_lines'].setVisible(self.is_grids_on)
-        self.atlas_view.himg.image_dict['grid_lines'].setVisible(self.is_grids_on)
-        self.atlas_view.slice_stack.image_dict['grid_lines'].setVisible(self.is_grids_on)
-        self.image_view.img_stacks.image_dict['grid_lines'].setVisible(self.is_grids_on)
+            self.actionGrids_Off.setText("Grids: On")
+        self.atlas_view.cimg.image_dict["grid_lines"].setVisible(self.is_grids_on)
+        self.atlas_view.simg.image_dict["grid_lines"].setVisible(self.is_grids_on)
+        self.atlas_view.himg.image_dict["grid_lines"].setVisible(self.is_grids_on)
+        self.atlas_view.slice_stack.image_dict["grid_lines"].setVisible(
+            self.is_grids_on
+        )
+        self.image_view.img_stacks.image_dict["grid_lines"].setVisible(self.is_grids_on)
 
     # display mode
     def switch_3d_display_mode(self):
-        if self.display_mode_3d == 'dark':
+        if self.display_mode_3d == "dark":
             self.view3d.setBackgroundColor(pg.mkColor(255, 255, 255))
-            self.atlas_view.mesh.setGLOptions('translucent')
-            self.atlas_view.ap_plate_mesh.setGLOptions('translucent')
-            self.atlas_view.dv_plate_mesh.setGLOptions('translucent')
-            self.atlas_view.ml_plate_mesh.setGLOptions('translucent')
-            self.display_mode_3d = 'light'
-            self.obj_display_mode = 'additive'
-            self.actionMode_Dark.setText('3D Mode: light')
+            self.atlas_view.mesh.setGLOptions("translucent")
+            self.atlas_view.ap_plate_mesh.setGLOptions("translucent")
+            self.atlas_view.dv_plate_mesh.setGLOptions("translucent")
+            self.atlas_view.ml_plate_mesh.setGLOptions("translucent")
+            self.display_mode_3d = "light"
+            self.obj_display_mode = "additive"
+            self.actionMode_Dark.setText("3D Mode: light")
         else:
             self.view3d.setBackgroundColor(pg.mkColor(0, 0, 0))
-            self.atlas_view.mesh.setGLOptions('additive')
-            self.atlas_view.ap_plate_mesh.setGLOptions('additive')
-            self.atlas_view.dv_plate_mesh.setGLOptions('additive')
-            self.atlas_view.ml_plate_mesh.setGLOptions('additive')
-            self.display_mode_3d = 'dark'
-            self.obj_display_mode = 'opaque'
-            self.actionMode_Dark.setText('3D Mode: dark')
+            self.atlas_view.mesh.setGLOptions("additive")
+            self.atlas_view.ap_plate_mesh.setGLOptions("additive")
+            self.atlas_view.dv_plate_mesh.setGLOptions("additive")
+            self.atlas_view.ml_plate_mesh.setGLOptions("additive")
+            self.display_mode_3d = "dark"
+            self.obj_display_mode = "opaque"
+            self.actionMode_Dark.setText("3D Mode: dark")
 
     def show_3d_planes(self):
         if self.is_planes_on:
             self.is_planes_on = False
-            self.actionPlanes_On.setText('Planes: Off')
+            self.actionPlanes_On.setText("Planes: Off")
         else:
             self.is_planes_on = True
-            self.actionPlanes_On.setText('Planes: On')
+            self.actionPlanes_On.setText("Planes: On")
         self.atlas_view.vis_3d_planes(self.is_planes_on)
 
     def show_3d_axes(self):
         if self.is_axis_on:
             self.is_axis_on = False
-            self.actionAxes_On.setText('Axes: Off')
+            self.actionAxes_On.setText("Axes: Off")
         else:
             self.is_axis_on = True
-            self.actionAxes_On.setText('Axes: On')
+            self.actionAxes_On.setText("Axes: On")
         self.atlas_view.vis_3d_axes(self.is_axis_on)
 
     def switch_2d_display_mode(self):
-        if self.display_mode_2d == 'dark':
-            self.atlas_view.cimg.setBackground('w')
-            self.atlas_view.simg.setBackground('w')
-            self.atlas_view.himg.setBackground('w')
-            self.display_mode_2d = 'light'
-            self.action2D_Mode_Dark.setText('2D Mode: Light')
-        else:
-            self.atlas_view.cimg.setBackground('k')
-            self.atlas_view.simg.setBackground('k')
-            self.atlas_view.himg.setBackground('k')
-            self.display_mode_2d = 'dark'
-            self.action2D_Mode_Dark.setText('2D Mode: Dark')
+        if self.display_mode_2d == "dark":
+            self.atlas_view.cimg.setBackground("w")
+            self.atlas_view.simg.setBackground("w")
+            self.atlas_view.himg.setBackground("w")
+            self.display_mode_2d = "light"
+            self.action2D_Mode_Dark.setText("2D Mode: Light")
+        else:
+            self.atlas_view.cimg.setBackground("k")
+            self.atlas_view.simg.setBackground("k")
+            self.atlas_view.himg.setBackground("k")
+            self.display_mode_2d = "dark"
+            self.action2D_Mode_Dark.setText("2D Mode: Dark")
 
     #
     # def clear_layout(self, layout):
     #     while layout.count() > 0:
     #         item = layout.takeAt(0)
     #         if not item:
     #             continue
@@ -812,81 +950,80 @@
             msg = self.multi_settings.check_multi_settings()
             if msg is not None:
                 self.print_message(msg, self.error_message_color)
                 return
             self.valid_multi_settings = True
 
     def save_probe_setting_called(self):
-        self.print_message('under development', self.error_message_color)
+        self.print_message("under development", self.error_message_color)
 
     def load_probe_setting_called(self):
-        self.print_message('under development', self.error_message_color)
-
-
-
-
-
-
-
-
-
-
-
+        self.print_message("under development", self.error_message_color)
 
     # ------------------------------------------------------------------
     #
     #                   Sidebar - Atlas panel related
     #
     # ------------------------------------------------------------------
     def display_changed(self):
         rbtn = self.sender()
         if rbtn.isChecked():
             if rbtn.text() == "Coronal":
                 self.coronalframe.setVisible(True)
                 self.sagitalframe.setVisible(False)
                 self.horizontalframe.setVisible(False)
-                self.atlas_display = 'coronal'
+                self.atlas_display = "coronal"
             elif rbtn.text() == "Sagittal":
                 self.coronalframe.setVisible(False)
                 self.sagitalframe.setVisible(True)
                 self.horizontalframe.setVisible(False)
-                self.atlas_display = 'sagittal'
+                self.atlas_display = "sagittal"
             else:
                 self.coronalframe.setVisible(False)
                 self.sagitalframe.setVisible(False)
                 self.horizontalframe.setVisible(True)
-                self.atlas_display = 'horizontal'
+                self.atlas_display = "horizontal"
         if self.atlas_view.atlas_data is None or self.atlas_view.atlas_label is None:
             return
         self.atlas_view.working_cut_changed(self.atlas_display)
         self.reset_tri_points_atlas()
-        self.working_atlas_data['atlas-mask'] = np.ones(self.atlas_view.slice_size).astype('uint8')
+        self.working_atlas_data["atlas-mask"] = np.ones(
+            self.atlas_view.slice_size
+        ).astype("uint8")
         # self.check_n_trajectory()
 
     def clear_tri_inside(self):
         self.atlas_tri_inside_data.clear()  # renew tri_inside data to empty
         inds = np.arange(len(self.working_atlas_text))[::-1]
         for da_ind in inds:
             self.atlas_view.working_atlas.vb.removeItem(self.working_atlas_text[da_ind])
             self.working_atlas_text[da_ind].deleteLater()
             del self.working_atlas_text[da_ind]
         self.working_atlas_text.clear()
 
     def reset_tri_onside_atlas(self):
-        self.atlas_rect = (0, 0, int(self.atlas_view.slice_size[1]), int(self.atlas_view.slice_size[0]))
+        self.atlas_rect = (
+            0,
+            0,
+            int(self.atlas_view.slice_size[1]),
+            int(self.atlas_view.slice_size[0]),
+        )
         self.atlas_corner_points = self.atlas_view.corner_points.copy()
         self.atlas_side_lines = self.atlas_view.side_lines.copy()
-        self.atlas_tri_onside_data = num_side_pnt_changed(self.np_onside, self.atlas_corner_points,
-                                                          self.atlas_side_lines)
+        self.atlas_tri_onside_data = num_side_pnt_changed(
+            self.np_onside, self.atlas_corner_points, self.atlas_side_lines
+        )
         self.atlas_tri_data = self.atlas_tri_onside_data + self.atlas_tri_inside_data
-        self.atlas_view.working_atlas.image_dict['tri_pnts'].setData(pos=np.asarray(self.atlas_tri_data))
-        if self.tool_box.checkable_btn_dict['triang_btn'].isChecked():
-            self.atlas_view.working_atlas.image_dict['tri_pnts'].setVisible(True)
+        self.atlas_view.working_atlas.image_dict["tri_pnts"].setData(
+            pos=np.asarray(self.atlas_tri_data)
+        )
+        if self.tool_box.checkable_btn_dict["triang_btn"].isChecked():
+            self.atlas_view.working_atlas.image_dict["tri_pnts"].setVisible(True)
         else:
-            self.atlas_view.working_atlas.image_dict['tri_pnts'].setVisible(False)
+            self.atlas_view.working_atlas.image_dict["tri_pnts"].setVisible(False)
         if self.tool_box.triang_vis_btn.isChecked():
             self.update_atlas_tri_lines()
 
     def reset_tri_points_atlas(self):
         self.clear_tri_inside()
         self.reset_tri_onside_atlas()
         self.small_atlas_rect = None
@@ -895,31 +1032,40 @@
     def reset_corners_hist(self):
         self.histo_tri_inside_data = []  # renew tri_inside data to empty
         for da_item in self.working_img_text:
             self.image_view.img_stacks.vb.removeItem(da_item)
             da_item.deleteLater()
             del da_item
         self.working_img_text = []
-        self.histo_rect = (0, 0, int(self.image_view.img_size[1]), int(self.image_view.img_size[0]))
+        self.histo_rect = (
+            0,
+            0,
+            int(self.image_view.img_size[1]),
+            int(self.image_view.img_size[0]),
+        )
         self.histo_corner_points = self.image_view.corner_points.copy()
         self.histo_side_lines = self.image_view.side_lines.copy()
-        self.histo_tri_onside_data = num_side_pnt_changed(self.np_onside, self.histo_corner_points, self.histo_side_lines)
+        self.histo_tri_onside_data = num_side_pnt_changed(
+            self.np_onside, self.histo_corner_points, self.histo_side_lines
+        )
 
         self.histo_tri_data = self.histo_tri_onside_data + self.histo_tri_inside_data
-        self.image_view.img_stacks.image_dict['tri_pnts'].setData(pos=np.asarray(self.histo_tri_data))
-        if self.tool_box.checkable_btn_dict['triang_btn'].isChecked():
-            self.image_view.img_stacks.image_dict['tri_pnts'].setVisible(True)
+        self.image_view.img_stacks.image_dict["tri_pnts"].setData(
+            pos=np.asarray(self.histo_tri_data)
+        )
+        if self.tool_box.checkable_btn_dict["triang_btn"].isChecked():
+            self.image_view.img_stacks.image_dict["tri_pnts"].setVisible(True)
         else:
-            self.image_view.img_stacks.image_dict['tri_pnts'].setVisible(False)
+            self.image_view.img_stacks.image_dict["tri_pnts"].setVisible(False)
         if self.tool_box.triang_vis_btn.isChecked():
             self.update_histo_tri_lines()
         self.small_atlas_rect = None
         self.small_histo_rect = None
 
-        self.white_img = np.ones(self.image_view.img_size).astype('uint8')
+        self.white_img = np.ones(self.image_view.img_size).astype("uint8")
 
     def vis_atlas_boundary(self):
         if self.atlas_view.atlas_data is None:
             return
         if self.atlas_view.show_boundary_btn.isChecked():
             self.atlas_view.cimg.boundary.setVisible(True)
             self.atlas_view.simg.boundary.setVisible(True)
@@ -932,171 +1078,234 @@
     # ------------------------------------------------------------------
     #
     #                  Menu Bar ---- Edit ----- related
     #
     # ------------------------------------------------------------------
     def clear_all_layers(self):  # except img-process and atlas-slice
         if not self.layer_ctrl.layer_link:
-            self.print_message('No layer data can be removed.', self.reminder_color)
+            self.print_message("No layer data can be removed.", self.reminder_color)
             return
         self.image_view.clear_image_stacks()
         self.atlas_view.clear_atlas_stacks()
         self.layer_ctrl.clear_all()
         for da_key in list(self.working_img_type.keys()):
-            if self.working_img_type[da_key] == 'vector':
+            if self.working_img_type[da_key] == "vector":
                 self.working_img_data[da_key] = []
             else:
                 self.working_img_data[da_key] = None
         for da_key in list(self.working_atlas_type.keys()):
             # if da_key == 'atlas-slice':
             #     continue
-            if self.working_atlas_type[da_key] == 'vector':
+            if self.working_atlas_type[da_key] == "vector":
                 self.working_atlas_data[da_key] = []
             else:
                 self.working_atlas_data[da_key] = None
-        self.working_img_data['cell_count'] = [0 for _ in range(5)]
-        self.working_atlas_data['cell_count'] = [0 for _ in range(5)]
+        self.working_img_data["cell_count"] = [0 for _ in range(5)]
+        self.working_atlas_data["cell_count"] = [0 for _ in range(5)]
         self.remove_h2a_transferred_layers()
         self.remove_a2h_transferred_layers()
 
     def shift_setting_changed(self):
-        shift_setting = LayerSettingDialog('Layer Shifting Setting', 0, 100, self.layer_shift_val)
+        shift_setting = LayerSettingDialog(
+            "Layer Shifting Setting", 0, 100, self.layer_shift_val
+        )
         shift_setting.exec()
         self.layer_shift_val = shift_setting.val
 
     def rotate_setting_changed(self):
-        rotate_setting = LayerSettingDialog('Layer Rotating Setting', 0, 50, self.layer_rotate_val)
+        rotate_setting = LayerSettingDialog(
+            "Layer Rotating Setting", 0, 50, self.layer_rotate_val
+        )
         rotate_setting.exec()
         self.layer_rotate_val = rotate_setting.val
-        print(self.layer_rotate_val)
+        # print(self.layer_rotate_val)
 
     def get_valid_layer(self):
         if not self.layer_ctrl.current_layer_index or not self.h2a_transferred:
-            self.print_message('Translation only works for layers on atlas window.', self.reminder_color)
+            self.print_message(
+                "Translation only works for layers on atlas window.",
+                self.reminder_color,
+            )
             return []
-        selected_links = [self.layer_ctrl.layer_link[ind] for ind in self.layer_ctrl.current_layer_index]
-        valid_links = [da_link for da_link in selected_links if 'atlas' in da_link]
+        selected_links = [
+            self.layer_ctrl.layer_link[ind]
+            for ind in self.layer_ctrl.current_layer_index
+        ]
+        valid_links = [da_link for da_link in selected_links if "atlas" in da_link]
         return valid_links
 
     def move_layers(self, da_link, moving_vec):
-        if da_link in ['img-process', 'atlas-slice']:
-            self.print_message('Transform only works on overlay and transferred layers.', self.reminder_color)
+        if da_link in ["img-process", "atlas-slice"]:
+            self.print_message(
+                "Transform only works on overlay and transferred layers.",
+                self.reminder_color,
+            )
             return
-        if 'img-' in da_link:
-            if self.working_img_type[da_link] == 'vector':
+        if "img-" in da_link:
+            if self.working_img_type[da_link] == "vector":
                 temp = np.asarray(self.working_img_data[da_link]).copy()
                 temp = temp + moving_vec
                 self.working_img_data[da_link] = temp.tolist()
                 self.image_view.img_stacks.image_dict[da_link].setData(
-                    pos=np.asarray(self.working_img_data[da_link]))
+                    pos=np.asarray(self.working_img_data[da_link])
+                )
             else:
                 shift_mat = np.float32([[1, 0, moving_vec[0]], [0, 1, moving_vec[1]]])
                 da_img = self.working_img_data[da_link].copy()
-                self.working_img_data[da_link] = cv2.warpAffine(da_img, shift_mat, da_img.shape[:2])
-                self.image_view.img_stacks.image_dict[da_link].setImage(self.working_img_data[da_link])
+                self.working_img_data[da_link] = cv2.warpAffine(
+                    da_img, shift_mat, da_img.shape[:2]
+                )
+                self.image_view.img_stacks.image_dict[da_link].setImage(
+                    self.working_img_data[da_link]
+                )
         else:
-            if self.working_atlas_type[da_link] == 'vector':
+            if self.working_atlas_type[da_link] == "vector":
                 temp = np.asarray(self.working_atlas_data[da_link]).copy()
                 temp = temp + moving_vec
                 self.working_atlas_data[da_link] = temp.tolist()
                 self.atlas_view.working_atlas.image_dict[da_link].setData(
-                    pos=np.asarray(self.working_atlas_data[da_link]))
+                    pos=np.asarray(self.working_atlas_data[da_link])
+                )
             else:
                 shift_mat = np.float32([[1, 0, moving_vec[0]], [0, 1, moving_vec[1]]])
                 da_img = self.working_atlas_data[da_link].copy()
-                self.working_atlas_data[da_link] = cv2.warpAffine(da_img, shift_mat, da_img.shape[:2])
-                self.atlas_view.working_atlas.image_dict[da_link].setImage(self.working_atlas_data[da_link])
-        if da_link == 'atlas-overlay':
-            print('record after transferred action for later accept.')
+                self.working_atlas_data[da_link] = cv2.warpAffine(
+                    da_img, shift_mat, da_img.shape[:2]
+                )
+                self.atlas_view.working_atlas.image_dict[da_link].setImage(
+                    self.working_atlas_data[da_link]
+                )
+        if da_link == "atlas-overlay":
+            print("record after transferred action for later accept.")
 
     def rotate_layers(self, da_link, rotate_angle):
         theta = np.radians(rotate_angle)
-        rot_mat = np.array(((np.cos(theta), -np.sin(theta)), (np.sin(theta), np.cos(theta))))
-
-        if da_link in ['img-process', 'atlas-slice']:
-            self.print_message('Transform only works on overlay and transferred layers.', self.reminder_color)
+        rot_mat = np.array(
+            ((np.cos(theta), -np.sin(theta)), (np.sin(theta), np.cos(theta)))
+        )
+
+        if da_link in ["img-process", "atlas-slice"]:
+            self.print_message(
+                "Transform only works on overlay and transferred layers.",
+                self.reminder_color,
+            )
             return
         else:
-            if 'img-' in da_link:
+            if "img-" in da_link:
                 img_rect = cv2.boundingRect(self.histo_tri_onside_data)
-                img_center = np.array([img_rect[0] + 0.5 * img_rect[2], img_rect[1] + 0.5 * img_rect[3]]).astype(int)
-                if self.working_img_type[da_link] == 'vector':
-                    temp = np.asarray(self.working_img_data[da_link]).copy() - img_center
+                img_center = np.array(
+                    [img_rect[0] + 0.5 * img_rect[2], img_rect[1] + 0.5 * img_rect[3]]
+                ).astype(int)
+                if self.working_img_type[da_link] == "vector":
+                    temp = (
+                        np.asarray(self.working_img_data[da_link]).copy() - img_center
+                    )
                     temp = np.dot(rot_mat, temp) + img_center
                     self.working_img_data[da_link] = temp.tolist()
                     self.image_view.img_stacks.image_dict[da_link].setData(
-                        pos=np.asarray(self.working_img_data[da_link]))
+                        pos=np.asarray(self.working_img_data[da_link])
+                    )
                 else:
-                    temp = rotate(self.working_img_data[da_link], rotate_angle, img_center)
+                    temp = rotate(
+                        self.working_img_data[da_link], rotate_angle, img_center
+                    )
                     self.working_img_data[da_link] = temp.copy()
-                    self.image_view.img_stacks.image_dict[da_link].setImage(self.working_img_data[da_link])
+                    self.image_view.img_stacks.image_dict[da_link].setImage(
+                        self.working_img_data[da_link]
+                    )
             else:
                 atlas_rect = cv2.boundingRect(self.histo_tri_onside_data)
-                atlas_center = np.array([atlas_rect[0] + 0.5 * atlas_rect[2], atlas_rect[1] + 0.5 * atlas_rect[3]])
+                atlas_center = np.array(
+                    [
+                        atlas_rect[0] + 0.5 * atlas_rect[2],
+                        atlas_rect[1] + 0.5 * atlas_rect[3],
+                    ]
+                )
                 atlas_center = atlas_center.astype(int)
-                if self.working_atlas_type[da_link] == 'vector':
-                    temp = np.asarray(self.working_atlas_data[da_link]).copy() - atlas_center
+                if self.working_atlas_type[da_link] == "vector":
+                    temp = (
+                        np.asarray(self.working_atlas_data[da_link]).copy()
+                        - atlas_center
+                    )
                     temp = np.dot(rot_mat, temp) + atlas_center
                     self.working_atlas_data[da_link] = temp.tolist()
                     self.atlas_view.working_atlas.image_dict[da_link].setData(
-                        pos=np.asarray(self.working_atlas_data[da_link]))
+                        pos=np.asarray(self.working_atlas_data[da_link])
+                    )
                 else:
-                    temp = rotate(self.working_atlas_data[da_link], rotate_angle, atlas_center)
+                    temp = rotate(
+                        self.working_atlas_data[da_link], rotate_angle, atlas_center
+                    )
                     self.working_atlas_data[da_link] = temp.copy()
-                    self.atlas_view.working_atlas.image_dict[da_link].setImage(self.working_atlas_data[da_link])
+                    self.atlas_view.working_atlas.image_dict[da_link].setImage(
+                        self.working_atlas_data[da_link]
+                    )
 
     def vertical_translation_pressed(self, moving_direction):
         valid_links = self.get_valid_layer()
 
-        if moving_direction == 'up':
-            moving_vec = np.array([0, - self.layer_shift_val])
+        if moving_direction == "up":
+            moving_vec = np.array([0, -self.layer_shift_val])
         else:
             moving_vec = np.array([0, self.layer_shift_val])
 
         for da_link in valid_links:
             self.move_layers(da_link, moving_vec)
 
         if self.a2h_transferred or self.h2a_transferred:
-            self.layer_action_after_matching.append({'action': 'shift', 'val': moving_vec})
+            self.layer_action_after_matching.append(
+                {"action": "shift", "val": moving_vec}
+            )
 
     def horizontal_translation_pressed(self, moving_direction):
         valid_links = self.get_valid_layer()
 
-        if moving_direction == 'right':
+        if moving_direction == "right":
             moving_vec = np.array([self.layer_shift_val, 0])
         else:
-            moving_vec = np.array([- self.layer_shift_val, 0])
+            moving_vec = np.array([-self.layer_shift_val, 0])
 
         for da_link in valid_links:
             self.move_layers(da_link, moving_vec)
 
         if self.a2h_transferred or self.h2a_transferred:
-            self.layer_action_after_matching.append({'action': 'shift', 'val': moving_vec})
+            self.layer_action_after_matching.append(
+                {"action": "shift", "val": moving_vec}
+            )
 
     def layer_rotation_pressed(self, rotating_direction):
         valid_links = self.get_valid_layer()
 
-        if rotating_direction == 'clockwise':
+        if rotating_direction == "clockwise":
             rotating_val = self.layer_rotate_val * 1
         else:
             rotating_val = self.layer_rotate_val * -1
 
         for da_link in valid_links:
             self.rotate_layers(da_link, rotating_val)
 
         if self.a2h_transferred or self.h2a_transferred:
-            self.layer_action_after_matching.append({'action': 'rotate', 'val': rotating_val})
+            self.layer_action_after_matching.append(
+                {"action": "rotate", "val": rotating_val}
+            )
 
     def save_current_action(self, current_tool, layer_link, data, layer_tb):
         if self.action_id != 0:
-            del_index = np.arange(len(self.action_list) + self.action_id, len(self.action_list))[::-1]
+            del_index = np.arange(
+                len(self.action_list) + self.action_id, len(self.action_list)
+            )[::-1]
             for da_ind in del_index:
                 del self.action_list[da_ind]
             self.action_id = 0
-        current_action = {'tool': current_tool, 'link': layer_link, 'data': data, 'layer': layer_tb}
+        current_action = {
+            "tool": current_tool,
+            "link": layer_link,
+            "data": data,
+            "layer": layer_tb,
+        }
         self.action_list.append(current_action)
         if len(self.action_list) > 6:
             del self.action_list[0]
 
     def redo_called(self):
         self.action_id += 1
         if self.action_id > 0:
@@ -1109,135 +1318,165 @@
         if abs(self.action_id) >= len(self.action_list):
             self.action_id += 1
             return
         self.set_undo_redo_data()
 
     def set_undo_redo_data(self):
         current_action = self.action_list[self.action_id - 1]
-        current_data = current_action['data']
-        layer_link = current_action['link']
-        current_tool = current_action['tool']
-        da_layer = current_action['layer']
-        if current_tool != 'delete':
+        current_data = current_action["data"]
+        layer_link = current_action["link"]
+        current_tool = current_action["tool"]
+        da_layer = current_action["layer"]
+        if current_tool != "delete":
             self.tool_box.checkable_btn_dict[current_tool].setChecked(True)
-        if 'img' in layer_link:
-            if layer_link == 'img-process':
-                self.image_view.processing_img = current_data['data']
+        if "img" in layer_link:
+            if layer_link == "img-process":
+                self.image_view.processing_img = current_data["data"]
                 self.image_view.img_stacks.set_data(self.image_view.processing_img)
-            elif layer_link in ['img-mask', 'img-virus']:
-                self.working_img_data[layer_link] = current_data['data']
-                self.image_view.img_stacks.image_dict[layer_link].setImage(self.working_img_data[layer_link])
-            elif layer_link == 'img-cells':
-                self.working_img_data[layer_link] = current_data['data']
-                self.working_img_data['cell_size'] = current_data['size']
-                self.working_img_data['cell_symbol'] = current_data['symbol']
-                self.working_img_data['cell_layer_index'] = current_data['index']
-                self.working_img_data['cell_count'] = current_data['count']
+            elif layer_link in ["img-mask", "img-virus"]:
+                self.working_img_data[layer_link] = current_data["data"]
+                self.image_view.img_stacks.image_dict[layer_link].setImage(
+                    self.working_img_data[layer_link]
+                )
+            elif layer_link == "img-cells":
+                self.working_img_data[layer_link] = current_data["data"]
+                self.working_img_data["cell_size"] = current_data["size"]
+                self.working_img_data["cell_symbol"] = current_data["symbol"]
+                self.working_img_data["cell_layer_index"] = current_data["index"]
+                self.working_img_data["cell_count"] = current_data["count"]
                 self.image_view.img_stacks.image_dict[layer_link].setData(
-                    pos=np.asarray(self.working_img_data[layer_link]), symbol=self.working_img_data['cell_symbol'])
+                    pos=np.asarray(self.working_img_data[layer_link]),
+                    symbol=self.working_img_data["cell_symbol"],
+                )
                 for i in range(5):
-                    self.tool_box.cell_count_val_list[i].setText(str(self.working_img_data['cell_count'][i]))
-            elif layer_link == 'img-drawing':
-                self.working_img_data[layer_link] = current_data['data']
-                if current_data['closed']:
+                    self.tool_box.cell_count_val_list[i].setText(
+                        str(self.working_img_data["cell_count"][i])
+                    )
+            elif layer_link == "img-drawing":
+                self.working_img_data[layer_link] = current_data["data"]
+                if current_data["closed"]:
                     self.set_img_pencil_closed_style()
                 else:
                     self.clear_img_pencil_closed_style()
                 self.image_view.img_stacks.image_dict[layer_link].setData(
-                    np.asarray(self.working_img_data[layer_link]))
-            elif layer_link == 'img-contour':
-                self.working_img_data[layer_link] = current_data['data']
+                    np.asarray(self.working_img_data[layer_link])
+                )
+            elif layer_link == "img-contour":
+                self.working_img_data[layer_link] = current_data["data"]
                 self.image_view.img_stacks.image_dict[layer_link].setData(
-                    np.asarray(self.working_img_data[layer_link]))
-            elif layer_link == 'img-probe':
-                self.working_img_data[layer_link] = current_data['data']
+                    np.asarray(self.working_img_data[layer_link])
+                )
+            elif layer_link == "img-probe":
+                self.working_img_data[layer_link] = current_data["data"]
                 self.image_view.img_stacks.image_dict[layer_link].setData(
-                    pos=np.asarray(self.working_img_data[layer_link]))
-        elif 'atlas' in layer_link:
-            if layer_link == 'atlas-slice':
-                print('process')
-            elif layer_link == 'atlas-mask':
-                print('mask')
-            elif layer_link == 'atlas-probe':
-                print('cells')
+                    pos=np.asarray(self.working_img_data[layer_link])
+                )
+        elif "atlas" in layer_link:
+            if layer_link == "atlas-slice":
+                print("process")
+            elif layer_link == "atlas-mask":
+                print("mask")
+            elif layer_link == "atlas-probe":
+                print("cells")
             else:
-                print('others')
+                print("others")
         else:
             return
         da_index = np.where(np.ravel(self.layer_ctrl.layer_link) == layer_link)[0][0]
         self.layer_ctrl.layer_list[da_index].set_thumbnail_data(da_layer)
 
     # ------------------------------------------------------------------
     #
     #                  Menu Bar ---- Image ----- related
     #
     # ------------------------------------------------------------------
     def hide_image(self):
         if self.image_view.image_file is None:
-            self.print_message('No histological image file is loaded.', self.error_message_color)
+            self.print_message(
+                "No histological image file is loaded.", self.error_message_color
+            )
             return
         if self.actionHide.isChecked():
             for i in range(self.image_view.image_file.n_channels):
                 self.image_view.img_stacks.image_list[i].setVisible(False)
         else:
             for i in range(self.image_view.image_file.n_channels):
                 self.image_view.img_stacks.image_list[i].setVisible(True)
 
     def turn_current_to_process(self):
         if self.image_view.image_file is None:
-            self.print_message('No histological image file is loaded.', self.error_message_color)
+            self.print_message(
+                "No histological image file is loaded.", self.error_message_color
+            )
             return
         self.image_view.processing_img = self.image_view.current_img.copy()
-        if self.image_view.image_file.pixel_type == 'rgb24':
+        if self.image_view.image_file.pixel_type == "rgb24":
             input_img = self.image_view.current_img.copy()
         else:
             channel_hsv = self.image_view.image_file.hsv_colors
-            img_temp = merge_channels_into_single_img(self.image_view.processing_img, channel_hsv)
-            input_img = cv2.normalize(img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
+            img_temp = merge_channels_into_single_img(
+                self.image_view.processing_img, channel_hsv
+            )
+            input_img = cv2.normalize(
+                img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U
+            )
         temp = gamma_correction(input_img, 1.45)
         res = cv2.resize(temp, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-        self.layer_ctrl.master_layers(res, layer_type='img-process', color=[])
+        self.layer_ctrl.master_layers(res, layer_type="img-process", color=[])
         self.sidebar_tab_state(3)
-        self.print_message('Processing image is created.', self.normal_color)
+        self.print_message("Processing image is created.", self.normal_color)
 
     def reset_current_image(self):
         if self.image_view.image_file is None:
             return
         if self.image_view.processing_img is None:
             return
         self.image_view.set_data_to_img_stacks()
         self.image_view.processing_img = None
-        remove_index = np.where(np.ravel(self.layer_ctrl.layer_link) == 'img-process')[0][0]
+        remove_index = np.where(np.ravel(self.layer_ctrl.layer_link) == "img-process")[
+            0
+        ][0]
         self.layer_ctrl.delete_layer(remove_index)
         self.reset_corners_hist()
-        self.print_message('Processing image is deleted.', self.normal_color)
+        self.print_message("Processing image is deleted.", self.normal_color)
         self.action_list = []
         self.action_id = 0
 
     def cut_image(self):
         if self.image_view.image_file is None:
-            self.print_message('Please load histological image.', self.reminder_color)
+            self.print_message("Please load histological image.", self.reminder_color)
             return
         if self.img_lasso_is_closure:
-            cut_rect = cv2.boundingRect(np.asarray(self.working_img_data['lasso_path']).astype('int'))
+            cut_rect = cv2.boundingRect(
+                np.asarray(self.working_img_data["lasso_path"]).astype("int")
+            )
             temp = self.image_view.current_img.copy()
-            self.image_view.processing_img = temp[cut_rect[1]:(cut_rect[1] + cut_rect[3]), cut_rect[0]:(cut_rect[0] + cut_rect[2])]
+            self.image_view.processing_img = temp[
+                cut_rect[1] : (cut_rect[1] + cut_rect[3]),
+                cut_rect[0] : (cut_rect[0] + cut_rect[2]),
+            ]
             for i in range(self.image_view.image_file.n_channels):
                 self.image_view.img_stacks.image_list[i].clear()
             self.image_view.set_data_and_size(self.image_view.processing_img)
             self.reset_corners_hist()
-            if self.image_view.image_file.pixel_type == 'rgb24':
+            if self.image_view.image_file.pixel_type == "rgb24":
                 input_img = self.image_view.processing_img.copy()
             else:
                 channel_hsv = self.image_view.image_file.hsv_colors
-                img_temp = merge_channels_into_single_img(self.image_view.processing_img, channel_hsv)
-                input_img = cv2.normalize(img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
+                img_temp = merge_channels_into_single_img(
+                    self.image_view.processing_img, channel_hsv
+                )
+                input_img = cv2.normalize(
+                    img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U
+                )
             temp = gamma_correction(input_img, 1.45)
-            res = cv2.resize(temp, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='img-process', color=[])
+            res = cv2.resize(
+                temp, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(res, layer_type="img-process", color=[])
             self.inactive_lasso()
             self.action_list = []
             self.action_id = 0
 
     # ------------------------------------------------------------------
     #
     #                  Menu Bar ---- Atlas ----- related
@@ -1251,25 +1490,41 @@
             return
 
         atlas_data = np.transpose(wax.worker.atlas_data, [2, 0, 1])[::-1, :, :]
         atlas_info = wax.worker.atlas_info
 
         label_info = wax.worker.label_info
 
-        segmentation_data = np.transpose(wax.worker.segmentation_data, [2, 0, 1])[::-1, :, :]
+        segmentation_data = np.transpose(wax.worker.segmentation_data, [2, 0, 1])[
+            ::-1, :, :
+        ]
         unique_label = wax.worker.unique_label
 
-        s_boundary = np.transpose(wax.worker.boundary['s_contour'], [2, 0, 1])[::-1, :, :]
-        c_boundary = np.transpose(wax.worker.boundary['c_contour'], [2, 0, 1])[::-1, :, :]
-        h_boundary = np.transpose(wax.worker.boundary['h_contour'], [2, 0, 1])[::-1, :, :]
-
-        boundary = {'s_contour': s_boundary, 'c_contour': c_boundary, 'h_contour': h_boundary}
-
-        self.set_volume_atlas_to_view(atlas_data, segmentation_data, atlas_info, label_info, boundary)
-        self.set_volume_atlas_3d(unique_label, wax.worker.mesh_data, wax.worker.small_mesh_list)
+        s_boundary = np.transpose(wax.worker.boundary["s_contour"], [2, 0, 1])[
+            ::-1, :, :
+        ]
+        c_boundary = np.transpose(wax.worker.boundary["c_contour"], [2, 0, 1])[
+            ::-1, :, :
+        ]
+        h_boundary = np.transpose(wax.worker.boundary["h_contour"], [2, 0, 1])[
+            ::-1, :, :
+        ]
+
+        boundary = {
+            "s_contour": s_boundary,
+            "c_contour": c_boundary,
+            "h_contour": h_boundary,
+        }
+
+        self.set_volume_atlas_to_view(
+            atlas_data, segmentation_data, atlas_info, label_info, boundary
+        )
+        self.set_volume_atlas_3d(
+            unique_label, wax.worker.mesh_data, wax.worker.small_mesh_list
+        )
 
         wax.worker.deleteLater()
         wax.deleteLater()
 
     def download_allen_mice_atlas(self):
         aln = AllenDownloader()
         aln.exec()
@@ -1277,147 +1532,190 @@
             return
 
         atlas_data = np.transpose(aln.worker.atlas_data, [2, 0, 1])[::-1, :, :]
         atlas_info = aln.worker.atlas_info
 
         label_info = aln.worker.label_info
 
-        segmentation_data = np.transpose(aln.worker.segmentation_data, [2, 0, 1])[::-1, :, :]
+        segmentation_data = np.transpose(aln.worker.segmentation_data, [2, 0, 1])[
+            ::-1, :, :
+        ]
         unique_label = aln.worker.unique_label
 
-        s_boundary = np.transpose(aln.worker.boundary['s_contour'], [2, 0, 1])[::-1, :, :]
-        c_boundary = np.transpose(aln.worker.boundary['c_contour'], [2, 0, 1])[::-1, :, :]
-        h_boundary = np.transpose(aln.worker.boundary['h_contour'], [2, 0, 1])[::-1, :, :]
-
-        boundary = {'s_contour': s_boundary, 'c_contour': c_boundary, 'h_contour': h_boundary}
-
-        self.set_volume_atlas_to_view(atlas_data, segmentation_data, atlas_info, label_info, boundary)
-        self.set_volume_atlas_3d(unique_label, aln.worker.mesh_data, aln.worker.small_mesh_list)
+        s_boundary = np.transpose(aln.worker.boundary["s_contour"], [2, 0, 1])[
+            ::-1, :, :
+        ]
+        c_boundary = np.transpose(aln.worker.boundary["c_contour"], [2, 0, 1])[
+            ::-1, :, :
+        ]
+        h_boundary = np.transpose(aln.worker.boundary["h_contour"], [2, 0, 1])[
+            ::-1, :, :
+        ]
+
+        boundary = {
+            "s_contour": s_boundary,
+            "c_contour": c_boundary,
+            "h_contour": h_boundary,
+        }
+
+        self.set_volume_atlas_to_view(
+            atlas_data, segmentation_data, atlas_info, label_info, boundary
+        )
+        self.set_volume_atlas_3d(
+            unique_label, aln.worker.mesh_data, aln.worker.small_mesh_list
+        )
 
         aln.worker.deleteLater()
         aln.deleteLater()
 
     def process_raw_atlas_data(self):
         process_atlas_window = AtlasProcessor()
         process_atlas_window.exec()
 
     def load_atlas_slice(self):
-        msg = 'Load Atlas Slice ... This process will clear the current Atlas layers (if any).'
+        msg = "Load Atlas Slice ... This process will clear the current Atlas layers (if any)."
         self.print_message(msg, self.normal_color)
         file_title = "Select Atlas Slice File"
         file_filter = "JPEG (*.jpg);;PNG (*.png);;Pickle File (*.pkl)"
         if self.atlas_img_path is None:
             file_path = self.home_path
         else:
             file_path = self.atlas_img_path
         file_options = QFileDialog.Options()
         file_options |= QFileDialog.DontUseNativeDialog
         file_dialog = QFileDialog()
         file_dialog.setFileMode(QFileDialog.ExistingFiles)
-        image_file_path = file_dialog.getOpenFileName(self, file_title, file_path, file_filter, options=file_options)
+        image_file_path = file_dialog.getOpenFileName(
+            self, file_title, file_path, file_filter, options=file_options
+        )
 
-        if image_file_path[0] != '':
+        if image_file_path[0] != "":
             self.load_slice_atlas(image_file_path[0])
 
             if self.image_view.image_file is not None:
                 self.show_slice_and_histology()
             else:
                 self.show_only_slice_window()
 
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     def register_slice_info(self):
         if self.atlas_view.slice_image_data is None:
-            msg = 'No Slice Data is loaded.  Please load Slice through <Atlas Menu>.'
+            msg = "No Slice Data is loaded.  Please load Slice through <Atlas Menu>."
             self.print_message(msg, self.error_message_color)
             return
         slice_info = SliceSettingDialog()
         slice_info.exec()
         self.atlas_view.set_slice_info(slice_info)
 
     def crop_slice(self):
         if self.atlas_view.slice_image_data is None:
-            self.print_message('Please load Atlas Slice image.', self.reminder_color)
+            self.print_message("Please load Atlas Slice image.", self.reminder_color)
             return
         if self.atlas_lasso_is_closure:
-            print(self.atlas_view.slice_bregma)
-            cut_rect = cv2.boundingRect(np.asarray(self.working_atlas_data['lasso_path']).astype('int'))
+            # print(self.atlas_view.slice_bregma)
+            cut_rect = cv2.boundingRect(
+                np.asarray(self.working_atlas_data["lasso_path"]).astype("int")
+            )
             if self.atlas_view.slice_bregma:
-                self.atlas_view.slice_bregma[0] = self.atlas_view.slice_bregma[0] - cut_rect[0]
-                self.atlas_view.slice_bregma[1] = self.atlas_view.slice_bregma[1] - cut_rect[1]
-                self.atlas_view.slice_stack.image_dict['bregma_pnt'].setData(
-                    pos=np.array([self.atlas_view.slice_bregma]))
+                self.atlas_view.slice_bregma[0] = (
+                    self.atlas_view.slice_bregma[0] - cut_rect[0]
+                )
+                self.atlas_view.slice_bregma[1] = (
+                    self.atlas_view.slice_bregma[1] - cut_rect[1]
+                )
+                self.atlas_view.slice_stack.image_dict["bregma_pnt"].setData(
+                    pos=np.array([self.atlas_view.slice_bregma])
+                )
 
-            print(self.atlas_view.slice_bregma)
+            # print(self.atlas_view.slice_bregma)
 
             temp = self.atlas_view.slice_image_data.copy()
-            cut_img = temp[cut_rect[1]:(cut_rect[1] + cut_rect[3]), cut_rect[0]:(cut_rect[0] + cut_rect[2])]
+            cut_img = temp[
+                cut_rect[1] : (cut_rect[1] + cut_rect[3]),
+                cut_rect[0] : (cut_rect[0] + cut_rect[2]),
+            ]
             self.atlas_view.processing_slice = cut_img
             self.atlas_view.set_slice_data(self.atlas_view.processing_slice)
             self.reset_tri_points_atlas()
-            res = cv2.resize(self.atlas_view.processing_slice[:, :, :3], self.atlas_view.slice_tb_size,
-                             interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-slice', color=[])
+            res = cv2.resize(
+                self.atlas_view.processing_slice[:, :, :3],
+                self.atlas_view.slice_tb_size,
+                interpolation=cv2.INTER_AREA,
+            )
+            self.layer_ctrl.master_layers(res, layer_type="atlas-slice", color=[])
             self.inactive_slice_window_lasso()
 
     def process_slice(self):
         if self.atlas_view.slice_image_data is None:
-            self.print_message('Please load Atlas Slice image.', self.reminder_color)
+            self.print_message("Please load Atlas Slice image.", self.reminder_color)
             return
         self.inactive_slice_window_lasso()
         self.atlas_view.processing_slice = self.atlas_view.slice_image_data.copy()
-        res = cv2.resize(self.atlas_view.processing_slice[:, :, :3], self.atlas_view.slice_tb_size,
-                         interpolation=cv2.INTER_AREA)
-        self.layer_ctrl.master_layers(res, layer_type='atlas-slice', color=[])
+        res = cv2.resize(
+            self.atlas_view.processing_slice[:, :, :3],
+            self.atlas_view.slice_tb_size,
+            interpolation=cv2.INTER_AREA,
+        )
+        self.layer_ctrl.master_layers(res, layer_type="atlas-slice", color=[])
 
     def pick_bregma(self):
         if self.actionBregma_Picker.isChecked():
             self.set_all_toolbox_btns_unchecked()
             self.current_checked_tool = None
-            self.show_triangle_points('triang')
+            self.show_triangle_points("triang")
             self.vis_eraser_symbol(False)
 
     def save_processed_slice(self):
         if self.atlas_view.slice_image_data is None:
-            self.print_message('No Atlas Slice to save.', self.error_message_color)
+            self.print_message("No Atlas Slice to save.", self.error_message_color)
             return
         if not self.atlas_view.slice_info_ready:
-            self.print_message('No Slice information is given.', self.error_message_color)
-            return
-        path = QFileDialog.getSaveFileName(self, "Save Processed Slice", self.home_path, "Pickle File (*.pkl)")
-        if path[0] != '':
+            self.print_message(
+                "No Slice information is given.", self.error_message_color
+            )
+            return
+        path = QFileDialog.getSaveFileName(
+            self, "Save Processed Slice", self.home_path, "Pickle File (*.pkl)"
+        )
+        if path[0] != "":
             data = self.atlas_view.save_slice_data_and_info()
-            with open(path[0], 'wb') as handle:
+            with open(path[0], "wb") as handle:
                 pickle.dump(data, handle, protocol=pickle.HIGHEST_PROTOCOL)
-            self.print_message('Current Slice is saved successfully.', self.normal_color)
+            self.print_message(
+                "Current Slice is saved successfully.", self.normal_color
+            )
 
     def switch_atlas(self):
-        if self.atlas_view.atlas_data is None or self.atlas_view.slice_image_data is None:
-            msg = 'Atlas can be switched only after both two types of Atlas are loaded.'
+        if (
+            self.atlas_view.atlas_data is None
+            or self.atlas_view.slice_image_data is None
+        ):
+            msg = "Atlas can be switched only after both two types of Atlas are loaded."
             self.print_message(msg, self.error_message_color)
             return
         self.delete_all_atlas_layer()
 
-        if self.current_atlas == 'volume':
+        if self.current_atlas == "volume":
             self.current_atlas_path = self.volume_atlas_path
-            self.actionSwitch_Atlas.setText('Switch Atlas: Slice')
-            self.current_atlas = 'slice'
+            self.actionSwitch_Atlas.setText("Switch Atlas: Slice")
+            self.current_atlas = "slice"
             self.atlascontrolpanel.setEnabled(False)
             self.treeviewpanel.setEnabled(False)
             self.atlas_view.set_slice_data(self.atlas_view.slice_image_data)
             self.reset_tri_points_atlas()
             self.actionBregma_Picker.setEnabled(True)
             self.actionCreate_Slice_Layer.setEnabled(True)
             self.object_ctrl.add_object_btn.setEnabled(False)
             self.object_ctrl.merge_probe_btn.setEnabled(False)
         else:
             self.current_atlas_path = self.slice_atlas_path
-            self.actionSwitch_Atlas.setText('Switch Atlas: Volume')
-            self.current_atlas = 'volume'
+            self.actionSwitch_Atlas.setText("Switch Atlas: Volume")
+            self.current_atlas = "volume"
             self.atlascontrolpanel.setEnabled(True)
             self.treeviewpanel.setEnabled(True)
             self.atlas_view.working_cut_changed(self.atlas_display)
             self.reset_tri_points_atlas()
             self.actionBregma_Picker.setEnabled(False)
             self.actionCreate_Slice_Layer.setEnabled(False)
             self.object_ctrl.add_object_btn.setEnabled(True)
@@ -1425,63 +1723,76 @@
 
     def reset_atlas_slice(self):
         self.atlas_view.slice_stack.set_data(self.atlas_view.slice_image_data)
         self.atlas_view.processing_slice = None
 
     # save triangle points for the atlas
     def save_triangulation_points(self):
-        path = QFileDialog.getSaveFileName(self, "Save Triangulation Points Data",
-                                           self.home_path, "Pickle File (*.pkl)")
-        if path[0] != '':
-            data = {'atlas_corner_points': self.atlas_corner_points,
-                    'atlas_side_lines': self.atlas_side_lines,
-                    'atlas_tri_data': self.atlas_tri_data,
-                    'atlas_tri_inside_data': self.atlas_tri_inside_data,
-                    'atlas_tri_onside_data': self.atlas_tri_onside_data,
-                    'working_atlas_text': self.working_atlas_text,
-                    'atlas_display': self.atlas_display}
-            with open(path[0], 'wb') as handle:
+        path = QFileDialog.getSaveFileName(
+            self,
+            "Save Triangulation Points Data",
+            self.home_path,
+            "Pickle File (*.pkl)",
+        )
+        if path[0] != "":
+            data = {
+                "atlas_corner_points": self.atlas_corner_points,
+                "atlas_side_lines": self.atlas_side_lines,
+                "atlas_tri_data": self.atlas_tri_data,
+                "atlas_tri_inside_data": self.atlas_tri_inside_data,
+                "atlas_tri_onside_data": self.atlas_tri_onside_data,
+                "working_atlas_text": self.working_atlas_text,
+                "atlas_display": self.atlas_display,
+            }
+            with open(path[0], "wb") as handle:
                 pickle.dump(data, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
     # load triangulation points
     def load_triangulation_points(self):
         if self.atlas_view.atlas_data is None:
-            self.print_message('Atlas need to be loaded first.', self.reminder_color)
+            self.print_message("Atlas need to be loaded first.", self.reminder_color)
             return
         filter = "Pickle File (*.pkl)"
         dlg = QFileDialog()
         dlg.setFileMode(QFileDialog.ExistingFiles)
-        pnt_path = dlg.getOpenFileName(self, "Load Triangulation Points", self.home_path, filter)
-        print(pnt_path)
+        pnt_path = dlg.getOpenFileName(
+            self, "Load Triangulation Points", self.home_path, filter
+        )
+        # print(pnt_path)
 
-        if pnt_path[0] != '':
-            infile = open(pnt_path[0], 'rb')
+        if pnt_path[0] != "":
+            infile = open(pnt_path[0], "rb")
             tri_data = pickle.load(infile)
             infile.close()
 
-            if 'atlas_corner_points' not in list(tri_data.keys()):
-                self.print_message('Loaded data is not triangulation points data !!!', self.error_message_color)
+            if "atlas_corner_points" not in list(tri_data.keys()):
+                self.print_message(
+                    "Loaded data is not triangulation points data !!!",
+                    self.error_message_color,
+                )
                 return
 
-            self.atlas_display = tri_data['atlas_display']
-            self.atlas_corner_points = tri_data['atlas_corner_points']
-            self.atlas_side_lines = tri_data['atlas_side_lines']
-            self.atlas_tri_data = tri_data['atlas_tri_data']
-            self.atlas_tri_inside_data = tri_data['atlas_tri_inside_data']
-            self.atlas_tri_onside_data = tri_data['atlas_tri_onside_data']
-            self.working_atlas_text = tri_data['working_atlas_text']
+            self.atlas_display = tri_data["atlas_display"]
+            self.atlas_corner_points = tri_data["atlas_corner_points"]
+            self.atlas_side_lines = tri_data["atlas_side_lines"]
+            self.atlas_tri_data = tri_data["atlas_tri_data"]
+            self.atlas_tri_inside_data = tri_data["atlas_tri_inside_data"]
+            self.atlas_tri_onside_data = tri_data["atlas_tri_onside_data"]
+            self.working_atlas_text = tri_data["working_atlas_text"]
 
-            if tri_data['atlas_display'] == 'coronal':
+            if tri_data["atlas_display"] == "coronal":
                 self.atlas_view.section_rabnt1.setChecked(True)
-            elif tri_data['atlas_display'] == 'sagittal':
+            elif tri_data["atlas_display"] == "sagittal":
                 self.atlas_view.section_rabnt2.setChecked(True)
             else:
                 self.atlas_view.section_rabnt3.setChecked(True)
             if self.atlas_tri_data:
-                self.atlas_view.working_atlas.image_dict['tri_pnts'].setData(self.atlas_tri_data)
+                self.atlas_view.working_atlas.image_dict["tri_pnts"].setData(
+                    self.atlas_tri_data
+                )
                 for i in range(len(self.atlas_tri_data)):
                     self.atlas_view.working_atlas.vb.addItem(self.working_atlas_text[i])
 
     # ------------------------------------------------------------------
     #
     #                      ToolBar layout and connections
     #
@@ -1496,31 +1807,53 @@
         self.tool_box.vis2.triggered.connect(self.show_2_windows)
         self.tool_box.vis3.triggered.connect(self.show_3_windows)
         self.tool_box.vis4.triggered.connect(self.show_4_windows)
         self.tool_box.toh_btn.triggered.connect(self.transfer_to_hist_clicked)
         self.tool_box.toa_btn.triggered.connect(self.transfer_to_atlas_clicked)
         self.tool_box.check_btn.triggered.connect(self.transform_accept)
 
-        self.tool_box.checkable_btn_dict['lasso_btn'].triggered.connect(self.lasso_btn_clicked)
-        self.tool_box.checkable_btn_dict['magic_wand_btn'].triggered.connect(self.magic_wand_btn_clicked)
-        self.tool_box.checkable_btn_dict['pencil_btn'].triggered.connect(self.pencil_btn_clicked)
-        self.tool_box.checkable_btn_dict['eraser_btn'].triggered.connect(self.eraser_btn_clicked)
-        self.tool_box.checkable_btn_dict['probe_btn'].triggered.connect(self.probe_btn_clicked)
-        self.tool_box.checkable_btn_dict['triang_btn'].triggered.connect(self.triang_btn_clicked)
-        self.tool_box.checkable_btn_dict['loc_btn'].triggered.connect(self.loc_btn_clicked)
-        self.tool_box.checkable_btn_dict['ruler_btn'].triggered.connect(self.ruler_btn_clicked)
+        self.tool_box.checkable_btn_dict["lasso_btn"].triggered.connect(
+            self.lasso_btn_clicked
+        )
+        self.tool_box.checkable_btn_dict["magic_wand_btn"].triggered.connect(
+            self.magic_wand_btn_clicked
+        )
+        self.tool_box.checkable_btn_dict["pencil_btn"].triggered.connect(
+            self.pencil_btn_clicked
+        )
+        self.tool_box.checkable_btn_dict["eraser_btn"].triggered.connect(
+            self.eraser_btn_clicked
+        )
+        self.tool_box.checkable_btn_dict["probe_btn"].triggered.connect(
+            self.probe_btn_clicked
+        )
+        self.tool_box.checkable_btn_dict["triang_btn"].triggered.connect(
+            self.triang_btn_clicked
+        )
+        self.tool_box.checkable_btn_dict["loc_btn"].triggered.connect(
+            self.loc_btn_clicked
+        )
+        self.tool_box.checkable_btn_dict["ruler_btn"].triggered.connect(
+            self.ruler_btn_clicked
+        )
         # magic_wand related
-        self.tool_box.magic_color_btn.sigColorChanged.connect(self.change_magic_wand_color)
+        self.tool_box.magic_color_btn.sigColorChanged.connect(
+            self.change_magic_wand_color
+        )
         self.tool_box.magic_wand_virus_register.clicked.connect(self.get_virus_img)
         self.tool_box.magic_wand_bnd_register.clicked.connect(self.get_contour_img)
         self.tool_box.magic_wand_kernel.currentTextChanged.connect(self.kernel_changed)
         self.tool_box.magic_wand_ksize.valueChanged.connect(self.kernel_changed)
         # triangle related
-        self.tool_box.triang_color_btn.sigColorChanged.connect(self.change_triangle_color)
-        self.tool_box.bound_pnts_num.editingFinished.connect(self.number_of_side_points_changed)
+        self.tool_box.triang_color_btn.sigColorChanged.connect(
+            self.change_triangle_color
+        )
+        self.tool_box.bound_pnts_num.editingFinished.connect(
+            self.number_of_side_points_changed
+        )
         self.tool_box.triang_vis_btn.clicked.connect(self.vis_tri_lines_btn_clicked)
         self.tool_box.triang_match_bnd.clicked.connect(self.matching_tri_bnd)
         # cell related
         self.tool_box.cell_color_btn.sigColorChanged.connect(self.change_cell_color)
         self.tool_box.cell_radar_btn.clicked.connect(self.cell_detect_btn_clicked)
         self.tool_box.cell_selector_btn.clicked.connect(self.cell_select_btn_clicked)
         self.tool_box.cell_aim_btn.clicked.connect(self.cell_aim_btn_clicked)
@@ -1528,17 +1861,23 @@
         self.tool_box.pencil_color_btn.sigColorChanged.connect(self.change_pencil_color)
         self.tool_box.pencil_size_valt.textChanged.connect(self.change_pencil_size)
         # ruler related
         self.tool_box.ruler_color_btn.sigColorChanged.connect(self.change_ruler_color)
         self.tool_box.ruler_size_valt.textChanged.connect(self.change_ruler_size)
         # probe_related
         self.tool_box.probe_color_btn.sigColorChanged.connect(self.probe_color_changed)
-        self.tool_box.probe_type_combo.currentIndexChanged.connect(self.probe_type_changed)
-        self.tool_box.pre_site_face_combo.currentIndexChanged.connect(self.site_face_changed)
-        self.tool_box.after_site_face_combo.currentIndexChanged.connect(self.site_face_changed)
+        self.tool_box.probe_type_combo.currentIndexChanged.connect(
+            self.probe_type_changed
+        )
+        self.tool_box.pre_site_face_combo.currentIndexChanged.connect(
+            self.site_face_changed
+        )
+        self.tool_box.after_site_face_combo.currentIndexChanged.connect(
+            self.site_face_changed
+        )
         self.tool_box.linear_silicon_list.clicked.connect(self.set_linear_silicon)
         self.tool_box.multi_prb_btn.clicked.connect(self.multi_shanks_btn_clicked)
         # eraser_related
         self.tool_box.eraser_color_btn.sigColorChanged.connect(self.change_eraser_color)
         # lasso related
         self.tool_box.lasso_color_btn.sigColorChanged.connect(self.lasso_color_changed)
 
@@ -1563,171 +1902,174 @@
         eraser_action = self.toolbar.addWidget(self.tool_box.eraser_wrap)
         lasso_action = self.toolbar.addWidget(self.tool_box.lasso_wrap)
         probe_action = self.toolbar.addWidget(self.tool_box.probe_wrap)
         triang_action = self.toolbar.addWidget(self.tool_box.triang_wrap)
         loc_action = self.toolbar.addWidget(self.tool_box.cell_count_wrap)
         ruler_action = self.toolbar.addWidget(self.tool_box.ruler_wrap)
 
-        self.toolbar_wrap_action_dict['pencil_act'] = pencil_action
-        self.toolbar_wrap_action_dict['eraser_act'] = eraser_action
-        self.toolbar_wrap_action_dict['lasso_act'] = lasso_action
-        self.toolbar_wrap_action_dict['magic_wand_act'] = magic_wand_action
-        self.toolbar_wrap_action_dict['probe_act'] = probe_action
-        self.toolbar_wrap_action_dict['triang_act'] = triang_action
-        self.toolbar_wrap_action_dict['loc_act'] = loc_action
-        self.toolbar_wrap_action_dict['ruler_act'] = ruler_action
+        self.toolbar_wrap_action_dict["pencil_act"] = pencil_action
+        self.toolbar_wrap_action_dict["eraser_act"] = eraser_action
+        self.toolbar_wrap_action_dict["lasso_act"] = lasso_action
+        self.toolbar_wrap_action_dict["magic_wand_act"] = magic_wand_action
+        self.toolbar_wrap_action_dict["probe_act"] = probe_action
+        self.toolbar_wrap_action_dict["triang_act"] = triang_action
+        self.toolbar_wrap_action_dict["loc_act"] = loc_action
+        self.toolbar_wrap_action_dict["ruler_act"] = ruler_action
 
         toolbar_wrap_action_keys = list(self.toolbar_wrap_action_dict.keys())
         for da_key in toolbar_wrap_action_keys:
             self.toolbar_wrap_action_dict[da_key].setVisible(False)
 
-
     # ------------------------------------------------------------------
     #              ToolBar checkable btn clicked
     # ------------------------------------------------------------------
     def ruler_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('ruler')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("ruler")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def lasso_btn_clicked(self):
-        self.set_toolbox_btns_unchecked('lasso')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("lasso")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def magic_wand_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('magic_wand')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("magic_wand")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def pencil_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('pencil')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("pencil")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def eraser_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('eraser')
-        if self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
+        self.set_toolbox_btns_unchecked("eraser")
+        if self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
             self.vis_eraser_symbol(True)
         else:
             self.vis_eraser_symbol(False)
 
     def rotation_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('rotation')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("rotation")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def triang_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('triang')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("triang")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def probe_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('probe')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("probe")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def loc_btn_clicked(self):
         self.inactive_lasso()
         self.inactive_slice_window_lasso()
-        self.set_toolbox_btns_unchecked('loc')
-        self.show_triangle_points('triang')
+        self.set_toolbox_btns_unchecked("loc")
+        self.show_triangle_points("triang")
         self.vis_eraser_symbol(False)
 
     def set_all_toolbox_btns_unchecked(self):
         for da_key in self.tool_box.toolbox_btn_keys:
             self.tool_box.checkable_btn_dict[da_key].setChecked(False)
         for da_key in list(self.toolbar_wrap_action_dict.keys()):
             self.toolbar_wrap_action_dict[da_key].setVisible(False)
 
     def set_toolbox_btns_unchecked(self, current_btn):
         self.actionBregma_Picker.setChecked(False)
-        btn_checked = self.tool_box.checkable_btn_dict['{}_btn'.format(current_btn)].isChecked()
+        btn_checked = self.tool_box.checkable_btn_dict[
+            "{}_btn".format(current_btn)
+        ].isChecked()
         if btn_checked:
             self.current_checked_tool = current_btn
             for da_key in self.tool_box.toolbox_btn_keys:
                 if current_btn in da_key:
                     continue
                 else:
                     self.tool_box.checkable_btn_dict[da_key].setChecked(False)
             for da_key in list(self.toolbar_wrap_action_dict.keys()):
                 if current_btn in da_key:
                     self.toolbar_wrap_action_dict[da_key].setVisible(True)
                 else:
                     self.toolbar_wrap_action_dict[da_key].setVisible(False)
         else:
             self.current_checked_tool = None
-            self.toolbar_wrap_action_dict['{}_act'.format(current_btn)].setVisible(False)
+            self.toolbar_wrap_action_dict["{}_act".format(current_btn)].setVisible(
+                False
+            )
 
     def vis_eraser_symbol(self, vis):
-        self.image_view.img_stacks.image_dict['circle_follow'].setVisible(vis)
-        self.atlas_view.slice_stack.image_dict['circle_follow'].setVisible(vis)
+        self.image_view.img_stacks.image_dict["circle_follow"].setVisible(vis)
+        self.atlas_view.slice_stack.image_dict["circle_follow"].setVisible(vis)
 
     # ------------------------------------------------------------------
     #
     #                      SideBar layout and connections
     #
     # ------------------------------------------------------------------
     def init_side_bar(self):
-        decor_label_style = read_qss_file('qss/decor_label.qss')
-        tab_style = read_qss_file('qss/tabs.qss')
+        decor_label_style = read_qss_file("qss/decor_label.qss")
+        tab_style = read_qss_file("qss/tabs.qss")
         self.sidebar.setStyleSheet(tab_style)
         self.sidebar.setIconSize(QSize(24, 24))
-        self.sidebar.setTabIcon(0, QIcon('icons/sidebar/atlascontrol.svg'))
-        self.sidebar.setTabIcon(1, QIcon('icons/sidebar/treeview.svg'))
-        self.sidebar.setTabIcon(2, QIcon('icons/sidebar/tool.svg'))
-        self.sidebar.setTabIcon(3, QIcon('icons/sidebar/layers.svg'))
-        self.sidebar.setTabIcon(4, QIcon('icons/sidebar/object.svg'))
+        self.sidebar.setTabIcon(0, QIcon("icons/sidebar/atlascontrol.svg"))
+        self.sidebar.setTabIcon(1, QIcon("icons/sidebar/treeview.svg"))
+        self.sidebar.setTabIcon(2, QIcon("icons/sidebar/tool.svg"))
+        self.sidebar.setTabIcon(3, QIcon("icons/sidebar/layers.svg"))
+        self.sidebar.setTabIcon(4, QIcon("icons/sidebar/object.svg"))
 
         # ---------------------------- atlas control panel
         atlas_panel_layout = QVBoxLayout(self.atlascontrolpanel)
         atlas_panel_layout.setContentsMargins(0, 0, 0, 0)
         atlas_panel_layout.setAlignment(Qt.AlignTop)
-        atlas_control_label = QLabel('Atlasing Controller')
+        atlas_control_label = QLabel("Atlasing Controller")
         atlas_control_label.setStyleSheet(decor_label_style)
 
         atlas_panel_layout.addWidget(atlas_control_label)
         atlas_panel_layout.addWidget(self.atlas_view.sidebar_wrap)
 
         # ---------------------------- Label Panel
         label_panel_layout = QVBoxLayout(self.treeviewpanel)
         label_panel_layout.setContentsMargins(0, 0, 0, 0)
         label_panel_layout.setAlignment(Qt.AlignTop)
-        label_control_label = QLabel('Segmentation View Controller')
+        label_control_label = QLabel("Segmentation View Controller")
         label_control_label.setStyleSheet(decor_label_style)
 
         label_tree_container = QFrame()
         label_container_layout = QVBoxLayout(label_tree_container)
         # label_container_layout.setContentsMargins(0, 0, 0, 0)
         label_container_layout.setSpacing(0)
         label_container_layout.setAlignment(Qt.AlignTop)
         show_3d_button = QPushButton()
         # show_3d_button.setStyleSheet(sidebar_button_style)
         show_3d_button.setCheckable(True)
-        show_3d_button.setText('Show in 3D view')
+        show_3d_button.setText("Show in 3D view")
         show_3d_button.clicked.connect(self.show_small_area_in_3d)
 
-        composition_label = QLabel('Composition: ')
+        composition_label = QLabel("Composition: ")
         self.composition_combo = QComboBox()
         self.composition_combo.setFixedHeight(22)
-        self.composition_combo.addItems(['opaque', 'translucent', 'additive'])
+        self.composition_combo.addItems(["opaque", "translucent", "additive"])
         self.composition_combo.currentIndexChanged.connect(self.composition_3d_changed)
 
         label_container_layout.addWidget(show_3d_button)
         label_container_layout.addSpacing(10)
         label_container_layout.addWidget(self.composition_combo)
         label_container_layout.addSpacing(10)
         label_container_layout.addWidget(self.atlas_view.label_tree)
@@ -1736,15 +2078,15 @@
         label_panel_layout.addWidget(label_tree_container)
 
         # ---------------------------- image panel
         image_panel_layout = QVBoxLayout(self.imagecontrolpanel)
         image_panel_layout.setContentsMargins(0, 0, 0, 0)
         image_panel_layout.setSpacing(0)
         image_panel_layout.setAlignment(Qt.AlignTop)
-        image_control_label = QLabel('Image View Controller')
+        image_control_label = QLabel("Image View Controller")
         image_control_label.setStyleSheet(decor_label_style)
 
         image_panel_layout.addWidget(image_control_label)
 
         space_item = QSpacerItem(300, 10, QSizePolicy.Expanding)
 
         image_container = QFrame()
@@ -1759,19 +2101,19 @@
         image_panel_layout.insertStretch(-1, 1)
 
         # ---------------------------- layer panel
         layer_panel_layout = QVBoxLayout(self.layerpanel)
         layer_panel_layout.setContentsMargins(0, 0, 0, 0)
         layer_panel_layout.setSpacing(0)
         layer_panel_layout.setAlignment(Qt.AlignTop)
-        layer_control_label = QLabel('Layer View Controller')
+        layer_control_label = QLabel("Layer View Controller")
         layer_control_label.setStyleSheet(decor_label_style)
 
         layer_btm_ctrl = QFrame()
-        layer_btm_ctrl.setStyleSheet('background-color:rgb(65, 65, 65);')
+        layer_btm_ctrl.setStyleSheet("background-color:rgb(65, 65, 65);")
         layer_btm_ctrl.setFixedHeight(24)
         layer_btm_layout = QHBoxLayout(layer_btm_ctrl)
         layer_btm_layout.setContentsMargins(0, 0, 0, 0)
         layer_btm_layout.setSpacing(5)
         layer_btm_layout.setAlignment(Qt.AlignRight)
         layer_btm_layout.addWidget(self.layer_ctrl.add_layer_btn)
         layer_btm_layout.addWidget(self.layer_ctrl.delete_layer_btn)
@@ -1782,19 +2124,19 @@
         # self.layerpanel.setEnabled(False)
 
         # ---------------------------- object panel
         object_panel_layout = QVBoxLayout(self.probecontrolpanel)
         object_panel_layout.setContentsMargins(0, 0, 0, 0)
         object_panel_layout.setSpacing(0)
         object_panel_layout.setAlignment(Qt.AlignTop)
-        object_control_label = QLabel('Object View Controller')
+        object_control_label = QLabel("Object View Controller")
         object_control_label.setStyleSheet(decor_label_style)
 
         object_btm_ctrl = QFrame()
-        object_btm_ctrl.setStyleSheet('background-color:rgb(65, 65, 65);')
+        object_btm_ctrl.setStyleSheet("background-color:rgb(65, 65, 65);")
         object_btm_ctrl.setFixedHeight(24)
         object_btm_layout = QHBoxLayout(object_btm_ctrl)
         object_btm_layout.setContentsMargins(0, 0, 0, 0)
         object_btm_layout.setSpacing(5)
         object_btm_layout.setAlignment(Qt.AlignRight)
 
         # object_btm_layout.addSpacing(10)
@@ -1819,162 +2161,226 @@
     #
     #               ToolBar ruler btn related
     #
     # ------------------------------------------------------------------
     def change_ruler_color(self, ev):
         color = np.ravel(ev.color().getRgb())
         width = self.tool_box.ruler_width_slider.value()
-        self.image_view.img_stacks.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.cimg.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.himg.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.simg.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.slice_stack.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.image_view.img_stacks.image_dict['ruler_path'].setSymbolPen(color=color)
-        self.atlas_view.cimg.image_dict['ruler_path'].setSymbolPen(color=color)
-        self.atlas_view.himg.image_dict['ruler_path'].setSymbolPen(color=color)
-        self.atlas_view.simg.image_dict['ruler_path'].setSymbolPen(color=color)
-        self.atlas_view.slice_stack.image_dict['ruler_path'].setSymbolPen(color=color)
-        self.image_view.img_stacks.image_dict['ruler_path'].setSymbolBrush(color=color)
-        self.atlas_view.cimg.image_dict['ruler_path'].setSymbolBrush(color=color)
-        self.atlas_view.himg.image_dict['ruler_path'].setSymbolBrush(color=color)
-        self.atlas_view.simg.image_dict['ruler_path'].setSymbolBrush(color=color)
-        self.atlas_view.slice_stack.image_dict['ruler_path'].setSymbolBrush(color=color)
+        self.image_view.img_stacks.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.cimg.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.himg.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.simg.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.slice_stack.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.image_view.img_stacks.image_dict["ruler_path"].setSymbolPen(color=color)
+        self.atlas_view.cimg.image_dict["ruler_path"].setSymbolPen(color=color)
+        self.atlas_view.himg.image_dict["ruler_path"].setSymbolPen(color=color)
+        self.atlas_view.simg.image_dict["ruler_path"].setSymbolPen(color=color)
+        self.atlas_view.slice_stack.image_dict["ruler_path"].setSymbolPen(color=color)
+        self.image_view.img_stacks.image_dict["ruler_path"].setSymbolBrush(color=color)
+        self.atlas_view.cimg.image_dict["ruler_path"].setSymbolBrush(color=color)
+        self.atlas_view.himg.image_dict["ruler_path"].setSymbolBrush(color=color)
+        self.atlas_view.simg.image_dict["ruler_path"].setSymbolBrush(color=color)
+        self.atlas_view.slice_stack.image_dict["ruler_path"].setSymbolBrush(color=color)
 
     def change_ruler_size(self):
         width = int(self.tool_box.ruler_size_valt.text())
         self.tool_box.ruler_width_slider.setValue(width)
         color = np.ravel(self.tool_box.ruler_color_btn.color().getRgb())
-        self.image_view.img_stacks.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.cimg.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.himg.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.simg.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.atlas_view.slice_stack.image_dict['ruler_path'].setPen(pg.mkPen(color, width=width, style=Qt.DashLine))
-        self.image_view.img_stacks.image_dict['ruler_path'].setSymbolSize(width)
-        self.atlas_view.cimg.image_dict['ruler_path'].setSymbolSize(width)
-        self.atlas_view.himg.image_dict['ruler_path'].setSymbolSize(width)
-        self.atlas_view.simg.image_dict['ruler_path'].setSymbolSize(width)
-        self.atlas_view.slice_stack.image_dict['ruler_path'].setSymbolSize(width)
+        self.image_view.img_stacks.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.cimg.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.himg.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.simg.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.atlas_view.slice_stack.image_dict["ruler_path"].setPen(
+            pg.mkPen(color, width=width, style=Qt.DashLine)
+        )
+        self.image_view.img_stacks.image_dict["ruler_path"].setSymbolSize(width)
+        self.atlas_view.cimg.image_dict["ruler_path"].setSymbolSize(width)
+        self.atlas_view.himg.image_dict["ruler_path"].setSymbolSize(width)
+        self.atlas_view.simg.image_dict["ruler_path"].setSymbolSize(width)
+        self.atlas_view.slice_stack.image_dict["ruler_path"].setSymbolSize(width)
 
     def inactive_atlas_ruler(self):
-        self.atlas_view.working_atlas.image_dict['ruler_path'].clear()
-        self.atlas_view.working_atlas.image_dict['ruler_path'].updateItems()
-        self.working_atlas_data['ruler_path'] = []
+        self.atlas_view.working_atlas.image_dict["ruler_path"].clear()
+        self.atlas_view.working_atlas.image_dict["ruler_path"].updateItems()
+        self.working_atlas_data["ruler_path"] = []
 
     def atlas_ruler_points_clicked(self, points, ev):
         clicked_ind = ev[0].index()
         pos = ev[0].pos()
-        if clicked_ind != 0 and len(self.working_atlas_data['ruler_path']) == 1:
-            self.working_atlas_data['ruler_path'].append([pos.x(), pos.y()])
-            self.atlas_view.working_atlas.image_dict['ruler_path'].setData(
-                np.asarray(self.working_atlas_data['ruler_path']))
+        if clicked_ind != 0 and len(self.working_atlas_data["ruler_path"]) == 1:
+            self.working_atlas_data["ruler_path"].append([pos.x(), pos.y()])
+            self.atlas_view.working_atlas.image_dict["ruler_path"].setData(
+                np.asarray(self.working_atlas_data["ruler_path"])
+            )
             self.set_ruler_length()
         else:
             self.inactive_atlas_ruler()
 
     def set_ruler_length(self):
-        if len(self.working_atlas_data['ruler_path']) == 2:
-            data = np.asarray(self.working_atlas_data['ruler_path'])
-            if self.current_atlas == 'volume':
+        if len(self.working_atlas_data["ruler_path"]) == 2:
+            data = np.asarray(self.working_atlas_data["ruler_path"])
+            if self.current_atlas == "volume":
                 dist = np.sqrt(np.sum((data[0] - data[1]) ** 2))
-                self.tool_box.ruler_length_label.setText('Length: {} um'.format(
-                    round(dist * self.atlas_view.vox_size_um, 2)))
+                self.tool_box.ruler_length_label.setText(
+                    "Length: {} um".format(round(dist * self.atlas_view.vox_size_um, 2))
+                )
             else:
                 if not self.atlas_view.slice_info_ready:
                     dist = np.sqrt(np.sum((data[0] - data[1]) ** 2))
-                    self.tool_box.ruler_length_label.setText('Length: {} px'.format(int(dist)))
+                    self.tool_box.ruler_length_label.setText(
+                        "Length: {} px".format(int(dist))
+                    )
                 else:
                     xv, yv, zv = self.atlas_view.get_slice_coords(data)
-                    dist = np.sqrt((xv[0] - xv[1]) ** 2 + (yv[0] - yv[1]) ** 2 + (zv[0] - zv[1]) ** 2)
-                    self.tool_box.ruler_length_label.setText('Length: {} um'.format(round(dist, 2)))
+                    dist = np.sqrt(
+                        (xv[0] - xv[1]) ** 2
+                        + (yv[0] - yv[1]) ** 2
+                        + (zv[0] - zv[1]) ** 2
+                    )
+                    self.tool_box.ruler_length_label.setText(
+                        "Length: {} um".format(round(dist, 2))
+                    )
 
     def inactive_img_ruler(self):
-        self.image_view.img_stacks.image_dict['ruler_path'].clear()
-        self.image_view.img_stacks.image_dict['ruler_path'].updateItems()
-        self.working_img_data['ruler_path'] = []
+        self.image_view.img_stacks.image_dict["ruler_path"].clear()
+        self.image_view.img_stacks.image_dict["ruler_path"].updateItems()
+        self.working_img_data["ruler_path"] = []
 
     def img_ruler_points_clicked(self, points, ev):
         clicked_ind = ev[0].index()
         pos = ev[0].pos()
-        if clicked_ind != 0 and len(self.working_img_data['ruler_path']) == 1:
-            self.working_img_data['ruler_path'].append([pos.x(), pos.y()])
-            self.image_view.img_stacks.image_dict['ruler_path'].setData(
-                np.asarray(self.working_img_data['ruler_path']))
+        if clicked_ind != 0 and len(self.working_img_data["ruler_path"]) == 1:
+            self.working_img_data["ruler_path"].append([pos.x(), pos.y()])
+            self.image_view.img_stacks.image_dict["ruler_path"].setData(
+                np.asarray(self.working_img_data["ruler_path"])
+            )
             self.set_img_ruler_length()
         else:
             self.inactive_img_ruler()
 
     def set_img_ruler_length(self):
-        if len(self.working_img_data['ruler_path']) == 2:
-            data = np.asarray(self.working_img_data['ruler_path'])
+        if len(self.working_img_data["ruler_path"]) == 2:
+            data = np.asarray(self.working_img_data["ruler_path"])
             dist = np.sqrt(np.sum((data[0] - data[1]) ** 2))
             if self.image_view.image_file.scaling_val is None:
-                self.tool_box.ruler_length_label.setText('Length: {} px'.format(int(dist)))
-            else:
-                self.tool_box.ruler_length_label.setText('Length: {} um'.format(
-                    round(dist * self.image_view.image_file.scaling_val / self.image_view.current_scale, 2)))
+                self.tool_box.ruler_length_label.setText(
+                    "Length: {} px".format(int(dist))
+                )
+            else:
+                self.tool_box.ruler_length_label.setText(
+                    "Length: {} um".format(
+                        round(
+                            dist
+                            * self.image_view.image_file.scaling_val
+                            / self.image_view.current_scale,
+                            2,
+                        )
+                    )
+                )
 
     # ------------------------------------------------------------------
     #
     #               ToolBar lasso btn related
     #
     # ------------------------------------------------------------------
     def lasso_color_changed(self, ev):
         lasso_color = np.ravel(ev.color().getRgb())
-        self.lasso_color = (int(lasso_color[0]), int(lasso_color[1]), int(lasso_color[2]))
+        self.lasso_color = (
+            int(lasso_color[0]),
+            int(lasso_color[1]),
+            int(lasso_color[2]),
+        )
         if self.img_lasso_is_closure:
-            self.image_view.img_stacks.image_dict['lasso_path'].setPen(
-                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine))
-        else:
-            self.image_view.img_stacks.image_dict['lasso_path'].setPen(
-                pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine))
-        self.image_view.img_stacks.image_dict['lasso_path'].setSymbolPen(color=self.lasso_color)
+            self.image_view.img_stacks.image_dict["lasso_path"].setPen(
+                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine)
+            )
+        else:
+            self.image_view.img_stacks.image_dict["lasso_path"].setPen(
+                pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine)
+            )
+        self.image_view.img_stacks.image_dict["lasso_path"].setSymbolPen(
+            color=self.lasso_color
+        )
         if self.atlas_lasso_is_closure:
-            self.atlas_view.slice_stack.image_dict['lasso_path'].setPen(
-                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine))
-        else:
-            self.atlas_view.slice_stack.image_dict['lasso_path'].setPen(
-                pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine))
-        self.atlas_view.working_atlas.image_dict['lasso_path'].setSymbolPen(color=self.lasso_color)
+            self.atlas_view.slice_stack.image_dict["lasso_path"].setPen(
+                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine)
+            )
+        else:
+            self.atlas_view.slice_stack.image_dict["lasso_path"].setPen(
+                pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine)
+            )
+        self.atlas_view.working_atlas.image_dict["lasso_path"].setSymbolPen(
+            color=self.lasso_color
+        )
 
     def inactive_lasso(self):
-        self.working_img_data['lasso_path'] = []
-        self.image_view.img_stacks.image_dict['lasso_path'].clear()
-        self.image_view.img_stacks.image_dict['lasso_path'].updateItems()
-        self.image_view.img_stacks.image_dict['lasso_path'].setPen(
-            pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine))
+        self.working_img_data["lasso_path"] = []
+        self.image_view.img_stacks.image_dict["lasso_path"].clear()
+        self.image_view.img_stacks.image_dict["lasso_path"].updateItems()
+        self.image_view.img_stacks.image_dict["lasso_path"].setPen(
+            pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine)
+        )
         self.img_lasso_is_closure = False
 
     def lasso_points_clicked(self, points, ev):
         clicked_ind = ev[0].index()
-        if clicked_ind == 0 and len(self.working_img_data['lasso_path']) >= 3:
-            self.working_img_data['lasso_path'].append(self.working_img_data['lasso_path'][0])
-            self.image_view.img_stacks.image_dict['lasso_path'].setData(np.asarray(self.working_img_data['lasso_path']))
+        if clicked_ind == 0 and len(self.working_img_data["lasso_path"]) >= 3:
+            self.working_img_data["lasso_path"].append(
+                self.working_img_data["lasso_path"][0]
+            )
+            self.image_view.img_stacks.image_dict["lasso_path"].setData(
+                np.asarray(self.working_img_data["lasso_path"])
+            )
             self.img_lasso_is_closure = True
-            self.image_view.img_stacks.image_dict['lasso_path'].setPen(
-                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine))
+            self.image_view.img_stacks.image_dict["lasso_path"].setPen(
+                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine)
+            )
         else:
             self.inactive_lasso()
 
     def inactive_slice_window_lasso(self):
-        self.working_atlas_data['lasso_path'] = []
-        self.atlas_view.slice_stack.image_dict['lasso_path'].clear()
-        self.atlas_view.slice_stack.image_dict['lasso_path'].updateItems()
-        self.atlas_view.slice_stack.image_dict['lasso_path'].setPen(
-            pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine))
+        self.working_atlas_data["lasso_path"] = []
+        self.atlas_view.slice_stack.image_dict["lasso_path"].clear()
+        self.atlas_view.slice_stack.image_dict["lasso_path"].updateItems()
+        self.atlas_view.slice_stack.image_dict["lasso_path"].setPen(
+            pg.mkPen(color=self.lasso_color, width=3, style=Qt.DashLine)
+        )
         self.atlas_lasso_is_closure = False
 
     def slice_window_lasso_points_clicked(self, points, ev):
         clicked_ind = ev[0].index()
-        if clicked_ind == 0 and len(self.working_atlas_data['lasso_path']) >= 3:
-            self.working_atlas_data['lasso_path'].append(self.working_atlas_data['lasso_path'][0])
-            self.atlas_view.slice_stack.image_dict['lasso_path'].setData(
-                np.asarray(self.working_atlas_data['lasso_path']))
+        if clicked_ind == 0 and len(self.working_atlas_data["lasso_path"]) >= 3:
+            self.working_atlas_data["lasso_path"].append(
+                self.working_atlas_data["lasso_path"][0]
+            )
+            self.atlas_view.slice_stack.image_dict["lasso_path"].setData(
+                np.asarray(self.working_atlas_data["lasso_path"])
+            )
             self.atlas_lasso_is_closure = True
-            self.atlas_view.slice_stack.image_dict['lasso_path'].setPen(
-                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine))
+            self.atlas_view.slice_stack.image_dict["lasso_path"].setPen(
+                pg.mkPen(color=self.lasso_color, width=3, style=Qt.SolidLine)
+            )
         else:
             self.inactive_slice_window_lasso()
 
     # ------------------------------------------------------------------
     #
     #               ToolBar probe btn related
     #
@@ -1987,27 +2393,30 @@
                 site_face = self.tool_box.pre_site_face_combo.currentIndex()
                 if self.site_face in [0, 1]:
                     x_vals = np.ravel(self.probe_settings.multi_shanks)
                     y_vals = np.zeros(n_shanks)
                 else:
                     y_vals = np.ravel(self.probe_settings.multi_shanks)
                     x_vals = np.zeros(n_shanks)
-                multi_settings = {'x_vals': x_vals,
-                                  'y_vals': y_vals,
-                                  'faces': [site_face for _ in range(len(self.probe_settings.multi_shanks))]}
+                multi_settings = {
+                    "x_vals": x_vals,
+                    "y_vals": y_vals,
+                    "faces": [
+                        site_face for _ in range(len(self.probe_settings.multi_shanks))
+                    ],
+                }
                 self.multi_settings.set_multi_probes(multi_settings)
                 self.valid_multi_settings = True
         else:
             self.multi_shanks = False
 
-
     def check_n_trajectory(self):
         if self.image_view.image_file is None:
             if self.probe_settings.probe_type == 1:
-                if self.atlas_display in ['coronal', 'horizontal']:
+                if self.atlas_display in ["coronal", "horizontal"]:
                     if self.site_face in [0, 1]:
                         self.n_pre_trajectory = 4
                     else:
                         self.n_pre_trajectory = 1
                 else:
                     if self.site_face in [2, 3]:
                         self.n_pre_trajectory = 4
@@ -2039,78 +2448,104 @@
                 self.tool_box.linear_silicon_list.setVisible(False)
             self.probe_settings.set_tetrode()
             self.valid_probe_settings = True
 
         self.probe_type = index
         self.atlas_view.pre_trajectory_changed()
         # self.check_n_trajectory()
-        self.atlas_view.working_atlas.image_dict['atlas-probe'].clear()
-        self.working_atlas_data['atlas-probe'].clear()
+        self.atlas_view.working_atlas.image_dict["atlas-probe"].clear()
+        self.working_atlas_data["atlas-probe"].clear()
         self.multi_shanks_btn_clicked()
 
     def set_linear_silicon(self):
         temp_settings = self.probe_settings.get_settings()
-        if temp_settings['probe_length'] is None:
+        if temp_settings["probe_length"] is None:
             temp_settings = None
         ls_probe_info = LinearSiliconInfoDialog(temp_settings)
         rsp = ls_probe_info.exec_()
         if rsp == QDialog.Accepted:
             self.probe_settings.set_linear_silicon(ls_probe_info.probe_settings)
             if self.probe_settings.probe_length == 0:
                 self.valid_probe_settings = False
-                self.print_message('Linear Silicon Probe can not be length 0 um.', self.error_message_color)
+                self.print_message(
+                    "Linear Silicon Probe can not be length 0 um.",
+                    self.error_message_color,
+                )
                 return
             if self.probe_settings.tip_length == 0:
-                self.print_message('Linear Silicon Probe has tip length 0 um. Is that correct?', self.reminder_color)
+                self.print_message(
+                    "Linear Silicon Probe has tip length 0 um. Is that correct?",
+                    self.reminder_color,
+                )
                 return
             if self.probe_settings.site_height == 0:
                 self.valid_probe_settings = False
-                self.print_message('Site height can not be 0 um.', self.error_message_color)
+                self.print_message(
+                    "Site height can not be 0 um.", self.error_message_color
+                )
                 return
             if self.probe_settings.site_width == 0:
                 self.valid_probe_settings = False
-                self.print_message('Site width can not be 0 um.', self.error_message_color)
+                self.print_message(
+                    "Site width can not be 0 um.", self.error_message_color
+                )
                 return
-            if self.probe_settings.site_height * self.probe_settings.sites_distance[0] > self.probe_settings.probe_length:
+            if (
+                self.probe_settings.site_height * self.probe_settings.sites_distance[0]
+                > self.probe_settings.probe_length
+            ):
                 self.valid_probe_settings = False
-                self.print_message('Total sites length can not be larger than probe length', self.error_message_color)
+                self.print_message(
+                    "Total sites length can not be larger than probe length",
+                    self.error_message_color,
+                )
                 return
 
     def site_face_changed(self, site_index):
         self.site_face = site_index
         if self.tool_box.pre_site_face_combo.isVisible():
             site_face_text = self.tool_box.pre_site_face_combo.currentText()
         else:
             site_face_text = self.tool_box.after_site_face_combo.currentText()
         self.probe_settings.probe_faces_changed(site_face_text)
         # self.check_n_trajectory()
         self.atlas_view.pre_trajectory_changed()
-        self.atlas_view.working_atlas.image_dict['atlas-probe'].clear()
+        self.atlas_view.working_atlas.image_dict["atlas-probe"].clear()
         self.multi_shanks_btn_clicked()
 
     def probe_color_changed(self, ev):
         probe_color = np.ravel(ev.color().getRgb())
-        self.probe_color = (int(probe_color[0]), int(probe_color[1]), int(probe_color[2]))
-        self.image_view.img_stacks.image_dict['img-probe'].setPen(color=self.probe_color)
-        self.atlas_view.cimg.image_dict['atlas-probe'].setPen(color=self.probe_color)
-        self.atlas_view.himg.image_dict['atlas-probe'].setPen(color=self.probe_color)
-        self.atlas_view.simg.image_dict['atlas-probe'].setPen(color=self.probe_color)
-        self.atlas_view.slice_stack.image_dict['atlas-probe'].setPen(color=self.probe_color)
-        self.image_view.img_stacks.image_dict['img-probe'].setBrush(color=self.probe_color)
-        self.atlas_view.cimg.image_dict['atlas-probe'].setBrush(color=self.probe_color)
-        self.atlas_view.himg.image_dict['atlas-probe'].setBrush(color=self.probe_color)
-        self.atlas_view.simg.image_dict['atlas-probe'].setBrush(color=self.probe_color)
-        self.atlas_view.slice_stack.image_dict['atlas-probe'].setBrush(color=self.probe_color)
+        self.probe_color = (
+            int(probe_color[0]),
+            int(probe_color[1]),
+            int(probe_color[2]),
+        )
+        self.image_view.img_stacks.image_dict["img-probe"].setPen(
+            color=self.probe_color
+        )
+        self.atlas_view.cimg.image_dict["atlas-probe"].setPen(color=self.probe_color)
+        self.atlas_view.himg.image_dict["atlas-probe"].setPen(color=self.probe_color)
+        self.atlas_view.simg.image_dict["atlas-probe"].setPen(color=self.probe_color)
+        self.atlas_view.slice_stack.image_dict["atlas-probe"].setPen(
+            color=self.probe_color
+        )
+        self.image_view.img_stacks.image_dict["img-probe"].setBrush(
+            color=self.probe_color
+        )
+        self.atlas_view.cimg.image_dict["atlas-probe"].setBrush(color=self.probe_color)
+        self.atlas_view.himg.image_dict["atlas-probe"].setBrush(color=self.probe_color)
+        self.atlas_view.simg.image_dict["atlas-probe"].setBrush(color=self.probe_color)
+        self.atlas_view.slice_stack.image_dict["atlas-probe"].setBrush(
+            color=self.probe_color
+        )
 
         self.atlas_view.cimg.pre_trajectory_color_changed(self.probe_color, 2)
         self.atlas_view.simg.pre_trajectory_color_changed(self.probe_color, 2)
         self.atlas_view.himg.pre_trajectory_color_changed(self.probe_color, 2)
 
-
-
     # ------------------------------------------------------------------
     #
     #               ToolBar moving btn related
     #
     # ------------------------------------------------------------------
     # def moving_left_btn_clicked(self):
     #     if not self.layer_ctrl.current_layer_id:
@@ -2136,156 +2571,203 @@
     #
     #               ToolBar pencil btn related
     #
     # ------------------------------------------------------------------
     def change_pencil_color(self, ev):
         pencil_color = ev.color()
         self.pencil_color = np.ravel(pencil_color.getRgb())
-        self.image_view.img_stacks.image_dict['img-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        self.atlas_view.cimg.image_dict['atlas-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        self.atlas_view.simg.image_dict['atlas-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        self.atlas_view.himg.image_dict['atlas-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        self.atlas_view.slice_stack.image_dict['atlas-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        if self.working_img_data['img-drawing'] and self.tool_box.is_closed:
-            self.image_view.img_stacks.image_dict['img-drawing'].setFillBrush(color=self.pencil_color)
-        if self.working_atlas_data['atlas-drawing'] and self.tool_box.is_closed:
-            self.atlas_view.working_atlas.image_dict['img-drawing'].setFillBrush(color=self.pencil_color)
+        self.image_view.img_stacks.image_dict["img-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        self.atlas_view.cimg.image_dict["atlas-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        self.atlas_view.simg.image_dict["atlas-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        self.atlas_view.himg.image_dict["atlas-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        self.atlas_view.slice_stack.image_dict["atlas-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        if self.working_img_data["img-drawing"] and self.tool_box.is_closed:
+            self.image_view.img_stacks.image_dict["img-drawing"].setFillBrush(
+                color=self.pencil_color
+            )
+        if self.working_atlas_data["atlas-drawing"] and self.tool_box.is_closed:
+            self.atlas_view.working_atlas.image_dict["img-drawing"].setFillBrush(
+                color=self.pencil_color
+            )
 
     def set_img_pencil_closed_style(self):
-        if not self.working_img_data['img-drawing']:
+        if not self.working_img_data["img-drawing"]:
             return
-        mid_line = np.mean(np.asarray(self.working_img_data['img-drawing'])[:, 1])
-        self.image_view.img_stacks.image_dict['img-drawing'].setFillLevel(level=mid_line)
-        self.image_view.img_stacks.image_dict['img-drawing'].setFillBrush(color=self.pencil_color)
+        mid_line = np.mean(np.asarray(self.working_img_data["img-drawing"])[:, 1])
+        self.image_view.img_stacks.image_dict["img-drawing"].setFillLevel(
+            level=mid_line
+        )
+        self.image_view.img_stacks.image_dict["img-drawing"].setFillBrush(
+            color=self.pencil_color
+        )
 
     def clear_img_pencil_closed_style(self):
-        self.image_view.img_stacks.image_dict['img-drawing'].setFillLevel(None)
-        self.image_view.img_stacks.image_dict['img-drawing'].setFillBrush(None)
+        self.image_view.img_stacks.image_dict["img-drawing"].setFillLevel(None)
+        self.image_view.img_stacks.image_dict["img-drawing"].setFillBrush(None)
 
     def set_atlas_pencil_closed_style(self):
-        if not self.working_atlas_data['atlas-drawing']:
+        if not self.working_atlas_data["atlas-drawing"]:
             return
-        mid_line = np.mean(np.asarray(self.working_atlas_data['atlas-drawing'])[:, 1])
-        self.atlas_view.working_atlas.image_dict['atlas-drawing'].setFillLevel(level=mid_line)
-        self.atlas_view.working_atlas.image_dict['atlas-drawing'].setFillBrush(color=self.pencil_color)
+        mid_line = np.mean(np.asarray(self.working_atlas_data["atlas-drawing"])[:, 1])
+        self.atlas_view.working_atlas.image_dict["atlas-drawing"].setFillLevel(
+            level=mid_line
+        )
+        self.atlas_view.working_atlas.image_dict["atlas-drawing"].setFillBrush(
+            color=self.pencil_color
+        )
 
     def clear_atlas_pencil_closed_style(self):
-        self.atlas_view.working_atlas.image_dict['atlas-drawing'].setFillLevel(None)
-        self.atlas_view.working_atlas.image_dict['atlas-drawing'].setFillBrush(None)
+        self.atlas_view.working_atlas.image_dict["atlas-drawing"].setFillLevel(None)
+        self.atlas_view.working_atlas.image_dict["atlas-drawing"].setFillBrush(None)
 
     def change_pencil_size(self):
         val = int(self.tool_box.pencil_size_valt.text())
         self.pencil_size = val
         self.tool_box.pencil_size_slider.setValue(val)
-        self.image_view.img_stacks.image_dict['img-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        self.atlas_view.cimg.image_dict['atlas-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        self.atlas_view.simg.image_dict['atlas-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
-        self.atlas_view.himg.image_dict['atlas-drawing'].setPen(
-            pg.mkPen(color=self.pencil_color, width=self.pencil_size))
+        self.image_view.img_stacks.image_dict["img-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        self.atlas_view.cimg.image_dict["atlas-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        self.atlas_view.simg.image_dict["atlas-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
+        self.atlas_view.himg.image_dict["atlas-drawing"].setPen(
+            pg.mkPen(color=self.pencil_color, width=self.pencil_size)
+        )
 
     def inactive_drawing(self):
-        self.working_img_data['img-drawing'] = []
-        self.image_view.img_stacks.image_dict['img-drawing'].clear()
-        self.image_view.img_stacks.image_dict['img-drawing'].updateItems()
-        self.drawing_img = np.zeros((self.image_view.img_size[0], self.image_view.img_size[1], 3))
+        self.working_img_data["img-drawing"] = []
+        self.image_view.img_stacks.image_dict["img-drawing"].clear()
+        self.image_view.img_stacks.image_dict["img-drawing"].updateItems()
+        self.drawing_img = np.zeros(
+            (self.image_view.img_size[0], self.image_view.img_size[1], 3)
+        )
 
     def img_drawing_pnts_clicked(self, points, ev):  # check mark
         clicked_ind = ev[0].index()
         pos = ev[0].pos()
-        if self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
-            del self.working_img_data['img-drawing'][clicked_ind]
-            if not self.working_img_data['img-drawing']:
+        if self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
+            del self.working_img_data["img-drawing"][clicked_ind]
+            if not self.working_img_data["img-drawing"]:
                 self.inactive_drawing()
         else:
             if clicked_ind == 0:
-                print('first point clicked')
+                print("first point clicked")
                 self.inactive_drawing()
-            elif clicked_ind == len(self.working_img_data['img-drawing']) - 1:
-                print('last point clicked')
+            elif clicked_ind == len(self.working_img_data["img-drawing"]) - 1:
+                print("last point clicked")
                 self.is_pencil_allowed = False
-                self.working_img_data['img-drawing'].append([pos.x(), pos.y()])
+                self.working_img_data["img-drawing"].append([pos.x(), pos.y()])
                 if self.tool_box.is_closed:
-                    self.working_img_data['img-drawing'].append([self.working_img_data['img-drawing'][0][0],
-                                                                 self.working_img_data['img-drawing'][0][1]])
-                self.image_view.img_stacks.image_dict['img-drawing'].setData(
-                    np.asarray(self.working_img_data['img-drawing']))
-                da_img = create_vis_img(self.image_view.img_size, self.working_img_data['img-drawing'],
-                                        self.pencil_color, 'l', self.tool_box.is_closed)
-                res = cv2.resize(da_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                self.layer_ctrl.master_layers(res, layer_type='img-drawing', color=self.pencil_color)
-                current_data = {'data': self.working_img_data['img-drawing'].copy(),
-                                'closed': self.tool_box.is_closed}
-                self.save_current_action('pencil_btn', 'img-drawing', current_data, res)
+                    self.working_img_data["img-drawing"].append(
+                        [
+                            self.working_img_data["img-drawing"][0][0],
+                            self.working_img_data["img-drawing"][0][1],
+                        ]
+                    )
+                self.image_view.img_stacks.image_dict["img-drawing"].setData(
+                    np.asarray(self.working_img_data["img-drawing"])
+                )
+                da_img = create_vis_img(
+                    self.image_view.img_size,
+                    self.working_img_data["img-drawing"],
+                    self.pencil_color,
+                    "l",
+                    self.tool_box.is_closed,
+                )
+                res = cv2.resize(
+                    da_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                )
+                self.layer_ctrl.master_layers(
+                    res, layer_type="img-drawing", color=self.pencil_color
+                )
+                current_data = {
+                    "data": self.working_img_data["img-drawing"].copy(),
+                    "closed": self.tool_box.is_closed,
+                }
+                self.save_current_action("pencil_btn", "img-drawing", current_data, res)
             else:
-                print('other point clicked')
+                print("other point clicked")
                 if not self.is_pencil_allowed:
                     self.inactive_drawing()
 
     # ------------------------------------------------------------------
     #
     #               ToolBar eraser btn related
     #
     # ------------------------------------------------------------------
     def change_eraser_color(self, ev):
         eraser_color = ev.color()
-        self.image_view.img_stacks.image_dict['circle_follow'].setPen(pg.mkPen(color=eraser_color))
-        self.atlas_view.working_atlas.image_dict['circle_follow'].setPen(pg.mkPen(color=eraser_color))
+        self.image_view.img_stacks.image_dict["circle_follow"].setPen(
+            pg.mkPen(color=eraser_color)
+        )
+        self.atlas_view.working_atlas.image_dict["circle_follow"].setPen(
+            pg.mkPen(color=eraser_color)
+        )
 
     # ------------------------------------------------------------------
     #
     #               ToolBar loc btn related
     #
     # ------------------------------------------------------------------
     def change_cell_color(self, ev):
         cell_color = np.ravel(ev.color().getRgb())
         self.cell_color = (int(cell_color[0]), int(cell_color[1]), int(cell_color[2]))
-        self.image_view.img_stacks.image_dict['img-cells'].setPen(color=self.cell_color)
-        self.image_view.img_stacks.image_dict['img-cells'].setBrush(color=self.cell_color)
-        self.atlas_view.cimg.image_dict['atlas-cells'].setPen(color=self.cell_color)
-        self.atlas_view.himg.image_dict['atlas-cells'].setPen(color=self.cell_color)
-        self.atlas_view.simg.image_dict['atlas-cells'].setPen(color=self.cell_color)
-        self.atlas_view.cimg.image_dict['atlas-cells'].setBrush(color=self.cell_color)
-        self.atlas_view.himg.image_dict['atlas-cells'].setBrush(color=self.cell_color)
-        self.atlas_view.simg.image_dict['atlas-cells'].setBrush(color=self.cell_color)
+        self.image_view.img_stacks.image_dict["img-cells"].setPen(color=self.cell_color)
+        self.image_view.img_stacks.image_dict["img-cells"].setBrush(
+            color=self.cell_color
+        )
+        self.atlas_view.cimg.image_dict["atlas-cells"].setPen(color=self.cell_color)
+        self.atlas_view.himg.image_dict["atlas-cells"].setPen(color=self.cell_color)
+        self.atlas_view.simg.image_dict["atlas-cells"].setPen(color=self.cell_color)
+        self.atlas_view.cimg.image_dict["atlas-cells"].setBrush(color=self.cell_color)
+        self.atlas_view.himg.image_dict["atlas-cells"].setBrush(color=self.cell_color)
+        self.atlas_view.simg.image_dict["atlas-cells"].setBrush(color=self.cell_color)
 
     def cell_select_btn_clicked(self):
         if self.tool_box.cell_aim_btn.isChecked():
             self.tool_box.cell_aim_btn.setChecked(False)
 
     def cell_aim_btn_clicked(self):
         if self.tool_box.cell_selector_btn.isChecked():
             self.tool_box.cell_selector_btn.setChecked(False)
 
-    def cell_detect_btn_clicked(self):   # ??????????
-        if not self.working_img_data['img-blob']:
+    def cell_detect_btn_clicked(self):  # ??????????
+        if not self.working_img_data["img-blob"]:
             return
 
-        locs = np.asarray(self.working_img_data['img-blob']).astype(int)
+        locs = np.asarray(self.working_img_data["img-blob"]).astype(int)
         da_width = np.max(locs[:, 0]) - np.min(locs[:, 0]) + 1
         da_height = np.max(locs[:, 1]) - np.min(locs[:, 1]) + 1
-        small_img = np.zeros((da_height, da_width), 'uint8')
+        small_img = np.zeros((da_height, da_width), "uint8")
         small_locs = locs - np.array([np.min(locs[:, 0]), np.min(locs[:, 1])])
         small_img[small_locs[:, 1], small_locs[:, 0]] = 1
-        ct, ht = cv2.findContours(small_img, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE)
+        ct, ht = cv2.findContours(
+            small_img, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE
+        )
         cnt = ct[0]
         da_moment = cv2.moments(cnt)
         center_x = int(da_moment["m10"] / da_moment["m00"])
         center_y = int(da_moment["m01"] / da_moment["m00"])
         da_area = cv2.contourArea(cnt)
         da_perimeter = cv2.arcLength(cnt, True)
 
-        da_circularity = 4 * np.pi * da_area / (da_perimeter ** 2)
+        da_circularity = 4 * np.pi * da_area / (da_perimeter**2)
 
         params = cv2.SimpleBlobDetector_Params()
         # Change thresholds
         params.filterByArea = True
         params.minArea = da_area - 1
         params.maxArea = da_area + 1
         params.filterByCircularity = True
@@ -2293,15 +2775,15 @@
         params.filterByConvexity = True
         params.minConvexity = 0.87
         params.filterByInertia = True
         params.minInertiaRatio = 0.01
 
         temp = self.image_view.current_img.copy()
         if self.image_view.image_file.is_rgb:
-            if self.image_view.current_mode == 'rgb':
+            if self.image_view.current_mode == "rgb":
                 temp = cv2.cvtColor(temp, cv2.COLOR_RGB2GRAY)
                 layer_ind = 0
         else:
             da_layer = [ind for ind in range(4) if self.image_view.channel_visible[ind]]
             n_layers = len(da_layer)
             if n_layers == 0:
                 return
@@ -2324,203 +2806,295 @@
         if n_keypoints == 0:
             return
 
         for i in range(n_keypoints):
             x = keypoints[i].pt[0]
             y = keypoints[i].pt[1]
             size = keypoints[i].size
-            self.working_img_data['img-cells'].append([x, y])
-            self.working_img_data['cell_layer_index'].append(layer_ind)
-            self.working_img_data['cell_symbol'].append(self.cell_base_symbol[layer_ind])
-            self.working_img_data['cell_size'].append(size)
-        self.working_img_data['cell_count'][layer_ind] = self.working_img_data['cell_count'][layer_ind] + n_keypoints
-        self.tool_box.cell_count_val_list[layer_ind].setText(str(self.working_img_data['cell_count'][layer_ind]))
-
-        self.image_view.img_stacks.image_dict['img-cells'].setData(
-            pos=np.asarray(self.working_img_data['img-cells']), symbol=self.working_img_data['cell_symbol'])
+            self.working_img_data["img-cells"].append([x, y])
+            self.working_img_data["cell_layer_index"].append(layer_ind)
+            self.working_img_data["cell_symbol"].append(
+                self.cell_base_symbol[layer_ind]
+            )
+            self.working_img_data["cell_size"].append(size)
+        self.working_img_data["cell_count"][layer_ind] = (
+            self.working_img_data["cell_count"][layer_ind] + n_keypoints
+        )
+        self.tool_box.cell_count_val_list[layer_ind].setText(
+            str(self.working_img_data["cell_count"][layer_ind])
+        )
+
+        self.image_view.img_stacks.image_dict["img-cells"].setData(
+            pos=np.asarray(self.working_img_data["img-cells"]),
+            symbol=self.working_img_data["cell_symbol"],
+        )
 
-        self.working_img_data['img-blob'] = []
-        self.image_view.img_stacks.image_dict['img-blob'].clear()
+        self.working_img_data["img-blob"] = []
+        self.image_view.img_stacks.image_dict["img-blob"].clear()
 
     # ------------------------------------------------------------------
     #
     #               ToolBar magic wand btn related
     #
     # ------------------------------------------------------------------
     def change_magic_wand_color(self, ev):
         if self.image_view.image_file is None:
             return
         self.magic_wand_lut[1] = np.ravel(ev.color().getRgb())
-        self.image_view.img_stacks.image_dict['img-mask'].setLookupTable(self.magic_wand_lut)
-        self.atlas_view.cimg.image_dict['atlas-mask'].setLookupTable(self.magic_wand_lut)
-        self.atlas_view.himg.image_dict['atlas-mask'].setLookupTable(self.magic_wand_lut)
-        self.atlas_view.simg.image_dict['atlas-mask'].setLookupTable(self.magic_wand_lut)
-        self.atlas_view.slice_stack.image_dict['atlas-mask'].setLookupTable(self.magic_wand_lut)
-        self.image_view.img_stacks.image_dict['img-mask'].updateImage()
-        self.atlas_view.cimg.image_dict['atlas-mask'].updateImage()
-        self.atlas_view.himg.image_dict['atlas-mask'].updateImage()
-        self.atlas_view.simg.image_dict['atlas-mask'].updateImage()
-        self.atlas_view.slice_stack.image_dict['atlas-mask'].updateImage()
+        self.image_view.img_stacks.image_dict["img-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.atlas_view.cimg.image_dict["atlas-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.atlas_view.himg.image_dict["atlas-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.atlas_view.simg.image_dict["atlas-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.atlas_view.slice_stack.image_dict["atlas-mask"].setLookupTable(
+            self.magic_wand_lut
+        )
+        self.image_view.img_stacks.image_dict["img-mask"].updateImage()
+        self.atlas_view.cimg.image_dict["atlas-mask"].updateImage()
+        self.atlas_view.himg.image_dict["atlas-mask"].updateImage()
+        self.atlas_view.simg.image_dict["atlas-mask"].updateImage()
+        self.atlas_view.slice_stack.image_dict["atlas-mask"].updateImage()
 
     def get_virus_img(self):
-        if 'img-mask' not in self.layer_ctrl.layer_link:
-            self.print_message('Need Mask Data to transfer to Virus Data.', self.reminder_color)
+        if "img-mask" not in self.layer_ctrl.layer_link:
+            self.print_message(
+                "Need Mask Data to transfer to Virus Data.", self.reminder_color
+            )
             return
         self.virus_lut = self.magic_wand_lut.copy()
-        self.atlas_view.working_atlas.image_dict['atlas-virus'].setPen(color=self.virus_lut[1])
-        self.atlas_view.working_atlas.image_dict['atlas-virus'].setBrush(color=self.virus_lut[1])
-        self.image_view.img_stacks.image_dict['img-virus'].setLookupTable(self.virus_lut)
-        self.working_img_data['img-virus'] = self.working_img_data['img-mask'].copy()
-        self.image_view.img_stacks.image_dict['img-virus'].setImage(self.working_img_data['img-virus'])
-        temp = color_vis_img(self.working_img_data['img-virus'], self.virus_lut[1])
+        self.atlas_view.working_atlas.image_dict["atlas-virus"].setPen(
+            color=self.virus_lut[1]
+        )
+        self.atlas_view.working_atlas.image_dict["atlas-virus"].setBrush(
+            color=self.virus_lut[1]
+        )
+        self.image_view.img_stacks.image_dict["img-virus"].setLookupTable(
+            self.virus_lut
+        )
+        self.working_img_data["img-virus"] = self.working_img_data["img-mask"].copy()
+        self.image_view.img_stacks.image_dict["img-virus"].setImage(
+            self.working_img_data["img-virus"]
+        )
+        temp = color_vis_img(self.working_img_data["img-virus"], self.virus_lut[1])
         res = cv2.resize(temp, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-        self.layer_ctrl.master_layers(res, layer_type='img-virus', color=self.virus_lut[1])
-        self.remove_single_link_related('img-mask')
+        self.layer_ctrl.master_layers(
+            res, layer_type="img-virus", color=self.virus_lut[1]
+        )
+        self.remove_single_link_related("img-mask")
 
     def get_contour_img(self):
-        if 'img-mask' not in self.layer_ctrl.layer_link:
-            self.print_message('Need Mask Data to transfer to Contour Data.', self.reminder_color)
+        if "img-mask" not in self.layer_ctrl.layer_link:
+            self.print_message(
+                "Need Mask Data to transfer to Contour Data.", self.reminder_color
+            )
             return
         self.contour_color = self.magic_wand_lut[1].copy()
-        self.image_view.img_stacks.image_dict['img-contour'].setPen(color=self.contour_color)
-        self.image_view.img_stacks.image_dict['img-contour'].setBrush(color=self.contour_color)
-        self.atlas_view.working_atlas.image_dict['atlas-contour'].setPen(color=self.contour_color)
-        self.atlas_view.working_atlas.image_dict['atlas-contour'].setBrush(color=self.contour_color)
-        temp = self.working_img_data['img-mask'].astype('uint8')
+        self.image_view.img_stacks.image_dict["img-contour"].setPen(
+            color=self.contour_color
+        )
+        self.image_view.img_stacks.image_dict["img-contour"].setBrush(
+            color=self.contour_color
+        )
+        self.atlas_view.working_atlas.image_dict["atlas-contour"].setPen(
+            color=self.contour_color
+        )
+        self.atlas_view.working_atlas.image_dict["atlas-contour"].setBrush(
+            color=self.contour_color
+        )
+        temp = self.working_img_data["img-mask"].astype("uint8")
         contour_length = 0
         contour_points = None
-        ct, hc = cv2.findContours(image=temp, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE)
+        ct, hc = cv2.findContours(
+            image=temp, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE
+        )
         for j in range(len(ct)):
             da_contour = ct[j].copy()
             da_shp = da_contour.shape
             da_contour = np.reshape(da_contour, (da_shp[0], da_shp[2]))
             if len(da_contour) > contour_length:
                 contour_points = da_contour
                 contour_length = len(da_contour)
         if contour_points is None:
-            self.print_message('No contour can be created.', self.error_message_color)
+            self.print_message("No contour can be created.", self.error_message_color)
             return
-        self.working_img_data['img-contour'] = contour_points.tolist()
-        self.image_view.img_stacks.image_dict['img-contour'].setData(contour_points)
+        self.working_img_data["img-contour"] = contour_points.tolist()
+        self.image_view.img_stacks.image_dict["img-contour"].setData(contour_points)
         # make showing img
-        contour_img = create_vis_img(self.image_view.img_size, contour_points, self.contour_color, 'l')
-        res = cv2.resize(contour_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-        self.layer_ctrl.master_layers(res, layer_type='img-contour', color=self.contour_color)
-        self.remove_single_link_related('img-mask')
+        contour_img = create_vis_img(
+            self.image_view.img_size, contour_points, self.contour_color, "l"
+        )
+        res = cv2.resize(
+            contour_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+        )
+        self.layer_ctrl.master_layers(
+            res, layer_type="img-contour", color=self.contour_color
+        )
+        self.remove_single_link_related("img-mask")
 
     def kernel_changed(self):
         ksize = self.tool_box.magic_wand_ksize.value()
         kernel_shape = self.tool_box.magic_wand_kernel.currentText()
         if ksize != 0 and kernel_shape != "Kernel":
             if kernel_shape == "Rectangular":
                 self.kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (ksize, ksize))
             elif kernel_shape == "Elliptical":
-                self.kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (ksize, ksize))
+                self.kernel = cv2.getStructuringElement(
+                    cv2.MORPH_ELLIPSE, (ksize, ksize)
+                )
             else:
                 self.kernel = cv2.getStructuringElement(cv2.MORPH_CROSS, (ksize, ksize))
         else:
             self.kernel = None
 
     # ------------------------------------------------------------------
     #
     #               ToolBar triangle btn related
     #
     # ------------------------------------------------------------------
     def show_triangle_points(self, current_btn):
-        if self.tool_box.checkable_btn_dict['{}_btn'.format(current_btn)].isChecked():
+        if self.tool_box.checkable_btn_dict["{}_btn".format(current_btn)].isChecked():
             if self.atlas_tri_data:
-                if not self.atlas_view.working_atlas.image_dict['tri_pnts'].isVisible():
-                    self.atlas_view.working_atlas.image_dict['tri_pnts'].setVisible(True)
-                if self.atlas_tri_inside_data and not self.working_atlas_text[0].isVisible():
+                if not self.atlas_view.working_atlas.image_dict["tri_pnts"].isVisible():
+                    self.atlas_view.working_atlas.image_dict["tri_pnts"].setVisible(
+                        True
+                    )
+                if (
+                    self.atlas_tri_inside_data
+                    and not self.working_atlas_text[0].isVisible()
+                ):
                     for i in range(len(self.working_atlas_text)):
                         self.working_atlas_text[i].setVisible(True)
             if self.histo_tri_data:
-                if not self.image_view.img_stacks.image_dict['tri_pnts'].isVisible():
-                    self.image_view.img_stacks.image_dict['tri_pnts'].setVisible(True)
-                if self.histo_tri_inside_data and not self.working_img_text[0].isVisible():
+                if not self.image_view.img_stacks.image_dict["tri_pnts"].isVisible():
+                    self.image_view.img_stacks.image_dict["tri_pnts"].setVisible(True)
+                if (
+                    self.histo_tri_inside_data
+                    and not self.working_img_text[0].isVisible()
+                ):
                     for i in range(len(self.working_img_text)):
                         self.working_img_text[i].setVisible(True)
         else:
             if self.atlas_tri_data:
-                if self.atlas_view.working_atlas.image_dict['tri_pnts'].isVisible():
-                    self.atlas_view.working_atlas.image_dict['tri_pnts'].setVisible(False)
-                if self.atlas_tri_inside_data and self.working_atlas_text[0].isVisible():
+                if self.atlas_view.working_atlas.image_dict["tri_pnts"].isVisible():
+                    self.atlas_view.working_atlas.image_dict["tri_pnts"].setVisible(
+                        False
+                    )
+                if (
+                    self.atlas_tri_inside_data
+                    and self.working_atlas_text[0].isVisible()
+                ):
                     for i in range(len(self.working_atlas_text)):
                         self.working_atlas_text[i].setVisible(False)
             if self.histo_tri_data:
-                if self.image_view.img_stacks.image_dict['tri_pnts'].isVisible():
-                    self.image_view.img_stacks.image_dict['tri_pnts'].setVisible(False)
+                if self.image_view.img_stacks.image_dict["tri_pnts"].isVisible():
+                    self.image_view.img_stacks.image_dict["tri_pnts"].setVisible(False)
                 if self.histo_tri_inside_data and self.working_img_text[0].isVisible():
                     for i in range(len(self.working_img_text)):
                         self.working_img_text[i].setVisible(False)
 
     def number_of_side_points_changed(self):
         input_txt = self.tool_box.bound_pnts_num.text()
-        if input_txt == '':
-            msg = 'Number of boundary points can not be empty. Automatically set it to previous valid value. '
+        if input_txt == "":
+            msg = "Number of boundary points can not be empty. Automatically set it to previous valid value. "
             self.print_message(msg, self.reminder_color)
             self.tool_box.bound_pnts_num.setText(str(self.np_onside))
             return
-        if input_txt == '0' or input_txt == '1':
-            msg = 'Number of boundary points can not be less than 2. Automatically set it to previous valid value. '
+        if input_txt == "0" or input_txt == "1":
+            msg = "Number of boundary points can not be less than 2. Automatically set it to previous valid value. "
             self.print_message(msg, self.reminder_color)
             self.tool_box.bound_pnts_num.setText(str(self.np_onside))
             return
         self.np_onside = int(input_txt)
-        self.print_message('', self.normal_color)
-        if self.atlas_view.atlas_data is not None or self.atlas_view.slice_image_data is not None:
-            self.atlas_tri_onside_data = num_side_pnt_changed(self.np_onside, self.atlas_corner_points,
-                                                              self.atlas_side_lines)
-            self.atlas_tri_data = self.atlas_tri_onside_data + self.atlas_tri_inside_data
-            self.atlas_view.working_atlas.image_dict['tri_pnts'].setData(pos=np.asarray(self.atlas_tri_data))
+        self.print_message("", self.normal_color)
+        if (
+            self.atlas_view.atlas_data is not None
+            or self.atlas_view.slice_image_data is not None
+        ):
+            self.atlas_tri_onside_data = num_side_pnt_changed(
+                self.np_onside, self.atlas_corner_points, self.atlas_side_lines
+            )
+            self.atlas_tri_data = (
+                self.atlas_tri_onside_data + self.atlas_tri_inside_data
+            )
+            self.atlas_view.working_atlas.image_dict["tri_pnts"].setData(
+                pos=np.asarray(self.atlas_tri_data)
+            )
             if self.tool_box.triang_vis_btn.isChecked():
                 self.update_atlas_tri_lines()
         if self.image_view.current_img is not None:
-            self.histo_tri_onside_data = num_side_pnt_changed(self.np_onside, self.histo_corner_points,
-                                                              self.histo_side_lines)
-            self.histo_tri_data = self.histo_tri_onside_data + self.histo_tri_inside_data
-            self.image_view.img_stacks.image_dict['tri_pnts'].setData(pos=np.asarray(self.histo_tri_data))
+            self.histo_tri_onside_data = num_side_pnt_changed(
+                self.np_onside, self.histo_corner_points, self.histo_side_lines
+            )
+            self.histo_tri_data = (
+                self.histo_tri_onside_data + self.histo_tri_inside_data
+            )
+            self.image_view.img_stacks.image_dict["tri_pnts"].setData(
+                pos=np.asarray(self.histo_tri_data)
+            )
             if self.tool_box.triang_vis_btn.isChecked():
                 self.update_histo_tri_lines()
 
     def remove_histo_tri_lines(self):
         if self.image_view.img_stacks.tri_lines_list:
             for da_item in self.image_view.img_stacks.tri_lines_list:
                 self.image_view.img_stacks.vb.removeItem(da_item)
             self.image_view.img_stacks.tri_lines_list = []
 
     def update_histo_tri_lines(self):
         self.remove_histo_tri_lines()
-        point_data = self.image_view.img_stacks.image_dict['tri_pnts'].data['pos'].copy()
+        point_data = (
+            self.image_view.img_stacks.image_dict["tri_pnts"].data["pos"].copy()
+        )
         point_data = list(point_data)
         histo_tri_lines = get_tri_lines(self.histo_rect, self.histo_tri_data)
         for el in histo_tri_lines:
             pt1 = [el[0], el[1]]
             pt2 = [el[2], el[3]]
-            self.image_view.img_stacks.tri_lines_list.append(pg.PlotDataItem(pen=self.tool_box.tri_line_style))
-            self.image_view.img_stacks.tri_lines_list[-1].setData(np.asarray([pt1, pt2]))
-            self.image_view.img_stacks.vb.addItem(self.image_view.img_stacks.tri_lines_list[-1])
+            self.image_view.img_stacks.tri_lines_list.append(
+                pg.PlotDataItem(pen=self.tool_box.tri_line_style)
+            )
+            self.image_view.img_stacks.tri_lines_list[-1].setData(
+                np.asarray([pt1, pt2])
+            )
+            self.image_view.img_stacks.vb.addItem(
+                self.image_view.img_stacks.tri_lines_list[-1]
+            )
 
     def remove_atlas_tri_lines(self):
         if self.atlas_view.working_atlas.tri_lines_list:
             for da_item in self.atlas_view.working_atlas.tri_lines_list:
                 self.atlas_view.working_atlas.vb.removeItem(da_item)
             self.atlas_view.working_atlas.tri_lines_list = []
 
     def update_atlas_tri_lines(self):
         self.remove_atlas_tri_lines()
-        point_data = self.atlas_view.working_atlas.image_dict['tri_pnts'].data['pos'].copy()
+        point_data = (
+            self.atlas_view.working_atlas.image_dict["tri_pnts"].data["pos"].copy()
+        )
         point_data = list(point_data)
         atlas_tri_lines = get_tri_lines(self.atlas_rect, point_data)
         for el in atlas_tri_lines:
             pt1 = [el[0], el[1]]
             pt2 = [el[2], el[3]]
-            self.atlas_view.working_atlas.tri_lines_list.append(pg.PlotDataItem(pen=self.tool_box.tri_line_style))
-            self.atlas_view.working_atlas.tri_lines_list[-1].setData(np.asarray([pt1, pt2]))
-            self.atlas_view.working_atlas.vb.addItem(self.atlas_view.working_atlas.tri_lines_list[-1])
+            self.atlas_view.working_atlas.tri_lines_list.append(
+                pg.PlotDataItem(pen=self.tool_box.tri_line_style)
+            )
+            self.atlas_view.working_atlas.tri_lines_list[-1].setData(
+                np.asarray([pt1, pt2])
+            )
+            self.atlas_view.working_atlas.vb.addItem(
+                self.atlas_view.working_atlas.tri_lines_list[-1]
+            )
 
     def vis_tri_lines_btn_clicked(self):
         if self.tool_box.triang_vis_btn.isChecked():
             if self.atlas_tri_data:
                 self.update_atlas_tri_lines()
             if self.histo_tri_data:
                 self.update_histo_tri_lines()
@@ -2528,25 +3102,36 @@
             if self.atlas_tri_data:
                 self.remove_atlas_tri_lines()
             if self.histo_tri_data:
                 self.remove_histo_tri_lines()
 
     def matching_tri_bnd(self):
         if self.image_view.image_file is None:
-            self.print_message('No histological image is loaded.', self.error_message_color)
-            return
-        if self.atlas_view.atlas_data is None and self.atlas_view.slice_image_data is None:
-            self.print_message('No Atlas is loaded.', self.error_message_color)
+            self.print_message(
+                "No histological image is loaded.", self.error_message_color
+            )
+            return
+        if (
+            self.atlas_view.atlas_data is None
+            and self.atlas_view.slice_image_data is None
+        ):
+            self.print_message("No Atlas is loaded.", self.error_message_color)
             return
         if not self.histo_tri_inside_data:
-            self.print_message('No in-image triangulation points are selected.', self.error_message_color)
+            self.print_message(
+                "No in-image triangulation points are selected.",
+                self.error_message_color,
+            )
             return
-        if self.current_atlas == 'slice':
+        if self.current_atlas == "slice":
             if not self.atlas_tri_inside_data:
-                self.print_message('No in-slice triangulation points are selected.', self.error_message_color)
+                self.print_message(
+                    "No in-slice triangulation points are selected.",
+                    self.error_message_color,
+                )
                 return
 
         slice_size = self.atlas_view.slice_size
         image_size = self.image_view.img_size
 
         histo_pnts = np.asarray(self.histo_tri_inside_data)
         rect_img = cv2.boundingRect(histo_pnts.astype(np.float32))
@@ -2560,239 +3145,342 @@
         else:
             atlas_pnts = np.asarray(self.atlas_tri_inside_data)
         rect_atlas = cv2.boundingRect(atlas_pnts.astype(np.float32))
 
         self.small_atlas_rect = rect_atlas
         self.small_histo_rect = rect_img
 
-        update_atlas_rect, update_image_rect = match_sides_points(rect_atlas, slice_size, rect_img, image_size)
-
-        self.atlas_corner_points, self.atlas_side_lines = get_corner_line_from_rect(update_atlas_rect)
-        self.histo_corner_points, self.histo_side_lines = get_corner_line_from_rect(update_image_rect)
-
-        self.atlas_tri_onside_data = num_side_pnt_changed(self.np_onside, self.atlas_corner_points, self.atlas_side_lines)
+        update_atlas_rect, update_image_rect = match_sides_points(
+            rect_atlas, slice_size, rect_img, image_size
+        )
+
+        self.atlas_corner_points, self.atlas_side_lines = get_corner_line_from_rect(
+            update_atlas_rect
+        )
+        self.histo_corner_points, self.histo_side_lines = get_corner_line_from_rect(
+            update_image_rect
+        )
+
+        self.atlas_tri_onside_data = num_side_pnt_changed(
+            self.np_onside, self.atlas_corner_points, self.atlas_side_lines
+        )
         self.atlas_tri_data = self.atlas_tri_onside_data + self.atlas_tri_inside_data
-        self.atlas_view.working_atlas.image_dict['tri_pnts'].setData(pos=np.asarray(self.atlas_tri_data))
-
-        self.histo_tri_onside_data = num_side_pnt_changed(self.np_onside, self.histo_corner_points, self.histo_side_lines)
+        self.atlas_view.working_atlas.image_dict["tri_pnts"].setData(
+            pos=np.asarray(self.atlas_tri_data)
+        )
+
+        self.histo_tri_onside_data = num_side_pnt_changed(
+            self.np_onside, self.histo_corner_points, self.histo_side_lines
+        )
         self.histo_tri_data = self.histo_tri_onside_data + self.histo_tri_inside_data
-        self.image_view.img_stacks.image_dict['tri_pnts'].setData(pos=np.asarray(self.histo_tri_data))
+        self.image_view.img_stacks.image_dict["tri_pnts"].setData(
+            pos=np.asarray(self.histo_tri_data)
+        )
         if self.tool_box.triang_vis_btn.isChecked():
             self.update_histo_tri_lines()
             self.update_atlas_tri_lines()
 
     # change color for triangle points and text
     def change_triangle_color(self, ev):
         self.triangle_color = ev.color()
         # triang_color = np.ravel(triang_color.getRgb())
-        self.image_view.img_stacks.image_dict['tri_pnts'].scatter.setPen(color=self.triangle_color)
-        self.image_view.img_stacks.image_dict['tri_pnts'].scatter.setBrush(color=self.triangle_color)
+        self.image_view.img_stacks.image_dict["tri_pnts"].scatter.setPen(
+            color=self.triangle_color
+        )
+        self.image_view.img_stacks.image_dict["tri_pnts"].scatter.setBrush(
+            color=self.triangle_color
+        )
         if self.working_img_text:
             for i in range(len(self.working_img_text)):
                 self.working_img_text[i].setColor(self.triangle_color)
-        self.atlas_view.cimg.image_dict['tri_pnts'].scatter.setPen(color=self.triangle_color)
-        self.atlas_view.simg.image_dict['tri_pnts'].scatter.setPen(color=self.triangle_color)
-        self.atlas_view.himg.image_dict['tri_pnts'].scatter.setPen(color=self.triangle_color)
-        self.atlas_view.cimg.image_dict['tri_pnts'].scatter.setBrush(color=self.triangle_color)
-        self.atlas_view.simg.image_dict['tri_pnts'].scatter.setBrush(color=self.triangle_color)
-        self.atlas_view.himg.image_dict['tri_pnts'].scatter.setBrush(color=self.triangle_color)
+        self.atlas_view.cimg.image_dict["tri_pnts"].scatter.setPen(
+            color=self.triangle_color
+        )
+        self.atlas_view.simg.image_dict["tri_pnts"].scatter.setPen(
+            color=self.triangle_color
+        )
+        self.atlas_view.himg.image_dict["tri_pnts"].scatter.setPen(
+            color=self.triangle_color
+        )
+        self.atlas_view.cimg.image_dict["tri_pnts"].scatter.setBrush(
+            color=self.triangle_color
+        )
+        self.atlas_view.simg.image_dict["tri_pnts"].scatter.setBrush(
+            color=self.triangle_color
+        )
+        self.atlas_view.himg.image_dict["tri_pnts"].scatter.setBrush(
+            color=self.triangle_color
+        )
         if self.working_atlas_text:
             for i in range(len(self.working_atlas_text)):
                 self.working_atlas_text[i].setColor(self.triangle_color)
 
     # ------------------------------------------------------------------
     #
     #               ToolBar transform btn clicked
     #
     # ------------------------------------------------------------------
     def transfer_to_hist_clicked(self):
         if self.image_view.image_file is None:
-            self.print_message('No histological image data is loaded.', self.error_message_color)
-            return
-        if self.atlas_view.atlas_data is None and self.atlas_view.slice_image_data is None:
-            self.print_message('No Atlas data is loaded.', self.error_message_color)
-            return
-        self.print_message('Transfer atlas brain region segmentation to histological window.', self.normal_color)
+            self.print_message(
+                "No histological image data is loaded.", self.error_message_color
+            )
+            return
+        if (
+            self.atlas_view.atlas_data is None
+            and self.atlas_view.slice_image_data is None
+        ):
+            self.print_message("No Atlas data is loaded.", self.error_message_color)
+            return
+        self.print_message(
+            "Transfer atlas brain region segmentation to histological window.",
+            self.normal_color,
+        )
         if not self.a2h_transferred:
-            if self.current_atlas == 'volume':
+            if self.current_atlas == "volume":
                 label_img = self.atlas_view.working_atlas.label_img.image.copy()
                 lut = self.atlas_view.label_tree.current_lut.copy()
                 self.overlay_img = make_label_rgb_img(label_img, lut)
             else:
                 self.overlay_img = self.atlas_view.slice_stack.img_layer.image.copy()
 
             input_img = self.overlay_img.copy()
 
-            img_wrap = np.zeros((self.image_view.img_size[0], self.image_view.img_size[1], 3), np.float32)
+            img_wrap = np.zeros(
+                (self.image_view.img_size[0], self.image_view.img_size[1], 3),
+                np.float32,
+            )
 
             if self.histo_tri_inside_data and self.atlas_tri_inside_data:
                 a_temp = len(self.histo_tri_data)
                 b_temp = len(self.atlas_tri_data)
                 if a_temp != b_temp:
-                    self.print_message('Number of points in two windows are not matching.', self.error_message_color)
+                    self.print_message(
+                        "Number of points in two windows are not matching.",
+                        self.error_message_color,
+                    )
                     return
 
                 subdiv = cv2.Subdiv2D(self.histo_rect)
                 for p in self.histo_tri_data:
                     subdiv.insert(p)
 
                 tri_vet_inds = get_vertex_ind_in_triangle(subdiv)
                 for i in range(len(tri_vet_inds)):
                     da_inds = tri_vet_inds[i]
-                    t1 = [self.atlas_tri_data[da_inds[0]], self.atlas_tri_data[da_inds[1]], self.atlas_tri_data[da_inds[2]]]
-                    t2 = [self.histo_tri_data[da_inds[0]], self.histo_tri_data[da_inds[1]], self.histo_tri_data[da_inds[2]]]
+                    t1 = [
+                        self.atlas_tri_data[da_inds[0]],
+                        self.atlas_tri_data[da_inds[1]],
+                        self.atlas_tri_data[da_inds[2]],
+                    ]
+                    t2 = [
+                        self.histo_tri_data[da_inds[0]],
+                        self.histo_tri_data[da_inds[1]],
+                        self.histo_tri_data[da_inds[2]],
+                    ]
                     t1 = np.reshape(t1, (3, 2))
                     t2 = np.reshape(t2, (3, 2))
                     warp_triangle(input_img, img_wrap, t1, t2, True)
-                self.project_method = 'match to hist'
+                self.project_method = "match to hist"
                 self.register_method = 2
             else:
                 if self.small_atlas_rect is not None:
                     atlas_rect = self.small_atlas_rect
                     histo_rect = self.small_histo_rect
-                    self.project_method = 'match to hist'
+                    self.project_method = "match to hist"
                     self.register_method = 2
                 else:
                     atlas_rect = self.atlas_rect
                     histo_rect = self.histo_rect
-                    self.project_method = 'match to atlas'
+                    self.project_method = "match to atlas"
                     self.register_method = 1
                 src_xrange = (atlas_rect[0], atlas_rect[0] + atlas_rect[2])
                 src_yrange = (atlas_rect[1], atlas_rect[1] + atlas_rect[3])
-                src_img = input_img[src_yrange[0]:src_yrange[1], src_xrange[0]:src_xrange[1], :].copy()
+                src_img = input_img[
+                    src_yrange[0] : src_yrange[1], src_xrange[0] : src_xrange[1], :
+                ].copy()
 
                 da_dim = (histo_rect[2], histo_rect[3])
-                resized_des = cv2.resize(src_img, da_dim, interpolation=cv2.INTER_LINEAR)
+                resized_des = cv2.resize(
+                    src_img, da_dim, interpolation=cv2.INTER_LINEAR
+                )
 
                 des_xrange = (histo_rect[0], histo_rect[0] + histo_rect[2])
                 des_yrange = (histo_rect[1], histo_rect[1] + histo_rect[3])
-                img_wrap[des_yrange[0]:des_yrange[1], des_xrange[0]:des_xrange[1]] = resized_des
-
-            self.working_img_data['img-overlay'] = img_wrap
-            self.image_view.img_stacks.image_dict['img-overlay'].setImage(img_wrap)
-            res = cv2.resize(img_wrap, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='img-overlay', color=[])
+                img_wrap[
+                    des_yrange[0] : des_yrange[1], des_xrange[0] : des_xrange[1]
+                ] = resized_des
+
+            self.working_img_data["img-overlay"] = img_wrap
+            self.image_view.img_stacks.image_dict["img-overlay"].setImage(img_wrap)
+            res = cv2.resize(
+                img_wrap, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(res, layer_type="img-overlay", color=[])
             self.a2h_transferred = True
             self.tool_box.toh_btn.setIcon(self.tool_box.toh_btn_on_icon)
             self.tool_box.toa_btn.setEnabled(False)
-            self.print_message('Transfer finished.', self.normal_color)
+            self.print_message("Transfer finished.", self.normal_color)
         else:
             self.overlay_img = None
-            self.remove_single_link_related('img-overlay')
+            self.remove_single_link_related("img-overlay")
             self.a2h_transferred = False
             self.tool_box.toa_btn.setEnabled(True)
             self.tool_box.toh_btn.setIcon(self.tool_box.toh_btn_off_icon)
-            self.project_method = 'pre plan'
+            self.project_method = "pre plan"
             self.register_method = 0
-            self.print_message('Transfer deleted.', self.normal_color)
+            self.print_message("Transfer deleted.", self.normal_color)
 
     #
     def transfer_to_atlas_clicked(self):
         if self.image_view.image_file is None:
-            self.print_message('No histological image data is loaded.', self.error_message_color)
-            return
-        if self.atlas_view.atlas_data is None and self.atlas_view.slice_image_data is None:
-            self.print_message('No Atlas data is loaded.', self.error_message_color)
-            return
-        self.print_message('Transfer histological image to atlas window.', self.normal_color)
+            self.print_message(
+                "No histological image data is loaded.", self.error_message_color
+            )
+            return
+        if (
+            self.atlas_view.atlas_data is None
+            and self.atlas_view.slice_image_data is None
+        ):
+            self.print_message("No Atlas data is loaded.", self.error_message_color)
+            return
+        self.print_message(
+            "Transfer histological image to atlas window.", self.normal_color
+        )
         if not self.h2a_transferred:
             if self.image_view.processing_img is not None:
                 input_img = self.image_view.processing_img.copy()
             else:
                 input_img = self.image_view.current_img.copy()
 
-            if self.image_view.image_file.pixel_type == 'rgb24':
+            if self.image_view.image_file.pixel_type == "rgb24":
                 self.overlay_img = input_img.copy()
             else:
                 czi_img = input_img.copy()
                 channel_hsv = self.image_view.image_file.hsv_colors
                 img_temp = merge_channels_into_single_img(czi_img, channel_hsv)
-                self.overlay_img = cv2.normalize(img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
+                self.overlay_img = cv2.normalize(
+                    img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U
+                )
 
             working_img = self.overlay_img.copy()
 
-            img_wrap = np.zeros((self.atlas_view.slice_size[0], self.atlas_view.slice_size[1], 3), np.float32)
+            img_wrap = np.zeros(
+                (self.atlas_view.slice_size[0], self.atlas_view.slice_size[1], 3),
+                np.float32,
+            )
 
             if self.histo_tri_inside_data and self.atlas_tri_inside_data:
                 a_temp = len(self.histo_tri_data)
                 b_temp = len(self.atlas_tri_data)
                 if a_temp != b_temp:
-                    self.print_message('Number of points in two windows are not matching.', self.error_message_color)
+                    self.print_message(
+                        "Number of points in two windows are not matching.",
+                        self.error_message_color,
+                    )
                     return
                 subdiv = cv2.Subdiv2D(self.atlas_rect)
                 for p in self.atlas_tri_data:
                     subdiv.insert((int(p[0]), int(p[1])))
 
                 tri_vet_inds = get_vertex_ind_in_triangle(subdiv)
 
                 for i in range(len(tri_vet_inds)):
                     da_inds = tri_vet_inds[i]
-                    t2 = [self.atlas_tri_data[da_inds[0]], self.atlas_tri_data[da_inds[1]],
-                          self.atlas_tri_data[da_inds[2]]]
-                    t1 = [self.histo_tri_data[da_inds[0]], self.histo_tri_data[da_inds[1]],
-                          self.histo_tri_data[da_inds[2]]]
+                    t2 = [
+                        self.atlas_tri_data[da_inds[0]],
+                        self.atlas_tri_data[da_inds[1]],
+                        self.atlas_tri_data[da_inds[2]],
+                    ]
+                    t1 = [
+                        self.histo_tri_data[da_inds[0]],
+                        self.histo_tri_data[da_inds[1]],
+                        self.histo_tri_data[da_inds[2]],
+                    ]
                     t1 = np.reshape(t1, (3, 2))
                     t2 = np.reshape(t2, (3, 2))
                     warp_triangle(working_img, img_wrap, t1, t2, True)
             else:
                 if self.small_atlas_rect is not None:
                     atlas_rect = self.small_atlas_rect
                     histo_rect = self.small_histo_rect
                 else:
                     atlas_rect = self.atlas_rect
                     histo_rect = self.histo_rect
                 src_xrange = (histo_rect[0], histo_rect[0] + histo_rect[2])
                 src_yrange = (histo_rect[1], histo_rect[1] + histo_rect[3])
-                src_img = working_img[src_yrange[0]:src_yrange[1], src_xrange[0]:src_xrange[1], :].copy()
+                src_img = working_img[
+                    src_yrange[0] : src_yrange[1], src_xrange[0] : src_xrange[1], :
+                ].copy()
 
                 da_dim = (atlas_rect[2], atlas_rect[3])
-                resized_des = cv2.resize(src_img, da_dim, interpolation=cv2.INTER_LINEAR)
+                resized_des = cv2.resize(
+                    src_img, da_dim, interpolation=cv2.INTER_LINEAR
+                )
 
                 des_xrange = (atlas_rect[0], atlas_rect[0] + atlas_rect[2])
                 des_yrange = (atlas_rect[1], atlas_rect[1] + atlas_rect[3])
-                img_wrap[des_yrange[0]:des_yrange[1], des_xrange[0]:des_xrange[1]] = resized_des
-
-            self.working_atlas_data['atlas-overlay'] = img_wrap.astype('uint8')
-            self.atlas_view.working_atlas.image_dict['atlas-overlay'].setImage(img_wrap.astype('uint8'))
-            res = cv2.resize(img_wrap, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-overlay', color=[])
+                img_wrap[
+                    des_yrange[0] : des_yrange[1], des_xrange[0] : des_xrange[1]
+                ] = resized_des
+
+            self.working_atlas_data["atlas-overlay"] = img_wrap.astype("uint8")
+            self.atlas_view.working_atlas.image_dict["atlas-overlay"].setImage(
+                img_wrap.astype("uint8")
+            )
+            res = cv2.resize(
+                img_wrap, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(res, layer_type="atlas-overlay", color=[])
             self.h2a_transferred = True
             self.tool_box.toa_btn.setIcon(self.tool_box.toa_btn_on_icon)
-            self.project_method = 'match to atlas'
+            self.project_method = "match to atlas"
             self.register_method = 0
             self.tool_box.toh_btn.setEnabled(False)
-            self.print_message('Transfer finished.', self.normal_color)
+            self.print_message("Transfer finished.", self.normal_color)
         else:
             self.overlay_img = None
-            self.remove_single_link_related('atlas-overlay')
+            self.remove_single_link_related("atlas-overlay")
             self.h2a_transferred = False
             self.tool_box.toa_btn.setIcon(self.tool_box.toa_btn_off_icon)
-            self.project_method = 'pre plan'
+            self.project_method = "pre plan"
             self.register_method = 0
             self.tool_box.toh_btn.setEnabled(True)
-            self.atlas_tri_data = self.atlas_view.working_atlas.image_dict['tri_pnts'].data['pos'].tolist()
-            self.print_message('Transfer deleted.', self.normal_color)
+            self.atlas_tri_data = (
+                self.atlas_view.working_atlas.image_dict["tri_pnts"]
+                .data["pos"]
+                .tolist()
+            )
+            self.print_message("Transfer deleted.", self.normal_color)
 
     # ---------------------------
     #          Accept
     # ---------------------------
     def transfer_pnt(self, pnt, tri_vet_inds):
         res_pnts = np.zeros((len(pnt), 2))
         res_pnts[:] = np.nan
-        loc = get_pnts_triangle_ind(tri_vet_inds, self.histo_tri_data, self.image_view.img_size, pnt)
+        loc = get_pnts_triangle_ind(
+            tri_vet_inds, self.histo_tri_data, self.image_view.img_size, pnt
+        )
         loc = np.ravel(loc)
         if np.any(np.isnan(loc)):
-            msg = 'Some of the selected points are out of triangles, the points are deleted.'
+            msg = "Some of the selected points are out of triangles, the points are deleted."
             self.print_message(msg, self.reminder_color)
         for i in range(len(tri_vet_inds)):
             da_inds = tri_vet_inds[i]
-            t2 = [self.atlas_tri_data[da_inds[0]], self.atlas_tri_data[da_inds[1]],
-                  self.atlas_tri_data[da_inds[2]]]
-            t1 = [self.histo_tri_data[da_inds[0]], self.histo_tri_data[da_inds[1]],
-                  self.histo_tri_data[da_inds[2]]]
+            t2 = [
+                self.atlas_tri_data[da_inds[0]],
+                self.atlas_tri_data[da_inds[1]],
+                self.atlas_tri_data[da_inds[2]],
+            ]
+            t1 = [
+                self.histo_tri_data[da_inds[0]],
+                self.histo_tri_data[da_inds[1]],
+                self.histo_tri_data[da_inds[2]],
+            ]
             t1 = np.reshape(t1, (3, 2))
             t2 = np.reshape(t2, (3, 2))
             inds = np.where(loc == i)
             if len(inds) > 0:
                 pnts_inside = pnt[inds[0]]
                 res = warp_points(pnts_inside, t1, t2)
                 res_pnts[inds[0]] = res
@@ -2803,291 +3491,486 @@
         temp_pnts = np.where(img_data != 0)
         data = np.stack([temp_pnts[1], temp_pnts[0]], axis=1) + 0.5
         res_pnts = self.transfer_pnt(data, tri_vet_inds)
         return res_pnts
 
     def transform_accept(self):
         if not self.h2a_transferred:
-            self.print_message('Please transfer image to atlas first', self.error_message_color)
-            return
-        self.print_message('Transform accepted, start transferring...', self.normal_color)
+            self.print_message(
+                "Please transfer image to atlas first", self.error_message_color
+            )
+            return
+        self.print_message(
+            "Transform accepted, start transferring...", self.normal_color
+        )
         self.sidebar_tab_state(3)
         subdiv = cv2.Subdiv2D(self.atlas_rect)
-        self.atlas_tri_data = list(self.atlas_view.working_atlas.image_dict['tri_pnts'].data['pos'])
+        self.atlas_tri_data = list(
+            self.atlas_view.working_atlas.image_dict["tri_pnts"].data["pos"]
+        )
         for p in self.atlas_tri_data:
             subdiv.insert((int(p[0]), int(p[1])))
 
         tri_vet_inds = get_vertex_ind_in_triangle(subdiv)
 
-        if self.working_img_data['img-contour']:
-            self.print_message('Transferring contour...', self.normal_color)
-            res_pnts = self.transfer_pnt(np.asarray(self.working_img_data['img-contour']), tri_vet_inds)
-            self.working_atlas_data['atlas-contour'] = res_pnts.tolist()
-            self.atlas_view.working_atlas.image_dict['atlas-contour'].setData(
-                np.asarray(self.working_atlas_data['atlas-contour']))
-            vis_img = create_vis_img(self.atlas_view.slice_size, res_pnts, self.contour_color, vis_type='l')
-            res = cv2.resize(vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-contour', color=self.contour_color)
+        if self.working_img_data["img-contour"]:
+            self.print_message("Transferring contour...", self.normal_color)
+            res_pnts = self.transfer_pnt(
+                np.asarray(self.working_img_data["img-contour"]), tri_vet_inds
+            )
+            self.working_atlas_data["atlas-contour"] = res_pnts.tolist()
+            self.atlas_view.working_atlas.image_dict["atlas-contour"].setData(
+                np.asarray(self.working_atlas_data["atlas-contour"])
+            )
+            vis_img = create_vis_img(
+                self.atlas_view.slice_size, res_pnts, self.contour_color, vis_type="l"
+            )
+            res = cv2.resize(
+                vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="atlas-contour", color=self.contour_color
+            )
             # self.remove_single_link_related('img-contour')
-            self.working_img_data['img-contour'].clear()
-            self.print_message('Contour transferred.', self.normal_color)
+            self.working_img_data["img-contour"].clear()
+            self.print_message("Contour transferred.", self.normal_color)
 
-        if self.working_img_data['img-probe']:
-            res_pnts = self.transfer_pnt(np.asarray(self.working_img_data['img-probe']), tri_vet_inds)
-            self.working_atlas_data['atlas-probe'] = res_pnts.tolist()
-            self.atlas_view.working_atlas.image_dict['atlas-probe'].setData(
-                pos=np.asarray(self.working_atlas_data['atlas-probe']))
-            if len(self.working_atlas_data['atlas-probe']) > 1:
+        if self.working_img_data["img-probe"]:
+            res_pnts = self.transfer_pnt(
+                np.asarray(self.working_img_data["img-probe"]), tri_vet_inds
+            )
+            self.working_atlas_data["atlas-probe"] = res_pnts.tolist()
+            self.atlas_view.working_atlas.image_dict["atlas-probe"].setData(
+                pos=np.asarray(self.working_atlas_data["atlas-probe"])
+            )
+            if len(self.working_atlas_data["atlas-probe"]) > 1:
                 current_img = self.atlas_view.working_atlas.label_img.image.copy()
-                vis_points, msg = line_fit_2d(self.working_atlas_data['atlas-probe'], current_img)
-                self.atlas_view.working_atlas.image_dict['atlas-trajectory'].setData(vis_points)
-            vis_img = create_vis_img(self.atlas_view.slice_size, res_pnts, self.probe_color, vis_type='p')
-            res = cv2.resize(vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-probe', color=self.probe_color)
+                vis_points, msg = line_fit_2d(
+                    self.working_atlas_data["atlas-probe"], current_img
+                )
+                self.atlas_view.working_atlas.image_dict["atlas-trajectory"].setData(
+                    vis_points
+                )
+            vis_img = create_vis_img(
+                self.atlas_view.slice_size, res_pnts, self.probe_color, vis_type="p"
+            )
+            res = cv2.resize(
+                vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="atlas-probe", color=self.probe_color
+            )
             # self.remove_single_link_related('img-probe')
-            self.working_img_data['img-probe'].clear()
-            self.print_message('Probe transferred.', self.normal_color)
+            self.working_img_data["img-probe"].clear()
+            self.print_message("Probe transferred.", self.normal_color)
 
-        if self.working_img_data['img-drawing']:
-            res_pnts = self.transfer_pnt(np.asarray(self.working_img_data['img-drawing']), tri_vet_inds)
-            self.working_atlas_data['atlas-drawing'] = res_pnts.tolist()
+        if self.working_img_data["img-drawing"]:
+            res_pnts = self.transfer_pnt(
+                np.asarray(self.working_img_data["img-drawing"]), tri_vet_inds
+            )
+            self.working_atlas_data["atlas-drawing"] = res_pnts.tolist()
             if self.tool_box.is_closed:
                 self.set_atlas_pencil_closed_style()
             else:
                 self.clear_atlas_pencil_closed_style()
-            self.atlas_view.working_atlas.image_dict['atlas-drawing'].setData(
-                np.asarray(self.working_atlas_data['atlas-drawing']))
-            vis_img = create_vis_img(self.atlas_view.slice_size, res_pnts, self.pencil_color, 'l',
-                                     self.tool_box.is_closed)
-            res = cv2.resize(vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-drawing', color=self.pencil_color)
+            self.atlas_view.working_atlas.image_dict["atlas-drawing"].setData(
+                np.asarray(self.working_atlas_data["atlas-drawing"])
+            )
+            vis_img = create_vis_img(
+                self.atlas_view.slice_size,
+                res_pnts,
+                self.pencil_color,
+                "l",
+                self.tool_box.is_closed,
+            )
+            res = cv2.resize(
+                vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="atlas-drawing", color=self.pencil_color
+            )
             # self.remove_single_link_related('img-drawing')
-            self.working_img_data['img-drawing'].clear()
-            self.print_message('Drawing transferred.', self.normal_color)
+            self.working_img_data["img-drawing"].clear()
+            self.print_message("Drawing transferred.", self.normal_color)
 
-        if self.working_img_data['img-cells']:
-            res_pnts = self.transfer_pnt(np.asarray(self.working_img_data['img-cells']), tri_vet_inds)
-            self.working_atlas_data['atlas-cells'] = res_pnts.tolist()
-            self.working_atlas_data['cell_count'] = self.working_img_data['cell_count'].copy()
-            self.working_atlas_data['cell_size'] = self.working_img_data['cell_size'].copy()
-            self.working_atlas_data['cell_symbol'] = self.working_img_data['cell_symbol'].copy()
-            self.working_atlas_data['cell_layer_index'] = self.working_img_data['cell_layer_index'].copy()
-            self.atlas_view.working_atlas.image_dict['atlas-cells'].setData(
-                pos=np.asarray(self.working_atlas_data['atlas-cells']), symbol=self.working_img_data['cell_symbol'])
-            vis_img = create_vis_img(self.atlas_view.slice_size, res_pnts, self.cell_color, vis_type='p')
-            res = cv2.resize(vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-cells', color=self.cell_color)
+        if self.working_img_data["img-cells"]:
+            res_pnts = self.transfer_pnt(
+                np.asarray(self.working_img_data["img-cells"]), tri_vet_inds
+            )
+            self.working_atlas_data["atlas-cells"] = res_pnts.tolist()
+            self.working_atlas_data["cell_count"] = self.working_img_data[
+                "cell_count"
+            ].copy()
+            self.working_atlas_data["cell_size"] = self.working_img_data[
+                "cell_size"
+            ].copy()
+            self.working_atlas_data["cell_symbol"] = self.working_img_data[
+                "cell_symbol"
+            ].copy()
+            self.working_atlas_data["cell_layer_index"] = self.working_img_data[
+                "cell_layer_index"
+            ].copy()
+            self.atlas_view.working_atlas.image_dict["atlas-cells"].setData(
+                pos=np.asarray(self.working_atlas_data["atlas-cells"]),
+                symbol=self.working_img_data["cell_symbol"],
+            )
+            vis_img = create_vis_img(
+                self.atlas_view.slice_size, res_pnts, self.cell_color, vis_type="p"
+            )
+            res = cv2.resize(
+                vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="atlas-cells", color=self.cell_color
+            )
             # self.remove_single_link_related('img-cells')
-            self.working_img_data['img-cells'].clear()
-            self.working_img_data['cell_size'].clear()
-            self.working_img_data['cell_symbol'].clear()
-            self.working_img_data['cell_layer_index'].clear()
-            self.working_img_data['cell_count'] = [0 for _ in range(5)]
-            self.print_message('Cells transferred.', self.normal_color)
-
-        if self.working_img_data['img-virus'] is not None:
-            input_virus_img = self.working_img_data['img-virus'].copy()
-            img_wrap = np.zeros((self.atlas_view.slice_size[0], self.atlas_view.slice_size[1]), np.float32)
+            self.working_img_data["img-cells"].clear()
+            self.working_img_data["cell_size"].clear()
+            self.working_img_data["cell_symbol"].clear()
+            self.working_img_data["cell_layer_index"].clear()
+            self.working_img_data["cell_count"] = [0 for _ in range(5)]
+            self.print_message("Cells transferred.", self.normal_color)
+
+        if self.working_img_data["img-virus"] is not None:
+            input_virus_img = self.working_img_data["img-virus"].copy()
+            img_wrap = np.zeros(
+                (self.atlas_view.slice_size[0], self.atlas_view.slice_size[1]),
+                np.float32,
+            )
 
             for i in range(len(tri_vet_inds)):
                 da_inds = tri_vet_inds[i]
-                t2 = [self.atlas_tri_data[da_inds[0]], self.atlas_tri_data[da_inds[1]],
-                      self.atlas_tri_data[da_inds[2]]]
-                t1 = [self.histo_tri_data[da_inds[0]], self.histo_tri_data[da_inds[1]],
-                      self.histo_tri_data[da_inds[2]]]
+                t2 = [
+                    self.atlas_tri_data[da_inds[0]],
+                    self.atlas_tri_data[da_inds[1]],
+                    self.atlas_tri_data[da_inds[2]],
+                ]
+                t1 = [
+                    self.histo_tri_data[da_inds[0]],
+                    self.histo_tri_data[da_inds[1]],
+                    self.histo_tri_data[da_inds[2]],
+                ]
                 t1 = np.reshape(t1, (3, 2))
                 t2 = np.reshape(t2, (3, 2))
                 warp_triangle(input_virus_img, img_wrap, t1, t2, False)
 
             temp_pnts = np.where(img_wrap != 0)
             res_pnts = np.stack([temp_pnts[1], temp_pnts[0]], axis=1) + 0.5
 
-            self.working_atlas_data['atlas-virus'] = res_pnts.tolist()
-            self.atlas_view.working_atlas.image_dict['atlas-virus'].setData(
-                pos=np.asarray(self.working_atlas_data['atlas-virus']))
-            vis_img = create_vis_img(self.atlas_view.slice_size, res_pnts, self.virus_lut[1], 'p')
-            res = cv2.resize(vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-virus', color=self.virus_lut[1])
+            self.working_atlas_data["atlas-virus"] = res_pnts.tolist()
+            self.atlas_view.working_atlas.image_dict["atlas-virus"].setData(
+                pos=np.asarray(self.working_atlas_data["atlas-virus"])
+            )
+            vis_img = create_vis_img(
+                self.atlas_view.slice_size, res_pnts, self.virus_lut[1], "p"
+            )
+            res = cv2.resize(
+                vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="atlas-virus", color=self.virus_lut[1]
+            )
             # self.remove_single_link_related('img-virus')
-            self.working_img_data['img-virus'] = None
-            self.print_message('Virus transferred.', self.normal_color)
+            self.working_img_data["img-virus"] = None
+            self.print_message("Virus transferred.", self.normal_color)
 
-        self.print_message('All objects transferred.', self.normal_color)
+        self.print_message("All objects transferred.", self.normal_color)
 
     # ------------------------------------------------------------------
     #
     #              Image window - Image Processing
     #
     # ------------------------------------------------------------------
     def update_histo_tri_onside_data(self):
-        print('image_changed')
-        self.white_img = np.ones(self.image_view.img_size).astype('uint8')
+        print("image_changed")
+        self.white_img = np.ones(self.image_view.img_size).astype("uint8")
         if self.image_view.processing_img is not None:
             self.image_view.processing_img = None
         self.reset_corners_hist()
-        self.drawing_img = np.zeros((self.image_view.img_size[0], self.image_view.img_size[1], 3))
-        self.cell_img = np.zeros((self.image_view.img_size[0], self.image_view.img_size[1], 3))
-        self.probe_img = np.zeros((self.image_view.img_size[0], self.image_view.img_size[1], 3))
+        self.drawing_img = np.zeros(
+            (self.image_view.img_size[0], self.image_view.img_size[1], 3)
+        )
+        self.cell_img = np.zeros(
+            (self.image_view.img_size[0], self.image_view.img_size[1], 3)
+        )
+        self.probe_img = np.zeros(
+            (self.image_view.img_size[0], self.image_view.img_size[1], 3)
+        )
         self.delete_all_atlas_layer()
         self.action_list = []
         self.action_id = 0
 
-
     def img_stacks_clicked(self, pos):
         x = pos[0]
         y = pos[1]
-        print(self.image_view.img_stacks.image_list[0].image[int(y), int(x)])
+        # print(self.image_view.img_stacks.image_list[0].image[int(y), int(x)])
         if self.image_view.image_file is None:
             return
         # ------------------------- pencil
-        if self.tool_box.checkable_btn_dict['pencil_btn'].isChecked():
-            if not self.working_img_data['img-drawing']:
+        if self.tool_box.checkable_btn_dict["pencil_btn"].isChecked():
+            if not self.working_img_data["img-drawing"]:
                 self.is_pencil_allowed = True
-                self.working_img_data['img-drawing'].append([x, y])
-                self.image_view.img_stacks.image_dict['img-drawing'].setData(
-                    np.asarray(self.working_img_data['img-drawing']))
-                da_img = create_vis_img(self.image_view.img_size, self.working_img_data['img-drawing'],
-                                        self.pencil_color, 'p', False)
+                self.working_img_data["img-drawing"].append([x, y])
+                self.image_view.img_stacks.image_dict["img-drawing"].setData(
+                    np.asarray(self.working_img_data["img-drawing"])
+                )
+                da_img = create_vis_img(
+                    self.image_view.img_size,
+                    self.working_img_data["img-drawing"],
+                    self.pencil_color,
+                    "p",
+                    False,
+                )
                 self.drawing_img = da_img
-                res = cv2.resize(self.drawing_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                self.layer_ctrl.master_layers(res, layer_type='img-drawing', color=self.pencil_color)
+                res = cv2.resize(
+                    self.drawing_img,
+                    self.image_view.tb_size,
+                    interpolation=cv2.INTER_AREA,
+                )
+                self.layer_ctrl.master_layers(
+                    res, layer_type="img-drawing", color=self.pencil_color
+                )
                 # save action
-                current_data = {'data': self.working_img_data['img-drawing'].copy(),
-                                'closed': self.tool_box.is_closed}
-                self.save_current_action('pencil_btn', 'img-drawing', current_data, res)
+                current_data = {
+                    "data": self.working_img_data["img-drawing"].copy(),
+                    "closed": self.tool_box.is_closed,
+                }
+                self.save_current_action("pencil_btn", "img-drawing", current_data, res)
             else:
                 if self.is_pencil_allowed:
-                    print('not click on ')
-                    self.working_img_data['img-drawing'].append([x, y])
+                    print("not click on ")
+                    self.working_img_data["img-drawing"].append([x, y])
                     if self.tool_box.is_closed:
-                        self.working_img_data['img-drawing'].append([self.working_img_data['img-drawing'][0][0],
-                                                                     self.working_img_data['img-drawing'][0][1]])
+                        self.working_img_data["img-drawing"].append(
+                            [
+                                self.working_img_data["img-drawing"][0][0],
+                                self.working_img_data["img-drawing"][0][1],
+                            ]
+                        )
                         self.set_img_pencil_closed_style()
-                    self.image_view.img_stacks.image_dict['img-drawing'].setData(
-                        np.asarray(self.working_img_data['img-drawing']))
+                    self.image_view.img_stacks.image_dict["img-drawing"].setData(
+                        np.asarray(self.working_img_data["img-drawing"])
+                    )
                     self.is_pencil_allowed = False
-                    da_img = create_vis_img(self.image_view.img_size, self.working_img_data['img-drawing'],
-                                            self.pencil_color, 'l', self.tool_box.is_closed)
-                    res = cv2.resize(da_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                    self.layer_ctrl.master_layers(res, layer_type='img-drawing', color=self.pencil_color)
+                    da_img = create_vis_img(
+                        self.image_view.img_size,
+                        self.working_img_data["img-drawing"],
+                        self.pencil_color,
+                        "l",
+                        self.tool_box.is_closed,
+                    )
+                    res = cv2.resize(
+                        da_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                    )
+                    self.layer_ctrl.master_layers(
+                        res, layer_type="img-drawing", color=self.pencil_color
+                    )
                     # save action
-                    current_data = {'data': self.working_img_data['img-drawing'].copy(),
-                                    'closed': self.tool_box.is_closed}
-                    self.save_current_action('pencil_btn', 'img-drawing', current_data, res)
+                    current_data = {
+                        "data": self.working_img_data["img-drawing"].copy(),
+                        "closed": self.tool_box.is_closed,
+                    }
+                    self.save_current_action(
+                        "pencil_btn", "img-drawing", current_data, res
+                    )
                 else:
                     self.inactive_drawing()
                     self.clear_img_pencil_closed_style()
 
         # ------------------------- ruler
-        if self.tool_box.checkable_btn_dict['ruler_btn'].isChecked():
-            if len(self.working_img_data['ruler_path']) == 2:
+        if self.tool_box.checkable_btn_dict["ruler_btn"].isChecked():
+            if len(self.working_img_data["ruler_path"]) == 2:
                 self.inactive_img_ruler()
-                self.tool_box.ruler_length_label.setText('Length:')
+                self.tool_box.ruler_length_label.setText("Length:")
             else:
-                self.working_img_data['ruler_path'].append([x, y])
-                self.image_view.img_stacks.image_dict['ruler_path'].setData(
-                    np.asarray(self.working_img_data['ruler_path']))
+                self.working_img_data["ruler_path"].append([x, y])
+                self.image_view.img_stacks.image_dict["ruler_path"].setData(
+                    np.asarray(self.working_img_data["ruler_path"])
+                )
         # ------------------------- eraser
-        elif self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
-            if not self.layer_ctrl.layer_id or len(self.layer_ctrl.current_layer_index) > 1:
-                self.print_message('Eraser only works on one single layer.', self.error_message_color)
+        elif self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
+            if (
+                not self.layer_ctrl.layer_id
+                or len(self.layer_ctrl.current_layer_index) > 1
+            ):
+                self.print_message(
+                    "Eraser only works on one single layer.", self.error_message_color
+                )
                 return
             else:
                 r = self.tool_box.eraser_size_slider.value()
                 mask_img = np.zeros(self.image_view.img_size, dtype=np.uint8)
-                cv2.circle(mask_img, center=(int(x), int(y)), radius=r, color=255, thickness=-1)
+                cv2.circle(
+                    mask_img, center=(int(x), int(y)), radius=r, color=255, thickness=-1
+                )
                 mask_img = 255 - mask_img
 
-                da_link = self.layer_ctrl.layer_link[self.layer_ctrl.current_layer_index[0]]
-                if da_link in ['img-mask', 'img-virus']:
+                da_link = self.layer_ctrl.layer_link[
+                    self.layer_ctrl.current_layer_index[0]
+                ]
+                if da_link in ["img-mask", "img-virus"]:
                     temp = self.working_img_data[da_link].astype(np.uint8)
                     dst = cv2.bitwise_and(temp, temp, mask=mask_img)
                     self.image_view.img_stacks.image_dict[da_link].setImage(dst)
                     self.working_img_data[da_link] = dst
-                    vis_img = color_vis_img(dst, self.layer_ctrl.layer_color[self.layer_ctrl.current_layer_index[0]])
-                    res = cv2.resize(vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                    self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
+                    vis_img = color_vis_img(
+                        dst,
+                        self.layer_ctrl.layer_color[
+                            self.layer_ctrl.current_layer_index[0]
+                        ],
+                    )
+                    res = cv2.resize(
+                        vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                    )
+                    self.layer_ctrl.layer_list[
+                        self.layer_ctrl.current_layer_index[0]
+                    ].set_thumbnail_data(res)
                     # save action
-                    current_data = {'data': self.working_img_data[da_link].copy()}
-                    self.save_current_action('eraser_btn', da_link, current_data, res)
-                elif da_link == 'img-process':
+                    current_data = {"data": self.working_img_data[da_link].copy()}
+                    self.save_current_action("eraser_btn", da_link, current_data, res)
+                elif da_link == "img-process":
                     temp = self.image_view.processing_img.copy()
                     dst = cv2.bitwise_and(temp, temp, mask=mask_img)
-                    if self.image_view.image_file.pixel_type != 'rgb24':
+                    if self.image_view.image_file.pixel_type != "rgb24":
                         channel_hsv = self.image_view.image_file.hsv_colors
                         img_temp = merge_channels_into_single_img(dst, channel_hsv)
-                        input_img = cv2.normalize(img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
+                        input_img = cv2.normalize(
+                            img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U
+                        )
                     else:
                         input_img = dst.copy()
-                    res = cv2.resize(input_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                    self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
+                    res = cv2.resize(
+                        input_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                    )
+                    self.layer_ctrl.layer_list[
+                        self.layer_ctrl.current_layer_index[0]
+                    ].set_thumbnail_data(res)
                     self.image_view.img_stacks.set_data(dst)
                     self.image_view.processing_img = dst
-                    current_data = {'data': self.image_view.processing_img.copy()}
-                    self.save_current_action('eraser_btn', da_link, current_data, res)
+                    current_data = {"data": self.image_view.processing_img.copy()}
+                    self.save_current_action("eraser_btn", da_link, current_data, res)
                 else:
                     if not self.working_img_data[da_link]:
                         return
                     temp = np.asarray(self.working_img_data[da_link])
-                    remain_points, del_indexes = delete_points_inside_eraser(temp, np.array([x, y]), r)
+                    remain_points, del_indexes = delete_points_inside_eraser(
+                        temp, np.array([x, y]), r
+                    )
                     if remain_points is None:
                         return
                     self.working_img_data[da_link] = remain_points.tolist()
                     if self.working_img_data[da_link]:
-                        if da_link == 'img-contour':
-                            self.image_view.img_stacks.image_dict[da_link].setData(remain_points)
-                            da_color = self.layer_ctrl.layer_color[self.layer_ctrl.current_layer_index[0]]
-                            vis_img = create_vis_img(self.image_view.img_size, self.working_img_data[da_link],
-                                                     da_color, 'l')
-                            res = cv2.resize(vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                            self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
-                        elif da_link == 'img-drawing':
-                            self.image_view.img_stacks.image_dict[da_link].setData(remain_points)
-                            da_color = self.layer_ctrl.layer_color[self.layer_ctrl.current_layer_index[0]]
-                            vis_img = create_vis_img(self.image_view.img_size, self.working_img_data[da_link],
-                                                     da_color, 'l', self.tool_box.is_closed)
-                            res = cv2.resize(vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                            self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
+                        if da_link == "img-contour":
+                            self.image_view.img_stacks.image_dict[da_link].setData(
+                                remain_points
+                            )
+                            da_color = self.layer_ctrl.layer_color[
+                                self.layer_ctrl.current_layer_index[0]
+                            ]
+                            vis_img = create_vis_img(
+                                self.image_view.img_size,
+                                self.working_img_data[da_link],
+                                da_color,
+                                "l",
+                            )
+                            res = cv2.resize(
+                                vis_img,
+                                self.image_view.tb_size,
+                                interpolation=cv2.INTER_AREA,
+                            )
+                            self.layer_ctrl.layer_list[
+                                self.layer_ctrl.current_layer_index[0]
+                            ].set_thumbnail_data(res)
+                        elif da_link == "img-drawing":
+                            self.image_view.img_stacks.image_dict[da_link].setData(
+                                remain_points
+                            )
+                            da_color = self.layer_ctrl.layer_color[
+                                self.layer_ctrl.current_layer_index[0]
+                            ]
+                            vis_img = create_vis_img(
+                                self.image_view.img_size,
+                                self.working_img_data[da_link],
+                                da_color,
+                                "l",
+                                self.tool_box.is_closed,
+                            )
+                            res = cv2.resize(
+                                vis_img,
+                                self.image_view.tb_size,
+                                interpolation=cv2.INTER_AREA,
+                            )
+                            self.layer_ctrl.layer_list[
+                                self.layer_ctrl.current_layer_index[0]
+                            ].set_thumbnail_data(res)
                         else:
-                            if da_link == 'img-cells':
+                            if da_link == "img-cells":
                                 del_inds = np.sort(del_indexes)[::-1]
                                 for da_ind in del_inds:
-                                    del self.working_img_data['cell_size'][da_ind]
-                                    del self.working_img_data['cell_symbol'][da_ind]
-                                    del self.working_img_data['cell_layer_index'][da_ind]
-                                cell_layer_index = self.working_img_data['cell_layer_index'].copy()
-                                self.working_img_data['cell_count'] = get_cell_count(cell_layer_index)
-                                self.tool_box.update_cell_count_label(self.working_img_data['cell_count'])
+                                    del self.working_img_data["cell_size"][da_ind]
+                                    del self.working_img_data["cell_symbol"][da_ind]
+                                    del self.working_img_data["cell_layer_index"][
+                                        da_ind
+                                    ]
+                                cell_layer_index = self.working_img_data[
+                                    "cell_layer_index"
+                                ].copy()
+                                self.working_img_data["cell_count"] = get_cell_count(
+                                    cell_layer_index
+                                )
+                                self.tool_box.update_cell_count_label(
+                                    self.working_img_data["cell_count"]
+                                )
 
                                 self.image_view.img_stacks.image_dict[da_link].setData(
-                                    pos=remain_points, symbol=self.working_img_data['cell_symbol'])
+                                    pos=remain_points,
+                                    symbol=self.working_img_data["cell_symbol"],
+                                )
                             else:
-                                self.image_view.img_stacks.image_dict[da_link].setData(pos=remain_points)
-                            da_color = self.layer_ctrl.layer_color[self.layer_ctrl.current_layer_index[0]]
-                            vis_img = create_vis_img(self.image_view.img_size, self.working_img_data[da_link],
-                                                     da_color, 'p')
-                            res = cv2.resize(vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                            self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
+                                self.image_view.img_stacks.image_dict[da_link].setData(
+                                    pos=remain_points
+                                )
+                            da_color = self.layer_ctrl.layer_color[
+                                self.layer_ctrl.current_layer_index[0]
+                            ]
+                            vis_img = create_vis_img(
+                                self.image_view.img_size,
+                                self.working_img_data[da_link],
+                                da_color,
+                                "p",
+                            )
+                            res = cv2.resize(
+                                vis_img,
+                                self.image_view.tb_size,
+                                interpolation=cv2.INTER_AREA,
+                            )
+                            self.layer_ctrl.layer_list[
+                                self.layer_ctrl.current_layer_index[0]
+                            ].set_thumbnail_data(res)
                     else:
                         return
                     # save action
-                    if da_link == 'img-cells':
-                        current_data = {'data': self.working_img_data[da_link].copy(),
-                                        'size': self.working_img_data['cell_size'],
-                                        'symbol': self.working_img_data['cell_symbol'],
-                                        'index': self.working_img_data['cell_layer_index'],
-                                        'count': self.working_img_data['cell_count']}
-                    elif da_link == 'img-drawing':
-                        current_data = {'data': self.working_img_data[da_link].copy(),
-                                        'closed': self.tool_box.is_closed}
+                    if da_link == "img-cells":
+                        current_data = {
+                            "data": self.working_img_data[da_link].copy(),
+                            "size": self.working_img_data["cell_size"],
+                            "symbol": self.working_img_data["cell_symbol"],
+                            "index": self.working_img_data["cell_layer_index"],
+                            "count": self.working_img_data["cell_count"],
+                        }
+                    elif da_link == "img-drawing":
+                        current_data = {
+                            "data": self.working_img_data[da_link].copy(),
+                            "closed": self.tool_box.is_closed,
+                        }
                     else:
-                        current_data = {'data': self.working_img_data[da_link].copy()}
-                    self.save_current_action('eraser_btn', da_link, current_data, res)
+                        current_data = {"data": self.working_img_data[da_link].copy()}
+                    self.save_current_action("eraser_btn", da_link, current_data, res)
         # ------------------------- magic wand
-        elif self.tool_box.checkable_btn_dict['magic_wand_btn'].isChecked():
+        elif self.tool_box.checkable_btn_dict["magic_wand_btn"].isChecked():
             tol_val = float(self.tool_box.magic_tol_val.text())
             if self.image_view.processing_img is None:
                 src_img = self.image_view.current_img.copy()
             else:
                 src_img = self.image_view.processing_img.copy()
 
             # if self.image_view.image_file.is_rgb:
@@ -3099,257 +3982,360 @@
             # else:
             mask_img = self.white_img.copy()
             for i in range(self.image_view.image_file.n_channels):
                 if not self.image_view.channel_visible[i]:
                     continue
                 temp = src_img[:, :, i]
                 selected_color = temp[int(y), int(x)]
-                print(selected_color)
-                lower_val, upper_val = get_bound_color(selected_color, tol_val, self.image_view.image_file.level,
-                                                       'gray')
-                ret, thresh = cv2.threshold(temp, lower_val, upper_val, cv2.THRESH_BINARY)
-                mask_img = cv2.bitwise_and(mask_img, mask_img, mask=thresh.astype(np.uint8))
+                # print("selected color", selected_color)
+                lower_val, upper_val = get_bound_color(
+                    selected_color, tol_val, self.image_view.image_file.level, "gray"
+                )
+                ret, thresh = cv2.threshold(
+                    temp, lower_val, upper_val, cv2.THRESH_BINARY
+                )
+                mask_img = cv2.bitwise_and(
+                    mask_img, mask_img, mask=thresh.astype(np.uint8)
+                )
             modifiers = QApplication.keyboardModifiers()
             if modifiers == Qt.ShiftModifier:
-                if self.working_img_data['img-mask'] is None:
-                    self.working_img_data['img-mask'] = cv2.bitwise_or(mask_img, mask_img, mask=self.white_img)
+                if self.working_img_data["img-mask"] is None:
+                    self.working_img_data["img-mask"] = cv2.bitwise_or(
+                        mask_img, mask_img, mask=self.white_img
+                    )
                 else:
-                    self.working_img_data['img-mask'] = cv2.bitwise_or(self.working_img_data['img-mask'],
-                                                                       mask_img, mask=self.white_img)
+                    self.working_img_data["img-mask"] = cv2.bitwise_or(
+                        self.working_img_data["img-mask"], mask_img, mask=self.white_img
+                    )
             else:
-                self.working_img_data['img-mask'] = mask_img.copy()
+                self.working_img_data["img-mask"] = mask_img.copy()
 
             if self.kernel is not None:
-                temp = self.working_img_data['img-mask'].copy()
+                temp = self.working_img_data["img-mask"].copy()
                 open_img = cv2.morphologyEx(temp, cv2.MORPH_OPEN, self.kernel)
                 close_img = cv2.morphologyEx(open_img, cv2.MORPH_CLOSE, self.kernel)
-                self.working_img_data['img-mask'] = close_img.copy()
-            self.image_view.img_stacks.image_dict['img-mask'].setImage(self.working_img_data['img-mask'])
-            temp = color_vis_img(self.working_img_data['img-mask'], self.magic_wand_lut[1])
-            res = cv2.resize(temp, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='img-mask', color=self.magic_wand_lut[1])
+                self.working_img_data["img-mask"] = close_img.copy()
+            self.image_view.img_stacks.image_dict["img-mask"].setImage(
+                self.working_img_data["img-mask"]
+            )
+            temp = color_vis_img(
+                self.working_img_data["img-mask"], self.magic_wand_lut[1]
+            )
+            res = cv2.resize(
+                temp, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="img-mask", color=self.magic_wand_lut[1]
+            )
             # save action
-            current_data = {'data': self.working_img_data['img-mask'].copy()}
-            self.save_current_action('magic_wand_btn', 'img-mask', current_data, res)
+            current_data = {"data": self.working_img_data["img-mask"].copy()}
+            self.save_current_action("magic_wand_btn", "img-mask", current_data, res)
 
         # ------------------------- lasso
-        elif self.tool_box.checkable_btn_dict['lasso_btn'].isChecked():
-            if self.working_atlas_data['lasso_path']:
+        elif self.tool_box.checkable_btn_dict["lasso_btn"].isChecked():
+            if self.working_atlas_data["lasso_path"]:
                 self.inactive_slice_window_lasso()
             if self.img_lasso_is_closure:
                 self.inactive_lasso()
                 return
             new_pnt = np.array([x, y])
-            if len(self.working_img_data['lasso_path']) > 1:
-                dists = np.sum((np.asarray(self.working_img_data['lasso_path'][0]) - new_pnt) ** 2)
+            if len(self.working_img_data["lasso_path"]) > 1:
+                dists = np.sum(
+                    (np.asarray(self.working_img_data["lasso_path"][0]) - new_pnt) ** 2
+                )
             else:
                 dists = 1e5
             if dists < np.min(self.image_view.img_size) * 0.05:
-                self.working_img_data['lasso_path'].append(self.working_img_data['lasso_path'][0])
-                self.image_view.img_stacks.image_dict['lasso_path'].setPen(
-                    pg.mkPen(color='r', width=3, style=Qt.SolidLine))
+                self.working_img_data["lasso_path"].append(
+                    self.working_img_data["lasso_path"][0]
+                )
+                self.image_view.img_stacks.image_dict["lasso_path"].setPen(
+                    pg.mkPen(color="r", width=3, style=Qt.SolidLine)
+                )
                 self.img_lasso_is_closure = True
             else:
-                self.working_img_data['lasso_path'].append([x, y])
-            drawing_pnts = np.asarray(self.working_img_data['lasso_path'])
-            self.image_view.img_stacks.image_dict['lasso_path'].setData(drawing_pnts)
+                self.working_img_data["lasso_path"].append([x, y])
+            drawing_pnts = np.asarray(self.working_img_data["lasso_path"])
+            self.image_view.img_stacks.image_dict["lasso_path"].setData(drawing_pnts)
             # save action
-            current_data = {'data': self.working_img_data['lasso_path']}
-            self.save_current_action('lasso_btn', 'lasso_path', current_data, None)
+            current_data = {"data": self.working_img_data["lasso_path"]}
+            self.save_current_action("lasso_btn", "lasso_path", current_data, None)
         # ------------------------- triang -- triangulation pnts
-        elif self.tool_box.checkable_btn_dict['triang_btn'].isChecked():
+        elif self.tool_box.checkable_btn_dict["triang_btn"].isChecked():
             if self.a2h_transferred or self.h2a_transferred:
                 return
             self.histo_tri_inside_data.append([int(x), int(y)])
-            self.histo_tri_data = self.histo_tri_onside_data + self.histo_tri_inside_data
-            self.image_view.img_stacks.image_dict['tri_pnts'].setData(pos=np.asarray(self.histo_tri_data))
-            self.working_img_text.append(pg.TextItem(str(len(self.histo_tri_inside_data))))
+            self.histo_tri_data = (
+                self.histo_tri_onside_data + self.histo_tri_inside_data
+            )
+            self.image_view.img_stacks.image_dict["tri_pnts"].setData(
+                pos=np.asarray(self.histo_tri_data)
+            )
+            self.working_img_text.append(
+                pg.TextItem(str(len(self.histo_tri_inside_data)))
+            )
             self.working_img_text[-1].setColor(self.triangle_color)
             self.image_view.img_stacks.vb.addItem(self.working_img_text[-1])
             self.working_img_text[-1].setPos(x, y)
             if self.tool_box.triang_vis_btn.isChecked():
                 self.update_histo_tri_lines()
         # ------------------------- loc -- cell
-        elif self.tool_box.checkable_btn_dict['loc_btn'].isChecked():
+        elif self.tool_box.checkable_btn_dict["loc_btn"].isChecked():
             if self.tool_box.cell_selector_btn.isChecked():
-                if 'rgb' in self.image_view.image_file.pixel_type:
+                if "rgb" in self.image_view.image_file.pixel_type:
                     layer_ind = 0
                 else:
                     # only one layer is allowed to work on
-                    da_layer = [ind for ind in range(4) if self.image_view.channel_visible[ind]]
+                    da_layer = [
+                        ind for ind in range(4) if self.image_view.channel_visible[ind]
+                    ]
                     n_layers = len(da_layer)
                     if n_layers == 0:
-                        self.print_message('No image layer is visualised.', self.error_message_color)
+                        self.print_message(
+                            "No image layer is visualised.", self.error_message_color
+                        )
                         return
                     if n_layers > 1:
-                        self.print_message('Only one image layer is allowed to select cells.', self.error_message_color)
+                        self.print_message(
+                            "Only one image layer is allowed to select cells.",
+                            self.error_message_color,
+                        )
                         return
                     layer_ind = da_layer[0] + 1
 
-                self.working_img_data['img-cells'].append([x, y])
-                self.working_img_data['cell_size'].append(1)
-                self.working_img_data['cell_symbol'].append(self.cell_base_symbol[layer_ind])
-                self.working_img_data['cell_layer_index'].append(layer_ind)
-                self.working_img_data['cell_count'][layer_ind] += 1
-                self.tool_box.update_single_cell_count_label(self.working_img_data['cell_count'], layer_ind)
-
-                self.image_view.img_stacks.image_dict['img-cells'].setData(
-                    pos=np.asarray(self.working_img_data['img-cells']))
-                self.image_view.img_stacks.image_dict['img-cells'].setSymbol(
-                    symbol=self.working_img_data['cell_symbol'])
+                self.working_img_data["img-cells"].append([x, y])
+                self.working_img_data["cell_size"].append(1)
+                self.working_img_data["cell_symbol"].append(
+                    self.cell_base_symbol[layer_ind]
+                )
+                self.working_img_data["cell_layer_index"].append(layer_ind)
+                self.working_img_data["cell_count"][layer_ind] += 1
+                self.tool_box.update_single_cell_count_label(
+                    self.working_img_data["cell_count"], layer_ind
+                )
+
+                self.image_view.img_stacks.image_dict["img-cells"].setData(
+                    pos=np.asarray(self.working_img_data["img-cells"])
+                )
+                self.image_view.img_stacks.image_dict["img-cells"].setSymbol(
+                    symbol=self.working_img_data["cell_symbol"]
+                )
 
                 # print(self.image_view.img_stacks.image_dict['img-cells'].data)
                 # print(self.image_view.img_stacks.image_dict['img-cells'].)
 
+                cv2.circle(
+                    self.cell_img,
+                    (int(x), int(y)),
+                    radius=2,
+                    color=self.cell_color,
+                    thickness=-1,
+                )
+                res = cv2.resize(
+                    self.cell_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                )
+                self.layer_ctrl.master_layers(
+                    res, layer_type="img-cells", color=self.cell_color
+                )
+
+                current_data = {
+                    "data": self.working_img_data["img-cells"].copy(),
+                    "size": self.working_img_data["cell_size"].copy(),
+                    "symbol": self.working_img_data["cell_symbol"].copy(),
+                    "index": self.working_img_data["cell_layer_index"].copy(),
+                    "count": self.working_img_data["cell_count"].copy(),
+                }
 
-                cv2.circle(self.cell_img, (int(x), int(y)), radius=2, color=self.cell_color, thickness=-1)
-                res = cv2.resize(self.cell_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                self.layer_ctrl.master_layers(res, layer_type='img-cells', color=self.cell_color)
-
-                current_data = {'data': self.working_img_data['img-cells'].copy(),
-                                'size': self.working_img_data['cell_size'].copy(),
-                                'symbol': self.working_img_data['cell_symbol'].copy(),
-                                'index': self.working_img_data['cell_layer_index'].copy(),
-                                'count': self.working_img_data['cell_count'].copy()}
-
-                self.save_current_action('loc_btn', 'img-cells', current_data, res)
+                self.save_current_action("loc_btn", "img-cells", current_data, res)
             if self.tool_box.cell_aim_btn.isChecked():
-                self.working_img_data['img-blob'].append([x, y])
-                self.image_view.img_stacks.image_dict['img-blob'].setData(
-                    pos=np.asarray(self.working_img_data['img-blob']))
+                self.working_img_data["img-blob"].append([x, y])
+                self.image_view.img_stacks.image_dict["img-blob"].setData(
+                    pos=np.asarray(self.working_img_data["img-blob"])
+                )
         # ------------------------- probe
-        elif self.tool_box.checkable_btn_dict['probe_btn'].isChecked():
-            self.working_img_data['img-probe'].append([x, y])
-            self.image_view.img_stacks.image_dict['img-probe'].setData(
-                pos=np.asarray(self.working_img_data['img-probe']))
-            if len(self.working_img_data['img-probe']) > 1:
-                vis_points, msg = line_fit_2d(self.working_img_data['img-probe'])
+        elif self.tool_box.checkable_btn_dict["probe_btn"].isChecked():
+            self.working_img_data["img-probe"].append([x, y])
+            self.image_view.img_stacks.image_dict["img-probe"].setData(
+                pos=np.asarray(self.working_img_data["img-probe"])
+            )
+            if len(self.working_img_data["img-probe"]) > 1:
+                vis_points, msg = line_fit_2d(self.working_img_data["img-probe"])
                 if msg is not None:
                     self.print_message(msg, self.error_message_color)
                     return
-                self.image_view.img_stacks.image_dict['img-trajectory'].setData(vis_points)
-            vis_img = create_vis_img(self.image_view.img_size, self.working_img_data['img-probe'], self.probe_color, 'p')
-            res = cv2.resize(vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='img-probe', color=self.probe_color)
-            current_data = {'data': self.working_img_data['img-probe'].copy()}
-            self.save_current_action('probe_btn', 'img-probe', current_data, res)
+                self.image_view.img_stacks.image_dict["img-trajectory"].setData(
+                    vis_points
+                )
+            vis_img = create_vis_img(
+                self.image_view.img_size,
+                self.working_img_data["img-probe"],
+                self.probe_color,
+                "p",
+            )
+            res = cv2.resize(
+                vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="img-probe", color=self.probe_color
+            )
+            current_data = {"data": self.working_img_data["img-probe"].copy()}
+            self.save_current_action("probe_btn", "img-probe", current_data, res)
         else:
             return
 
     def img_stacks_hovered(self, event):
         if event.isExit():
             return
         try:
-            pos = (event.pos())
+            pos = event.pos()
         except (IndexError, AttributeError):
             return
         y = pos.y()
         x = pos.x()
-        if self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
+        if self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
             r = self.tool_box.eraser_size_slider.value()
             shp = self.image_view.current_img.shape
             if x - r > 0 and x + r < shp[1] and y - r > 0 and y + r < shp[0]:
-                if not self.image_view.img_stacks.image_dict['circle_follow'].isVisible():
+                if not self.image_view.img_stacks.image_dict[
+                    "circle_follow"
+                ].isVisible():
                     self.vis_eraser_symbol(True)
                 data = self.tool_box.circle.copy()
                 data[:, 0] = data[:, 0] + x
                 data[:, 1] = data[:, 1] + y
-                self.image_view.img_stacks.image_dict['circle_follow'].setData(data)
+                self.image_view.img_stacks.image_dict["circle_follow"].setData(data)
             else:
-                if self.image_view.img_stacks.image_dict['circle_follow'].isVisible():
+                if self.image_view.img_stacks.image_dict["circle_follow"].isVisible():
                     self.vis_eraser_symbol(False)
         # ------------------------- ruler
-        elif self.tool_box.checkable_btn_dict['ruler_btn'].isChecked():
-            if len(self.working_img_data['ruler_path']) == 1:
-                temp = self.working_img_data['ruler_path'].copy()
+        elif self.tool_box.checkable_btn_dict["ruler_btn"].isChecked():
+            if len(self.working_img_data["ruler_path"]) == 1:
+                temp = self.working_img_data["ruler_path"].copy()
                 temp.append([x, y])
-                self.image_view.img_stacks.image_dict['ruler_path'].setData(np.asarray(temp))
+                self.image_view.img_stacks.image_dict["ruler_path"].setData(
+                    np.asarray(temp)
+                )
         # ------------------------ pencil
-        elif self.tool_box.checkable_btn_dict['pencil_btn'].isChecked():
+        elif self.tool_box.checkable_btn_dict["pencil_btn"].isChecked():
             if self.is_pencil_allowed:
-                self.working_img_data['img-drawing'].append([x, y])
-                self.image_view.img_stacks.image_dict['img-drawing'].setData(
-                    np.asarray(self.working_img_data['img-drawing']))
-        msg = 'Histological image coordinates: {}, {}'.format(round(x, 3), round(y, 3))
+                self.working_img_data["img-drawing"].append([x, y])
+                self.image_view.img_stacks.image_dict["img-drawing"].setData(
+                    np.asarray(self.working_img_data["img-drawing"])
+                )
+        msg = "Histological image coordinates: {}, {}".format(round(x, 3), round(y, 3))
         self.print_message(msg, self.normal_color)
 
     def img_stacks_key_pressed(self, action):
         if len(self.layer_ctrl.current_layer_index) != 1:
-            msg = 'Delete only works on single layer. Multiple or No layer is selected.'
+            msg = "Delete only works on single layer. Multiple or No layer is selected."
             self.print_message(msg, self.reminder_color)
             return
         da_link = self.layer_ctrl.layer_link[self.layer_ctrl.current_layer_index[0]]
 
-        if action == 'delete':
+        if action == "delete":
             if self.img_lasso_is_closure:
                 mask = np.zeros(self.image_view.img_size, dtype=np.uint8)
-                pts = np.int32(self.working_img_data['lasso_path'])
+                pts = np.int32(self.working_img_data["lasso_path"])
                 cv2.fillPoly(mask, pts=[pts], color=255)
                 if not self.tool_box.remove_inside:
                     mask = 255 - mask
-                if da_link == 'img-mask':
-                    dst = cv2.bitwise_and(self.working_img_data[da_link], self.working_img_data[da_link], mask=mask)
+                if da_link == "img-mask":
+                    dst = cv2.bitwise_and(
+                        self.working_img_data[da_link],
+                        self.working_img_data[da_link],
+                        mask=mask,
+                    )
                     self.image_view.img_stacks.image_dict[da_link].setImage(dst)
                     self.working_img_data[da_link] = dst
-                    vis_img = color_vis_img(dst, self.layer_ctrl.layer_color[self.layer_ctrl.current_layer_index[0]])
-                    res = cv2.resize(vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                    current_data = {'data': self.working_img_data[da_link].copy()}
-                    self.save_current_action('delete', da_link, current_data, res)
-                elif da_link == 'img-process':
-                    dst = cv2.bitwise_and(self.image_view.processing_img, self.image_view.processing_img, mask=mask)
+                    vis_img = color_vis_img(
+                        dst,
+                        self.layer_ctrl.layer_color[
+                            self.layer_ctrl.current_layer_index[0]
+                        ],
+                    )
+                    res = cv2.resize(
+                        vis_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                    )
+                    current_data = {"data": self.working_img_data[da_link].copy()}
+                    self.save_current_action("delete", da_link, current_data, res)
+                elif da_link == "img-process":
+                    dst = cv2.bitwise_and(
+                        self.image_view.processing_img,
+                        self.image_view.processing_img,
+                        mask=mask,
+                    )
                     self.image_view.img_stacks.set_data(dst)
                     self.image_view.processing_img = dst
-                    if self.image_view.image_file.pixel_type != 'rgb24':
+                    if self.image_view.image_file.pixel_type != "rgb24":
                         channel_hsv = self.image_view.image_file.hsv_colors
                         img_temp = merge_channels_into_single_img(dst, channel_hsv)
-                        input_img = cv2.normalize(img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
+                        input_img = cv2.normalize(
+                            img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U
+                        )
                     else:
                         input_img = dst.copy()
-                    res = cv2.resize(input_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                    current_data = {'data': self.image_view.processing_img.copy()}
-                    self.save_current_action('delete', da_link, current_data, res)
+                    res = cv2.resize(
+                        input_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                    )
+                    current_data = {"data": self.image_view.processing_img.copy()}
+                    self.save_current_action("delete", da_link, current_data, res)
                 else:
-                    msg = 'Lasso Tool only works on process layer, slice layer and mask layer.'
+                    msg = "Lasso Tool only works on process layer, slice layer and mask layer."
                     self.print_message(msg, self.reminder_color)
                     return
             else:
-                if self.working_img_data['img-mask'] is None or da_link != 'img-process':
+                if (
+                    self.working_img_data["img-mask"] is None
+                    or da_link != "img-process"
+                ):
                     return
-                mask = self.working_img_data['img-mask'].copy()
+                mask = self.working_img_data["img-mask"].copy()
                 mask = 255 - mask * 255
                 temp = self.image_view.processing_img.copy()
                 dst = cv2.bitwise_and(temp, temp, mask=mask)
                 input_img = dst.copy()
                 self.image_view.img_stacks.set_data(dst)
                 self.image_view.processing_img = dst
-                if self.image_view.image_file.pixel_type != 'rgb24':
+                if self.image_view.image_file.pixel_type != "rgb24":
                     channel_hsv = self.image_view.image_file.hsv_colors
                     img_temp = merge_channels_into_single_img(dst, channel_hsv)
-                    input_img = cv2.normalize(img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
-                res = cv2.resize(input_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA)
-                self.remove_single_link_related('img-mask')
-                current_data = {'data': self.image_view.processing_img.copy()}
-                self.save_current_action('delete', da_link, current_data, res)
-
-            self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
+                    input_img = cv2.normalize(
+                        img_temp, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U
+                    )
+                res = cv2.resize(
+                    input_img, self.image_view.tb_size, interpolation=cv2.INTER_AREA
+                )
+                self.remove_single_link_related("img-mask")
+                current_data = {"data": self.image_view.processing_img.copy()}
+                self.save_current_action("delete", da_link, current_data, res)
+
+            self.layer_ctrl.layer_list[
+                self.layer_ctrl.current_layer_index[0]
+            ].set_thumbnail_data(res)
 
     def hist_window_tri_pnts_moving(self, ev_obj):
         ev = ev_obj[0]
         ind = ev_obj[1]
         da_num = (self.np_onside - 1) * 4
         if ind < da_num:
             return
 
         if self.a2h_transferred:
             old_pnts = self.histo_tri_data.copy()
             new_pnts = self.histo_tri_data.copy()
-            da_new_pnt = self.image_view.img_stacks.image_dict['tri_pnts'].data['pos'][ind].copy()
+            da_new_pnt = (
+                self.image_view.img_stacks.image_dict["tri_pnts"]
+                .data["pos"][ind]
+                .copy()
+            )
             new_pnts[ind] = [int(da_new_pnt[0]), int(da_new_pnt[1])]
 
-            img_overlay = self.image_view.img_stacks.image_dict['img-overlay'].image.copy()
+            img_overlay = self.image_view.img_stacks.image_dict[
+                "img-overlay"
+            ].image.copy()
             img_wrap = img_overlay.copy()
 
             img_size = img_wrap.shape[:2]
             rect = (0, 0, img_size[1], img_size[0])
 
             subdiv = cv2.Subdiv2D(rect)
             for p in new_pnts:
@@ -3360,146 +4346,192 @@
                 da_inds = tri_vet_inds[i]
                 # if ind not in da_inds:
                 #     continue
                 t1 = [old_pnts[da_inds[0]], old_pnts[da_inds[1]], old_pnts[da_inds[2]]]
                 t2 = [new_pnts[da_inds[0]], new_pnts[da_inds[1]], new_pnts[da_inds[2]]]
                 t1 = np.reshape(t1, (3, 2))
                 t2 = np.reshape(t2, (3, 2))
-                warp_triangle(img_overlay, img_wrap,  t1, t2, True)
-            self.image_view.img_stacks.image_dict['img-overlay'].setImage(img_wrap)
+                warp_triangle(img_overlay, img_wrap, t1, t2, True)
+            self.image_view.img_stacks.image_dict["img-overlay"].setImage(img_wrap)
             self.histo_tri_data = new_pnts
         else:
-            da_new_pnt = self.image_view.img_stacks.image_dict['tri_pnts'].data['pos'][ind].copy()
+            da_new_pnt = (
+                self.image_view.img_stacks.image_dict["tri_pnts"]
+                .data["pos"][ind]
+                .copy()
+            )
             self.histo_tri_data[ind] = [int(da_new_pnt[0]), int(da_new_pnt[1])]
-        self.histo_tri_inside_data[ind - da_num] = [int(da_new_pnt[0]), int(da_new_pnt[1])]
+        self.histo_tri_inside_data[ind - da_num] = [
+            int(da_new_pnt[0]),
+            int(da_new_pnt[1]),
+        ]
         self.working_img_text[ind - da_num].setPos(da_new_pnt[0], da_new_pnt[1])
         if self.tool_box.triang_vis_btn.isChecked():
             self.update_histo_tri_lines()
 
     def img_probe_pnts_clicked(self, points, ev):
-        if not self.tool_box.checkable_btn_dict['eraser_btn'].isChecked() or not self.working_img_data['img-probe']:
+        if (
+            not self.tool_box.checkable_btn_dict["eraser_btn"].isChecked()
+            or not self.working_img_data["img-probe"]
+        ):
             return
         clicked_ind = ev[0].index()
-        del self.working_img_data['img-probe'][clicked_ind]
-        self.image_view.img_stacks.image_dict['img-probe'].setData(np.asarray(self.working_img_data['img-probe']))
-
+        del self.working_img_data["img-probe"][clicked_ind]
+        self.image_view.img_stacks.image_dict["img-probe"].setData(
+            np.asarray(self.working_img_data["img-probe"])
+        )
 
     def img_cell_pnts_clicked(self, points, ev):
-        if not self.tool_box.checkable_btn_dict['eraser_btn'].isChecked() or not self.working_img_data['img-cells']:
+        if (
+            not self.tool_box.checkable_btn_dict["eraser_btn"].isChecked()
+            or not self.working_img_data["img-cells"]
+        ):
             return
         clicked_ind = ev[0].index()
-        layer_ind = self.working_img_data['cell_layer_index'][clicked_ind]
-        self.working_img_data['cell_count'][layer_ind] -= 1
-        self.tool_box.update_single_cell_count_label(self.working_img_data['cell_count'], layer_ind)
-        del self.working_img_data['img-cells'][clicked_ind]
-        del self.working_img_data['cell_symbol'][clicked_ind]
-        del self.working_img_data['cell_size'][clicked_ind]
-        del self.working_img_data['cell_layer_index'][clicked_ind]
-        self.image_view.img_stacks.image_dict['img-cells'].setData(pos=np.asarray(self.working_img_data['img-cells']),
-                                                     symbol=self.working_img_data['cell_symbol'])
+        layer_ind = self.working_img_data["cell_layer_index"][clicked_ind]
+        self.working_img_data["cell_count"][layer_ind] -= 1
+        self.tool_box.update_single_cell_count_label(
+            self.working_img_data["cell_count"], layer_ind
+        )
+        del self.working_img_data["img-cells"][clicked_ind]
+        del self.working_img_data["cell_symbol"][clicked_ind]
+        del self.working_img_data["cell_size"][clicked_ind]
+        del self.working_img_data["cell_layer_index"][clicked_ind]
+        self.image_view.img_stacks.image_dict["img-cells"].setData(
+            pos=np.asarray(self.working_img_data["img-cells"]),
+            symbol=self.working_img_data["cell_symbol"],
+        )
 
     def hist_window_tri_pnts_clicked(self, ev):
-        if not self.tool_box.checkable_btn_dict['eraser_btn'].isChecked() or not self.histo_tri_data:
+        if (
+            not self.tool_box.checkable_btn_dict["eraser_btn"].isChecked()
+            or not self.histo_tri_data
+        ):
             return
         if self.a2h_transferred or self.h2a_transferred:
             return
         self.inactive_lasso()
         clicked_ind = ev[1]
         num = (self.np_onside - 1) * 4
         if clicked_ind < num:
             return
         self.image_view.img_stacks.vb.removeItem(self.working_img_text[-1])
         del self.working_img_text[-1]
         del self.histo_tri_data[clicked_ind]
         del self.histo_tri_inside_data[clicked_ind - num]
-        self.image_view.img_stacks.image_dict['tri_pnts'].setData(pos=np.asarray(self.histo_tri_data))
+        self.image_view.img_stacks.image_dict["tri_pnts"].setData(
+            pos=np.asarray(self.histo_tri_data)
+        )
         for i in range(len(self.working_img_text)):
             pnt_id = i + num
-            self.working_img_text[i].setPos(self.histo_tri_data[pnt_id][0], self.histo_tri_data[pnt_id][1])
+            self.working_img_text[i].setPos(
+                self.histo_tri_data[pnt_id][0], self.histo_tri_data[pnt_id][1]
+            )
         if self.tool_box.triang_vis_btn.isChecked():
             self.update_histo_tri_lines()
 
     # ------------------------------------------------------------------
     #
     #                       Atlas Window Related
     #
     # ------------------------------------------------------------------
     def slice_stack_hovered(self, event):
         if event.isExit():
             return
         try:
-            pos = (event.pos())
+            pos = event.pos()
         except (IndexError, AttributeError):
             return
         y = pos.y()
         x = pos.x()
-        if self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
+        if self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
             r = self.tool_box.eraser_size_slider.value()
             shp = self.atlas_view.slice_stack.base_layer.image.shape
             if x - r > 0 and x + r < shp[1] and y - r > 0 and y + r < shp[0]:
-                if not self.atlas_view.slice_stack.image_dict['circle_follow'].isVisible():
+                if not self.atlas_view.slice_stack.image_dict[
+                    "circle_follow"
+                ].isVisible():
                     self.vis_eraser_symbol(True)
                 data = self.tool_box.circle.copy()
                 data[:, 0] = data[:, 0] + x
                 data[:, 1] = data[:, 1] + y
-                self.atlas_view.slice_stack.image_dict['circle_follow'].setData(data)
+                self.atlas_view.slice_stack.image_dict["circle_follow"].setData(data)
             else:
-                if self.atlas_view.slice_stack.image_dict['circle_follow'].isVisible():
+                if self.atlas_view.slice_stack.image_dict["circle_follow"].isVisible():
                     self.vis_eraser_symbol(False)
-        elif self.tool_box.checkable_btn_dict['ruler_btn'].isChecked():
-            if len(self.working_atlas_data['ruler_path']) == 1:
-                temp = self.working_atlas_data['ruler_path'].copy()
+        elif self.tool_box.checkable_btn_dict["ruler_btn"].isChecked():
+            if len(self.working_atlas_data["ruler_path"]) == 1:
+                temp = self.working_atlas_data["ruler_path"].copy()
                 temp.append([x, y])
-                self.atlas_view.slice_stack.image_dict['ruler_path'].setData(np.asarray(temp))
+                self.atlas_view.slice_stack.image_dict["ruler_path"].setData(
+                    np.asarray(temp)
+                )
         # ---------  probe  ----------
-        elif self.tool_box.checkable_btn_dict['probe_btn'].isChecked():
+        elif self.tool_box.checkable_btn_dict["probe_btn"].isChecked():
             if self.image_view.image_file is None:
-                if len(self.working_atlas_data['atlas-probe']) == 1:
-                    points2d = self.working_atlas_data['atlas-probe'].copy()
+                if len(self.working_atlas_data["atlas-probe"]) == 1:
+                    points2d = self.working_atlas_data["atlas-probe"].copy()
                     points2d.append([x, y])
                     if self.multi_shanks and self.valid_multi_settings:
                         base_loc_1d = get_pre_multi_shank_vis_base(
-                            self.multi_settings.x_vals, self.multi_settings.y_vals)
+                            self.multi_settings.x_vals, self.multi_settings.y_vals
+                        )
                     else:
                         base_loc_1d = np.array([0])
 
-                    start_pnt, end_pnt = self.atlas_view.get_pre_vis_data_for_slice_atlas(
-                        np.asarray(points2d), base_loc_1d)
+                    (
+                        start_pnt,
+                        end_pnt,
+                    ) = self.atlas_view.get_pre_vis_data_for_slice_atlas(
+                        np.asarray(points2d), base_loc_1d
+                    )
                     self.atlas_view.set_pre_vis_data(start_pnt, end_pnt)
 
         if not self.atlas_view.slice_info_ready:
-            msg = 'Atlas Slice Image coordinates: {} px, {} px'.format(int(x), int(y))
+            msg = "Atlas Slice Image coordinates: {} px, {} px".format(int(x), int(y))
         else:
             xc, yc, zc = self.atlas_view.get_slice_coords(np.asarray([[x, y]]))
-            msg = 'Atlas Slice Image coordinates: {} um, {} um, {} um w.r.t. Bregma.'.format(
-                round(xc[0], 2), round(yc[0], 2), round(zc[0], 2))
+            msg = "Atlas Slice Image coordinates: {} um, {} um, {} um w.r.t. Bregma.".format(
+                round(xc[0], 2), round(yc[0], 2), round(zc[0], 2)
+            )
         self.print_message(msg, self.normal_color)
 
     def coronal_slice_stacks_hovered(self, pos):
         y = pos.y()
         x = pos.x()
 
         if self.num_windows != 4:
-            if self.tool_box.checkable_btn_dict['ruler_btn'].isChecked():
-                if len(self.working_atlas_data['ruler_path']) == 1:
-                    temp = self.working_atlas_data['ruler_path'].copy()
+            if self.tool_box.checkable_btn_dict["ruler_btn"].isChecked():
+                if len(self.working_atlas_data["ruler_path"]) == 1:
+                    temp = self.working_atlas_data["ruler_path"].copy()
                     temp.append([x, y])
-                    self.atlas_view.cimg.image_dict['ruler_path'].setData(np.asarray(temp))
-
-            if self.tool_box.checkable_btn_dict['probe_btn'].isChecked() and self.image_view.image_file is None:
-                if len(self.working_atlas_data['atlas-probe']) == 1:
-                    points2d = self.working_atlas_data['atlas-probe'].copy()
+                    self.atlas_view.cimg.image_dict["ruler_path"].setData(
+                        np.asarray(temp)
+                    )
+
+            if (
+                self.tool_box.checkable_btn_dict["probe_btn"].isChecked()
+                and self.image_view.image_file is None
+            ):
+                if len(self.working_atlas_data["atlas-probe"]) == 1:
+                    points2d = self.working_atlas_data["atlas-probe"].copy()
                     points2d.append([x, y])
                     if self.multi_shanks and self.valid_multi_settings:
                         base_loc_1d = get_pre_multi_shank_vis_base(
-                            self.multi_settings.x_vals, self.multi_settings.y_vals)
+                            self.multi_settings.x_vals, self.multi_settings.y_vals
+                        )
                     else:
                         base_loc_1d = np.array([0])
 
-                    start_pnt, end_pnt = self.atlas_view.get_pre_vis_data_for_volume_atlas(np.asarray(points2d), base_loc_1d)
+                    (
+                        start_pnt,
+                        end_pnt,
+                    ) = self.atlas_view.get_pre_vis_data_for_volume_atlas(
+                        np.asarray(points2d), base_loc_1d
+                    )
                     self.atlas_view.set_pre_vis_data(start_pnt, end_pnt)
 
         c_id = self.atlas_view.current_coronal_index
         s_id = self.atlas_view.current_sagital_index
         h_id = self.atlas_view.atlas_size[0] - self.atlas_view.current_horizontal_index
 
         o_rot = np.array([h_id, s_id, c_id])
@@ -3510,59 +4542,82 @@
 
         da_label = self.atlas_view.cimg.label_img.image.copy()
         da_id = da_label[int(y), int(x)]
 
         vox_val = self.atlas_view.cimg.img.image[int(y), int(x)]
 
         if vox_val != 0:
-            coords = np.round((da_pnt - np.ravel(self.atlas_view.Bregma)) * self.atlas_view.vox_size_um, 2)
+            coords = np.round(
+                (da_pnt - np.ravel(self.atlas_view.Bregma))
+                * self.atlas_view.vox_size_um,
+                2,
+            )
             da_vec = self.atlas_view.cimg.img.image[:, int(da_pnt[1])]
             valid_inds = np.where(da_vec != 0)[0]
             # self.atlas_view.cimg.image_dict['atlas-probe'].setData(pos=[[x, valid_inds[0]]])
-            dv_val = np.round((valid_inds[0] - da_pnt[0]) * self.atlas_view.vox_size_um, 2)
-            pstr = 'Atlas voxel:({}, {}, {}), ML:{}um, AP:{}um, DV:{}um w.r.t Bregma, DV:{}um w.r.t Surface: {} '.format(
-                int(da_pnt[1]), int(da_pnt[2]), int(self.atlas_view.atlas_size[0] - da_pnt[0]),
-                coords[1], coords[2], -coords[0], dv_val, self.atlas_view.label_tree.describe(da_id))
+            dv_val = np.round(
+                (valid_inds[0] - da_pnt[0]) * self.atlas_view.vox_size_um, 2
+            )
+            pstr = "Atlas voxel:({}, {}, {}), ML:{}um, AP:{}um, DV:{}um w.r.t Bregma, DV:{}um w.r.t Surface: {} ".format(
+                int(da_pnt[1]),
+                int(da_pnt[2]),
+                int(self.atlas_view.atlas_size[0] - da_pnt[0]),
+                coords[1],
+                coords[2],
+                -coords[0],
+                dv_val,
+                self.atlas_view.label_tree.describe(da_id),
+            )
             self.print_message(pstr, self.normal_color)
 
             if self.atlas_view.navigation_btn.isChecked():
                 self.atlas_view.cimg.v_line.setPos(x)
                 self.atlas_view.cimg.h_line.setPos(y)
                 self.atlas_view.simg.v_line.setPos(c_id)
                 self.atlas_view.simg.h_line.setPos(y)
                 self.atlas_view.himg.v_line.setPos(c_id)
                 self.atlas_view.himg.h_line.setPos(x)
 
                 self.atlas_view.spage_ctrl.set_val(x)
-                self.atlas_view.hpage_ctrl.set_val(self.atlas_view.atlas_size[0] - int(y))
+                self.atlas_view.hpage_ctrl.set_val(
+                    self.atlas_view.atlas_size[0] - int(y)
+                )
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     def sagital_slice_stacks_hovered(self, pos):
         y = pos.y()
         x = pos.x()
 
         if self.num_windows != 4:
-            if self.tool_box.checkable_btn_dict['ruler_btn'].isChecked():
-                if len(self.working_atlas_data['ruler_path']) == 1:
-                    temp = self.working_atlas_data['ruler_path'].copy()
+            if self.tool_box.checkable_btn_dict["ruler_btn"].isChecked():
+                if len(self.working_atlas_data["ruler_path"]) == 1:
+                    temp = self.working_atlas_data["ruler_path"].copy()
                     temp.append([x, y])
-                    self.atlas_view.simg.image_dict['ruler_path'].setData(np.asarray(temp))
-
-            if self.tool_box.checkable_btn_dict['probe_btn'].isChecked() and self.image_view.image_file is None:
-                if len(self.working_atlas_data['atlas-probe']) == 1:
-                    points2d = self.working_atlas_data['atlas-probe'].copy()
+                    self.atlas_view.simg.image_dict["ruler_path"].setData(
+                        np.asarray(temp)
+                    )
+
+            if (
+                self.tool_box.checkable_btn_dict["probe_btn"].isChecked()
+                and self.image_view.image_file is None
+            ):
+                if len(self.working_atlas_data["atlas-probe"]) == 1:
+                    points2d = self.working_atlas_data["atlas-probe"].copy()
                     points2d.append([x, y])
                     if self.multi_shanks and self.valid_multi_settings:
                         base_loc_1d = get_pre_multi_shank_vis_base(
-                            self.multi_settings.x_vals, self.multi_settings.y_vals)
+                            self.multi_settings.x_vals, self.multi_settings.y_vals
+                        )
                     else:
                         base_loc_1d = np.array([0])
 
-                    start_pnt, end_pnt = self.atlas_view.get_pre_vis_data(np.asarray(points2d), base_loc_1d)
+                    start_pnt, end_pnt = self.atlas_view.get_pre_vis_data(
+                        np.asarray(points2d), base_loc_1d
+                    )
                     self.atlas_view.set_pre_vis_data(start_pnt, end_pnt)
 
         c_id = self.atlas_view.current_coronal_index
         s_id = self.atlas_view.current_sagital_index
         h_id = self.atlas_view.atlas_size[0] - self.atlas_view.current_horizontal_index
 
         o_rot = np.array([h_id, s_id, c_id])
@@ -3573,58 +4628,81 @@
 
         da_label = self.atlas_view.simg.label_img.image.copy()
         da_id = da_label[int(y), int(x)]
 
         vox_val = self.atlas_view.simg.img.image[int(y), int(x)]
 
         if vox_val != 0:
-            coords = np.round((da_pnt - np.ravel(self.atlas_view.Bregma)) * self.atlas_view.vox_size_um, 2)
+            coords = np.round(
+                (da_pnt - np.ravel(self.atlas_view.Bregma))
+                * self.atlas_view.vox_size_um,
+                2,
+            )
             da_vec = self.atlas_view.simg.img.image[:, int(da_pnt[2])]
             valid_inds = np.where(da_vec != 0)[0]
             # self.atlas_view.simg.image_dict['atlas-probe'].setData(pos=[[x, valid_inds[0]]])
-            dv_val = np.round((valid_inds[0] - da_pnt[0]) * self.atlas_view.vox_size_um, 2)
-            pstr = 'Atlas voxel:({}, {}, {}), ML:{}um, AP:{}um, DV:{}um w.r.t Bregma, DV:{}um w.r.t Surface: {} '.format(
-                int(da_pnt[1]), int(da_pnt[2]), int(self.atlas_view.atlas_size[0] - da_pnt[0]),
-                coords[1], coords[2], -coords[0], dv_val, self.atlas_view.label_tree.describe(da_id))
+            dv_val = np.round(
+                (valid_inds[0] - da_pnt[0]) * self.atlas_view.vox_size_um, 2
+            )
+            pstr = "Atlas voxel:({}, {}, {}), ML:{}um, AP:{}um, DV:{}um w.r.t Bregma, DV:{}um w.r.t Surface: {} ".format(
+                int(da_pnt[1]),
+                int(da_pnt[2]),
+                int(self.atlas_view.atlas_size[0] - da_pnt[0]),
+                coords[1],
+                coords[2],
+                -coords[0],
+                dv_val,
+                self.atlas_view.label_tree.describe(da_id),
+            )
             self.print_message(pstr, self.normal_color)
 
             if self.atlas_view.navigation_btn.isChecked():
                 self.atlas_view.simg.v_line.setPos(x)
                 self.atlas_view.simg.h_line.setPos(y)
                 self.atlas_view.cimg.v_line.setPos(s_id)
                 self.atlas_view.cimg.h_line.setPos(y)
                 self.atlas_view.himg.v_line.setPos(x)
                 self.atlas_view.himg.h_line.setPos(s_id)
 
                 self.atlas_view.cpage_ctrl.set_val(x)
-                self.atlas_view.hpage_ctrl.set_val(self.atlas_view.atlas_size[0] - int(y))
+                self.atlas_view.hpage_ctrl.set_val(
+                    self.atlas_view.atlas_size[0] - int(y)
+                )
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     def horizontal_slice_stacks_hovered(self, pos):
         y = pos.y()
         x = pos.x()
 
         if self.num_windows != 4:
-            if self.tool_box.checkable_btn_dict['ruler_btn'].isChecked():
-                if len(self.working_atlas_data['ruler_path']) == 1:
-                    temp = self.working_atlas_data['ruler_path'].copy()
+            if self.tool_box.checkable_btn_dict["ruler_btn"].isChecked():
+                if len(self.working_atlas_data["ruler_path"]) == 1:
+                    temp = self.working_atlas_data["ruler_path"].copy()
                     temp.append([x, y])
-                    self.atlas_view.himg.image_dict['ruler_path'].setData(np.asarray(temp))
-
-            if self.tool_box.checkable_btn_dict['probe_btn'].isChecked() and self.image_view.image_file is None:
-                if len(self.working_atlas_data['atlas-probe']) == 1:
-                    points2d = self.working_atlas_data['atlas-probe'].copy()
+                    self.atlas_view.himg.image_dict["ruler_path"].setData(
+                        np.asarray(temp)
+                    )
+
+            if (
+                self.tool_box.checkable_btn_dict["probe_btn"].isChecked()
+                and self.image_view.image_file is None
+            ):
+                if len(self.working_atlas_data["atlas-probe"]) == 1:
+                    points2d = self.working_atlas_data["atlas-probe"].copy()
                     points2d.append([x, y])
                     if self.multi_shanks and self.valid_multi_settings:
                         base_loc_1d = get_pre_multi_shank_vis_base(
-                            self.multi_settings.x_vals, self.multi_settings.y_vals)
+                            self.multi_settings.x_vals, self.multi_settings.y_vals
+                        )
                     else:
                         base_loc_1d = np.array([0])
-                    start_pnt, end_pnt = self.atlas_view.get_pre_vis_data(np.asarray(points2d), base_loc_1d)
+                    start_pnt, end_pnt = self.atlas_view.get_pre_vis_data(
+                        np.asarray(points2d), base_loc_1d
+                    )
                     self.atlas_view.set_pre_vis_data(start_pnt, end_pnt)
 
         c_id = self.atlas_view.current_coronal_index
         s_id = self.atlas_view.current_sagital_index
         h_id = self.atlas_view.atlas_size[0] - self.atlas_view.current_horizontal_index
 
         o_rot = np.array([h_id, s_id, c_id])
@@ -3635,322 +4713,449 @@
 
         da_label = self.atlas_view.himg.label_img.image.copy()
         da_id = da_label[int(y), int(x)]
 
         vox_val = self.atlas_view.himg.img.image[int(y), int(x)]
 
         if vox_val != 0:
-            coords = np.round((da_pnt - np.ravel(self.atlas_view.Bregma)) * self.atlas_view.vox_size_um, 2)
+            coords = np.round(
+                (da_pnt - np.ravel(self.atlas_view.Bregma))
+                * self.atlas_view.vox_size_um,
+                2,
+            )
             da_vec = self.atlas_view.atlas_data[:, int(da_pnt[1]), int(da_pnt[2])]
             valid_inds = np.where(da_vec != 0)[0]
             # self.atlas_view.cimg.image_dict['atlas-probe'].setData(pos=[[int(y), valid_inds[0]]])
             # self.atlas_view.simg.image_dict['atlas-probe'].setData(pos=[[int(x), valid_inds[0]]])
             dv_val = np.round((valid_inds[0] - h_id) * self.atlas_view.vox_size_um, 2)
-            pstr = 'Atlas voxel:({}, {}, {}), ML:{}um, AP:{}um, DV:{}um w.r.t. Bregma, DV:{}um w.r.t Surface: {} '.format(
-                int(da_pnt[1]), int(da_pnt[2]), int(self.atlas_view.atlas_size[0] - da_pnt[0]),
-                coords[1], coords[2], -coords[0], dv_val, self.atlas_view.label_tree.describe(da_id))
+            pstr = "Atlas voxel:({}, {}, {}), ML:{}um, AP:{}um, DV:{}um w.r.t. Bregma, DV:{}um w.r.t Surface: {} ".format(
+                int(da_pnt[1]),
+                int(da_pnt[2]),
+                int(self.atlas_view.atlas_size[0] - da_pnt[0]),
+                coords[1],
+                coords[2],
+                -coords[0],
+                dv_val,
+                self.atlas_view.label_tree.describe(da_id),
+            )
             self.print_message(pstr, self.normal_color)
 
             if self.atlas_view.navigation_btn.isChecked():
                 self.atlas_view.himg.v_line.setPos(x)
                 self.atlas_view.himg.h_line.setPos(y)
                 self.atlas_view.cimg.v_line.setPos(y)
                 self.atlas_view.cimg.h_line.setPos(h_id)
                 self.atlas_view.simg.v_line.setPos(x)
                 self.atlas_view.simg.h_line.setPos(h_id)
 
                 self.atlas_view.cpage_ctrl.set_val(int(x))
                 self.atlas_view.spage_ctrl.set_val(int(y))
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     def atlas_erasing_probe(self, pos):
         x = pos[0]
         y = pos[1]
         if self.h2a_transferred:
             return
-        if not self.working_atlas_data['atlas-probe']:
+        if not self.working_atlas_data["atlas-probe"]:
             return
         r = self.tool_box.eraser_size_slider.value()
-        temp = np.asarray(self.working_atlas_data['atlas-probe'])
-        remain_points, del_indexes = delete_points_inside_eraser(temp, np.array([x, y]), r)
+        temp = np.asarray(self.working_atlas_data["atlas-probe"])
+        remain_points, del_indexes = delete_points_inside_eraser(
+            temp, np.array([x, y]), r
+        )
         if remain_points is None:
-            self.remove_single_link_related('atlas-probe')
+            self.remove_single_link_related("atlas-probe")
             return
-        self.working_atlas_data['atlas-probe'] = remain_points.tolist()
-        self.atlas_view.working_atlas.image_dict['atlas-probe'].setData(pos=remain_points)
+        self.working_atlas_data["atlas-probe"] = remain_points.tolist()
+        self.atlas_view.working_atlas.image_dict["atlas-probe"].setData(
+            pos=remain_points
+        )
         da_color = self.layer_ctrl.layer_color[self.layer_ctrl.current_layer_index[0]]
-        vis_img = create_vis_img(self.atlas_view.slice_size, self.working_atlas_data['atlas-probe'], da_color, 'p')
-        res = cv2.resize(vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-        self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
+        vis_img = create_vis_img(
+            self.atlas_view.slice_size,
+            self.working_atlas_data["atlas-probe"],
+            da_color,
+            "p",
+        )
+        res = cv2.resize(
+            vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+        )
+        self.layer_ctrl.layer_list[
+            self.layer_ctrl.current_layer_index[0]
+        ].set_thumbnail_data(res)
 
     def atlas_stacks_clicked(self, pos):
         # print('atlas clicked')
         x = pos[0]
         y = pos[1]
         if self.num_windows == 4:
-            self.print_message('Atlas window can not be clicked when 4-window is on.', self.error_message_color)
+            self.print_message(
+                "Atlas window can not be clicked when 4-window is on.",
+                self.error_message_color,
+            )
             return
-        if self.current_atlas == 'volume':
+        if self.current_atlas == "volume":
             if self.atlas_view.atlas_data is None:
-                self.print_message('No volume atlas data is loaded.', self.error_message_color)
+                self.print_message(
+                    "No volume atlas data is loaded.", self.error_message_color
+                )
                 return
         else:
             if self.atlas_view.slice_image_data is None:
-                self.print_message('No slice atlas data is loaded.', self.error_message_color)
+                self.print_message(
+                    "No slice atlas data is loaded.", self.error_message_color
+                )
                 return
         # ------------------------- ruler
-        if self.tool_box.checkable_btn_dict['ruler_btn'].isChecked():
-            if len(self.working_atlas_data['ruler_path']) == 2:
+        if self.tool_box.checkable_btn_dict["ruler_btn"].isChecked():
+            if len(self.working_atlas_data["ruler_path"]) == 2:
                 self.inactive_atlas_ruler()
-                self.tool_box.ruler_length_label.setText('Length:')
+                self.tool_box.ruler_length_label.setText("Length:")
             else:
-                self.working_atlas_data['ruler_path'].append([x, y])
-                self.atlas_view.working_atlas.image_dict['ruler_path'].setData(
-                    np.asarray(self.working_atlas_data['ruler_path']))
+                self.working_atlas_data["ruler_path"].append([x, y])
+                self.atlas_view.working_atlas.image_dict["ruler_path"].setData(
+                    np.asarray(self.working_atlas_data["ruler_path"])
+                )
 
         # ------------------------- triangle
-        elif self.tool_box.checkable_btn_dict['triang_btn'].isChecked():
+        elif self.tool_box.checkable_btn_dict["triang_btn"].isChecked():
             if self.a2h_transferred or self.h2a_transferred:
                 return
             if self.np_onside is None:
-                print(self.np_onside)
-                self.print_message('Please set valid number of boundary points!', self.error_message_color)
+                # print(self.np_onside)
+                self.print_message(
+                    "Please set valid number of boundary points!",
+                    self.error_message_color,
+                )
                 return
             self.atlas_tri_inside_data.append([int(x), int(y)])
-            self.atlas_tri_data = self.atlas_tri_onside_data + self.atlas_tri_inside_data
-            self.atlas_view.working_atlas.image_dict['tri_pnts'].setData(pos=np.asarray(self.atlas_tri_data))
-            self.working_atlas_text.append(pg.TextItem(str(len(self.atlas_tri_inside_data))))
+            self.atlas_tri_data = (
+                self.atlas_tri_onside_data + self.atlas_tri_inside_data
+            )
+            self.atlas_view.working_atlas.image_dict["tri_pnts"].setData(
+                pos=np.asarray(self.atlas_tri_data)
+            )
+            self.working_atlas_text.append(
+                pg.TextItem(str(len(self.atlas_tri_inside_data)))
+            )
             self.working_atlas_text[-1].setColor(self.triangle_color)
             self.working_atlas_text[-1].setPos(x, y)
             self.atlas_view.working_atlas.vb.addItem(self.working_atlas_text[-1])
             if self.tool_box.triang_vis_btn.isChecked():
                 self.update_atlas_tri_lines()
         # ------------------------- eraser
-        elif self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
-            if not self.layer_ctrl.layer_id or len(self.layer_ctrl.current_layer_index) > 1:
-                self.print_message('Eraser only works on one single layer.', self.error_message_color)
+        elif self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
+            if (
+                not self.layer_ctrl.layer_id
+                or len(self.layer_ctrl.current_layer_index) > 1
+            ):
+                self.print_message(
+                    "Eraser only works on one single layer.", self.error_message_color
+                )
                 return
             da_link = self.layer_ctrl.layer_link[self.layer_ctrl.current_layer_index[0]]
-            if da_link == 'atlas-probe':
+            if da_link == "atlas-probe":
                 self.atlas_erasing_probe(pos)
             else:
-                if self.current_atlas == 'volume':
+                if self.current_atlas == "volume":
                     return
                 r = self.tool_box.eraser_size_slider.value()
-                mask_img = np.zeros(self.working_atlas_data[da_link].shape[:2], dtype=np.uint8)
-                cv2.circle(mask_img, center=(int(x), int(y)), radius=r, color=255, thickness=-1)
+                mask_img = np.zeros(
+                    self.working_atlas_data[da_link].shape[:2], dtype=np.uint8
+                )
+                cv2.circle(
+                    mask_img, center=(int(x), int(y)), radius=r, color=255, thickness=-1
+                )
                 mask_img = 255 - mask_img
-                if da_link in ['atlas-mask', 'atlas-slice']:
+                if da_link in ["atlas-mask", "atlas-slice"]:
                     temp = self.working_atlas_data[da_link].astype(np.uint8)
                     dst = cv2.bitwise_and(temp, temp, mask=mask_img)
-                    res = cv2.resize(dst, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
+                    res = cv2.resize(
+                        dst, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+                    )
                     self.atlas_view.slice_stack.image_dict[da_link].setImage(dst)
                     self.working_atlas_data[da_link] = dst
                 else:
                     return
-            self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
-            current_data = {'data': self.working_atlas_data[da_link].copy()}
-            self.save_current_action('eraser_btn', da_link, current_data, res)
+            self.layer_ctrl.layer_list[
+                self.layer_ctrl.current_layer_index[0]
+            ].set_thumbnail_data(res)
+            current_data = {"data": self.working_atlas_data[da_link].copy()}
+            self.save_current_action("eraser_btn", da_link, current_data, res)
         # ------------------------- lasso
-        elif self.tool_box.checkable_btn_dict['lasso_btn'].isChecked():
-            if self.working_img_data['lasso_path']:
+        elif self.tool_box.checkable_btn_dict["lasso_btn"].isChecked():
+            if self.working_img_data["lasso_path"]:
                 self.inactive_lasso()
             if self.atlas_lasso_is_closure:
                 self.inactive_slice_window_lasso()
                 return
-            if self.current_atlas == 'volume':
+            if self.current_atlas == "volume":
                 return
             new_pnt = np.array([x, y])
-            if len(self.working_atlas_data['lasso_path']) > 1:
-                dists = np.sum((np.asarray(self.working_atlas_data['lasso_path'][0]) - new_pnt) ** 2)
+            if len(self.working_atlas_data["lasso_path"]) > 1:
+                dists = np.sum(
+                    (np.asarray(self.working_atlas_data["lasso_path"][0]) - new_pnt)
+                    ** 2
+                )
             else:
                 dists = 1e5
             if dists < 5:
-                self.working_atlas_data['lasso_path'].append(self.working_atlas_data['lasso_path'][0])
-                self.atlas_view.slice_stack.image_dict['lasso_path'].setPen(
-                    pg.mkPen(color='r', width=3, style=Qt.SolidLine))
+                self.working_atlas_data["lasso_path"].append(
+                    self.working_atlas_data["lasso_path"][0]
+                )
+                self.atlas_view.slice_stack.image_dict["lasso_path"].setPen(
+                    pg.mkPen(color="r", width=3, style=Qt.SolidLine)
+                )
                 self.atlas_lasso_is_closure = True
             else:
-                self.working_atlas_data['lasso_path'].append([x, y])
-            drawing_pnts = np.asarray(self.working_atlas_data['lasso_path'])
-            self.atlas_view.slice_stack.image_dict['lasso_path'].setData(drawing_pnts)
-            current_data = {'data': self.working_atlas_data['lasso_path'].copy()}
-            self.save_current_action('lasso_btn', 'lasso_path', current_data, None)
+                self.working_atlas_data["lasso_path"].append([x, y])
+            drawing_pnts = np.asarray(self.working_atlas_data["lasso_path"])
+            self.atlas_view.slice_stack.image_dict["lasso_path"].setData(drawing_pnts)
+            current_data = {"data": self.working_atlas_data["lasso_path"].copy()}
+            self.save_current_action("lasso_btn", "lasso_path", current_data, None)
         # ------------------------- probe
-        elif self.tool_box.checkable_btn_dict['probe_btn'].isChecked():
-            self.working_atlas_data['atlas-probe'].append([x, y])
+        elif self.tool_box.checkable_btn_dict["probe_btn"].isChecked():
+            self.working_atlas_data["atlas-probe"].append([x, y])
 
-            if len(self.working_atlas_data['atlas-probe']) > 2:
-                self.working_atlas_data['atlas-probe'].clear()
-                self.atlas_view.working_atlas.image_dict['atlas-probe'].clear()
-                self.atlas_view.working_atlas.image_dict['atlas-trajectory'].clear()
+            if len(self.working_atlas_data["atlas-probe"]) > 2:
+                self.working_atlas_data["atlas-probe"].clear()
+                self.atlas_view.working_atlas.image_dict["atlas-probe"].clear()
+                self.atlas_view.working_atlas.image_dict["atlas-trajectory"].clear()
                 self.atlas_view.working_atlas.remove_pre_trajectories_vis_lines()
-            if len(self.working_atlas_data['atlas-probe']) == 0:
-                self.atlas_view.working_atlas.image_dict['atlas-probe'].clear()
+            if len(self.working_atlas_data["atlas-probe"]) == 0:
+                self.atlas_view.working_atlas.image_dict["atlas-probe"].clear()
                 self.atlas_view.working_atlas.remove_pre_trajectories_vis_lines()
                 return
             if self.image_view.image_file is None:
                 # pre-surgery
-                points2d = self.working_atlas_data['atlas-probe'].copy()
+                points2d = self.working_atlas_data["atlas-probe"].copy()
                 points2d = np.asarray(points2d)
 
                 if self.multi_shanks and self.valid_multi_settings:
                     base_loc_1d = get_pre_multi_shank_vis_base(
-                        self.multi_settings.x_vals, self.multi_settings.y_vals)
+                        self.multi_settings.x_vals, self.multi_settings.y_vals
+                    )
                 else:
                     base_loc_1d = np.array([0])
 
-                if self.current_atlas == 'volume':
-                    self.atlas_view.draw_pre_2d_vis_data_for_volume_atlas(points2d, base_loc_1d)
+                if self.current_atlas == "volume":
+                    self.atlas_view.draw_pre_2d_vis_data_for_volume_atlas(
+                        points2d, base_loc_1d
+                    )
                 else:
-                    self.atlas_view.draw_pre_2d_vis_data_for_slice_atlas(points2d, base_loc_1d)
+                    self.atlas_view.draw_pre_2d_vis_data_for_slice_atlas(
+                        points2d, base_loc_1d
+                    )
             else:
                 # after-surgery
-                self.atlas_view.working_atlas.image_dict['atlas-probe'].setData(
-                    pos=np.asarray(self.working_atlas_data['atlas-probe']))
-                if len(self.working_atlas_data['atlas-probe']) > 1:
-                    if self.current_atlas == 'volume':
-                        current_img = self.atlas_view.working_atlas.label_img.image.copy()
+                self.atlas_view.working_atlas.image_dict["atlas-probe"].setData(
+                    pos=np.asarray(self.working_atlas_data["atlas-probe"])
+                )
+                if len(self.working_atlas_data["atlas-probe"]) > 1:
+                    if self.current_atlas == "volume":
+                        current_img = (
+                            self.atlas_view.working_atlas.label_img.image.copy()
+                        )
                     else:
                         current_img = None
-                    vis_points, msg = line_fit_2d(self.working_atlas_data['atlas-probe'], current_img)
+                    vis_points, msg = line_fit_2d(
+                        self.working_atlas_data["atlas-probe"], current_img
+                    )
                     if msg is not None:
                         self.print_message(msg, self.error_message_color)
                         return
-                    self.atlas_view.working_atlas.image_dict['atlas-trajectory'].setData(vis_points)
+                    self.atlas_view.working_atlas.image_dict[
+                        "atlas-trajectory"
+                    ].setData(vis_points)
+
+            vis_img = create_vis_img(
+                self.atlas_view.slice_size,
+                self.working_atlas_data["atlas-probe"],
+                self.probe_color,
+                "p",
+            )
+            res = cv2.resize(
+                vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="atlas-probe", color=self.probe_color
+            )
 
-            vis_img = create_vis_img(self.atlas_view.slice_size, self.working_atlas_data['atlas-probe'],
-                                     self.probe_color, 'p')
-            res = cv2.resize(vis_img, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-probe', color=self.probe_color)
-
-            current_data = {'data': self.working_atlas_data['atlas-probe'].copy()}
-            self.save_current_action('probe_btn', 'atlas-probe', current_data, None)
+            current_data = {"data": self.working_atlas_data["atlas-probe"].copy()}
+            self.save_current_action("probe_btn", "atlas-probe", current_data, None)
         # ------------------------- magic wand -- mask
-        elif self.tool_box.checkable_btn_dict['magic_wand_btn'].isChecked():
-            if self.current_atlas == 'volume':
+        elif self.tool_box.checkable_btn_dict["magic_wand_btn"].isChecked():
+            if self.current_atlas == "volume":
                 if not self.h2a_transferred:
                     return
-                src_img = self.atlas_view.working_atlas.image_dict['atlas-overlay'].image.copy()
+                src_img = self.atlas_view.working_atlas.image_dict[
+                    "atlas-overlay"
+                ].image.copy()
             else:
                 src_img = self.atlas_view.slice_image_data.copy()
-            white_img = np.ones(self.atlas_view.slice_size).astype('uint8')
+            white_img = np.ones(self.atlas_view.slice_size).astype("uint8")
             tol_val = int(self.tool_box.magic_tol_val.text())
             da_color = src_img[int(y), int(x), :3]
-            lower_val, upper_val = get_bound_color(da_color, tol_val, 255, 'rgb')
-            mask_img = cv2.inRange(src_img[:, :, :3], np.array(lower_val, dtype='float'),
-                                   np.array(upper_val, dtype='float'))
+            lower_val, upper_val = get_bound_color(da_color, tol_val, 255, "rgb")
+            mask_img = cv2.inRange(
+                src_img[:, :, :3],
+                np.array(lower_val, dtype="float"),
+                np.array(upper_val, dtype="float"),
+            )
 
             modifiers = QApplication.keyboardModifiers()
             if modifiers == Qt.ShiftModifier:
-                if self.working_atlas_data['atlas-mask'] is None:
-                    self.working_atlas_data['atlas-mask'] = cv2.bitwise_or(mask_img, mask_img, mask=white_img)
+                if self.working_atlas_data["atlas-mask"] is None:
+                    self.working_atlas_data["atlas-mask"] = cv2.bitwise_or(
+                        mask_img, mask_img, mask=white_img
+                    )
                 else:
-                    self.working_atlas_data['atlas-mask'] = cv2.bitwise_or(self.working_atlas_data['atlas-mask'],
-                                                                           mask_img, mask=white_img)
+                    self.working_atlas_data["atlas-mask"] = cv2.bitwise_or(
+                        self.working_atlas_data["atlas-mask"], mask_img, mask=white_img
+                    )
             else:
-                self.working_atlas_data['atlas-mask'] = mask_img.copy()
+                self.working_atlas_data["atlas-mask"] = mask_img.copy()
 
             if self.kernel is not None:
-                temp = self.working_atlas_data['atlas-mask'].copy()
+                temp = self.working_atlas_data["atlas-mask"].copy()
                 open_img = cv2.morphologyEx(temp, cv2.MORPH_OPEN, self.kernel)
                 close_img = cv2.morphologyEx(open_img, cv2.MORPH_CLOSE, self.kernel)
-                self.working_atlas_data['atlas-mask'] = close_img.copy()
+                self.working_atlas_data["atlas-mask"] = close_img.copy()
 
-            self.atlas_view.working_atlas.image_dict['atlas-mask'].setImage(self.working_atlas_data['atlas-mask'])
-            res = cv2.resize(self.working_atlas_data['atlas-mask'],
-                             self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.master_layers(res, layer_type='atlas-mask', color=self.magic_wand_lut[1])
-            current_data = {'data': self.working_atlas_data['atlas-mask'].copy()}
-            self.save_current_action('magic_wand_btn', 'atlas-mask', current_data, res)
+            self.atlas_view.working_atlas.image_dict["atlas-mask"].setImage(
+                self.working_atlas_data["atlas-mask"]
+            )
+            res = cv2.resize(
+                self.working_atlas_data["atlas-mask"],
+                self.atlas_view.slice_tb_size,
+                interpolation=cv2.INTER_AREA,
+            )
+            self.layer_ctrl.master_layers(
+                res, layer_type="atlas-mask", color=self.magic_wand_lut[1]
+            )
+            current_data = {"data": self.working_atlas_data["atlas-mask"].copy()}
+            self.save_current_action("magic_wand_btn", "atlas-mask", current_data, res)
         # ------------------------- bregma picker
         elif self.actionBregma_Picker.isChecked():
             self.atlas_view.slice_bregma = [x, y]
-            self.atlas_view.slice_stack.image_dict['bregma_pnt'].setData(pos=np.array([self.atlas_view.slice_bregma]))
+            self.atlas_view.slice_stack.image_dict["bregma_pnt"].setData(
+                pos=np.array([self.atlas_view.slice_bregma])
+            )
             self.actionBregma_Picker.setChecked(False)
             self.atlas_view.check_info_ready()
         else:
             return
 
     def slice_stack_key_pressed(self, action):
         if len(self.layer_ctrl.current_layer_index) != 1:
-            msg = 'Delete only works on single layer. Multiple or No layer is selected.'
+            msg = "Delete only works on single layer. Multiple or No layer is selected."
             self.print_message(msg, self.reminder_color)
             return
         da_link = self.layer_ctrl.layer_link[self.layer_ctrl.current_layer_index[0]]
 
-        if action == 'delete':
+        if action == "delete":
             if self.atlas_lasso_is_closure:
                 mask = np.zeros(self.atlas_view.slice_size, dtype=np.uint8)
-                pts = np.int32(self.working_atlas_data['lasso_path'])
+                pts = np.int32(self.working_atlas_data["lasso_path"])
                 cv2.fillPoly(mask, pts=[pts], color=255)
                 if not self.tool_box.remove_inside:
                     mask = 255 - mask
-                if da_link == 'atlas-mask':
-                    dst = cv2.bitwise_and(self.working_atlas_data['atlas-mask'], self.working_atlas_data['atlas-mask'],
-                                          mask=mask)
-                    self.atlas_view.slice_stack.image_dict['atlas-mask'].setImage(dst)
-                    self.working_atlas_data['atlas-mask'] = dst
-                    res = cv2.resize(self.working_atlas_data['atlas-mask'], self.atlas_view.slice_tb_size,
-                                     interpolation=cv2.INTER_AREA)
-                elif da_link == 'atlas-slice':
-                    dst = cv2.bitwise_and(self.working_atlas_data[da_link], self.working_atlas_data[da_link], mask=mask)
+                if da_link == "atlas-mask":
+                    dst = cv2.bitwise_and(
+                        self.working_atlas_data["atlas-mask"],
+                        self.working_atlas_data["atlas-mask"],
+                        mask=mask,
+                    )
+                    self.atlas_view.slice_stack.image_dict["atlas-mask"].setImage(dst)
+                    self.working_atlas_data["atlas-mask"] = dst
+                    res = cv2.resize(
+                        self.working_atlas_data["atlas-mask"],
+                        self.atlas_view.slice_tb_size,
+                        interpolation=cv2.INTER_AREA,
+                    )
+                elif da_link == "atlas-slice":
+                    dst = cv2.bitwise_and(
+                        self.working_atlas_data[da_link],
+                        self.working_atlas_data[da_link],
+                        mask=mask,
+                    )
                     self.atlas_view.slice_stack.set_data(dst)
                     self.working_atlas_data[da_link] = dst
-                    res = cv2.resize(dst, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
+                    res = cv2.resize(
+                        dst, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+                    )
                 else:
                     return
             else:
-                if self.working_atlas_data['atlas-mask'] is None or da_link != 'atlas-slice':
+                if (
+                    self.working_atlas_data["atlas-mask"] is None
+                    or da_link != "atlas-slice"
+                ):
                     return
-                mask = self.working_atlas_data['atlas-mask'].copy()
+                mask = self.working_atlas_data["atlas-mask"].copy()
                 mask = 255 - mask
                 temp = self.atlas_view.processing_slice.copy()
                 dst = cv2.bitwise_and(temp, temp, mask=mask)
                 self.atlas_view.slice_stack.set_data(dst)
                 self.atlas_view.processing_slice = dst
-                res = cv2.resize(dst, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA)
-            self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].set_thumbnail_data(res)
-            current_data = {'data': self.working_atlas_data[da_link].copy()}
-            self.save_current_action('delete', da_link, current_data, res)
+                res = cv2.resize(
+                    dst, self.atlas_view.slice_tb_size, interpolation=cv2.INTER_AREA
+                )
+            self.layer_ctrl.layer_list[
+                self.layer_ctrl.current_layer_index[0]
+            ].set_thumbnail_data(res)
+            current_data = {"data": self.working_atlas_data[da_link].copy()}
+            self.save_current_action("delete", da_link, current_data, res)
         else:
             return
 
     #
     def atlas_window_tri_pnts_moving(self, ev_obj):
         ev = ev_obj[0]
         ind = ev_obj[1]
         da_num = (self.np_onside - 1) * 4
         if ind < da_num:
             return
         if self.h2a_transferred:
             old_pnts = self.atlas_tri_data.copy()
             new_pnts = self.atlas_tri_data.copy()
-            da_new_pnt = self.atlas_view.working_atlas.image_dict['tri_pnts'].data['pos'][ind].copy()
+            da_new_pnt = (
+                self.atlas_view.working_atlas.image_dict["tri_pnts"]
+                .data["pos"][ind]
+                .copy()
+            )
             new_pnts[ind] = [int(da_new_pnt[0]), int(da_new_pnt[1])]
-            print(self.atlas_tri_data[ind])
-            print(da_new_pnt)
-
+            # print(self.atlas_tri_data[ind])
+            # print(da_new_pnt)
 
             input_img = self.overlay_img.copy()
-            img_wrap = np.zeros((self.atlas_view.slice_size[0], self.atlas_view.slice_size[1], input_img.shape[2]),
-                                np.float32)
+            img_wrap = np.zeros(
+                (
+                    self.atlas_view.slice_size[0],
+                    self.atlas_view.slice_size[1],
+                    input_img.shape[2],
+                ),
+                np.float32,
+            )
 
             subdiv = cv2.Subdiv2D(self.atlas_rect)
             for p in self.atlas_tri_data:
                 subdiv.insert(p)
 
             tri_vet_inds = get_vertex_ind_in_triangle(subdiv)
             for i in range(len(tri_vet_inds)):
                 da_inds = tri_vet_inds[i]
-                t1 = [self.atlas_tri_data[da_inds[0]], self.atlas_tri_data[da_inds[1]],
-                      self.atlas_tri_data[da_inds[2]]]
-                t2 = [new_pnts[da_inds[0]], new_pnts[da_inds[1]],
-                      new_pnts[da_inds[2]]]
+                t1 = [
+                    self.atlas_tri_data[da_inds[0]],
+                    self.atlas_tri_data[da_inds[1]],
+                    self.atlas_tri_data[da_inds[2]],
+                ]
+                t2 = [new_pnts[da_inds[0]], new_pnts[da_inds[1]], new_pnts[da_inds[2]]]
                 t1 = np.reshape(t1, (3, 2))
                 t2 = np.reshape(t2, (3, 2))
                 warp_triangle(input_img, img_wrap, t1, t2, True)
 
             #
 
             # # img_overlay = self.atlas_view.working_atlas.overlay_img.image.copy()
@@ -3969,79 +5174,93 @@
             #     if ind not in da_inds:
             #         continue
             #     t1 = [old_pnts[da_inds[0]], old_pnts[da_inds[1]], old_pnts[da_inds[2]]]
             #     t2 = [new_pnts[da_inds[0]], new_pnts[da_inds[1]], new_pnts[da_inds[2]]]
             #     t1 = np.reshape(t1, (3, 2))
             #     t2 = np.reshape(t2, (3, 2))
             #     warp_triangle(img_overlay, img_wrap,  t1, t2, True)
-            self.atlas_view.working_atlas.image_dict['atlas-overlay'].setImage(img_wrap)
+            self.atlas_view.working_atlas.image_dict["atlas-overlay"].setImage(img_wrap)
             # self.atlas_tri_data = new_pnts
         else:
-            da_new_pnt = self.atlas_view.working_atlas.image_dict['tri_pnts'].data['pos'][ind].copy()
+            da_new_pnt = (
+                self.atlas_view.working_atlas.image_dict["tri_pnts"]
+                .data["pos"][ind]
+                .copy()
+            )
             self.atlas_tri_data[ind] = [int(da_new_pnt[0]), int(da_new_pnt[1])]
-        self.atlas_tri_inside_data[ind - da_num] = [int(da_new_pnt[0]), int(da_new_pnt[1])]
+        self.atlas_tri_inside_data[ind - da_num] = [
+            int(da_new_pnt[0]),
+            int(da_new_pnt[1]),
+        ]
         self.working_atlas_text[ind - da_num].setPos(da_new_pnt[0], da_new_pnt[1])
         if self.tool_box.triang_vis_btn.isChecked():
             self.update_atlas_tri_lines()
 
     def atlas_window_tri_pnts_clicked(self, ev):
-        print(self.atlas_tri_data)
-        if not self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
+        # print(self.atlas_tri_data)
+        if not self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
             return
         if self.a2h_transferred or self.h2a_transferred:
             return
         self.inactive_lasso()
         clicked_ind = ev[1]
         num = (self.np_onside - 1) * 4
         if clicked_ind < num:
             return
         self.atlas_view.working_atlas.vb.removeItem(self.working_atlas_text[-1])
         del self.working_atlas_text[-1]
         del self.atlas_tri_inside_data[clicked_ind - num]
         self.atlas_tri_data = self.atlas_tri_onside_data + self.atlas_tri_inside_data
-        self.atlas_view.working_atlas.image_dict['tri_pnts'].setData(pos=np.asarray(self.atlas_tri_data))
+        self.atlas_view.working_atlas.image_dict["tri_pnts"].setData(
+            pos=np.asarray(self.atlas_tri_data)
+        )
         for i in range(len(self.working_atlas_text)):
             pnt_id = i + num
-            self.working_atlas_text[i].setPos(self.atlas_tri_data[pnt_id][0], self.atlas_tri_data[pnt_id][1])
+            self.working_atlas_text[i].setPos(
+                self.atlas_tri_data[pnt_id][0], self.atlas_tri_data[pnt_id][1]
+            )
         if self.tool_box.triang_vis_btn.isChecked():
             self.update_atlas_tri_lines()
 
     def atlas_probe_pnts_clicked(self, points, ev):
-        if self.num_windows == 4 or not self.working_atlas_data['atlas-probe']:
+        if self.num_windows == 4 or not self.working_atlas_data["atlas-probe"]:
             return
-        if not self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
+        if not self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
             return
         if not self.layer_ctrl.layer_id or len(self.layer_ctrl.current_layer_index) > 1:
-            self.print_message('Eraser only works on one single layer.', self.error_message_color)
+            self.print_message(
+                "Eraser only works on one single layer.", self.error_message_color
+            )
             return
         da_link = self.layer_ctrl.layer_link[self.layer_ctrl.current_layer_index[0]]
-        if da_link != 'atlas-probe':
+        if da_link != "atlas-probe":
             return
         clicked_ind = ev[0].index()
-        pos = self.working_atlas_data['atlas-probe'][clicked_ind]
+        pos = self.working_atlas_data["atlas-probe"][clicked_ind]
         self.atlas_erasing_probe(pos)
         # del self.working_atlas_data['atlas-probe'][clicked_ind]
         # if self.working_atlas_data['atlas-probe']:
         #     self.atlas_view.working_atlas.image_dict['atlas-probe'].setData(
         #         pos=np.asarray(self.working_atlas_data['atlas-probe']))
         # else:
         #     self.atlas_view.working_atlas.image_dict['atlas-probe'].clear()
 
     def atlas_contour_pnts_clicked(self, points, ev):
-        if self.num_windows == 4 or not self.working_atlas_data['atlas-contour']:
+        if self.num_windows == 4 or not self.working_atlas_data["atlas-contour"]:
             return
-        if not self.tool_box.checkable_btn_dict['eraser_btn'].isChecked():
+        if not self.tool_box.checkable_btn_dict["eraser_btn"].isChecked():
             return
         clicked_ind = ev[0].index()
-        del self.working_atlas_data['atlas-contour'][clicked_ind]
-        if self.working_atlas_data['atlas-contour']:
-            self.atlas_view.working_atlas.image_dict['atlas-contour'].setData(
-                pos=np.asarray(self.working_atlas_data['atlas-contour']))
+        del self.working_atlas_data["atlas-contour"][clicked_ind]
+        if self.working_atlas_data["atlas-contour"]:
+            self.atlas_view.working_atlas.image_dict["atlas-contour"].setData(
+                pos=np.asarray(self.working_atlas_data["atlas-contour"])
+            )
         else:
-            self.atlas_view.working_atlas.image_dict['atlas-contour'].clear()
+            self.atlas_view.working_atlas.image_dict["atlas-contour"].clear()
 
     # ------------------------------------------------------------------
     #
     #                       Atlas 3D control
     #
     # ------------------------------------------------------------------
     def show_small_area_in_3d(self):
@@ -4051,15 +5270,17 @@
             self.show_child_mesh = True
 
     def composition_3d_changed(self):
         if self.atlas_view.atlas_data is None:
             return
         all_keys = list(self.small_mesh_list.keys())
         for da_key in all_keys:
-            self.small_mesh_list[da_key].setGLOptions(self.composition_combo.currentText())
+            self.small_mesh_list[da_key].setGLOptions(
+                self.composition_combo.currentText()
+            )
 
     def sig_label_changed(self):
         if self.atlas_view.atlas_data is None or self.atlas_view.atlas_label is None:
             return
 
         lut = self.atlas_view.label_tree.lookup_table()
 
@@ -4071,21 +5292,29 @@
             return
         valid_id = list(self.small_mesh_list.keys())
         current_checked_label = list(self.atlas_view.label_tree.checked)
         n_current_label = len(current_checked_label)
         n_previous_label = len(self.previous_checked_label)
         if self.show_child_mesh:
             if n_current_label > n_previous_label:
-                label_to_show = [id for id in current_checked_label if id not in self.previous_checked_label]
+                label_to_show = [
+                    id
+                    for id in current_checked_label
+                    if id not in self.previous_checked_label
+                ]
                 label_to_show = list(np.ravel(label_to_show).astype(str))
                 for id in label_to_show:
                     if id in valid_id:
                         self.small_mesh_list[id].setVisible(True)
             else:
-                label_to_hide = [id for id in self.previous_checked_label if id not in current_checked_label]
+                label_to_hide = [
+                    id
+                    for id in self.previous_checked_label
+                    if id not in current_checked_label
+                ]
                 label_to_hide = list(np.ravel(label_to_hide).astype(str))
                 for id in label_to_hide:
                     if id in valid_id:
                         self.small_mesh_list[id].setVisible(False)
         self.previous_checked_label = current_checked_label
 
         check_id = list(self.atlas_view.label_tree.checked)
@@ -4109,518 +5338,689 @@
         self.atlas_view.himg.label_img.setLookupTable(lut=lut)
 
         col_to_set = ev[1] / 255
         label_id = str(ev[0])
         all_keys = self.small_mesh_list.keys()
         if label_id not in all_keys:
             return
-        self.small_mesh_list[label_id].setColor((col_to_set[0], col_to_set[1], col_to_set[2], col_to_set[3]))
+        self.small_mesh_list[label_id].setColor(
+            (col_to_set[0], col_to_set[1], col_to_set[2], col_to_set[3])
+        )
 
     def sig_reset_labels(self):
         lut = self.atlas_view.label_tree.lookup_table()
 
         self.atlas_view.cimg.label_img.setLookupTable(lut=lut)
         self.atlas_view.simg.label_img.setLookupTable(lut=lut)
         self.atlas_view.himg.label_img.setLookupTable(lut=lut)
 
         valid_id = list(self.small_mesh_list.keys())
         for label_id in valid_id:
             col_to_set = lut[int(label_id)] / 255
-            self.small_mesh_list[label_id].setColor((col_to_set[0], col_to_set[1], col_to_set[2], col_to_set[3]))
+            self.small_mesh_list[label_id].setColor(
+                (col_to_set[0], col_to_set[1], col_to_set[2], col_to_set[3])
+            )
 
     # ------------------------------------------------------------------
     #
     #                      Sidebar - Layer Panel
     #
     # ------------------------------------------------------------------
     def remove_h2a_transferred_layers(self):
         if self.h2a_transferred:
             self.h2a_transferred = False
             self.tool_box.toa_btn.setIcon(self.tool_box.toa_btn_off_icon)
-            self.project_method = 'pre plan'
+            self.project_method = "pre plan"
             self.register_method = 0
             self.tool_box.toh_btn.setEnabled(True)
 
     def remove_a2h_transferred_layers(self):
         if self.a2h_transferred:
             self.a2h_transferred = False
             self.tool_box.toh_btn.setIcon(self.tool_box.toh_btn_off_icon)
-            self.project_method = 'pre plan'
+            self.project_method = "pre plan"
             self.register_method = 0
             self.tool_box.toa_btn.setEnabled(True)
 
     def remove_single_link_related(self, link_type):
         del_index = np.where(np.ravel(self.layer_ctrl.layer_link) == link_type)[0][0]
         self.layer_ctrl.delete_layer(del_index)
         self.layers_exist_changed(link_type)
 
     def delete_all_atlas_layer(self):
         if not self.layer_ctrl.layer_link:
             return
         for da_link in self.layer_ctrl.layer_link:
-            if 'atlas' not in da_link:
+            if "atlas" not in da_link:
                 continue
             da_index = np.where(np.ravel(self.layer_ctrl.layer_link) == da_link)[0][0]
             self.layer_ctrl.delete_layer(da_index)
             self.layers_exist_changed(da_link)
         self.remove_h2a_transferred_layers()
 
-
-
     def layers_opacity_changed(self, ev):
         da_link = ev[0]
         da_color = ev[1]
         val = ev[2]
-        if da_link == 'img-process':
+        if da_link == "img-process":
             for i in range(self.image_view.image_file.n_channels):
                 self.image_view.img_stacks.image_list[i].setOpts(opacity=val * 0.01)
-        elif da_link == 'atlas-slice':
+        elif da_link == "atlas-slice":
             self.atlas_view.slice_stack.img_layer.setOpts(opacity=val * 0.01)
         else:
-            if 'img' in da_link:
-                if self.working_img_type[da_link] == 'pixel':
-                    self.image_view.img_stacks.image_dict[da_link].setOpts(opacity=val * 0.01)
+            if "img" in da_link:
+                if self.working_img_type[da_link] == "pixel":
+                    self.image_view.img_stacks.image_dict[da_link].setOpts(
+                        opacity=val * 0.01
+                    )
                 else:
-                    self.image_view.img_stacks.image_dict[da_link].setPen((da_color[0], da_color[1], da_color[2],
-                                                                           int(val * 255 * 0.01)))
-            else:
-                if self.working_atlas_type[da_link] == 'pixel':
-                    self.atlas_view.working_atlas.image_dict[da_link].setOpts(opacity=val * 0.01)
+                    self.image_view.img_stacks.image_dict[da_link].setPen(
+                        (da_color[0], da_color[1], da_color[2], int(val * 255 * 0.01))
+                    )
+            else:
+                if self.working_atlas_type[da_link] == "pixel":
+                    self.atlas_view.working_atlas.image_dict[da_link].setOpts(
+                        opacity=val * 0.01
+                    )
                 else:
-                    self.atlas_view.working_atlas.image_dict[da_link].setPen((da_color[0], da_color[1], da_color[2],
-                                                                              int(val * 255 * 0.01)))
+                    self.atlas_view.working_atlas.image_dict[da_link].setPen(
+                        (da_color[0], da_color[1], da_color[2], int(val * 255 * 0.01))
+                    )
 
     def layers_visible_changed(self, event):
         da_link = event[1]
         vis = event[2]
-        if da_link == 'img-process':
+        if da_link == "img-process":
             for i in range(self.image_view.image_file.n_channels):
                 self.image_view.img_stacks.image_list[i].setVisible(vis)
-        elif da_link == 'atlas-slice':
+        elif da_link == "atlas-slice":
             self.atlas_view.slice_stack.img_layer.setVisible(vis)
         else:
-            if 'img' in da_link:
+            if "img" in da_link:
                 self.image_view.img_stacks.image_dict[da_link].setVisible(vis)
             else:
                 self.atlas_view.working_atlas.image_dict[da_link].setVisible(vis)
 
     def layers_exist_changed(self, da_link):  # delete
-        if da_link == 'img-process':
+        if da_link == "img-process":
             self.reset_current_image()
-        elif da_link == 'atlas-slice':
+        elif da_link == "atlas-slice":
             self.reset_atlas_slice()
         else:
-            if 'img' in da_link:
+            if "img" in da_link:
                 self.image_view.img_stacks.image_dict[da_link].clear()
-                if self.working_img_type[da_link] == 'pixel':
+                if self.working_img_type[da_link] == "pixel":
                     self.working_img_data[da_link] = None
                 else:
                     self.working_img_data[da_link] = []
-                    if 'drawing' in da_link:
+                    if "drawing" in da_link:
                         self.image_view.img_stacks.image_dict[da_link].updateItems()
             else:
                 self.atlas_view.working_atlas.image_dict[da_link].clear()
-                if self.working_atlas_type[da_link] == 'pixel':
+                if self.working_atlas_type[da_link] == "pixel":
                     self.working_atlas_data[da_link] = None
                 else:
                     self.working_atlas_data[da_link] = []
-                    if 'drawing' in da_link:
+                    if "drawing" in da_link:
                         self.atlas_view.working_atlas.image_dict[da_link].updateItems()
 
             # if da_link == 'atlas-probe':
             #     for i in range(4):
             #         self.atlas_view.working_atlas.pre_trajectory_list[i].clear()
             #     self.atlas_view.working_atlas.image_dict['atlas-trajectory'].clear()
 
-            if da_link == 'img-cells':
-                for da_key in ['cell_count', 'cell_size', 'cell_symbol', 'cell_layer_index']:
+            if da_link == "img-cells":
+                for da_key in [
+                    "cell_count",
+                    "cell_size",
+                    "cell_symbol",
+                    "cell_layer_index",
+                ]:
                     self.working_img_data[da_key] = []
-                self.working_img_data['cell_count'] = [0 for i in range(5)]
+                self.working_img_data["cell_count"] = [0 for i in range(5)]
                 if self.a2h_transferred or not self.h2a_transferred:
                     for i in range(5):
-                        self.tool_box.cell_count_val_list[i].setText('0')
+                        self.tool_box.cell_count_val_list[i].setText("0")
 
-            if da_link == 'atlas-cells':
-                for da_key in ['cell_count', 'cell_size', 'cell_symbol', 'cell_layer_index']:
+            if da_link == "atlas-cells":
+                for da_key in [
+                    "cell_count",
+                    "cell_size",
+                    "cell_symbol",
+                    "cell_layer_index",
+                ]:
                     self.working_atlas_data[da_key] = []
                 for i in range(5):
-                    self.tool_box.cell_count_val_list[i].setText('0')
+                    self.tool_box.cell_count_val_list[i].setText("0")
 
-            if da_link == 'atlas-overlay':
+            if da_link == "atlas-overlay":
                 self.remove_h2a_transferred_layers()
 
-
     def layers_blend_mode_changed(self, ev):
         da_link = ev[0]
         blend_mode = ev[1]
-        if blend_mode == 'Plus':
+        if blend_mode == "Plus":
             da_mode = QPainter.CompositionMode_Plus
-        elif blend_mode == 'Multiply':
+        elif blend_mode == "Multiply":
             da_mode = QPainter.CompositionMode_Multiply
-        elif blend_mode == 'Overlay':
+        elif blend_mode == "Overlay":
             da_mode = QPainter.CompositionMode_Overlay
-        elif blend_mode == 'SourceOver':
+        elif blend_mode == "SourceOver":
             da_mode = QPainter.CompositionMode_SourceOver
         else:
             return
-        if da_link == 'img-process':
+        if da_link == "img-process":
             for i in range(self.image_view.image_file.n_channels):
                 self.image_view.img_stacks.image_list[i].setCompositionMode(da_mode)
-        elif da_link == 'atlas-slice':
+        elif da_link == "atlas-slice":
             self.atlas_view.slice_stack.img_layer.setCompositionMode(da_mode)
         else:
-            if 'img' in da_link:
-                if self.working_img_type[da_link] == 'pixel':
-                    self.image_view.img_stacks.image_dict[da_link].setCompositionMode(da_mode)
-            else:
-                if self.working_atlas_type[da_link] == 'pixel':
-                    self.atlas_view.working_atlas.image_dict[da_link].setCompositionMode(da_mode)
+            if "img" in da_link:
+                if self.working_img_type[da_link] == "pixel":
+                    self.image_view.img_stacks.image_dict[da_link].setCompositionMode(
+                        da_mode
+                    )
+            else:
+                if self.working_atlas_type[da_link] == "pixel":
+                    self.atlas_view.working_atlas.image_dict[
+                        da_link
+                    ].setCompositionMode(da_mode)
 
     # ------------------------------------------------------------------
     #
     #              Sidebar - Object Control
     #
     # ------------------------------------------------------------------
     def display_object_in_2d_atlas(self):
         if not self.object_ctrl.obj_list:
-            self.print_message('No object to display.', self.reminder_color)
+            self.print_message("No object to display.", self.reminder_color)
             return
-        if self.object_ctrl.obj_type[self.object_ctrl.current_obj_index] != 'merged probe':
-            self.print_message('At the moment only merged probe can be displayed.', self.reminder_color)
+        if (
+            self.object_ctrl.obj_type[self.object_ctrl.current_obj_index]
+            != "merged probe"
+        ):
+            self.print_message(
+                "At the moment only merged probe can be displayed.", self.reminder_color
+            )
             return
 
         if self.atlas_view.has_display_objects:
             self.atlas_view.clear_all_display_obj()
 
         if self.object_ctrl.linked_indexes:
-            self.print_message('Displaying linked objects is under development.', self.reminder_color)
+            self.print_message(
+                "Displaying linked objects is under development.", self.reminder_color
+            )
             return
             # linked_data = []
             # for link_index in self.object_ctrl.linked_indexes:
             #     linked_data.append(self.object_ctrl.obj_data[link_index])
         else:
-            display_data = self.object_ctrl.obj_data[self.object_ctrl.current_obj_index].copy()
+            display_data = self.object_ctrl.obj_data[
+                self.object_ctrl.current_obj_index
+            ].copy()
 
             self.atlas_view.rotate_cs_plane_after_merging_probe(display_data)
 
         # display all linked object, for probe, all probe limited in some angle
 
         # for cell/virus, show only on the current page
 
     def compare_object(self):
         if len(self.object_ctrl.linked_indexes) < 2:
-            self.print_message('Need at least 2 objects to compare.', self.reminder_color)
-            return
-        objects_type = np.ravel(self.object_ctrl.obj_type)[np.ravel(self.object_ctrl.linked_indexes)]
+            self.print_message(
+                "Need at least 2 objects to compare.", self.reminder_color
+            )
+            return
+        objects_type = np.ravel(self.object_ctrl.obj_type)[
+            np.ravel(self.object_ctrl.linked_indexes)
+        ]
         if len(np.unique(objects_type)) > 1:
-            self.print_message('Only the same type of objects can be compared.', self.reminder_color)
-            return
-        if 'probe' not in np.unique(objects_type)[0]:
-            self.print_message('Only probes can be compared at the moment.', self.reminder_color)
+            self.print_message(
+                "Only the same type of objects can be compared.", self.reminder_color
+            )
+            return
+        if "probe" not in np.unique(objects_type)[0]:
+            self.print_message(
+                "Only probes can be compared at the moment.", self.reminder_color
+            )
             return
         self.object_ctrl.compare_obj_called()
 
     def make_probe_piece(self):
         if not self.valid_probe_settings:
-            msg = 'Not valid probe settings given. Please provide a valid setting.'
+            msg = "Not valid probe settings given. Please provide a valid setting."
             self.print_message(msg, self.error_message_color)
             return
         if self.a2h_transferred:
-            data_tobe_registered = self.working_img_data['img-probe']
+            data_tobe_registered = self.working_img_data["img-probe"]
         else:
-            data_tobe_registered = self.working_atlas_data['atlas-probe']
+            data_tobe_registered = self.working_atlas_data["atlas-probe"]
 
         if data_tobe_registered:
             center_data_2d = np.asarray(data_tobe_registered)
-            center_data_3d = self.atlas_view.get_3d_data_from_2d_view(center_data_2d, self.atlas_display)
+            center_data_3d = self.atlas_view.get_3d_data_from_2d_view(
+                center_data_2d, self.atlas_display
+            )
             order_index = np.argsort(center_data_3d[:, 2])[::-1]
             center_data_3d = center_data_3d[order_index, :]
 
             if self.image_view.image_file is None:
                 if len(center_data_2d) != 2:
-                    msg = 'Pre-plan probe requires two points.'
+                    msg = "Pre-plan probe requires two points."
                     self.print_message(msg, self.error_message_color)
                     return
 
                 if self.multi_shanks and self.valid_multi_settings:
                     direction = center_data_3d[1] - center_data_3d[0]
                     r_hat = direction / np.linalg.norm(direction)
-                    base_length = np.sqrt(np.sum((center_data_3d[1] - center_data_3d[0]) ** 2))
+                    base_length = np.sqrt(
+                        np.sum((center_data_3d[1] - center_data_3d[0]) ** 2)
+                    )
                     n_hat = self.atlas_view.get_plane_norm_vector(self.atlas_display)
                     u_hat = np.cross(n_hat, r_hat)
-                    line_data = get_center_lines(center_data_3d, r_hat, n_hat, u_hat, self.multi_settings.x_vals,
-                                                 self.multi_settings.y_vals, base_length, self.site_face,
-                                                 self.atlas_view.vox_size_um)
+                    line_data = get_center_lines(
+                        center_data_3d,
+                        r_hat,
+                        n_hat,
+                        u_hat,
+                        self.multi_settings.x_vals,
+                        self.multi_settings.y_vals,
+                        base_length,
+                        self.site_face,
+                        self.atlas_view.vox_size_um,
+                    )
                 else:
                     line_data = [center_data_3d]
 
                 for i in range(len(line_data)):
-                    self.object_ctrl.add_object(object_name='probe {} - piece'.format(i),
-                                                object_type='probe piece',
-                                                object_data=line_data[i],
-                                                object_mode=self.obj_display_mode)
-            else:
-                self.object_ctrl.add_object(object_name='probe - piece',
-                                            object_type='probe piece',
-                                            object_data=center_data_3d,
-                                            object_mode=self.obj_display_mode)
+                    self.object_ctrl.add_object(
+                        object_name="probe {} - piece".format(i),
+                        object_type="probe piece",
+                        object_data=line_data[i],
+                        object_mode=self.obj_display_mode,
+                    )
+            else:
+                self.object_ctrl.add_object(
+                    object_name="probe - piece",
+                    object_type="probe piece",
+                    object_data=center_data_3d,
+                    object_mode=self.obj_display_mode,
+                )
 
-            self.working_atlas_data['atlas-probe'].clear()
-            self.working_img_data['img-probe'].clear()
+            self.working_atlas_data["atlas-probe"].clear()
+            self.working_img_data["img-probe"].clear()
 
     def make_virus_piece(self):
         if self.h2a_transferred:
-            if not self.working_atlas_data['atlas-virus']:
+            if not self.working_atlas_data["atlas-virus"]:
                 return
-            processing_pnt = np.asarray(self.working_atlas_data['atlas-virus'])
+            processing_pnt = np.asarray(self.working_atlas_data["atlas-virus"])
         else:
-            if self.working_img_data['img-virus'] is None:
+            if self.working_img_data["img-virus"] is None:
                 return
-            inds = np.where(self.working_img_data['img-virus'] != 0)
+            inds = np.where(self.working_img_data["img-virus"] != 0)
             processing_pnt = np.vstack([inds[0], inds[1]]).T
 
-        data = self.atlas_view.get_3d_data_from_2d_view(processing_pnt, self.atlas_display)
-        self.object_ctrl.add_object(object_name='virus - piece',
-                                    object_type='virus piece',
-                                    object_data=data,
-                                    object_mode=self.obj_display_mode)
+        data = self.atlas_view.get_3d_data_from_2d_view(
+            processing_pnt, self.atlas_display
+        )
+        self.object_ctrl.add_object(
+            object_name="virus - piece",
+            object_type="virus piece",
+            object_data=data,
+            object_mode=self.obj_display_mode,
+        )
 
-        self.working_atlas_data['atlas-virus'] = []
+        self.working_atlas_data["atlas-virus"] = []
 
     def make_contour_piece(self):
         if self.h2a_transferred:
-            if not self.working_atlas_data['atlas-contour']:
+            if not self.working_atlas_data["atlas-contour"]:
                 return
-            processing_pnt = np.asarray(self.working_atlas_data['atlas-contour'])
+            processing_pnt = np.asarray(self.working_atlas_data["atlas-contour"])
         else:
-            if not self.working_img_data['img-contour']:
+            if not self.working_img_data["img-contour"]:
                 return
-            inds = np.where(self.working_img_data['img-contour'] != 0)
+            inds = np.where(self.working_img_data["img-contour"] != 0)
             processing_pnt = np.vstack([inds[0], inds[1]]).T
 
-        data = self.atlas_view.get_3d_data_from_2d_view(processing_pnt, self.atlas_display)
-        self.object_ctrl.add_object(object_name='contour - piece',
-                                    object_type='contour piece',
-                                    object_data=data,
-                                    object_mode=self.obj_display_mode)
+        data = self.atlas_view.get_3d_data_from_2d_view(
+            processing_pnt, self.atlas_display
+        )
+        self.object_ctrl.add_object(
+            object_name="contour - piece",
+            object_type="contour piece",
+            object_data=data,
+            object_mode=self.obj_display_mode,
+        )
 
-        self.working_atlas_data['atlas-contour'] = []
+        self.working_atlas_data["atlas-contour"] = []
 
     def make_drawing_piece(self):
         if self.a2h_transferred:
-            data_tobe_registered = self.working_img_data['img-drawing']
+            data_tobe_registered = self.working_img_data["img-drawing"]
         else:
-            data_tobe_registered = self.working_atlas_data['atlas-drawing']
+            data_tobe_registered = self.working_atlas_data["atlas-drawing"]
         if not data_tobe_registered:
             return
         processing_data = np.asarray(data_tobe_registered)
         if self.tool_box.is_closed:
             if np.any(processing_data[0] != processing_data[-1]):
                 processing_data = np.vstack([processing_data, processing_data[0]])
             temp_img = np.zeros(self.atlas_view.working_atlas.img.image.shape)
-            cv2.fillPoly(temp_img, pts=[processing_data.astype(int)], color=(255, 255, 255))
+            cv2.fillPoly(
+                temp_img, pts=[processing_data.astype(int)], color=(255, 255, 255)
+            )
             temp = np.where(temp_img != 0)
             processing_data = np.stack([temp[1], temp[0]], axis=1)
-            object_name = 'area drawing - piece'
+            object_name = "area drawing - piece"
         else:
-            object_name = 'line drawing - piece'
-        data = self.atlas_view.get_3d_data_from_2d_view(processing_data, self.atlas_display)
-        self.object_ctrl.add_object(object_name=object_name,
-                                    object_type='drawing piece',
-                                    object_data=data,
-                                    object_mode=self.obj_display_mode)
+            object_name = "line drawing - piece"
+        data = self.atlas_view.get_3d_data_from_2d_view(
+            processing_data, self.atlas_display
+        )
+        self.object_ctrl.add_object(
+            object_name=object_name,
+            object_type="drawing piece",
+            object_data=data,
+            object_mode=self.obj_display_mode,
+        )
 
-        self.working_atlas_data['atlas-drawing'] = []
+        self.working_atlas_data["atlas-drawing"] = []
 
     def make_cell_piece(self):
         if self.a2h_transferred:
-            data_tobe_registered = self.working_img_data['img-cells']
+            data_tobe_registered = self.working_img_data["img-cells"]
         else:
-            data_tobe_registered = self.working_atlas_data['atlas-cells']
+            data_tobe_registered = self.working_atlas_data["atlas-cells"]
 
         if not data_tobe_registered:
             return
         processing_data = np.asarray(data_tobe_registered)
-        data = self.atlas_view.get_3d_data_from_2d_view(processing_data, self.atlas_display)
+        data = self.atlas_view.get_3d_data_from_2d_view(
+            processing_data, self.atlas_display
+        )
         for i in range(5):
             if i == 0:
-                object_type = 'cells - piece'
+                object_type = "cells - piece"
             else:
-                object_type = 'cells {} - piece'.format(i)
-            if self.working_atlas_data['cell_count'][i] != 0:
-                piece_data = data[np.where(np.ravel(self.working_atlas_data['cell_layer_index']) == i)[0], :]
-                self.object_ctrl.add_object(object_name=object_type,
-                                            object_type='cells piece',
-                                            object_data=piece_data,
-                                            object_mode=self.obj_display_mode)
-
-        self.working_atlas_data['atlas-cells'].clear()
-        self.working_atlas_data['cell_size'].clear()
-        self.working_atlas_data['cell_symbol'].clear()
-        self.working_atlas_data['cell_layer_index'].clear()
-        self.working_atlas_data['cell_count'] = [0 for _ in range(5)]
-        self.tool_box.update_cell_count_label(self.working_atlas_data['cell_count'])
-
+                object_type = "cells {} - piece".format(i)
+            if self.working_atlas_data["cell_count"][i] != 0:
+                piece_data = data[
+                    np.where(
+                        np.ravel(self.working_atlas_data["cell_layer_index"]) == i
+                    )[0],
+                    :,
+                ]
+                self.object_ctrl.add_object(
+                    object_name=object_type,
+                    object_type="cells piece",
+                    object_data=piece_data,
+                    object_mode=self.obj_display_mode,
+                )
+
+        self.working_atlas_data["atlas-cells"].clear()
+        self.working_atlas_data["cell_size"].clear()
+        self.working_atlas_data["cell_symbol"].clear()
+        self.working_atlas_data["cell_layer_index"].clear()
+        self.working_atlas_data["cell_count"] = [0 for _ in range(5)]
+        self.tool_box.update_cell_count_label(self.working_atlas_data["cell_count"])
 
     def make_object_pieces(self):
         if self.num_windows == 4:
-            msg = 'Can not make pieces with all slice windows turned on.'
+            msg = "Can not make pieces with all slice windows turned on."
             self.print_message(msg, self.error_message_color)
             return
         self.make_probe_piece()
         self.make_virus_piece()
         self.make_cell_piece()
         self.make_drawing_piece()
         self.make_contour_piece()
 
     def add_3d_object(self, data_dict, obj_type):
-        if data_dict is None or 'piece' in obj_type:
+        if data_dict is None or "piece" in obj_type:
             self.object_3d_list.append([])
         else:
             obj_3d = make_3d_gl_widget(data_dict, obj_type)
-            if self.display_mode_3d == 'dark':
-                obj_3d.setGLOptions('opaque')
+            if self.display_mode_3d == "dark":
+                obj_3d.setGLOptions("opaque")
             else:
-                obj_3d.setGLOptions('additive')
+                obj_3d.setGLOptions("additive")
             self.object_3d_list.append(obj_3d)
             self.view3d.addItem(self.object_3d_list[-1])
 
     # probe related functions
     def merge_probes(self):
         if self.num_windows == 4:
-            msg = 'Can not merge probe pieces with all slice windows turned on.'
+            msg = "Can not merge probe pieces with all slice windows turned on."
             self.print_message(msg, self.error_message_color)
             return
-        probe_piece_count = len([da_piece for da_piece in self.object_ctrl.obj_type if da_piece == 'probe piece'])
+        probe_piece_count = len(
+            [
+                da_piece
+                for da_piece in self.object_ctrl.obj_type
+                if da_piece == "probe piece"
+            ]
+        )
         if probe_piece_count == 0:
             return
 
-        data, obj_names, pieces_names = self.object_ctrl.merge_pieces('probe piece')
+        data, obj_names, pieces_names = self.object_ctrl.merge_pieces("probe piece")
 
         label_data = np.transpose(self.atlas_view.atlas_label, (1, 2, 0))[:, :, ::-1]
         probe_setting_data = self.probe_settings.get_settings()
 
         merge_sites = self.tool_box.merge_sites
         if self.image_view.image_file is None:
             # pre-surgery
             if self.multi_shanks and self.valid_multi_settings:
                 site_face_vec = self.multi_settings.faces.copy()
             else:
                 site_face_vec = [self.site_face for _ in range(len(data))]
             for i in range(len(data)):
                 if len(data[i]) != 1:
-                    msg = 'For pre-surgery plan, the desired probe can be merged from only one piece.'
+                    msg = "For pre-surgery plan, the desired probe can be merged from only one piece."
                     self.print_message(msg, self.error_message_color)
                     return
                 else:
                     if len(data[i][0]) == 1:
-                        self.print_message('Can not merge probe with only one point.', self.error_message_color)
+                        self.print_message(
+                            "Can not merge probe with only one point.",
+                            self.error_message_color,
+                        )
                         return
 
                 n_hat = self.atlas_view.get_plane_norm_vector(self.atlas_display)
 
                 info_dict, error_index = calculate_probe_info(
-                    data[i], pieces_names[i], label_data, self.atlas_view.label_info, self.atlas_view.vox_size_um,
-                    probe_setting_data, merge_sites, self.atlas_view.origin_3d, site_face_vec[i], n_hat, True)
+                    data[i],
+                    pieces_names[i],
+                    label_data,
+                    self.atlas_view.label_info,
+                    self.atlas_view.vox_size_um,
+                    probe_setting_data,
+                    merge_sites,
+                    self.atlas_view.origin_3d,
+                    site_face_vec[i],
+                    n_hat,
+                    True,
+                )
 
                 if error_index != 0:
-                    msg = 'Error index: {}, please contact maintainers.'.format(error_index)
+                    msg = "Error index: {}, please contact maintainers.".format(
+                        error_index
+                    )
                     self.print_message(msg, self.error_message_color)
                     return
 
-                self.object_ctrl.add_object(obj_names[i], 'merged probe',
-                                            object_data=info_dict, object_mode=self.obj_display_mode)
+                self.object_ctrl.add_object(
+                    obj_names[i],
+                    "merged probe",
+                    object_data=info_dict,
+                    object_mode=self.obj_display_mode,
+                )
         else:
             # after-surgery
             for i in range(len(data)):
                 if len(data[i]) == 1:
                     if len(data[i][0]) == 1:
-                        self.print_message('Can not merge probe with only one point.', self.error_message_color)
+                        self.print_message(
+                            "Can not merge probe with only one point.",
+                            self.error_message_color,
+                        )
                         return
 
                 info_dict, error_index = calculate_probe_info(
-                    data[i], pieces_names[i], label_data, self.atlas_view.label_info, self.atlas_view.vox_size_um,
-                    probe_setting_data, merge_sites, self.atlas_view.origin_3d, self.site_face, None, False)
+                    data[i],
+                    pieces_names[i],
+                    label_data,
+                    self.atlas_view.label_info,
+                    self.atlas_view.vox_size_um,
+                    probe_setting_data,
+                    merge_sites,
+                    self.atlas_view.origin_3d,
+                    self.site_face,
+                    None,
+                    False,
+                )
 
                 if error_index != 0:
-                    msg = 'Error index: {}, please contact maintainers.'.format(error_index)
+                    msg = "Error index: {}, please contact maintainers.".format(
+                        error_index
+                    )
                     self.print_message(msg, self.error_message_color)
                     return
 
-                self.object_ctrl.add_object(obj_names[i], 'merged probe',
-                                            object_data=info_dict, object_mode=self.obj_display_mode)
+                self.object_ctrl.add_object(
+                    obj_names[i],
+                    "merged probe",
+                    object_data=info_dict,
+                    object_mode=self.obj_display_mode,
+                )
 
     # virus related functions
     def merge_virus(self):
-        virus_piece_count = len([da_piece for da_piece in self.object_ctrl.obj_type if da_piece == 'virus piece'])
+        virus_piece_count = len(
+            [
+                da_piece
+                for da_piece in self.object_ctrl.obj_type
+                if da_piece == "virus piece"
+            ]
+        )
         if virus_piece_count == 0:
             return
-        data, obj_names, pieces_names = self.object_ctrl.merge_pieces('virus piece')
+        data, obj_names, pieces_names = self.object_ctrl.merge_pieces("virus piece")
         label_data = np.transpose(self.atlas_view.atlas_label, (1, 2, 0))[:, :, ::-1]
 
         for i in range(len(data)):
-            info_dict = calculate_virus_info(data[i], pieces_names[i], label_data, self.atlas_view.label_info,
-                                             self.atlas_view.origin_3d)
-            self.object_ctrl.add_object(obj_names[i], 'merged virus',
-                                        object_data=info_dict, object_mode=self.obj_display_mode)
+            info_dict = calculate_virus_info(
+                data[i],
+                pieces_names[i],
+                label_data,
+                self.atlas_view.label_info,
+                self.atlas_view.origin_3d,
+            )
+            self.object_ctrl.add_object(
+                obj_names[i],
+                "merged virus",
+                object_data=info_dict,
+                object_mode=self.obj_display_mode,
+            )
 
     # cell related functions
     def merge_cells(self):
-        cells_piece_count = len([da_piece for da_piece in self.object_ctrl.obj_type if da_piece == 'cells piece'])
+        cells_piece_count = len(
+            [
+                da_piece
+                for da_piece in self.object_ctrl.obj_type
+                if da_piece == "cells piece"
+            ]
+        )
         if cells_piece_count == 0:
             return
-        data, obj_names, pieces_names = self.object_ctrl.merge_pieces('cells piece')
+        data, obj_names, pieces_names = self.object_ctrl.merge_pieces("cells piece")
         label_data = np.transpose(self.atlas_view.atlas_label, (1, 2, 0))[:, :, ::-1]
 
         for i in range(len(data)):
-            info_dict = calculate_cells_info(data[i], pieces_names[i], label_data, self.atlas_view.label_info,
-                                             self.atlas_view.origin_3d)
-            self.object_ctrl.add_object(obj_names[i], 'merged cells',
-                                        object_data=info_dict, object_mode=self.obj_display_mode)
-
+            info_dict = calculate_cells_info(
+                data[i],
+                pieces_names[i],
+                label_data,
+                self.atlas_view.label_info,
+                self.atlas_view.origin_3d,
+            )
+            self.object_ctrl.add_object(
+                obj_names[i],
+                "merged cells",
+                object_data=info_dict,
+                object_mode=self.obj_display_mode,
+            )
 
     # drawing related functions
     def merge_drawings(self):
         drawing_piece_count = len(
-            [da_piece for da_piece in self.object_ctrl.obj_type if da_piece == 'drawing piece'])
+            [
+                da_piece
+                for da_piece in self.object_ctrl.obj_type
+                if da_piece == "drawing piece"
+            ]
+        )
         if drawing_piece_count == 0:
             return
-        data, obj_names, pieces_names = self.object_ctrl.merge_pieces('drawing piece')
+        data, obj_names, pieces_names = self.object_ctrl.merge_pieces("drawing piece")
         label_data = np.transpose(self.atlas_view.atlas_label, (1, 2, 0))[:, :, ::-1]
 
         for i in range(len(data)):
             info_dict = calculate_drawing_info(
-                data[i], pieces_names[i], label_data, self.atlas_view.label_info, self.atlas_view.origin_3d)
+                data[i],
+                pieces_names[i],
+                label_data,
+                self.atlas_view.label_info,
+                self.atlas_view.origin_3d,
+            )
             self.object_ctrl.add_object(
-                obj_names[i], 'merged drawing', object_data=info_dict, object_mode=self.obj_display_mode)
-
+                obj_names[i],
+                "merged drawing",
+                object_data=info_dict,
+                object_mode=self.obj_display_mode,
+            )
 
     # contour related functions
     def merge_contour(self):
         contour_piece_count = len(
-            [da_piece for da_piece in self.object_ctrl.obj_type if da_piece == 'contour piece'])
+            [
+                da_piece
+                for da_piece in self.object_ctrl.obj_type
+                if da_piece == "contour piece"
+            ]
+        )
         if contour_piece_count == 0:
             return
-        data, obj_names, pieces_names = self.object_ctrl.merge_pieces('contour piece')
+        data, obj_names, pieces_names = self.object_ctrl.merge_pieces("contour piece")
 
         for i in range(len(data)):
-            info_dict = {'object_type': 'contour', 'data': data[i]}
-            self.object_ctrl.add_object(obj_names[i], 'merged contour',
-                                        object_data=info_dict, object_mode=self.obj_display_mode)
+            info_dict = {"object_type": "contour", "data": data[i]}
+            self.object_ctrl.add_object(
+                obj_names[i],
+                "merged contour",
+                object_data=info_dict,
+                object_mode=self.obj_display_mode,
+            )
 
     # common functions
     def obj_color_changed(self, ev):
         clicked_index = ev[0]
         color = ev[1]
-        self.object_ctrl.obj_data[clicked_index]['vis_color'] = color
+        self.object_ctrl.obj_data[clicked_index]["vis_color"] = color
         vis_color = get_object_vis_color(color)
         self.object_3d_list[clicked_index].setData(color=vis_color)
 
     def obj_opacity_changed(self, val):
-        col = self.object_ctrl.obj_data[self.object_ctrl.current_obj_index]['vis_color']
+        col = self.object_ctrl.obj_data[self.object_ctrl.current_obj_index]["vis_color"]
         vis_color = (col[0] / 255, col[1] / 255, col[2] / 255, val / 100)
         self.object_3d_list[self.object_ctrl.current_obj_index].setData(color=vis_color)
 
     def obj_blend_mode_changed(self, blend_mode):
         self.object_3d_list[self.object_ctrl.current_obj_index].setGLOptions(blend_mode)
 
     def obj_vis_changed(self, ev):
@@ -4633,78 +6033,92 @@
             self.view3d.removeItem(self.object_3d_list[ind])
             self.object_3d_list[ind].deleteLater()
         del self.object_3d_list[ind]
 
     def gl_object_added(self, obj):
         data_dict = obj[0]
         obj_type = obj[1]
-        if data_dict is None or 'piece' in obj_type:
+        if data_dict is None or "piece" in obj_type:
             self.object_3d_list.append([])
         else:
             obj_3d = make_3d_gl_widget(data_dict, obj_type)
-            if self.display_mode_3d == 'dark':
-                obj_3d.setGLOptions('opaque')
+            if self.display_mode_3d == "dark":
+                obj_3d.setGLOptions("opaque")
             else:
-                obj_3d.setGLOptions('additive')
+                obj_3d.setGLOptions("additive")
             self.object_3d_list.append(obj_3d)
             self.view3d.addItem(self.object_3d_list[-1])
 
     def obj_size_changed(self, ev):
         obj_type = ev[0]
         val = ev[1]
-        if 'probe' in obj_type or 'drawing' in obj_type or 'contour' in obj_type:
+
+        if "probe" in obj_type or "drawing" in obj_type or "contour" in obj_type:
             self.object_3d_list[self.object_ctrl.current_obj_index].setData(width=val)
         else:
             self.object_3d_list[self.object_ctrl.current_obj_index].setData(size=val)
 
     # ------------------------------------------------------------------
     #
     #                       Image Loader
     #
     # ------------------------------------------------------------------
     def load_image(self):
-        self.print_message('Load Image ...', self.normal_color)
+        self.print_message("Load Image ...", self.normal_color)
         file_title = "Select Histological Image File"
-        file_filter = "CZI (*.czi);;JPEG (*.jpg);;PNG (*.png);;TIFF (*.tif);;BMP (*.bmp)"
+        file_filter = (
+            "CZI (*.czi);;JPEG (*.jpg);;PNG (*.png);;TIFF (*.tif);;BMP (*.bmp)"
+        )
         if self.current_img_path is None:
             file_path = self.home_path
         else:
             file_path = self.current_img_path
         file_options = QFileDialog.Options()
         file_options |= QFileDialog.DontUseNativeDialog
         file_dialog = QFileDialog()
         file_dialog.setFileMode(QFileDialog.ExistingFiles)
-        image_file_path = file_dialog.getOpenFileName(self, file_title, file_path, file_filter, options=file_options)
+        image_file_path = file_dialog.getOpenFileName(
+            self, file_title, file_path, file_filter, options=file_options
+        )
 
-        if image_file_path[0] != '':
+        if image_file_path[0] != "":
             image_name, image_file_type = os.path.splitext(image_file_path[0])
             self.current_img_path = image_file_path[0]
-            self.current_img_name = os.path.basename(os.path.realpath(image_file_path[0]))
+            self.current_img_name = os.path.basename(
+                os.path.realpath(image_file_path[0])
+            )
             self.load_single_image_file(self.current_img_path, image_file_type)
             self.save_path = image_file_path[0]
-            self.project_method = 'pre plan'
+            self.project_method = "pre plan"
             self.tool_box.pre_site_face_combo.setVisible(False)
             self.tool_box.after_site_face_combo.setVisible(True)
         else:
             if self.image_view.image_file is None:
-                self.statusbar.showMessage('No image file is selected.')
+                self.statusbar.showMessage("No image file is selected.")
             else:
-                self.statusbar.showMessage('No new image file is selected.')
+                self.statusbar.showMessage("No new image file is selected.")
             return
 
-    def load_single_image_file(self, image_file_path, image_file_type, scene_index=None):
+    def load_single_image_file(
+        self, image_file_path, image_file_type, scene_index=None
+    ):
         with pg.BusyCursor():
-            if image_file_type == '.czi':
+            if image_file_type == ".czi":
                 try:
                     image_file = CZIReader(image_file_path)
                 except (IOError, OSError, IndexError, AttributeError):
-                    self.print_message('Load CZI file failed.', self.error_message_color)
+                    self.print_message(
+                        "Load CZI file failed.", self.error_message_color
+                    )
                     return
                 if image_file.error_index != 0:
-                    self.print_message('Error Index: {}'.format(image_file.error_index), self.error_message_color)
+                    self.print_message(
+                        "Error Index: {}".format(image_file.error_index),
+                        self.error_message_color,
+                    )
                     return
                 scale = self.image_view.scale_slider.value()
                 scale = scale * 0.01
                 if scene_index is None:
                     if self.image_view.check_scenes.isChecked():
                         image_file.read_data(scale, scene_index=None)
                     else:
@@ -4714,46 +6128,56 @@
                 if image_file.is_rgb:
                     self.tool_box.cell_count_label_list[0].setVisible(True)
                     self.tool_box.cell_count_val_list[0].setVisible(True)
                 else:
                     for i in range(image_file.n_channels):
                         self.tool_box.cell_count_label_list[i + 1].setVisible(True)
                         self.tool_box.cell_count_val_list[i + 1].setVisible(True)
-            elif image_file_type == '.tif':
+            elif image_file_type == ".tif":
                 try:
                     image_file = TIFFReader(image_file_path)
                 except (IOError, OSError, IndexError, AttributeError):
-                    self.print_message('Load TIF file failed.', self.error_message_color)
+                    self.print_message(
+                        "Load TIF file failed.", self.error_message_color
+                    )
                     return
                 if image_file.error_index != 0:
-                    self.print_message('Error Index: {}'.format(image_file.error_index), self.error_message_color)
+                    self.print_message(
+                        "Error Index: {}".format(image_file.error_index),
+                        self.error_message_color,
+                    )
                     return
                 if image_file.is_rgb:
                     self.tool_box.cell_count_label_list[0].setVisible(True)
                     self.tool_box.cell_count_val_list[0].setVisible(True)
                 else:
                     for i in range(image_file.n_channels):
                         self.tool_box.cell_count_label_list[i + 1].setVisible(True)
                         self.tool_box.cell_count_val_list[i + 1].setVisible(True)
             else:
                 try:
                     image_file = ImageReader(image_file_path)
                 except (IOError, OSError, IndexError, AttributeError):
-                    self.print_message('Load RGB image file failed.', self.error_message_color)
+                    self.print_message(
+                        "Load RGB image file failed.", self.error_message_color
+                    )
                     return
                 if image_file.error_index != 0:
-                    self.print_message('Error Index: {}'.format(image_file.error_index), self.error_message_color)
+                    self.print_message(
+                        "Error Index: {}".format(image_file.error_index),
+                        self.error_message_color,
+                    )
                     return
                 self.tool_box.cell_count_label_list[0].setVisible(True)
                 self.tool_box.cell_count_val_list[0].setVisible(True)
 
             self.image_view.set_data(image_file)
             self.reset_corners_hist()
             self.layerpanel.setEnabled(True)
-        self.statusbar.showMessage('Image file loaded.')
+        self.statusbar.showMessage("Image file loaded.")
 
         # if self.image_view.image_file.n_pages > 1:
         #     da_data = self.image_view.volume_img.copy()
         #     d2 = np.empty(da_data.shape + (4,), dtype=np.ubyte)
         #     d2[..., 0] = da_data * (255. / (da_data.max() / 1))
         #     d2[..., 1] = d2[..., 0]
         #     d2[..., 2] = d2[..., 0]
@@ -4792,136 +6216,161 @@
         else:
             self.show_2_windows()
 
         self.sidebar.setCurrentIndex(2)
 
     # load multiple images
     def load_images(self):
-        self.statusbar.showMessage('Selecte folder to load multiple images, files can not be .czi format ...')
-        images_folder = str(QFileDialog.getExistingDirectory(self, "Select Images Folder"))
-        if images_folder != '':
+        self.statusbar.showMessage(
+            "Selecte folder to load multiple images, files can not be .czi format ..."
+        )
+        images_folder = str(
+            QFileDialog.getExistingDirectory(self, "Select Images Folder")
+        )
+        if images_folder != "":
             # image_files_list = os.listdir(images_folder)
             # image_files_list = natsorted(image_files_list)
 
             with pg.BusyCursor():
                 with warnings.catch_warnings():
                     warnings.filterwarnings("error")
                     image_file = ImagesReader(images_folder)
                     self.image_view.set_data(image_file)
 
             self.sidebar.setCurrentIndex(3)
-            self.statusbar.showMessage('Image files loaded.')
+            self.statusbar.showMessage("Image files loaded.")
         else:
             return
 
     # ------------------------------------------------------------------
     #
     #              Menu Bar ---- File ----- related
     #
     # ------------------------------------------------------------------
     def load_slice_atlas(self, atlas_path):
         self.slice_atlas_path = atlas_path
         self.current_atlas_path = atlas_path
         self.atlas_view.clear_slice_info()
 
-        if atlas_path[-4:] in ['.jpg', '.png']:
+        if atlas_path[-4:] in [".jpg", ".png"]:
             try:
                 img_data = cv2.imread(atlas_path)
             except (IOError, OSError):
-                msg = 'Loading slice atlas is failed. Please check your image or contact maintainers.'
+                msg = "Loading slice atlas is failed. Please check your image or contact maintainers."
                 self.print_message(msg, self.error_message_color)
                 return
             img_data = cv2.cvtColor(img_data, cv2.COLOR_BGR2RGBA)
             self.atlas_view.set_slice_data(img_data)
         else:
             try:
-                with open(atlas_path, 'rb') as f:
+                with open(atlas_path, "rb") as f:
                     slice_data = pickle.load(f)
             except (IOError, OSError, pickle.PickleError, pickle.UnpicklingError):
-                msg = 'Loading slice atlas is failed. Please check your image or contact maintainers.'
+                msg = "Loading slice atlas is failed. Please check your image or contact maintainers."
                 self.print_message(msg, self.error_message_color)
                 return
             self.atlas_view.set_slice_data_and_info(slice_data)
 
         self.reset_tri_points_atlas()
 
         self.show_only_slice_window()
 
-        self.actionSwitch_Atlas.setText('Switch Atlas: Slice')
-        self.current_atlas = 'slice'
+        self.actionSwitch_Atlas.setText("Switch Atlas: Slice")
+        self.current_atlas = "slice"
         self.atlascontrolpanel.setEnabled(False)
         self.treeviewpanel.setEnabled(False)
         self.actionBregma_Picker.setEnabled(True)
         self.actionCreate_Slice_Layer.setEnabled(True)
         self.delete_all_atlas_layer()
 
         self.object_ctrl.add_object_btn.setEnabled(False)
         self.object_ctrl.merge_probe_btn.setEnabled(False)
 
-    def set_volume_atlas_to_view(self, atlas_data, segmentation_data, atlas_info, label_info, boundary):
+    def set_volume_atlas_to_view(
+        self, atlas_data, segmentation_data, atlas_info, label_info, boundary
+    ):
         if self.atlas_view.atlas_data is not None:
-            self.atlas_view.mesh.translate(self.atlas_view.origin_3d[0], self.atlas_view.origin_3d[1],
-                                           self.atlas_view.origin_3d[2])
+            self.atlas_view.mesh.translate(
+                self.atlas_view.origin_3d[0],
+                self.atlas_view.origin_3d[1],
+                self.atlas_view.origin_3d[2],
+            )
             for label_id in list(self.small_mesh_list.keys()):
                 self.view3d.removeItem(self.small_mesh_list[label_id])
             self.small_mesh_list.clear()
 
-        self.atlas_view.set_data(atlas_data, segmentation_data, atlas_info, label_info, boundary)
+        self.atlas_view.set_data(
+            atlas_data, segmentation_data, atlas_info, label_info, boundary
+        )
         self.atlas_view.working_cut_changed(self.atlas_display)
         self.reset_tri_points_atlas()
 
         if self.image_view.image_file is None:
-            if self.atlas_display == 'coronal':
+            if self.atlas_display == "coronal":
                 self.show_only_coronal_window()
-            elif self.atlas_display == 'sagittal':
+            elif self.atlas_display == "sagittal":
                 self.show_only_sagital_window()
             else:
                 self.show_only_horizontal_window()
         else:
             self.show_2_windows()
 
-        msg = 'Successfully set atlas data to view. Checking rendering for 3D visualisation...'
+        msg = "Successfully set atlas data to view. Checking rendering for 3D visualisation..."
         self.print_message(msg, self.normal_color)
 
     def set_volume_atlas_3d(self, unique_label, meshdata, small_meshdata_list):
         self.atlas_view.mesh.setMeshData(meshdata=meshdata)
         mesh_origin = np.ravel(self.atlas_view.origin_3d)
-        self.atlas_view.mesh.translate(-mesh_origin[0], -mesh_origin[1], -mesh_origin[2])
+        self.atlas_view.mesh.translate(
+            -mesh_origin[0], -mesh_origin[1], -mesh_origin[2]
+        )
 
-        self.print_message('Brain mesh is Loaded.', self.normal_color)
+        self.print_message("Brain mesh is Loaded.", self.normal_color)
 
         for id in unique_label:
             id = int(id)
             if id == 0:
                 continue
-            if id in self.atlas_view.label_info['index']:
-                color_to_set = self.atlas_view.label_info['color'][(self.atlas_view.label_info['index'] == id)][0] / 255
-                mesh = gl.GLMeshItem(meshdata=small_meshdata_list[str(id)], smooth=True,
-                                     color=(color_to_set[0], color_to_set[1], color_to_set[2], 0.8), shader='balloon')
-                mesh.setGLOptions('opaque')
+            if id in self.atlas_view.label_info["index"]:
+                color_to_set = (
+                    self.atlas_view.label_info["color"][
+                        (self.atlas_view.label_info["index"] == id)
+                    ][0]
+                    / 255
+                )
+                mesh = gl.GLMeshItem(
+                    meshdata=small_meshdata_list[str(id)],
+                    smooth=True,
+                    color=(color_to_set[0], color_to_set[1], color_to_set[2], 0.8),
+                    shader="balloon",
+                )
+                mesh.setGLOptions("opaque")
                 mesh.translate(-mesh_origin[0], -mesh_origin[1], -mesh_origin[2])
                 self.small_mesh_list[str(id)] = mesh
                 self.small_mesh_list[str(id)].setVisible(False)
 
         mesh_keys = list(self.small_mesh_list.keys())
         for i in range(len(self.small_mesh_list)):
             self.view3d.addItem(self.small_mesh_list[mesh_keys[i]])
 
         self.sidebar.setCurrentIndex(0)
 
-        self.print_message('Brain region mesh is Loaded.  Atlas loaded and set successfully.', self.normal_color)
+        self.print_message(
+            "Brain region mesh is Loaded.  Atlas loaded and set successfully.",
+            self.normal_color,
+        )
 
     # load volume atlas
     def load_volume_atlas(self, atlas_folder):
         self.volume_atlas_path = atlas_folder
         self.current_atlas_path = atlas_folder
         self.atlascontrolpanel.setEnabled(True)
         self.treeviewpanel.setEnabled(True)
-        self.actionSwitch_Atlas.setText('Switch Atlas: Volume')
-        self.current_atlas = 'volume'
+        self.actionSwitch_Atlas.setText("Switch Atlas: Volume")
+        self.current_atlas = "volume"
         self.actionBregma_Picker.setEnabled(False)
         self.actionCreate_Slice_Layer.setEnabled(False)
 
         if self.atlas_view.atlas_data is not None:
             self.delete_all_atlas_layer()
             # self.atlas_view.clear_atlas()
             # self.view3d.clear()
@@ -4934,584 +6383,770 @@
             # from Archived.HERBS.herbs.atlas_loader import AtlasLoader
             da_atlas = AtlasLoader(atlas_folder)
 
         if not da_atlas.success:
             self.statusbar.showMessage(da_atlas.msg)
             return
         else:
-            self.print_message('Atlas loaded successfully.', self.normal_color)
+            self.print_message("Atlas loaded successfully.", self.normal_color)
 
         # load mesh data
-        pre_made_meshdata_path = os.path.join(atlas_folder, 'atlas_meshdata.pkl')
-        pre_made_small_meshdata_path = os.path.join(atlas_folder, 'atlas_small_meshdata.pkl')
-
-        if not os.path.exists(pre_made_meshdata_path) or not os.path.exists(pre_made_small_meshdata_path):
-            msg = 'Brain mesh is not found! Please pre-process the atlas.'
+        pre_made_meshdata_path = os.path.join(atlas_folder, "atlas_meshdata.pkl")
+        pre_made_small_meshdata_path = os.path.join(
+            atlas_folder, "atlas_small_meshdata.pkl"
+        )
+
+        if not os.path.exists(pre_made_meshdata_path) or not os.path.exists(
+            pre_made_small_meshdata_path
+        ):
+            msg = "Brain mesh is not found! Please pre-process the atlas."
             self.print_message(msg, self.error_message_color)
 
         try:
-            infile = open(pre_made_meshdata_path, 'rb')
+            infile = open(pre_made_meshdata_path, "rb")
             meshdata = pickle.load(infile)
             infile.close()
-        except (IOError, OSError, ValueError, pickle.PickleError, pickle.UnpicklingError):
-            msg = 'Please pre-process mesh for the whole brain.'
+        except (
+            IOError,
+            OSError,
+            ValueError,
+            pickle.PickleError,
+            pickle.UnpicklingError,
+        ):
+            msg = "Please pre-process mesh for the whole brain."
             self.print_message(msg, self.error_message_color)
             return
 
         try:
-            infile = open(pre_made_small_meshdata_path, 'rb')
+            infile = open(pre_made_small_meshdata_path, "rb")
             small_meshdata_list = pickle.load(infile)
             infile.close()
-        except (IOError, OSError, ValueError, pickle.PickleError, pickle.UnpicklingError):
-            self.print_message('Please re-process meshes for each brain region.', self.error_message_color)
+        except (
+            IOError,
+            OSError,
+            ValueError,
+            pickle.PickleError,
+            pickle.UnpicklingError,
+        ):
+            self.print_message(
+                "Please re-process meshes for each brain region.",
+                self.error_message_color,
+            )
             return
 
         atlas_data = np.transpose(da_atlas.atlas_data, [2, 0, 1])[::-1, :, :]
         atlas_info = da_atlas.atlas_info
 
         label_info = da_atlas.label_info
 
-        segmentation_data = np.transpose(da_atlas.segmentation_data, [2, 0, 1])[::-1, :, :]
+        segmentation_data = np.transpose(da_atlas.segmentation_data, [2, 0, 1])[
+            ::-1, :, :
+        ]
         unique_label = da_atlas.unique_label
 
-        s_boundary = np.transpose(da_atlas.boundary['s_contour'], [2, 0, 1])[::-1, :, :]
-        c_boundary = np.transpose(da_atlas.boundary['c_contour'], [2, 0, 1])[::-1, :, :]
-        h_boundary = np.transpose(da_atlas.boundary['h_contour'], [2, 0, 1])[::-1, :, :]
-
-        boundary = {'s_contour': s_boundary, 'c_contour': c_boundary, 'h_contour': h_boundary}
-
-        self.set_volume_atlas_to_view(atlas_data, segmentation_data, atlas_info, label_info, boundary)
+        s_boundary = np.transpose(da_atlas.boundary["s_contour"], [2, 0, 1])[::-1, :, :]
+        c_boundary = np.transpose(da_atlas.boundary["c_contour"], [2, 0, 1])[::-1, :, :]
+        h_boundary = np.transpose(da_atlas.boundary["h_contour"], [2, 0, 1])[::-1, :, :]
+
+        boundary = {
+            "s_contour": s_boundary,
+            "c_contour": c_boundary,
+            "h_contour": h_boundary,
+        }
+
+        self.set_volume_atlas_to_view(
+            atlas_data, segmentation_data, atlas_info, label_info, boundary
+        )
 
         self.set_volume_atlas_3d(unique_label, meshdata, small_meshdata_list)
 
     # ------------------------------------------------------------------
     #
     #                       Atlas Loader
     #
     # ------------------------------------------------------------------
     def load_atlas_clicked(self):
-        self.print_message('Loading Brain Atlas...', self.normal_color)
+        self.print_message("Loading Brain Atlas...", self.normal_color)
 
         dialog_title = "Select Atlas Folder"
         if self.current_atlas_path is None:
             file_path = self.home_path
         else:
             file_path = self.current_atlas_path
         file_options = QFileDialog.Options()
         file_options |= QFileDialog.DontUseNativeDialog
-        atlas_folder = str(QFileDialog.getExistingDirectory(self, dialog_title, file_path, options=file_options))
-        with open('data/atlas_path.txt', 'w') as f:
+        atlas_folder = str(
+            QFileDialog.getExistingDirectory(
+                self, dialog_title, file_path, options=file_options
+            )
+        )
+        with open("data/atlas_path.txt", "w") as f:
             f.write(atlas_folder)
 
-        if atlas_folder != '':
+        if atlas_folder != "":
             self.load_volume_atlas(atlas_folder)
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     def load_previous_atlas(self):
         if self.atlas_view.atlas_data is not None:
             return
 
-        self.print_message('Loading Previous Loaded Volume Brain Atlas...', self.normal_color)
+        self.print_message(
+            "Loading Previous Loaded Volume Brain Atlas...", self.normal_color
+        )
 
-        if os.path.exists('data/atlas_path.txt'):
+        if os.path.exists("data/atlas_path.txt"):
             try:
-                with open('data/atlas_path.txt') as f:
+                with open("data/atlas_path.txt") as f:
                     lines = f.readlines()
                 atlas_folder = lines[0]
             except (IOError, OSError, IndexError):
-                atlas_folder = str(QFileDialog.getExistingDirectory(self, "Select Atlas Folder", self.home_path))
-                with open('data/atlas_path.txt', 'w') as f:
+                atlas_folder = str(
+                    QFileDialog.getExistingDirectory(
+                        self, "Select Atlas Folder", self.home_path
+                    )
+                )
+                with open("data/atlas_path.txt", "w") as f:
                     f.write(atlas_folder)
 
             if not os.path.exists(atlas_folder):
-                msg = 'The previous loaded volume atlas might be moved or deleted. Please selected atlas folder...'
+                msg = "The previous loaded volume atlas might be moved or deleted. Please selected atlas folder..."
                 self.print_message(msg, self.reminder_color)
-                atlas_folder = str(QFileDialog.getExistingDirectory(self, "Select Atlas Folder", self.home_path))
-                with open('data/atlas_path.txt', 'w') as f:
+                atlas_folder = str(
+                    QFileDialog.getExistingDirectory(
+                        self, "Select Atlas Folder", self.home_path
+                    )
+                )
+                with open("data/atlas_path.txt", "w") as f:
                     f.write(atlas_folder)
         else:
-            atlas_folder = str(QFileDialog.getExistingDirectory(self, "Select Atlas Folder", self.home_path))
-            with open('data/atlas_path.txt', 'w') as f:
+            atlas_folder = str(
+                QFileDialog.getExistingDirectory(
+                    self, "Select Atlas Folder", self.home_path
+                )
+            )
+            with open("data/atlas_path.txt", "w") as f:
                 f.write(atlas_folder)
 
-        if atlas_folder != '':
+        if atlas_folder != "":
             self.load_volume_atlas(atlas_folder)
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     # --------------------------------------------------------------------
     #                            save merged object
     # --------------------------------------------------------------------
     def save_merged_object(self, object_type):
         if not self.object_ctrl.obj_list:
-            self.print_message('No object is created ...', self.error_message_color)
+            self.print_message("No object is created ...", self.error_message_color)
             return
 
         otype = self.object_ctrl.obj_type
-        valid_index = [ind for ind in range(len(otype)) if object_type in otype[ind] and 'merged' in otype[ind]]
+        valid_index = [
+            ind
+            for ind in range(len(otype))
+            if object_type in otype[ind] and "merged" in otype[ind]
+        ]
 
         if not valid_index:
-            msg = 'No merged {} object is created ...'.format(object_type)
+            msg = "No merged {} object is created ...".format(object_type)
             self.print_message(msg, self.error_message_color)
             return
 
-        self.print_message('Saving {} objects ...'.format(object_type), self.normal_color)
-        save_path = str(QFileDialog.getExistingDirectory(self, "Select Folder to Save Objects", self.current_img_path))
-        if save_path != '':
+        self.print_message(
+            "Saving {} objects ...".format(object_type), self.normal_color
+        )
+        save_path = str(
+            QFileDialog.getExistingDirectory(
+                self, "Select Folder to Save Objects", self.current_img_path
+            )
+        )
+        if save_path != "":
             for da_ind in valid_index:
-                data = {'type': self.object_ctrl.obj_type[da_ind],
-                        'data': self.object_ctrl.obj_data[da_ind],
-                        'name': self.object_ctrl.obj_name[da_ind]}
+                data = {
+                    "type": self.object_ctrl.obj_type[da_ind],
+                    "data": self.object_ctrl.obj_data[da_ind],
+                    "name": self.object_ctrl.obj_name[da_ind],
+                }
                 s_path = os.path.join(save_path, self.object_ctrl.obj_name[da_ind])
-                with open('{}.pkl'.format(s_path), 'wb') as handle:
+                with open("{}.pkl".format(s_path), "wb") as handle:
                     pickle.dump(data, handle, protocol=pickle.HIGHEST_PROTOCOL)
         else:
             return
 
     def save_current_object(self):
         if self.object_ctrl.current_obj_index is None:
-            self.print_message('No object is created ...', self.error_message_color)
+            self.print_message("No object is created ...", self.error_message_color)
             return
-        file_name = QFileDialog.getSaveFileName(self, 'Save Current Object File', self.current_img_path,
-                                                "Pickle File (*.pkl)")
-        if file_name[0] != '':
-            da_data = {'type': self.object_ctrl.obj_type[self.object_ctrl.current_obj_index],
-                       'data': self.object_ctrl.obj_data[self.object_ctrl.current_obj_index],
-                       'name': self.object_ctrl.obj_name[self.object_ctrl.current_obj_index]}
-            with open(file_name[0], 'wb') as handle:
+        file_name = QFileDialog.getSaveFileName(
+            self,
+            "Save Current Object File",
+            self.current_img_path,
+            "Pickle File (*.pkl)",
+        )
+        if file_name[0] != "":
+            da_data = {
+                "type": self.object_ctrl.obj_type[self.object_ctrl.current_obj_index],
+                "data": self.object_ctrl.obj_data[self.object_ctrl.current_obj_index],
+                "name": self.object_ctrl.obj_name[self.object_ctrl.current_obj_index],
+            }
+            with open(file_name[0], "wb") as handle:
                 pickle.dump(da_data, handle, protocol=pickle.HIGHEST_PROTOCOL)
-            self.print_message('Current object is saved successfully.', self.normal_color)
+            self.print_message(
+                "Current object is saved successfully.", self.normal_color
+            )
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     # --------------------------------------------------------------------
     #                         Load object
     # --------------------------------------------------------------------
     def load_objects(self):
-        if self.atlas_view.atlas_data is None and self.atlas_view.slice_image_data is None:
-            self.print_message('Atlas need to be loaded first.', self.error_message_color)
+        if (
+            self.atlas_view.atlas_data is None
+            and self.atlas_view.slice_image_data is None
+        ):
+            self.print_message(
+                "Atlas need to be loaded first.", self.error_message_color
+            )
             return
         if self.num_windows == 4:
-            msg = 'Loading objects functions only when single atlas slice window displayed.'
+            msg = "Loading objects functions only when single atlas slice window displayed."
             self.print_message(msg, self.error_message_color)
             return
         file_options = QFileDialog.Options()
         file_options |= QFileDialog.DontUseNativeDialog
         dlg = QFileDialog()
         dlg.setFileMode(QFileDialog.ExistingFiles)
-        object_file_path = dlg.getOpenFileNames(self, "Load Object Files", self.home_path, "Pickle File (*.pkl)",
-                                                options=file_options)
+        object_file_path = dlg.getOpenFileNames(
+            self,
+            "Load Object Files",
+            self.home_path,
+            "Pickle File (*.pkl)",
+            options=file_options,
+        )
 
         if object_file_path[0]:
             n_files = len(object_file_path[0])
             problem_obj_name = []
             for i in range(n_files):
                 file_name = os.path.basename(object_file_path[0][i])
                 object_dict, msg = check_loading_pickle_file(object_file_path[0][i])
                 if msg is not None:
-                    self.print_message('Loading {} is failed. {}'.format(file_name, msg), self.error_message_color)
+                    self.print_message(
+                        "Loading {} is failed. {}".format(file_name, msg),
+                        self.error_message_color,
+                    )
                     return
 
-                if 'merged' in object_dict['type']:
-                    data_list = object_dict['data']['data']
+                if "merged" in object_dict["type"]:
+                    data_list = object_dict["data"]["data"]
                     data = data_list[0]
                     for j in range(1, len(data_list)):
-                        data = np.vstck([data, data_list[j]])
+                        data = np.vstack([data, data_list[j]])
                     max_val = np.max(data, 0)
                 else:
-                    max_val = np.max(object_dict['data'], 0)
+                    max_val = np.max(object_dict["data"], 0)
 
                 if np.any(max_val > self.atlas_view.atlas_size):
                     problem_obj_name.append(file_name)
                 else:
-                    self.object_ctrl.add_object(object_dict['name'], object_dict['type'],
-                                                object_dict['data'], self.obj_display_mode)
+                    self.object_ctrl.add_object(
+                        object_dict["name"],
+                        object_dict["type"],
+                        object_dict["data"],
+                        self.obj_display_mode,
+                    )
 
             if problem_obj_name:
-                msg = 'Objects {} not matching the atlas slice.'.format(','.join(problem_obj_name))
+                msg = "Objects {} not matching the atlas slice.".format(
+                    ",".join(problem_obj_name)
+                )
                 self.print_message(msg, self.error_message_color)
             else:
-                self.print_message('Objects loaded successfully.', self.normal_color)
+                self.print_message("Objects loaded successfully.", self.normal_color)
 
     # --------------------------------------------------------------------
     #                            save layer data
     # --------------------------------------------------------------------
     def save_current_layer(self):
         if len(self.layer_ctrl.current_layer_index) != 1:
-            msg = 'Saving current layer works only when single layer is active. Multiple or No layer is selected.'
+            msg = "Saving current layer works only when single layer is active. Multiple or No layer is selected."
             self.print_message(msg, self.error_message_color)
             return
-        self.print_message('Save current layer...', self.normal_color)
-        path = QFileDialog.getSaveFileName(self, "Save current layer", self.current_img_path)
-        if path[0] != '':
+        self.print_message("Save current layer...", self.normal_color)
+        path = QFileDialog.getSaveFileName(
+            self, "Save current layer", self.current_img_path
+        )
+        if path[0] != "":
             da_link = self.layer_ctrl.layer_link[self.layer_ctrl.current_layer_index[0]]
             color = self.layer_ctrl.layer_color[self.layer_ctrl.current_layer_index[0]]
-            tb_nail = self.layer_ctrl.layer_list[self.layer_ctrl.current_layer_index[0]].thumbnail_data
-            if 'img' in da_link:
+            tb_nail = self.layer_ctrl.layer_list[
+                self.layer_ctrl.current_layer_index[0]
+            ].thumbnail_data
+            if "img" in da_link:
                 self.save_hist_layer_data(da_link, color, tb_nail, path[0])
             else:
                 self.save_atlas_layer_data(da_link, color, tb_nail, path[0])
-            self.print_message('Current layer is saved.', self.normal_color)
+            self.print_message("Current layer is saved.", self.normal_color)
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     def save_all_layer(self):
         if not self.layer_ctrl.layer_link:
-            self.print_message('No layer is created.', self.error_message_color)
+            self.print_message("No layer is created.", self.error_message_color)
             return
-        self.print_message('Save all layers...', self.normal_color)
-        path = QFileDialog.getSaveFileName(self, "Save all layer", self.current_img_path)
-        if path[0] != '':
+        self.print_message("Save all layers...", self.normal_color)
+        path = QFileDialog.getSaveFileName(
+            self, "Save all layer", self.current_img_path
+        )
+        if path[0] != "":
             for da_link in self.layer_ctrl.layer_link:
                 da_ind = np.where(np.ravel(self.layer_ctrl.layer_link) == da_link)[0][0]
                 da_color = self.layer_ctrl.layer_color[da_ind]
                 tb_nail = self.layer_ctrl.layer_list[da_ind].thumbnail_data
-                if 'img' in da_link:
+                if "img" in da_link:
                     self.save_hist_layer_data(da_link, da_color, tb_nail, path[0])
                 else:
                     self.save_atlas_layer_data(da_link, da_color, tb_nail, path[0])
-            self.print_message('All layers are saved.', self.normal_color)
+            self.print_message("All layers are saved.", self.normal_color)
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     def get_hist_single_layer_vis_data(self, layer_link):
-        if layer_link == 'img-process':
+        if layer_link == "img-process":
             fdata = self.image_view.save_img_process_data()
         else:
-            if self.working_img_type[layer_link] == 'pixel':
+            if self.working_img_type[layer_link] == "pixel":
                 image_vis_data = self.image_view.img_stacks.image_dict[layer_link].image
             else:
-                image_vis_data = self.image_view.img_stacks.image_dict[layer_link].getData()
+                image_vis_data = self.image_view.img_stacks.image_dict[
+                    layer_link
+                ].getData()
                 image_vis_data = list(np.asarray(image_vis_data).T)
-            if layer_link == 'img-virus':
-                temp = np.where(self.working_img_data[layer_link] != 0)
+
+            if layer_link == "img-virus":
+                temp = np.where(image_vis_data != 0)
                 pnt_vec = np.stack([temp[1], temp[0]], axis=1) + 0.5
-                fdata = {'data': image_vis_data,
-                         'vector': pnt_vec.tolist()}
-            elif layer_link == 'img-cells':
+                fdata = {"data": image_vis_data, "vector": pnt_vec.tolist()}
+            elif layer_link == "img-cells":
                 temp_data = self.image_view.img_stacks.image_dict[layer_link].data
                 symbol_list = []
                 for i in range(len(temp_data)):
                     symbol_list.append(temp_data[i][3])
-                print('symbol list', symbol_list)
-                fdata = {'data': image_vis_data,
-                         'symbol': symbol_list,
-                         'cell_size': self.working_img_data['cell_size'],
-                         'cell_symbol': self.working_img_data['cell_symbol'],
-                         'cell_layer_index': self.working_img_data['cell_layer_index'],
-                         'cell_count': self.working_img_data['cell_count']}
+                # print("symbol list", symbol_list)
+                fdata = {
+                    "data": image_vis_data,
+                    "symbol": symbol_list,
+                    "cell_size": self.working_img_data["cell_size"],
+                    "cell_symbol": self.working_img_data["cell_symbol"],
+                    "cell_layer_index": self.working_img_data["cell_layer_index"],
+                    "cell_count": self.working_img_data["cell_count"],
+                }
             else:
-                fdata = {'data': image_vis_data}
+                fdata = {"data": image_vis_data}
 
         return fdata
 
     def save_hist_layer_data(self, layer_link, color, thumbnail, path):
         fdata = self.get_hist_single_layer_vis_data(layer_link)
 
-        fdata['layer_link'] = layer_link
-        fdata['color'] = color
-        fdata['thumbnail'] = thumbnail
+        fdata["layer_link"] = layer_link
+        fdata["color"] = color
+        fdata["thumbnail"] = thumbnail
 
-        fpath = '{}_{}.pkl'.format(path, layer_link)
-        with open(fpath, 'wb') as handle:
+        fpath = "{}_{}.pkl".format(path, layer_link)
+        with open(fpath, "wb") as handle:
             pickle.dump(fdata, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
-        if layer_link in ['img-process', 'img-mask', 'img-overlay']:
-            if layer_link == 'img-process':
-                if 'rgb' in self.image_view.image_file.pixel_type:
-                    print('rgb')
+        if layer_link in ["img-process", "img-mask", "img-overlay"]:
+            if layer_link == "img-process":
+                if "rgb" in self.image_view.image_file.pixel_type:
+                    print("rgb")
                     image_to_be_saved = self.image_view.processing_img.copy()
-                    if self.image_view.image_file.pixel_type != 'rgb24':
-                        image_to_be_saved = cv2.normalize(image_to_be_saved, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
+                    if self.image_view.image_file.pixel_type != "rgb24":
+                        image_to_be_saved = cv2.normalize(
+                            image_to_be_saved,
+                            None,
+                            0,
+                            255,
+                            cv2.NORM_MINMAX,
+                            dtype=cv2.CV_8U,
+                        )
                 else:
-                    image_to_be_saved = merge_channels_into_single_img(self.image_view.processing_img,
-                                                                       self.image_view.channel_color)
-            elif layer_link == 'img-mask':
-                image_to_be_saved = color_vis_img(self.working_img_data[layer_link], self.magic_wand_lut[1])
+                    image_to_be_saved = merge_channels_into_single_img(
+                        self.image_view.processing_img, self.image_view.channel_color
+                    )
+            elif layer_link == "img-mask":
+                image_to_be_saved = color_vis_img(
+                    self.working_img_data[layer_link], self.magic_wand_lut[1]
+                )
             else:
                 image_to_be_saved = self.working_img_data[layer_link]
 
-            fpath = '{}_{}.jpg'.format(path, layer_link)
+            fpath = "{}_{}.jpg".format(path, layer_link)
             da_img = cv2.cvtColor(image_to_be_saved, cv2.COLOR_RGB2BGR)
             cv2.imwrite(fpath, da_img)
         else:
             return
 
     def get_atlas_single_layer_vis_data(self, layer_link):
-        if layer_link == 'atlas-slice':
-            fdata = {'data': self.atlas_view.processing_slice}
+        if layer_link == "atlas-slice":
+            fdata = {"data": self.atlas_view.processing_slice}
         else:
-            if self.working_atlas_type[layer_link] == 'pixel':
-                image_vis_data = self.atlas_view.working_atlas.image_dict[layer_link].image
-            else:
-                image_vis_data = self.atlas_view.working_atlas.image_dict[layer_link].getData()
+            if self.working_atlas_type[layer_link] == "pixel":
+                image_vis_data = self.atlas_view.working_atlas.image_dict[
+                    layer_link
+                ].image
+            else:
+                image_vis_data = self.atlas_view.working_atlas.image_dict[
+                    layer_link
+                ].getData()
                 image_vis_data = list(np.asarray(image_vis_data).T)
-            if layer_link == 'atlas-cells':
+            if layer_link == "atlas-cells":
                 temp_data = self.atlas_view.working_atlas.image_dict[layer_link].data
                 symbol_list = []
                 for i in range(len(temp_data)):
                     symbol_list.append(temp_data[i][3])
-                fdata = {'data': image_vis_data,
-                         'symbol': symbol_list,
-                         'cell_size': self.working_atlas_data['cell_size'],
-                         'cell_symbol': self.working_atlas_data['cell_symbol'],
-                         'cell_layer_index': self.working_atlas_data['cell_layer_index'],
-                         'cell_count': self.working_atlas_data['cell_count']}
+                fdata = {
+                    "data": image_vis_data,
+                    "symbol": symbol_list,
+                    "cell_size": self.working_atlas_data["cell_size"],
+                    "cell_symbol": self.working_atlas_data["cell_symbol"],
+                    "cell_layer_index": self.working_atlas_data["cell_layer_index"],
+                    "cell_count": self.working_atlas_data["cell_count"],
+                }
             else:
-                fdata = {'data': image_vis_data}
+                fdata = {"data": image_vis_data}
 
         return fdata
 
     def save_atlas_layer_data(self, layer_link, color, thumbnail, path):
         fdata = self.get_atlas_single_layer_vis_data(layer_link)
 
-        fdata['layer_link'] = layer_link
-        fdata['color'] = color
-        fdata['thumbnail'] = thumbnail
+        fdata["layer_link"] = layer_link
+        fdata["color"] = color
+        fdata["thumbnail"] = thumbnail
 
-        fpath = '{}_{}.pkl'.format(path, layer_link)
-        with open(fpath, 'wb') as handle:
+        fpath = "{}_{}.pkl".format(path, layer_link)
+        with open(fpath, "wb") as handle:
             pickle.dump(fdata, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
-        if layer_link in ['atlas-slice', 'atlas-mask', 'atlas-overlay']:
-            if layer_link == 'atlas-slice':
+        if layer_link in ["atlas-slice", "atlas-mask", "atlas-overlay"]:
+            if layer_link == "atlas-slice":
                 image_to_be_saved = self.atlas_view.processing_slice.copy()
-            elif layer_link == 'atlas-mask':
-                image_to_be_saved = color_vis_img(self.working_atlas_data[layer_link], self.magic_wand_lut[1])
+            elif layer_link == "atlas-mask":
+                image_to_be_saved = color_vis_img(
+                    self.working_atlas_data[layer_link], self.magic_wand_lut[1]
+                )
             else:
                 image_to_be_saved = self.working_atlas_data[layer_link]
 
-            fpath = '{}_{}.jpg'.format(path, layer_link)
+            fpath = "{}_{}.jpg".format(path, layer_link)
             da_img = cv2.cvtColor(image_to_be_saved, cv2.COLOR_RGB2BGR)
             cv2.imwrite(fpath, da_img)
         else:
             return
 
     # --------------------------------------------------------------------
     #                            load layer data
     # --------------------------------------------------------------------
     def print_em_failed_layer(self, res, layer_link):
         if not res:
-            msg = 'Current loaded {} layer is not a wrong type or is not for current image.'.format(layer_link)
+            msg = "Current loaded {} layer is not a wrong type or is not for current image.".format(
+                layer_link
+            )
             self.print_message(msg, self.error_message_color)
         else:
             return
 
     def set_hist_layer_data(self, layer_dict):
-        layer_link = layer_dict['layer_link']
-        if layer_link == 'img-process':
+        layer_link = layer_dict["layer_link"]
+        if layer_link == "img-process":
             res = self.image_view.check_img_process_layer_data(layer_dict)
             self.print_em_failed_layer(res, layer_link)
             try:
-                self.image_view.processing_img = layer_dict['data']
+                self.image_view.processing_img = layer_dict["data"]
             except KeyError:
                 self.print_em_failed_layer(False, layer_link)
-        elif layer_link == 'img-virus':
+        elif layer_link == "img-virus":
             res = self.image_view.has_loaded_layer_the_same_size(layer_dict)
             self.print_em_failed_layer(res, layer_link)
             try:
-                self.working_img_data[layer_link] = layer_dict['data']
-                self.virus_lut[1] = layer_dict['color']
-                self.image_view.img_stacks.image_dict[layer_link].setLookupTable(self.virus_lut)
+                self.working_img_data[layer_link] = layer_dict["data"]
+                self.virus_lut[1] = layer_dict["color"]
+                self.image_view.img_stacks.image_dict[layer_link].setLookupTable(
+                    self.virus_lut
+                )
             except KeyError:
                 self.print_em_failed_layer(False, layer_link)
-        elif layer_link == 'img-mask':
+        elif layer_link == "img-mask":
             res = self.image_view.has_loaded_layer_the_same_size(layer_dict)
             self.print_em_failed_layer(res, layer_link)
             try:
-                self.tool_box.magic_color_btn.setColor(layer_dict['color'])
-                self.working_img_data[layer_link] = layer_dict['data']
-                self.magic_wand_lut[1] = layer_dict['color']
-                self.image_view.img_stacks.image_dict[layer_link].setLookupTable(self.magic_wand_lut)
+                self.tool_box.magic_color_btn.setColor(layer_dict["color"])
+                self.working_img_data[layer_link] = layer_dict["data"]
+                self.magic_wand_lut[1] = layer_dict["color"]
+                self.image_view.img_stacks.image_dict[layer_link].setLookupTable(
+                    self.magic_wand_lut
+                )
             except KeyError:
                 self.print_em_failed_layer(False, layer_link)
-        elif layer_link == 'img-drawing':
-            res = check_bounding_contains(np.asarray(layer_dict['data']), self.image_view.img_size)
+        elif layer_link == "img-drawing":
+            res = check_bounding_contains(
+                np.asarray(layer_dict["data"]), self.image_view.img_size
+            )
             self.print_em_failed_layer(res, layer_link)
             try:
-                self.working_img_data[layer_link] = layer_dict['data']
-                self.tool_box.pencil_color_btn.setColor(layer_dict['color'])
+                self.working_img_data[layer_link] = layer_dict["data"]
+                self.tool_box.pencil_color_btn.setColor(layer_dict["color"])
             except KeyError:
                 self.print_em_failed_layer(False, layer_link)
                 return
-            if np.all(self.working_img_data[layer_link][-1] == self.working_img_data[layer_link][0]):
+            if np.all(
+                self.working_img_data[layer_link][-1]
+                == self.working_img_data[layer_link][0]
+            ):
                 self.set_img_pencil_closed_style()
             else:
                 self.clear_img_pencil_closed_style()
-        elif layer_link == 'img-probe':
-            res = check_bounding_contains(np.asarray(layer_dict['data']), self.image_view.img_size)
+        elif layer_link == "img-probe":
+            res = check_bounding_contains(
+                np.asarray(layer_dict["data"]), self.image_view.img_size
+            )
             self.print_em_failed_layer(res, layer_link)
             try:
-                self.tool_box.probe_color_btn.setColor(layer_dict['color'])
-                self.working_img_data[layer_link] = layer_dict['data']
+                self.tool_box.probe_color_btn.setColor(layer_dict["color"])
+                self.working_img_data[layer_link] = layer_dict["data"]
             except KeyError:
                 self.print_em_failed_layer(False, layer_link)
                 return
-        elif layer_link == 'img-contour':
-            if not check_bounding_contains(np.asarray(layer_dict['data']), self.image_view.img_size):
-                msg = 'Current loaded img-contour layer is not for current image.'
-                self.print_message(msg,  self.error_message_color)
+        elif layer_link == "img-contour":
+            if not check_bounding_contains(
+                np.asarray(layer_dict["data"]), self.image_view.img_size
+            ):
+                msg = "Current loaded img-contour layer is not for current image."
+                self.print_message(msg, self.error_message_color)
                 return
-            self.contour_color = layer_dict['color']
-            self.working_img_data[layer_link] = layer_dict['data']
-            self.image_view.img_stacks.image_dict[layer_link].setPen(color=self.contour_color)
-        elif layer_link == 'img-cells':
-            if not check_bounding_contains(np.asarray(layer_dict['data']), self.image_view.img_size):
-                self.print_message('Current loaded img-cells layer is not for current image.', self.error_message_color)
+            self.contour_color = layer_dict["color"]
+            self.working_img_data[layer_link] = layer_dict["data"]
+            self.image_view.img_stacks.image_dict[layer_link].setPen(
+                color=self.contour_color
+            )
+        elif layer_link == "img-cells":
+            if not check_bounding_contains(
+                np.asarray(layer_dict["data"]), self.image_view.img_size
+            ):
+                self.print_message(
+                    "Current loaded img-cells layer is not for current image.",
+                    self.error_message_color,
+                )
                 return
-            self.tool_box.cell_color_btn.setColor(layer_dict['color'])
-            self.working_img_data[layer_link] = layer_dict['data']
-            self.working_img_data['cell_size'] = layer_dict['cell_size']
-            self.working_img_data['cell_symbol'] = layer_dict['cell_symbol']
-            self.working_img_data['cell_layer_index'] = layer_dict['cell_layer_index']
-            self.working_img_data['cell_count'] = layer_dict['cell_count']
-            self.tool_box.update_cell_count_label(self.working_img_data['cell_count'])
-        elif layer_link == 'img-overlay':
-            if not np.all(layer_dict['data'].shape[:2] == self.image_view.img_size):
-                msg = 'Current loaded img-overlay layer is not the same size as current image.'
+            self.tool_box.cell_color_btn.setColor(layer_dict["color"])
+            self.working_img_data[layer_link] = layer_dict["data"]
+            self.working_img_data["cell_size"] = layer_dict["cell_size"]
+            self.working_img_data["cell_symbol"] = layer_dict["cell_symbol"]
+            self.working_img_data["cell_layer_index"] = layer_dict["cell_layer_index"]
+            self.working_img_data["cell_count"] = layer_dict["cell_count"]
+            self.tool_box.update_cell_count_label(self.working_img_data["cell_count"])
+        elif layer_link == "img-overlay":
+            if not np.all(layer_dict["data"].shape[:2] == self.image_view.img_size):
+                msg = "Current loaded img-overlay layer is not the same size as current image."
                 self.print_message(msg, self.error_message_color)
                 return
-            self.working_img_data[layer_link] = layer_dict['data']
+            self.working_img_data[layer_link] = layer_dict["data"]
         else:
             return
 
     def set_hist_layer_to_hist_view(self, layer_link, vis_data_2d, symbol):
-        if layer_link == 'img-proces':
+        if layer_link == "img-proces":
             self.image_view.set_data_and_size(vis_data_2d)
-        elif layer_link == 'img-cells':
-            self.image_view.img_stacks.image_dict[layer_link].setData(pos=np.asarray(vis_data_2d), symbol=symbol)
-        elif layer_link == 'img-probe':
-            self.image_view.img_stacks.image_dict[layer_link].setData(pos=np.asarray(vis_data_2d))
-        elif layer_link in ['img-overlay', 'img-mask', 'img-virus']:
+        elif layer_link == "img-cells":
+            self.image_view.img_stacks.image_dict[layer_link].setData(
+                pos=np.asarray(vis_data_2d), symbol=symbol
+            )
+        elif layer_link == "img-probe":
+            self.image_view.img_stacks.image_dict[layer_link].setData(
+                pos=np.asarray(vis_data_2d)
+            )
+        elif layer_link in ["img-overlay", "img-mask", "img-virus"]:
             self.image_view.img_stacks.image_dict[layer_link].setImage(vis_data_2d)
-        elif layer_link in ['img-drawing', 'img-contour']:
-            self.image_view.img_stacks.image_dict[layer_link].setData(np.asarray(vis_data_2d))
+        elif layer_link in ["img-drawing", "img-contour"]:
+            self.image_view.img_stacks.image_dict[layer_link].setData(
+                np.asarray(vis_data_2d)
+            )
         else:
             return
 
     def set_atlas_layer_data(self, layer_dict):
-        layer_link = layer_dict['layer_link']
-        if layer_link == 'atlas-slice':
-            self.atlas_view.processing_slice = layer_dict['data']
-        elif layer_link == 'atlas-overlay':
-            self.working_atlas_data[layer_link] = layer_dict['data']
-        elif layer_link == 'atlas-mask':
-            self.working_atlas_data[layer_link] = layer_dict['data']
-            self.tool_box.magic_color_btn.setColor(layer_dict['color'])
-            self.magic_wand_lut[1] = layer_dict['color']
-            self.atlas_view.working_atlas.image_dict[layer_link].setLookupTable(self.magic_wand_lut)
-        elif layer_link == 'atlas-cells':
-            self.tool_box.cell_color_btn.setColor(layer_dict['color'])
-            self.working_atlas_data[layer_link] = layer_dict['data']
-            self.working_atlas_data['cell_count'] = layer_dict['cell_count']
-            self.working_atlas_data['cell_size'] = layer_dict['cell_size']
-            self.working_atlas_data['cell_symbol'] = layer_dict['cell_symbol']
-            self.working_atlas_data['cell_layer_index'] = layer_dict['cell_layer_index']
-            if not self.working_img_data['img-cells']:
+        layer_link = layer_dict["layer_link"]
+        if layer_link == "atlas-slice":
+            self.atlas_view.processing_slice = layer_dict["data"]
+        elif layer_link == "atlas-overlay":
+            self.working_atlas_data[layer_link] = layer_dict["data"]
+        elif layer_link == "atlas-mask":
+            self.working_atlas_data[layer_link] = layer_dict["data"]
+            self.tool_box.magic_color_btn.setColor(layer_dict["color"])
+            self.magic_wand_lut[1] = layer_dict["color"]
+            self.atlas_view.working_atlas.image_dict[layer_link].setLookupTable(
+                self.magic_wand_lut
+            )
+        elif layer_link == "atlas-cells":
+            self.tool_box.cell_color_btn.setColor(layer_dict["color"])
+            self.working_atlas_data[layer_link] = layer_dict["data"]
+            self.working_atlas_data["cell_count"] = layer_dict["cell_count"]
+            self.working_atlas_data["cell_size"] = layer_dict["cell_size"]
+            self.working_atlas_data["cell_symbol"] = layer_dict["cell_symbol"]
+            self.working_atlas_data["cell_layer_index"] = layer_dict["cell_layer_index"]
+            if not self.working_img_data["img-cells"]:
                 for i in range(5):
-                    self.tool_box.cell_count_val_list[i].setText(str(self.working_atlas_data['cell_count'][i]))
-        elif layer_link == 'atlas-drawing':
-            self.tool_box.pencil_color_btn.setColor(layer_dict['color'])
-            self.working_atlas_data[layer_link] = layer_dict['data']
-            if np.all(self.working_atlas_data[layer_link][-1] == self.working_atlas_data[layer_link][0]):
+                    self.tool_box.cell_count_val_list[i].setText(
+                        str(self.working_atlas_data["cell_count"][i])
+                    )
+        elif layer_link == "atlas-drawing":
+            self.tool_box.pencil_color_btn.setColor(layer_dict["color"])
+            self.working_atlas_data[layer_link] = layer_dict["data"]
+            if np.all(
+                self.working_atlas_data[layer_link][-1]
+                == self.working_atlas_data[layer_link][0]
+            ):
                 self.set_atlas_pencil_closed_style()
             else:
                 self.clear_atlas_pencil_closed_style()
-        elif layer_link == 'atlas-contour':
-            self.contour_color = layer_dict['color']
-            self.working_atlas_data[layer_link] = layer_dict['data']
-            self.atlas_view.working_atlas.image_dict[layer_link].setPen(color=self.contour_color)
-        elif layer_link == 'atlas-virus':
-            self.virus_lut[1] = layer_dict['color']
-            self.working_atlas_data[layer_link] = layer_dict['data']
-            self.atlas_view.working_atlas.image_dict[layer_link].setPen(layer_dict['color'])
-        elif layer_link == 'atlas-probe':
-            self.probe_color = layer_dict['color']
+        elif layer_link == "atlas-contour":
+            self.contour_color = layer_dict["color"]
+            self.working_atlas_data[layer_link] = layer_dict["data"]
+            self.atlas_view.working_atlas.image_dict[layer_link].setPen(
+                color=self.contour_color
+            )
+        elif layer_link == "atlas-virus":
+            self.virus_lut[1] = layer_dict["color"]
+            self.working_atlas_data[layer_link] = layer_dict["data"]
+            self.atlas_view.working_atlas.image_dict[layer_link].setPen(
+                layer_dict["color"]
+            )
+        elif layer_link == "atlas-probe":
+            self.probe_color = layer_dict["color"]
             self.tool_box.pencil_color_btn.setColor(self.probe_color)
-            self.working_atlas_data[layer_link] = layer_dict['data']
+            self.working_atlas_data[layer_link] = layer_dict["data"]
         else:
             return
 
     def set_atlas_layer_to_atlas_view(self, layer_link, vis_data_2d, symbol):
-        if layer_link == 'atlas-slice':
+        if layer_link == "atlas-slice":
             self.atlas_view.set_slice_data(vis_data_2d)
-        elif layer_link == 'atlas-cells':
-            self.atlas_view.working_atlas.image_dict[layer_link].setData(pos=np.asarray(vis_data_2d), symbol=symbol)
-        elif layer_link in ['atlas-overlay', 'atlas-mask']:
+        elif layer_link == "atlas-cells":
+            self.atlas_view.working_atlas.image_dict[layer_link].setData(
+                pos=np.asarray(vis_data_2d), symbol=symbol
+            )
+        elif layer_link in ["atlas-overlay", "atlas-mask"]:
             self.atlas_view.working_atlas.image_dict[layer_link].setImage(vis_data_2d)
-        elif layer_link in ['atlas-drawing', 'atlas-contour']:
-            self.atlas_view.working_atlas.image_dict[layer_link].setData(np.asarray(vis_data_2d))
-        elif layer_link in ['atlas-virus', 'atlas-probe']:
-            self.atlas_view.working_atlas.image_dict[layer_link].setData(pos=np.asarray(vis_data_2d))
+        elif layer_link in ["atlas-drawing", "atlas-contour"]:
+            self.atlas_view.working_atlas.image_dict[layer_link].setData(
+                np.asarray(vis_data_2d)
+            )
+        elif layer_link in ["atlas-virus", "atlas-probe"]:
+            self.atlas_view.working_atlas.image_dict[layer_link].setData(
+                pos=np.asarray(vis_data_2d)
+            )
         else:
             return
 
     def load_layers_called(self):
-        self.print_message('Loading layers ...', self.normal_color)
+        self.print_message("Loading layers ...", self.normal_color)
         file_options = QFileDialog.Options()
         file_options |= QFileDialog.DontUseNativeDialog
         dlg = QFileDialog()
         dlg.setFileMode(QFileDialog.ExistingFiles)
-        layer_files_path = dlg.getOpenFileNames(self, "Load Layer Files", self.home_path, "Pickle File (*.pkl)",
-                                                options=file_options)
+        layer_files_path = dlg.getOpenFileNames(
+            self,
+            "Load Layer Files",
+            self.home_path,
+            "Pickle File (*.pkl)",
+            options=file_options,
+        )
 
         if layer_files_path[0]:
             n_files = len(layer_files_path[0])
             for i in range(n_files):
                 file_path = layer_files_path[0][i]
                 layer_dict, msg = check_loading_pickle_file(file_path)
                 if msg is not None:
                     self.print_message(msg, self.error_message_color)
                     return
 
-                if 'img-' in layer_dict['layer_link']:
+                if "img-" in layer_dict["layer_link"]:
                     if self.image_view.current_img is None:
-                        self.print_message('Please load histological image first.', self.error_message_color)
+                        self.print_message(
+                            "Please load histological image first.",
+                            self.error_message_color,
+                        )
                         return
                     self.set_hist_layer_data(layer_dict)
-                    if 'cells' in layer_dict['layer_link']:
-                        symbol = layer_dict['symbol']
+                    if "cells" in layer_dict["layer_link"]:
+                        symbol = layer_dict["symbol"]
                     else:
                         symbol = None
-                    self.set_hist_layer_to_hist_view(layer_dict['layer_link'], layer_dict['data'], symbol)
+                    self.set_hist_layer_to_hist_view(
+                        layer_dict["layer_link"], layer_dict["data"], symbol
+                    )
                 else:
-                    if self.atlas_view.atlas_data is None and self.atlas_view.slice_image_data is None:
-                        self.print_message('Please load atlas first.', self.error_message_color)
+                    if (
+                        self.atlas_view.atlas_data is None
+                        and self.atlas_view.slice_image_data is None
+                    ):
+                        self.print_message(
+                            "Please load atlas first.", self.error_message_color
+                        )
                         return
                     self.set_atlas_layer_data(layer_dict)
-                    if 'cells' in layer_dict['layer_link']:
-                        symbol = layer_dict['symbol']
+                    if "cells" in layer_dict["layer_link"]:
+                        symbol = layer_dict["symbol"]
                     else:
                         symbol = None
-                    self.set_atlas_layer_to_atlas_view(layer_dict['layer_link'], layer_dict['data'], symbol)
-
-                self.layer_ctrl.master_layers(layer_dict['thumbnail'], layer_type=layer_dict['layer_link'], color=layer_dict['color'])
+                    self.set_atlas_layer_to_atlas_view(
+                        layer_dict["layer_link"], layer_dict["data"], symbol
+                    )
+
+                self.layer_ctrl.master_layers(
+                    layer_dict["thumbnail"],
+                    layer_type=layer_dict["layer_link"],
+                    color=layer_dict["color"],
+                )
                 # self.layer_ctrl.add_layer(layer_dict['layer_link'], layer_dict['color'])
                 # self.layer_ctrl.layer_list[-1].set_thumbnail_data(layer_dict['thumbnail'])
 
     # -------------------------------------------------------------
     #                    save project
     # -------------------------------------------------------------
     def save_project_called(self):
-        self.print_message('Saving Project ...', self.normal_color)
-        if self.atlas_view.atlas_data is None and self.atlas_view.slice_image_data is None and self.image_view.current_img is None:
-            self.print_message('No project can be saved.', self.reminder_color)
-            return
-        file_name = QFileDialog.getSaveFileName(self, 'Save Project', self.save_path, "Pickle File (*.pkl)")
-        if file_name[0] != '':
-            if self.current_atlas == 'slice':
+        self.print_message("Saving Project ...", self.normal_color)
+        if (
+            self.atlas_view.atlas_data is None
+            and self.atlas_view.slice_image_data is None
+            and self.image_view.current_img is None
+        ):
+            self.print_message("No project can be saved.", self.reminder_color)
+            return
+        file_name = QFileDialog.getSaveFileName(
+            self, "Save Project", self.save_path, "Pickle File (*.pkl)"
+        )
+        if file_name[0] != "":
+            if self.current_atlas == "slice":
                 atlas_ctrl_data = self.atlas_view.save_slice_data_and_info()
             else:
                 atlas_rotation = self.atlas_view.get_atlas_angles()
-                atlas_ctrl_data = {'atlas_display': self.atlas_display,
-                                   'coronal_index': self.atlas_view.current_coronal_index,
-                                   'sagittal_index': self.atlas_view.current_sagital_index,
-                                   'horizontal_index': self.atlas_view.current_horizontal_index,
-                                   'slice_rotation': atlas_rotation}
+                atlas_ctrl_data = {
+                    "atlas_display": self.atlas_display,
+                    "coronal_index": self.atlas_view.current_coronal_index,
+                    "sagittal_index": self.atlas_view.current_sagital_index,
+                    "horizontal_index": self.atlas_view.current_horizontal_index,
+                    "slice_rotation": atlas_rotation,
+                }
 
             if self.image_view.current_img is not None:
                 img_ctrl_data = self.image_view.get_img_ctrl_data()
             else:
                 img_ctrl_data = None
 
             setting_data = self.get_setting_data()
@@ -5520,158 +7155,172 @@
 
             if self.layer_ctrl.layer_link:
                 layer_data = self.layer_ctrl.get_layer_data()
                 all_2d_data = []
                 cells_symbol_atlas = None
                 cells_symbol_img = None
                 for single_layer_link in self.layer_ctrl.layer_link:
-                    if 'atlas' in single_layer_link:
-                        data_2d = self.get_atlas_single_layer_vis_data(single_layer_link)
-                        if 'cells' in single_layer_link:
-                            cells_symbol_atlas = data_2d['symbol']
+                    if "atlas" in single_layer_link:
+                        data_2d = self.get_atlas_single_layer_vis_data(
+                            single_layer_link
+                        )
+                        if "cells" in single_layer_link:
+                            cells_symbol_atlas = data_2d["symbol"]
                     else:
                         data_2d = self.get_hist_single_layer_vis_data(single_layer_link)
-                        if 'cells' in single_layer_link:
-                            cells_symbol_img = data_2d['symbol']
-                    all_2d_data.append(data_2d['data'])
-                layer_data['2d_data'] = all_2d_data
-                layer_data['cells_symbol_atlas'] = cells_symbol_atlas
-                layer_data['cells_symbol_img'] = cells_symbol_img
+                        if "cells" in single_layer_link:
+                            cells_symbol_img = data_2d["symbol"]
+                    all_2d_data.append(data_2d["data"])
+                layer_data["2d_data"] = all_2d_data
+                layer_data["cells_symbol_atlas"] = cells_symbol_atlas
+                layer_data["cells_symbol_img"] = cells_symbol_img
             else:
                 layer_data = None
 
             if self.object_ctrl.obj_name:
                 object_data = self.object_ctrl.get_obj_data()
-                object_data['object_3d_list'] = [[] for _ in range(len(self.object_3d_list))]
+                # object_data["object_3d_list"] = [
+                #     [] for _ in range(len(self.object_3d_list))
+                # ]
             else:
                 object_data = None
 
             # collect_probe_data
             probe_settings = self.probe_settings.get_settings()
 
-            project_data = {'atlas_path': self.current_atlas_path,
-                            'img_path': self.current_img_path,
-                            'current_atlas': self.current_atlas,
-                            'num_windows': self.num_windows,
-                            'probe_settings': probe_settings,
-                            'np_onside': self.np_onside,
-                            'processing_slice': self.atlas_view.processing_slice,
-                            'processing_img': self.image_view.processing_img,
-                            'overlay_img': self.overlay_img,
-                            'atlas_control': atlas_ctrl_data,
-                            'img_ctrl_data': img_ctrl_data,
-                            'setting_data': setting_data,
-                            'tool_data': tool_data,
-                            'layer_data': layer_data,
-                            'working_img_data': self.working_img_data,
-                            'working_atlas_data': self.working_atlas_data,
-                            'object_data': object_data}
+            project_data = {
+                "atlas_path": self.current_atlas_path,
+                "img_path": self.current_img_path,
+                "current_atlas": self.current_atlas,
+                "num_windows": self.num_windows,
+                "probe_settings": probe_settings,
+                "np_onside": self.np_onside,
+                "processing_slice": self.atlas_view.processing_slice,
+                "processing_img": self.image_view.processing_img,
+                "overlay_img": self.overlay_img,
+                "atlas_control": atlas_ctrl_data,
+                "img_ctrl_data": img_ctrl_data,
+                "setting_data": setting_data,
+                "tool_data": tool_data,
+                "layer_data": layer_data,
+                "working_img_data": self.working_img_data,
+                "working_atlas_data": self.working_atlas_data,
+                "object_data": object_data,
+            }
 
-            with open(file_name[0], 'wb') as handle:
+            with open(file_name[0], "wb") as handle:
                 pickle.dump(project_data, handle, protocol=pickle.HIGHEST_PROTOCOL)
-            self.print_message('Project saved successfully.', self.normal_color)
+            self.print_message("Project saved successfully.", self.normal_color)
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     # -------------------------------------------------------------
     #                    load project
     # -------------------------------------------------------------
     def load_project(self, p_dict):
-        self.current_atlas_path = p_dict['atlas_path']
-        self.current_img_path = p_dict['img_path']
-        self.current_atlas = p_dict['current_atlas']
-        self.num_windows = p_dict['num_windows']
-
-        self.np_onside = p_dict['np_onside']
-
-        self.atlas_view.processing_slice = p_dict['processing_slice']
-        self.image_view.processing_img = p_dict['processing_img']
-        self.overlay_img = p_dict['overlay_img']
-        self.working_atlas_data = p_dict['working_atlas_data']
-        self.working_img_data = p_dict['working_img_data']
+        self.current_atlas_path = p_dict["atlas_path"]
+        self.current_img_path = p_dict["img_path"]
+        self.current_atlas = p_dict["current_atlas"]
+        self.num_windows = p_dict["num_windows"]
+
+        self.np_onside = p_dict["np_onside"]
+
+        self.atlas_view.processing_slice = p_dict["processing_slice"]
+        self.image_view.processing_img = p_dict["processing_img"]
+        self.overlay_img = p_dict["overlay_img"]
+        self.working_atlas_data = p_dict["working_atlas_data"]
+        self.working_img_data = p_dict["working_img_data"]
 
         # load atlas data
         if self.current_atlas_path is not None:
-            atlas_ctrl_data = p_dict['atlas_control']
-            if self.current_atlas == 'volume':
+            atlas_ctrl_data = p_dict["atlas_control"]
+            if self.current_atlas == "volume":
                 if self.current_atlas_path is not None:
                     self.load_volume_atlas(self.current_atlas_path)
 
-                self.atlas_display = atlas_ctrl_data['atlas_display']
+                self.atlas_display = atlas_ctrl_data["atlas_display"]
 
-                if self.atlas_display == 'coronal':
+                if self.atlas_display == "coronal":
                     self.atlas_view.section_rabnt1.setChecked(True)
-                elif self.atlas_display == 'sagittal':
+                elif self.atlas_display == "sagittal":
                     self.atlas_view.section_rabnt2.setChecked(True)
                 else:
                     self.atlas_view.section_rabnt3.setChecked(True)
 
                 self.atlas_view.set_volume_atlas_ctrl_data(atlas_ctrl_data)
             else:
                 self.atlas_view.set_slice_data_and_info(atlas_ctrl_data)
                 if self.atlas_view.processing_slice is not None:
-                    self.atlas_view.slice_stack.set_data(self.atlas_view.processing_slice)
-                self.actionSwitch_Atlas.setText('Switch Atlas: Slice')
+                    self.atlas_view.slice_stack.set_data(
+                        self.atlas_view.processing_slice
+                    )
+                self.actionSwitch_Atlas.setText("Switch Atlas: Slice")
                 self.atlascontrolpanel.setEnabled(False)
                 self.treeviewpanel.setEnabled(False)
                 self.actionBregma_Picker.setEnabled(True)
                 self.actionCreate_Slice_Layer.setEnabled(True)
                 self.show_only_slice_window()
 
         # load image data
         if self.current_img_path is not None:
             if not os.path.exists(self.current_img_path):
-                msg = 'Can not find the image. Image file may be deleted or moved to another location'
+                msg = "Can not find the image. Image file may be deleted or moved to another location"
                 self.print_message(msg, self.error_message_color)
                 return
 
-            img_ctrl_data = p_dict['img_ctrl_data']
+            img_ctrl_data = p_dict["img_ctrl_data"]
 
             self.image_view.scale_slider.blockSignals(True)
-            self.image_view.scale_slider.setValue(img_ctrl_data['current_scale'])
-            self.image_view.scale_label.setText('{}%'.format(img_ctrl_data['current_scale']))
+            self.image_view.scale_slider.setValue(img_ctrl_data["current_scale"])
+            self.image_view.scale_label.setText(
+                "{}%".format(img_ctrl_data["current_scale"])
+            )
             self.image_view.scale_slider.blockSignals(False)
 
             filename, file_extension = os.path.splitext(self.current_img_path)
 
-            scene_index = img_ctrl_data['current_scene']
-            self.load_single_image_file(self.current_img_path, file_extension, scene_index)
+            scene_index = img_ctrl_data["current_scene"]
+            self.load_single_image_file(
+                self.current_img_path, file_extension, scene_index
+            )
             self.save_path = self.current_img_path
 
             self.image_view.load_img_ctrl_data(img_ctrl_data)
 
             if self.image_view.processing_img is not None:
                 self.image_view.set_data_and_size(self.image_view.processing_img)
-                self.image_view.img_stacks.set_lut(self.image_view.color_lut_list, self.image_view.image_file.level)
+                self.image_view.img_stacks.set_lut(
+                    self.image_view.color_lut_list, self.image_view.image_file.level
+                )
             else:
                 self.image_view.set_data_to_img_stacks()
             if self.current_atlas_path is not None:
-                if self.current_atlas == 'volume':
+                if self.current_atlas == "volume":
                     self.show_2_windows()
                 else:
                     self.show_slice_and_histology()
             else:
                 self.show_only_image_window()
 
         # tool
         self.tool_box.bound_pnts_num.setText(str(self.np_onside))
-        tool_settings = p_dict['tool_data']
+        tool_settings = p_dict["tool_data"]
         self.tool_box.set_tool_data(tool_settings)
 
         try:
-            self.probe_type = p_dict['probe_settings']['probe_type']
+            self.probe_type = p_dict["probe_settings"]["probe_type"]
         except KeyError:
-            self.probe_type = p_dict['probe_type']
+            self.probe_type = p_dict["probe_type"]
 
         self.tool_box.probe_type_combo.setCurrentIndex(self.probe_type)
         if self.probe_type == 2:
-            self.probe_settings.set_linear_silicon(p_dict['probe_settings'])
+            self.probe_settings.set_linear_silicon(p_dict["probe_settings"])
 
         # settings
-        setting_data = p_dict['setting_data']
+        setting_data = p_dict["setting_data"]
         self.set_setting_data(setting_data)
 
         if self.h2a_transferred:
             self.tool_box.toa_btn.setIcon(self.tool_box.toa_btn_on_icon)
             self.tool_box.toh_btn.setEnabled(False)
         else:
             self.tool_box.toa_btn.setIcon(self.tool_box.toa_btn_off_icon)
@@ -5681,135 +7330,176 @@
             self.tool_box.toh_btn.setIcon(self.tool_box.toh_btn_on_icon)
             self.tool_box.toa_btn.setEnabled(False)
         else:
             self.tool_box.toh_btn.setIcon(self.tool_box.toh_btn_off_icon)
             self.tool_box.toa_btn.setEnabled(True)
 
         # load layer data
-        layer_data = p_dict['layer_data']
+        layer_data = p_dict["layer_data"]
         if layer_data is not None:
             self.layer_ctrl.set_layer_data(layer_data)
         for i in range(len(self.layer_ctrl.layer_link)):
             da_link = self.layer_ctrl.layer_link[i]
 
-            if da_link == 'img-virus':
+            if da_link == "img-virus":
                 self.virus_lut[1] = self.layer_ctrl.layer_color[i]
-                self.image_view.img_stacks.image_dict[da_link].setLookupTable(self.virus_lut)
-            elif da_link == 'img-contour':
+                self.image_view.img_stacks.image_dict[da_link].setLookupTable(
+                    self.virus_lut
+                )
+            elif da_link == "img-contour":
                 self.contour_color = self.layer_ctrl.layer_color[i]
-                self.image_view.img_stacks.image_dict[da_link].setPen(self.contour_color)
-
-            if da_link == 'atlas-virus':
-                self.atlas_view.working_atlas.image_dict[da_link].setPen(color=(self.layer_ctrl.layer_color[i]))
-                self.atlas_view.working_atlas.image_dict[da_link].setBrush(color=(self.layer_ctrl.layer_color[i]))
-            elif da_link == 'atlas-contour':
-                self.atlas_view.working_atlas.image_dict[da_link].setPen(color=(self.layer_ctrl.layer_color[i]))
-
-            if 'img' in da_link:
-                if 'cells' in da_link:
-                    symbol = layer_data['cells_symbol_img']
+                self.image_view.img_stacks.image_dict[da_link].setPen(
+                    self.contour_color
+                )
+
+            if da_link == "atlas-virus":
+                self.atlas_view.working_atlas.image_dict[da_link].setPen(
+                    color=(self.layer_ctrl.layer_color[i])
+                )
+                self.atlas_view.working_atlas.image_dict[da_link].setBrush(
+                    color=(self.layer_ctrl.layer_color[i])
+                )
+            elif da_link == "atlas-contour":
+                self.atlas_view.working_atlas.image_dict[da_link].setPen(
+                    color=(self.layer_ctrl.layer_color[i])
+                )
+
+            if "img" in da_link:
+                if "cells" in da_link:
+                    symbol = layer_data["cells_symbol_img"]
                 else:
                     symbol = None
-                self.set_hist_layer_to_hist_view(da_link, layer_data['2d_data'][i], symbol)
+                self.set_hist_layer_to_hist_view(
+                    da_link, layer_data["2d_data"][i], symbol
+                )
             else:
-                if 'cells' in da_link:
-                    symbol = layer_data['cells_symbol_atlas']
+                if "cells" in da_link:
+                    symbol = layer_data["cells_symbol_atlas"]
                 else:
                     symbol = None
-                self.set_atlas_layer_to_atlas_view(da_link, layer_data['2d_data'][i], symbol)
+                self.set_atlas_layer_to_atlas_view(
+                    da_link, layer_data["2d_data"][i], symbol
+                )
 
         # load object related
-        object_data = p_dict['object_data']
+        object_data = p_dict["object_data"]
         if object_data is not None:
-            self.object_3d_list = object_data['object_3d_list']
+            # self.object_3d_list = object_data["object_3d_list"]
             self.object_ctrl.set_obj_data(object_data)
 
-        self.print_message('Project loaded successfully.', self.normal_color)
+        self.print_message("Project loaded successfully.", self.normal_color)
 
     def get_setting_data(self):
-        data = {'atlas_rect': self.atlas_rect,
-                'histo_rect': self.histo_rect,
-                'small_atlas_rect': self.small_atlas_rect,
-                'small_histo_rect': self.small_histo_rect,
-                'atlas_corner_points': self.atlas_corner_points,
-                'atlas_side_lines': self.atlas_side_lines,
-                'atlas_tri_data': self.atlas_tri_data,
-                'atlas_tri_inside_data': self.atlas_tri_inside_data,
-                'atlas_tri_onside_data': self.atlas_tri_onside_data,
-                'histo_corner_points': self.histo_corner_points,
-                'histo_side_lines': self.histo_side_lines,
-                'histo_tri_data': self.histo_tri_data,
-                'histo_tri_inside_data': self.histo_tri_inside_data,
-                'histo_tri_onside_data': self.histo_tri_onside_data,
-                'a2h_transferred': self.a2h_transferred,
-                'h2a_transferred': self.h2a_transferred,
-                'project_method': self.project_method,
-                'register_method': self.register_method}
+        data = {
+            "atlas_rect": self.atlas_rect,
+            "histo_rect": self.histo_rect,
+            "small_atlas_rect": self.small_atlas_rect,
+            "small_histo_rect": self.small_histo_rect,
+            "atlas_corner_points": self.atlas_corner_points,
+            "atlas_side_lines": self.atlas_side_lines,
+            "atlas_tri_data": self.atlas_tri_data,
+            "atlas_tri_inside_data": self.atlas_tri_inside_data,
+            "atlas_tri_onside_data": self.atlas_tri_onside_data,
+            "histo_corner_points": self.histo_corner_points,
+            "histo_side_lines": self.histo_side_lines,
+            "histo_tri_data": self.histo_tri_data,
+            "histo_tri_inside_data": self.histo_tri_inside_data,
+            "histo_tri_onside_data": self.histo_tri_onside_data,
+            "a2h_transferred": self.a2h_transferred,
+            "h2a_transferred": self.h2a_transferred,
+            "project_method": self.project_method,
+            "register_method": self.register_method,
+        }
         return data
 
     def set_setting_data(self, setting_data):
-        self.atlas_rect = setting_data['atlas_rect']
-        self.histo_rect = setting_data['histo_rect']
-        self.small_atlas_rect = setting_data['small_atlas_rect']
-        self.small_histo_rect = setting_data['small_histo_rect']
-        self.atlas_corner_points = setting_data['atlas_corner_points']
-        self.atlas_side_lines = setting_data['atlas_side_lines']
-        self.atlas_tri_data = setting_data['atlas_tri_data']
-        self.atlas_tri_inside_data = setting_data['atlas_tri_inside_data']
-        self.atlas_tri_onside_data = setting_data['atlas_tri_onside_data']
-        self.histo_corner_points = setting_data['histo_corner_points']
-        self.histo_side_lines = setting_data['histo_side_lines']
-        self.histo_tri_data = setting_data['histo_tri_data']
-        self.histo_tri_inside_data = setting_data['histo_tri_inside_data']
-        self.histo_tri_onside_data = setting_data['histo_tri_onside_data']
-        self.a2h_transferred = setting_data['a2h_transferred']
-        self.h2a_transferred = setting_data['h2a_transferred']
-        self.project_method = setting_data['project_method']
-        self.register_method = setting_data['register_method']
+        self.atlas_rect = setting_data["atlas_rect"]
+        self.histo_rect = setting_data["histo_rect"]
+        self.small_atlas_rect = setting_data["small_atlas_rect"]
+        self.small_histo_rect = setting_data["small_histo_rect"]
+        self.atlas_corner_points = setting_data["atlas_corner_points"]
+        self.atlas_side_lines = setting_data["atlas_side_lines"]
+        self.atlas_tri_data = setting_data["atlas_tri_data"]
+        self.atlas_tri_inside_data = setting_data["atlas_tri_inside_data"]
+        self.atlas_tri_onside_data = setting_data["atlas_tri_onside_data"]
+        self.histo_corner_points = setting_data["histo_corner_points"]
+        self.histo_side_lines = setting_data["histo_side_lines"]
+        self.histo_tri_data = setting_data["histo_tri_data"]
+        self.histo_tri_inside_data = setting_data["histo_tri_inside_data"]
+        self.histo_tri_onside_data = setting_data["histo_tri_onside_data"]
+        self.a2h_transferred = setting_data["a2h_transferred"]
+        self.h2a_transferred = setting_data["h2a_transferred"]
+        self.project_method = setting_data["project_method"]
+        self.register_method = setting_data["register_method"]
 
         if self.current_atlas_path is not None and self.atlas_tri_inside_data:
-            self.atlas_view.working_atlas.image_dict['tri_pnts'].setData(pos=np.asarray(self.atlas_tri_data))
+            self.atlas_view.working_atlas.image_dict["tri_pnts"].setData(
+                pos=np.asarray(self.atlas_tri_data)
+            )
             for i in range(len(self.atlas_tri_inside_data)):
                 self.working_atlas_text.append(pg.TextItem(str(i)))
                 self.working_atlas_text[-1].setColor(self.triangle_color)
-                self.working_atlas_text[-1].setPos(self.atlas_tri_inside_data[i][0], self.atlas_tri_inside_data[i][1])
+                self.working_atlas_text[-1].setPos(
+                    self.atlas_tri_inside_data[i][0], self.atlas_tri_inside_data[i][1]
+                )
                 self.atlas_view.working_atlas.vb.addItem(self.working_atlas_text[-1])
                 self.working_atlas_text[-1].setVisible(False)
 
         if self.image_view.current_img is not None and self.histo_tri_inside_data:
-            self.image_view.img_stacks.image_dict['tri_pnts'].setData(pos=np.asarray(self.histo_tri_data))
+            self.image_view.img_stacks.image_dict["tri_pnts"].setData(
+                pos=np.asarray(self.histo_tri_data)
+            )
             for i in range(len(self.histo_tri_inside_data)):
                 self.working_img_text.append(pg.TextItem(str(i)))
                 self.working_img_text[-1].setColor(self.triangle_color)
-                self.working_img_text[-1].setPos(self.histo_tri_inside_data[i][0], self.histo_tri_inside_data[i][1])
+                self.working_img_text[-1].setPos(
+                    self.histo_tri_inside_data[i][0], self.histo_tri_inside_data[i][1]
+                )
                 self.image_view.img_stacks.vb.addItem(self.working_img_text[-1])
                 self.working_img_text[-1].setVisible(False)
 
     def load_project_called(self):
-        if self.atlas_view.atlas_data is not None or self.atlas_view.slice_image_data is not None or self.image_view.image_file is not None:
-            reply = QMessageBox.question(self, 'Message',
-                                         "Saving current project?", QMessageBox.Yes, QMessageBox.No)
+        if (
+            self.atlas_view.atlas_data is not None
+            or self.atlas_view.slice_image_data is not None
+            or self.image_view.image_file is not None
+        ):
+            reply = QMessageBox.question(
+                self,
+                "Message",
+                "Saving current project?",
+                QMessageBox.Yes,
+                QMessageBox.No,
+            )
 
             if reply == QMessageBox.Yes:
                 self.save_project_called()
 
             self.object_ctrl.clear_all()
 
-        self.print_message('Loading project....', self.normal_color)
+        self.print_message("Loading project....", self.normal_color)
         file_options = QFileDialog.Options()
         file_options |= QFileDialog.DontUseNativeDialog
         dlg = QFileDialog()
         dlg.setFileMode(QFileDialog.ExistingFiles)
-        project_path = dlg.getOpenFileName(self, "Load Project", self.home_path, "Pickle File (*.pkl)",
-                                           options=file_options)
+        project_path = dlg.getOpenFileName(
+            self,
+            "Load Project",
+            self.home_path,
+            "Pickle File (*.pkl)",
+            options=file_options,
+        )
 
-        if project_path[0] != '':
+        if project_path[0] != "":
             p_dict, msg = check_loading_pickle_file(project_path[0])
             if msg is not None:
-                self.print_message('Loading project is failed. {}'.format(msg), self.error_message_color)
+                self.print_message(
+                    "Loading project is failed. {}".format(msg),
+                    self.error_message_color,
+                )
                 return
 
             if self.object_3d_list:
                 for _ in range(len(self.object_3d_list)):
                     if not isinstance(self.object_3d_list[-1], list):
                         self.view3d.removeItem(self.object_3d_list[-1])
                         self.object_3d_list[-1].deleteLater()
@@ -5821,79 +7511,94 @@
             # if self.image_view.image_file is not None:
             #     self.delete_all
             self.layer_ctrl.clear_all()
 
             self.load_project(p_dict)
 
         else:
-            self.print_message('', self.normal_color)
+            self.print_message("", self.normal_color)
 
     # ------------------- file menu related ----------------
     def load_external_cells_called(self):
         if self.volume_atlas_path is None:
             return
-        file_path = os.path.join(self.volume_atlas_path, 'atlas_axis_info.pkl')
+        file_path = os.path.join(self.volume_atlas_path, "atlas_axis_info.pkl")
         if not os.path.exists(file_path):
-            msg = 'No atlas rotation information saved. Please contact maintainers.'
+            msg = "No atlas rotation information saved. Please contact maintainers."
             self.print_message(msg, self.error_message_color)
             return
 
         try:
-            with open(file_path, 'rb') as f:
+            with open(file_path, "rb") as f:
                 axis_info = pickle.load(f)
-            transpose_order = axis_info['to_HERBS']
-            atlas_size = axis_info['size']
-            direction_change = axis_info['direction_change']
+            transpose_order = axis_info["to_HERBS"]
+            atlas_size = axis_info["size"]
+            direction_change = axis_info["direction_change"]
             print(axis_info)
-        except (IOError, OSError, ValueError, KeyError, IndexError, pickle.PickleError, pickle.UnpicklingError):
-            msg = 'Can not open atlas axis information file, please check the Tutorial on GitHub.'
+        except (
+            IOError,
+            OSError,
+            ValueError,
+            KeyError,
+            IndexError,
+            pickle.PickleError,
+            pickle.UnpicklingError,
+        ):
+            msg = "Can not open atlas axis information file, please check the Tutorial on GitHub."
             self.print_message(msg, self.error_message_color)
             return
 
         file_options = QFileDialog.Options()
         file_options |= QFileDialog.DontUseNativeDialog
         dlg = QFileDialog()
         dlg.setFileMode(QFileDialog.ExistingFiles)
-        data_file_path = dlg.getOpenFileName(self, "Load Point Data", self.home_path,
-                                             "Numpy File (*.npy);;Pickle File (*.pkl)", options=file_options)
+        data_file_path = dlg.getOpenFileName(
+            self,
+            "Load Point Data",
+            self.home_path,
+            "Numpy File (*.npy);;Pickle File (*.pkl)",
+            options=file_options,
+        )
 
-        if data_file_path[0] != '':
+        if data_file_path[0] != "":
             data, msg = load_point_data(data_file_path[0])
             if msg is not None:
                 self.print_message(msg, self.error_message_color)
                 return
             if isinstance(data[0, 1], float):
                 extra_vox = 0
             elif isinstance(data[0, 1], int):
                 extra_vox = 1
             else:
-                msg = 'Data is in wrong type, please check the Tutorial on GitHub.'
+                msg = "Data is in wrong type, please check the Tutorial on GitHub."
                 self.print_message(msg, self.error_message_color)
                 return
 
             data_temp = data.copy()
             for i in range(data.shape[1]):
                 if direction_change[i]:
                     data_temp[:, i] = atlas_size[i] - extra_vox - data_temp[:, i]
             if transpose_order != (0, 1, 2):
                 pnt_vox = data_temp[:, transpose_order]
             else:
                 pnt_vox = data_temp.copy()
 
             pnt_vis = pnt_vox - self.atlas_view.origin_3d
 
-            self.object_ctrl.add_object(object_name='loaded point data',
-                                        object_type='cells piece',
-                                        object_data=pnt_vis,
-                                        object_mode=self.obj_display_mode)
+            self.object_ctrl.add_object(
+                object_name="loaded point data",
+                object_type="cells piece",
+                object_data=pnt_vis,
+                object_mode=self.obj_display_mode,
+            )
 
     # status
     def print_message(self, msg, col):
         self.statusbar.setStyleSheet(get_statusbar_style(col))
-        self.statusbar.showMessage('  ' + msg)
+        self.statusbar.showMessage("  " + msg)
 
     # about herbs
     def about_herbs_info(self):
         dlg = AboutHERBSWindow()
         dlg.exec()
 
 
@@ -5905,15 +7610,7 @@
     # print(sys.flags.interactive)  # 0
     # print(hasattr(QtCore, 'PYQT_VERSION')) # true
     # if (sys.flags.interactive != 1) or not hasattr(QtCore, 'PYQT_VERSION'):
     #     app.instance().exec_()
     window = HERBS()
     window.show()
     exit(app.exec_())
-
-
-
-
-
-
-
-
```

### Comparing `herbs-0.2.2/herbs/icons/backward.svg` & `herbs-0.2.3/herbs/icons/backward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/dot.svg` & `herbs-0.2.3/herbs/icons/dot.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/down-arrow.svg` & `herbs-0.2.3/herbs/icons/down-arrow.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/fast_backward.svg` & `herbs-0.2.3/herbs/icons/fast_backward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/fast_forward.svg` & `herbs-0.2.3/herbs/icons/fast_forward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/forward.svg` & `herbs-0.2.3/herbs/icons/forward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/layers/add.png` & `herbs-0.2.3/herbs/icons/layers/add.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/layers/ai.png` & `herbs-0.2.3/herbs/icons/layers/ai.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/layers/eye_off.png` & `herbs-0.2.3/herbs/icons/layers/eye_off.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/layers/eye_on.png` & `herbs-0.2.3/herbs/icons/layers/eye_on.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/layers/eye_white.png` & `herbs-0.2.3/herbs/icons/layers/eye_white.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/layers/hi.png` & `herbs-0.2.3/herbs/icons/layers/hi.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/layers/trash.png` & `herbs-0.2.3/herbs/icons/layers/trash.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/object.svg` & `herbs-0.2.3/herbs/icons/object.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/add.png` & `herbs-0.2.3/herbs/icons/sidebar/add.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/atlascontrol.png` & `herbs-0.2.3/herbs/icons/sidebar/atlascontrol.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/atlascontrol.svg` & `herbs-0.2.3/herbs/icons/sidebar/atlascontrol.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/bnd.svg` & `herbs-0.2.3/herbs/icons/sidebar/bnd.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/c_section.png` & `herbs-0.2.3/herbs/icons/sidebar/c_section.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/c_section2.png` & `herbs-0.2.3/herbs/icons/sidebar/c_section2.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/cell.svg` & `herbs-0.2.3/herbs/icons/sidebar/cell.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/check.svg` & `herbs-0.2.3/herbs/icons/sidebar/check.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/compare.svg` & `herbs-0.2.3/herbs/icons/sidebar/compare.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/contour.svg` & `herbs-0.2.3/herbs/icons/sidebar/contour.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/h_section.png` & `herbs-0.2.3/herbs/icons/sidebar/h_section.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/info.svg` & `herbs-0.2.3/herbs/icons/sidebar/info.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/layers.png` & `herbs-0.2.3/herbs/icons/sidebar/layers.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/layers.svg` & `herbs-0.2.3/herbs/icons/sidebar/layers.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/line.svg` & `herbs-0.2.3/herbs/icons/sidebar/line.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/link.svg` & `herbs-0.2.3/herbs/icons/sidebar/link.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/link_off.svg` & `herbs-0.2.3/herbs/icons/sidebar/link_off.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/merge.svg` & `herbs-0.2.3/herbs/icons/sidebar/merge.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/object.svg` & `herbs-0.2.3/herbs/icons/sidebar/object.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/probe.png` & `herbs-0.2.3/herbs/icons/sidebar/probe.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/probe.svg` & `herbs-0.2.3/herbs/icons/sidebar/probe.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/rotation_horizontal.svg` & `herbs-0.2.3/herbs/icons/sidebar/rotation_horizontal.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/rotation_vertical.svg` & `herbs-0.2.3/herbs/icons/sidebar/rotation_vertical.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/s_section.png` & `herbs-0.2.3/herbs/icons/sidebar/s_section.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/tool.png` & `herbs-0.2.3/herbs/icons/sidebar/tool.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/tool.svg` & `herbs-0.2.3/herbs/icons/sidebar/tool.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/trash.png` & `herbs-0.2.3/herbs/icons/sidebar/trash.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/tree_checked.svg` & `herbs-0.2.3/herbs/icons/sidebar/tree_checked.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/treeview.png` & `herbs-0.2.3/herbs/icons/sidebar/treeview.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/treeview.svg` & `herbs-0.2.3/herbs/icons/sidebar/treeview.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/treeview2.png` & `herbs-0.2.3/herbs/icons/sidebar/treeview2.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/sidebar/virus.svg` & `herbs-0.2.3/herbs/icons/sidebar/virus.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/tdown.svg` & `herbs-0.2.3/herbs/icons/tdown.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/accept.svg` & `herbs-0.2.3/herbs/icons/toolbar/accept.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/accept2.svg` & `herbs-0.2.3/herbs/icons/toolbar/accept2.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/aim.svg` & `herbs-0.2.3/herbs/icons/toolbar/aim.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/aim_not.svg` & `herbs-0.2.3/herbs/icons/toolbar/aim_not.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/anchor.svg` & `herbs-0.2.3/herbs/icons/toolbar/anchor.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/anticlockwise_rotation.svg` & `herbs-0.2.3/herbs/icons/toolbar/anticlockwise_rotation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/atlas_icon.png` & `herbs-0.2.3/herbs/icons/toolbar/atlas_icon.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/boundary_register.svg` & `herbs-0.2.3/herbs/icons/toolbar/boundary_register.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/cancel.svg` & `herbs-0.2.3/herbs/icons/toolbar/cancel.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/cell_select.svg` & `herbs-0.2.3/herbs/icons/toolbar/cell_select.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/cell_select_not.svg` & `herbs-0.2.3/herbs/icons/toolbar/cell_select_not.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/check.svg` & `herbs-0.2.3/herbs/icons/toolbar/check.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/clockwise_rotation.svg` & `herbs-0.2.3/herbs/icons/toolbar/clockwise_rotation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/closed_path.svg` & `herbs-0.2.3/herbs/icons/toolbar/closed_path.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/closed_path2 copy.svg` & `herbs-0.2.3/herbs/icons/toolbar/closed_path2 copy.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/closed_path2.svg` & `herbs-0.2.3/herbs/icons/toolbar/closed_path2.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/eraser.png` & `herbs-0.2.3/herbs/icons/toolbar/eraser.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/eraser.svg` & `herbs-0.2.3/herbs/icons/toolbar/eraser.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/eye.svg` & `herbs-0.2.3/herbs/icons/toolbar/eye.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/eye_closed.svg` & `herbs-0.2.3/herbs/icons/toolbar/eye_closed.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/fill.svg` & `herbs-0.2.3/herbs/icons/toolbar/fill.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/gps.svg` & `herbs-0.2.3/herbs/icons/toolbar/gps.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/h_flip.png` & `herbs-0.2.3/herbs/icons/toolbar/h_flip.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/handle.png` & `herbs-0.2.3/herbs/icons/toolbar/handle.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/image_icon.png` & `herbs-0.2.3/herbs/icons/toolbar/image_icon.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/image_icon.svg` & `herbs-0.2.3/herbs/icons/toolbar/image_icon.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/info.svg` & `herbs-0.2.3/herbs/icons/toolbar/info.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/inpart.png` & `herbs-0.2.3/herbs/icons/toolbar/inpart.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/inpart.svg` & `herbs-0.2.3/herbs/icons/toolbar/inpart.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/lasso.png` & `herbs-0.2.3/herbs/icons/toolbar/lasso.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/lasso.svg` & `herbs-0.2.3/herbs/icons/toolbar/lasso.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/left90.png` & `herbs-0.2.3/herbs/icons/toolbar/left90.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/line.svg` & `herbs-0.2.3/herbs/icons/toolbar/line.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/line_sites.svg` & `herbs-0.2.3/herbs/icons/toolbar/line_sites.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/linear_silicon.png` & `herbs-0.2.3/herbs/icons/toolbar/linear_silicon.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/linear_silicon.svg` & `herbs-0.2.3/herbs/icons/toolbar/linear_silicon.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/list.svg` & `herbs-0.2.3/herbs/icons/toolbar/list.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/location.svg` & `herbs-0.2.3/herbs/icons/toolbar/location.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/magic-wand.svg` & `herbs-0.2.3/herbs/icons/toolbar/magic-wand.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/magic_white.png` & `herbs-0.2.3/herbs/icons/toolbar/magic_white.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/mask.svg` & `herbs-0.2.3/herbs/icons/toolbar/mask.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/match.svg` & `herbs-0.2.3/herbs/icons/toolbar/match.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/matchbnd.svg` & `herbs-0.2.3/herbs/icons/toolbar/matchbnd.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/matching.svg` & `herbs-0.2.3/herbs/icons/toolbar/matching.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/merge.svg` & `herbs-0.2.3/herbs/icons/toolbar/merge.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/move_down.png` & `herbs-0.2.3/herbs/icons/toolbar/move_down.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/move_left.png` & `herbs-0.2.3/herbs/icons/toolbar/move_left.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/move_right.png` & `herbs-0.2.3/herbs/icons/toolbar/move_right.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/move_up.png` & `herbs-0.2.3/herbs/icons/toolbar/move_up.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/moving.png` & `herbs-0.2.3/herbs/icons/toolbar/moving.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/multi-probe.svg` & `herbs-0.2.3/herbs/icons/toolbar/multi-probe.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/multi_pencil.svg` & `herbs-0.2.3/herbs/icons/toolbar/multi_pencil.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/multi_probe.png` & `herbs-0.2.3/herbs/icons/toolbar/multi_probe.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/object.svg` & `herbs-0.2.3/herbs/icons/toolbar/object.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/open_path.svg` & `herbs-0.2.3/herbs/icons/toolbar/open_path.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/outpart.png` & `herbs-0.2.3/herbs/icons/toolbar/outpart.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/outpart.svg` & `herbs-0.2.3/herbs/icons/toolbar/outpart.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/pencil.png` & `herbs-0.2.3/herbs/icons/toolbar/pencil.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/pencil.svg` & `herbs-0.2.3/herbs/icons/toolbar/pencil.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/plasso.png` & `herbs-0.2.3/herbs/icons/toolbar/plasso.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/probe.svg` & `herbs-0.2.3/herbs/icons/toolbar/probe.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/radar.svg` & `herbs-0.2.3/herbs/icons/toolbar/radar.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/rotation.svg` & `herbs-0.2.3/herbs/icons/toolbar/rotation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/rotation_clockwise.svg` & `herbs-0.2.3/herbs/icons/toolbar/rotation_clockwise.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/rotation_counter_clockwise.svg` & `herbs-0.2.3/herbs/icons/toolbar/rotation_counter_clockwise.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/ruler.svg` & `herbs-0.2.3/herbs/icons/toolbar/ruler.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/separate_sites.svg` & `herbs-0.2.3/herbs/icons/toolbar/separate_sites.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/single_pencil.svg` & `herbs-0.2.3/herbs/icons/toolbar/single_pencil.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/toa.svg` & `herbs-0.2.3/herbs/icons/toolbar/toa.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/toa_delete.svg` & `herbs-0.2.3/herbs/icons/toolbar/toa_delete.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/toaa.svg` & `herbs-0.2.3/herbs/icons/toolbar/toaa.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/toh.svg` & `herbs-0.2.3/herbs/icons/toolbar/toh.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/toh_delete.svg` & `herbs-0.2.3/herbs/icons/toolbar/toh_delete.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/tohh.svg` & `herbs-0.2.3/herbs/icons/toolbar/tohh.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/trans.png` & `herbs-0.2.3/herbs/icons/toolbar/trans.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/trans.svg` & `herbs-0.2.3/herbs/icons/toolbar/trans.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/triangulation.svg` & `herbs-0.2.3/herbs/icons/toolbar/triangulation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/two_window.png` & `herbs-0.2.3/herbs/icons/toolbar/two_window.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/unmerge.svg` & `herbs-0.2.3/herbs/icons/toolbar/unmerge.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/v_flip.png` & `herbs-0.2.3/herbs/icons/toolbar/v_flip.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/virus.svg` & `herbs-0.2.3/herbs/icons/toolbar/virus.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/virus_register.svg` & `herbs-0.2.3/herbs/icons/toolbar/virus_register.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/vis2d.svg` & `herbs-0.2.3/herbs/icons/toolbar/vis2d.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/window2.png` & `herbs-0.2.3/herbs/icons/toolbar/window2.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/window3.png` & `herbs-0.2.3/herbs/icons/toolbar/window3.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/toolbar/window4.png` & `herbs-0.2.3/herbs/icons/toolbar/window4.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/tree_close.svg` & `herbs-0.2.3/herbs/icons/tree_close.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/tree_open.svg` & `herbs-0.2.3/herbs/icons/tree_open.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/icons/up-arrow.svg` & `herbs-0.2.3/herbs/icons/up-arrow.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/image_curves.py` & `herbs-0.2.3/herbs/image_curves.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/image_reader.py` & `herbs-0.2.3/herbs/image_reader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/image_stacks.py` & `herbs-0.2.3/herbs/image_stacks.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/image_view.py` & `herbs-0.2.3/herbs/image_view.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/label_tree.py` & `herbs-0.2.3/herbs/label_tree.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/layers_control.py` & `herbs-0.2.3/herbs/layers_control.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/main_window.ui` & `herbs-0.2.3/herbs/main_window.ui`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/movable_points.py` & `herbs-0.2.3/herbs/movable_points.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/obj_items.py` & `herbs-0.2.3/herbs/obj_items.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/object_control.py` & `herbs-0.2.3/herbs/object_control.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,116 +6,123 @@
 from PyQt5.QtWidgets import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 from .wtiles import QDoubleButton
 from .uuuuuu import read_qss_file
 
 
-eye_button_style = '''
+eye_button_style = """
     border-left: None;
     border-right: 1px solid gray;
     border-top: None;
     border-bottom: None;
     border-radius: 0px;
     background: transparent;
-'''
+"""
 
 
-line_edit_style = '''
+line_edit_style = """
 QLineEdit {
     background: transparent;
     border: 1px solid green;
     border-radius:0px;
     text-align:left; 
     color: white; 
     padding-left: 5px;    
     margin: 0px;
     height: 40px;
     width: 220px; 
 }
-'''
+"""
 
 
 class ObjectTextButton(QPushButton):
     def __init__(self):
         QPushButton.__init__(self)
-        btn_style = read_qss_file('qss/object_text_button.qss')
+        btn_style = read_qss_file("qss/object_text_button.qss")
         self.setStyleSheet(btn_style)
         self.setFixedSize(QSize(150, 40))
 
 
 class CompareWindow(QDialog):
     def __init__(self, obj_names, obj_data):
         super().__init__()
 
         self.setWindowTitle("Compare Information Window")
 
         n_object = len(obj_names)
-        print(n_object)
-        print(obj_data)
+        # print(n_object)
+        # print(obj_data)
         all_label_names = []
         all_label_acronym = []
         all_label_color = []
         all_label_channels = []
         for i in range(n_object):
-            all_label_names.append(obj_data[i]['label_name'])
-            all_label_acronym.append(obj_data[i]['label_acronym'])
-            all_label_color.append(obj_data[i]['label_color'])
-            all_label_channels.append(obj_data[i]['region_sites'])
+            all_label_names.append(obj_data[i]["label_name"])
+            all_label_acronym.append(obj_data[i]["label_acronym"])
+            all_label_color.append(obj_data[i]["label_color"])
+            all_label_channels.append(obj_data[i]["region_sites"])
         all_label_names = np.concatenate(all_label_names)
         all_label_acronym = np.concatenate(all_label_acronym)
         all_label_color = np.concatenate(all_label_color)
         all_label_channels = np.concatenate(all_label_channels)
 
-        print(all_label_names)
-        print(all_label_acronym )
-        print(all_label_color)
-        print(all_label_channels)
+        # print(all_label_names)
+        # print(all_label_acronym)
+        # print(all_label_color)
+        # print(all_label_channels)
 
         unique_label_names = np.unique(all_label_names)
         unique_label_acronym = []
         unique_label_color = []
         unique_label_channels = []
         for i in range(len(unique_label_names)):
             c_ind = np.where(all_label_names == unique_label_names[i])[0]
             unique_label_acronym.append(all_label_acronym[c_ind[0]])
             unique_label_color.append(all_label_color[c_ind[0]])
             unique_label_channels.append(np.sum(all_label_channels[c_ind]))
 
         layout = QVBoxLayout()
         full_name = obj_names[0]
         for i in range(1, n_object):
-            full_name = full_name + ', '
+            full_name = full_name + ", "
             full_name = full_name + obj_names[i]
 
-        self.label = QLabel('Compare {}'.format(full_name))
+        self.label = QLabel("Compare {}".format(full_name))
         color = QColor(128, 128, 128, 128)
-        label_style = 'QLabel {background-color: ' + color.name() + '; font-size: 20px}'
+        label_style = "QLabel {background-color: " + color.name() + "; font-size: 20px}"
         self.label.setStyleSheet(label_style)
 
         sec_group = QGroupBox()
         slayout = QGridLayout(sec_group)
-        lb1 = QLabel('Brain Region')
-        lb2 = QLabel('Acronym')
-        lb3 = QLabel('Channels')
-        lb4 = QLabel('Color')
+        lb1 = QLabel("Brain Region")
+        lb2 = QLabel("Acronym")
+        lb3 = QLabel("Channels")
+        lb4 = QLabel("Color")
         slayout.addWidget(lb1, 0, 0, 1, 1)
         slayout.addWidget(lb2, 0, 1, 1, 1)
         slayout.addWidget(lb3, 0, 2, 1, 1)
         slayout.addWidget(lb4, 0, 3, 1, 1)
 
         channels = np.ravel(unique_label_channels).astype(int)
 
         for i in range(len(unique_label_names)):
             slayout.addWidget(QLabel(unique_label_names[i]), i + 1, 0, 1, 1)
             slayout.addWidget(QLabel(unique_label_acronym[i]), i + 1, 1, 1, 1)
             slayout.addWidget(QLabel(str(channels[i])), i + 1, 2, 1, 1)
             clb = QLabel()
-            da_color = QColor(unique_label_color[i][0], unique_label_color[i][1], unique_label_color[i][2], 255).name()
-            clb.setStyleSheet('QLabel {background-color: ' + da_color + '; width: 20px; height: 20px}')
+            da_color = QColor(
+                unique_label_color[i][0],
+                unique_label_color[i][1],
+                unique_label_color[i][2],
+                255,
+            ).name()
+            clb.setStyleSheet(
+                "QLabel {background-color: " + da_color + "; width: 20px; height: 20px}"
+            )
             slayout.addWidget(clb, i + 1, 3, 1, 1)
 
         # make plot data
         plot_frame = QFrame()
         plot_frame.setMaximumWidth(300)
         plot_frame.setMinimumWidth(300)
         view_layout = QHBoxLayout(plot_frame)
@@ -125,55 +132,74 @@
         w = pg.GraphicsLayoutWidget()
         view = w.addViewBox()
         view.setAspectLocked()
 
         view_layout.addWidget(w)
 
         for k in range(n_object):
-            vis_data = obj_data[k]['vis_data']
+            vis_data = obj_data[k]["vis_data"]
             n_column = len(vis_data)
 
             plot_center_x_val = k * 10 + 0.5 * n_column
 
-            probe_type_name = obj_data[k]['probe_type_name']
+            probe_type_name = obj_data[k]["probe_type_name"]
             # draw tips
-            if probe_type_name != 'Tetrode':
-                da_tip_loc = np.array([[0, 0], [0.5 * n_column, - 2 * n_column], [n_column, 0]])
+            if probe_type_name != "Tetrode":
+                da_tip_loc = np.array(
+                    [[0, 0], [0.5 * n_column, -2 * n_column], [n_column, 0]]
+                )
                 da_tip_loc = da_tip_loc + np.array([plot_center_x_val, 0])
-                tips = pg.PlotDataItem(da_tip_loc, connect='all', fillLevel=0,
-                                       fillBrush=pg.mkBrush(color=(128, 128, 128)))
+                tips = pg.PlotDataItem(
+                    da_tip_loc,
+                    connect="all",
+                    fillLevel=0,
+                    fillBrush=pg.mkBrush(color=(128, 128, 128)),
+                )
                 view.addItem(tips)
 
             # draw area
-            region_label = obj_data[k]['region_label']
+            region_label = obj_data[k]["region_label"]
 
-            group_color = obj_data[k]['label_color']
-            sites_label = obj_data[k]['sites_label']
+            group_color = obj_data[k]["label_color"]
+            sites_label = obj_data[k]["sites_label"]
             for i in range(n_column):
-                group_id = vis_data[i]['group_id'].astype(int)
-                start_loc = vis_data[i]['start_loc']
-                end_loc = vis_data[i]['end_loc']
-                sites_loc_column = vis_data[i]['sites']
+                group_id = vis_data[i]["group_id"].astype(int)
+                start_loc = vis_data[i]["start_loc"]
+                end_loc = vis_data[i]["end_loc"]
+                sites_loc_column = vis_data[i]["sites"]
 
                 for j in range(len(group_id)):
                     area_data = np.array([[i, end_loc[j]], [i + 1, end_loc[j]]])
                     area_data = area_data + np.array([plot_center_x_val, 0])
-                    da_item = pg.PlotDataItem(area_data, fillLevel=start_loc[j],
-                                              fillBrush=group_color[group_id[j]], pen=None)
+                    da_item = pg.PlotDataItem(
+                        area_data,
+                        fillLevel=start_loc[j],
+                        fillBrush=group_color[group_id[j]],
+                        pen=None,
+                    )
                     view.addItem(da_item)
 
                 sites_color = []
                 for j in range(len(sites_label[i])):
                     color_ind = np.where(region_label == sites_label[i][j])[0][0]
                     sites_color.append(group_color[color_ind])
 
-                pnt_data = np.stack([np.repeat(i + 0.5, len(sites_loc_column)), sites_loc_column], axis=1)
+                pnt_data = np.stack(
+                    [np.repeat(i + 0.5, len(sites_loc_column)), sites_loc_column],
+                    axis=1,
+                )
                 pnt_data = pnt_data + np.array([plot_center_x_val, 0])
-                da_item = pg.ScatterPlotItem(pos=pnt_data, pen=(128, 128, 128, 128), brush=sites_color,
-                                             symbol='s', size=3, hoverSize=8)
+                da_item = pg.ScatterPlotItem(
+                    pos=pnt_data,
+                    pen=(128, 128, 128, 128),
+                    brush=sites_color,
+                    symbol="s",
+                    size=3,
+                    hoverSize=8,
+                )
                 view.addItem(da_item)
 
         channel_info_frame = QFrame()
         channel_info_layout = QHBoxLayout(channel_info_frame)
         channel_info_layout.setContentsMargins(0, 0, 0, 0)
         channel_info_layout.setSpacing(10)
         channel_info_layout.addWidget(plot_frame)
@@ -197,42 +223,53 @@
     def __init__(self, name, data):
         super().__init__()
 
         self.setWindowTitle("Cell Information Window")
 
         layout = QVBoxLayout()
         self.label = QLabel(name)
-        color = QColor(data['vis_color'][0], data['vis_color'][1], data['vis_color'][2], data['vis_color'][3])
-        label_style = 'QLabel {background-color: ' + color.name() + '; font-size: 20px}'
+        color = QColor(
+            data["vis_color"][0],
+            data["vis_color"][1],
+            data["vis_color"][2],
+            data["vis_color"][3],
+        )
+        label_style = "QLabel {background-color: " + color.name() + "; font-size: 20px}"
         self.label.setStyleSheet(label_style)
 
-        data_mat = data['data'][0]
-        for i in range(1, len(data['data'])):
-            data_mat = np.vstack([data_mat, data['data'][i]])
+        data_mat = data["data"][0]
+        for i in range(1, len(data["data"])):
+            data_mat = np.vstack([data_mat, data["data"][i]])
 
-        sec_group = QGroupBox('Total Count: {}'.format(len(data_mat)))
+        sec_group = QGroupBox("Total Count: {}".format(len(data_mat)))
         slayout = QGridLayout(sec_group)
-        lb1 = QLabel('Brain Region')
-        lb2 = QLabel('Acronym')
-        lb3 = QLabel('Color')
-        lb4 = QLabel('Count')
+        lb1 = QLabel("Brain Region")
+        lb2 = QLabel("Acronym")
+        lb3 = QLabel("Color")
+        lb4 = QLabel("Count")
         slayout.addWidget(lb1, 0, 0, 1, 1)
         slayout.addWidget(lb2, 0, 1, 1, 1)
         slayout.addWidget(lb3, 0, 2, 1, 1)
         slayout.addWidget(lb4, 0, 3, 1, 1)
 
-        for i in range(len(data['label_name'])):
-            slayout.addWidget(QLabel(data['label_name'][i]), i + 1, 0, 1, 1)
-            slayout.addWidget(QLabel(data['label_acronym'][i]), i + 1, 1, 1, 1)
+        for i in range(len(data["label_name"])):
+            slayout.addWidget(QLabel(data["label_name"][i]), i + 1, 0, 1, 1)
+            slayout.addWidget(QLabel(data["label_acronym"][i]), i + 1, 1, 1, 1)
             clb = QLabel()
-            da_color = QColor(data['label_color'][i][0], data['label_color'][i][1], data['label_color'][i][2],
-                              255).name()
-            clb.setStyleSheet('QLabel {background-color: ' + da_color + '; width: 20px; height: 20px}')
+            da_color = QColor(
+                data["label_color"][i][0],
+                data["label_color"][i][1],
+                data["label_color"][i][2],
+                255,
+            ).name()
+            clb.setStyleSheet(
+                "QLabel {background-color: " + da_color + "; width: 20px; height: 20px}"
+            )
             slayout.addWidget(clb, i + 1, 2, 1, 1)
-            slayout.addWidget(QLabel(str(data['region_count'][i])), i + 1, 3, 1, 1)
+            slayout.addWidget(QLabel(str(data["region_count"][i])), i + 1, 3, 1, 1)
 
         # ok button, used to close window
         ok_btn = QDialogButtonBox(QDialogButtonBox.Ok)
         ok_btn.accepted.connect(self.accept)
 
         # add widget to layout
         layout.addWidget(self.label)
@@ -240,51 +277,72 @@
         layout.addWidget(ok_btn)
         self.setLayout(layout)
 
     def accept(self) -> None:
         self.close()
 
     def set_probe_color(self, color):
-        self.label.setStyleSheet('QLabel {background-color: ' + color + ';}')
+        self.label.setStyleSheet("QLabel {background-color: " + color + ";}")
 
 
 class VirusInfoWindow(QDialog):
     def __init__(self, name, data):
         super().__init__()
 
         self.setWindowTitle("Virus Information Window")
 
         layout = QVBoxLayout()
         self.label = QLabel(name)
-        color = QColor(data['vis_color'][0], data['vis_color'][1], data['vis_color'][2], data['vis_color'][3])
-        label_style = 'QLabel {background-color: ' + color.name() + '; font-size: 20px}'
+        color = QColor(
+            data["vis_color"][0],
+            data["vis_color"][1],
+            data["vis_color"][2],
+            data["vis_color"][3],
+        )
+        label_style = "QLabel {background-color: " + color.name() + "; font-size: 20px}"
         self.label.setStyleSheet(label_style)
 
-        region_label = data['label_id']
-        region_name = data['label_name']
-        region_acronym = data['label_acronym']
-        virus_volume = data['virus_volume']
-        region_volume = data['region_volume']
-        region_color = data['label_color']
+        region_label = data["label_id"]
+        region_name = data["label_name"]
+        region_acronym = data["label_acronym"]
+        virus_volume = data["virus_volume"]
+        region_volume = data["region_volume"]
+        region_color = data["label_color"]
         proportion = np.round(np.ravel(virus_volume) / np.ravel(region_volume) * 100, 2)
 
         sec_group = QGroupBox()
         sec_layout = QGridLayout(sec_group)
-        column_names = [QLabel('ID'), QLabel('Brain Region'), QLabel('Acronym'),
-                        QLabel('Volume (stk voxel)'), QLabel('Proportion (%)'), QLabel('Color')]
+        column_names = [
+            QLabel("ID"),
+            QLabel("Brain Region"),
+            QLabel("Acronym"),
+            QLabel("Volume (stk voxel)"),
+            QLabel("Proportion (%)"),
+            QLabel("Color"),
+        ]
         for i in range(len(column_names)):
             sec_layout.addWidget(column_names[i], 0, i, 1, 1)
 
         for i in range(len(region_label)):
             clb = QLabel()
-            da_color = QColor(region_color[i][0], region_color[i][1], region_color[i][2], 255).name()
-            clb.setStyleSheet('QLabel {background-color: ' + da_color + '; width: 20px; height: 20px}')
-
-            row_val = [QLabel(str(region_label[i])), QLabel(region_name[i]), QLabel(region_acronym[i]),
-                       QLabel(str(virus_volume[i])), QLabel(str(proportion[i])), clb]
+            da_color = QColor(
+                region_color[i][0], region_color[i][1], region_color[i][2], 255
+            ).name()
+            clb.setStyleSheet(
+                "QLabel {background-color: " + da_color + "; width: 20px; height: 20px}"
+            )
+
+            row_val = [
+                QLabel(str(region_label[i])),
+                QLabel(region_name[i]),
+                QLabel(region_acronym[i]),
+                QLabel(str(virus_volume[i])),
+                QLabel(str(proportion[i])),
+                clb,
+            ]
 
             for j in range(len(row_val)):
                 sec_layout.addWidget(row_val[j], i + 1, j, 1, 1)
 
         # ok button, used to close window
         ok_btn = QDialogButtonBox(QDialogButtonBox.Ok)
         ok_btn.accepted.connect(self.accept)
@@ -295,60 +353,69 @@
         layout.addWidget(ok_btn)
         self.setLayout(layout)
 
     def accept(self) -> None:
         self.close()
 
     def set_probe_color(self, color):
-        self.label.setStyleSheet('QLabel {background-color: ' + color + ';}')
+        self.label.setStyleSheet("QLabel {background-color: " + color + ";}")
 
 
 class ProbeInfoWindow(QDialog):
     def __init__(self, name, data):
         super().__init__()
 
         self.setWindowTitle("Probe Information Window")
 
         self.label = QLabel(name)
         # self.label = QLabel("Probe % d " % group_id)
-        color = QColor(data['vis_color'][0], data['vis_color'][1], data['vis_color'][2], data['vis_color'][3])
-        label_style = 'QLabel {background-color: ' + color.name() + '; font-size: 20px}'
+        color = QColor(
+            data["vis_color"][0],
+            data["vis_color"][1],
+            data["vis_color"][2],
+            data["vis_color"][3],
+        )
+        label_style = "QLabel {background-color: " + color.name() + "; font-size: 20px}"
         self.label.setStyleSheet(label_style)
 
-        ap_angle_label = QLabel('AP Angle : ')
+        ap_angle_label = QLabel("AP Angle : ")
         ap_angle_label.setAlignment(Qt.AlignCenter)
-        ml_angle_label = QLabel('ML Angle : ')
+        ml_angle_label = QLabel("ML Angle : ")
         ml_angle_label.setAlignment(Qt.AlignCenter)
-        probe_length_label = QLabel('Probe Length : ')
+        probe_length_label = QLabel("Probe Length : ")
         probe_length_label.setAlignment(Qt.AlignCenter)
-        dv_label = QLabel('DV : ')
+        dv_label = QLabel("DV : ")
         dv_label.setAlignment(Qt.AlignCenter)
-        insertion_coords_label = QLabel('Insertion coordinates : ')
+        insertion_coords_label = QLabel("Insertion coordinates : ")
         insertion_coords_label.setAlignment(Qt.AlignCenter)
-        insertion_voxels_label = QLabel('Insertion voxels : ')
+        insertion_voxels_label = QLabel("Insertion voxels : ")
         insertion_voxels_label.setAlignment(Qt.AlignCenter)
 
-        terminus_coords_label = QLabel('Terminus coordinates : ')
+        terminus_coords_label = QLabel("Terminus coordinates : ")
         terminus_coords_label.setAlignment(Qt.AlignCenter)
-        terminus_voxels_label = QLabel('Terminus voxels : ')
+        terminus_voxels_label = QLabel("Terminus voxels : ")
         terminus_voxels_label.setAlignment(Qt.AlignCenter)
 
-        ap_angle_value = QLabel('{} \u00B0'.format(np.round(data['ap_angle'], 2)))
-        ml_angle_value = QLabel('{} \u00B0'.format(np.round(data['ml_angle'], 2)))
-        probe_length = QLabel('{} \u03BCm'.format(np.round(data['probe_length'], 2)))
-        dv = QLabel('{} \u03BCm'.format(np.round(data['dv'], 2)))
-        ic_val = np.round(data['insertion_coords'], 2)
-        insertion_coords = QLabel('ML: {}\u03BCm,  AP: {}\u03BCm'.format(ic_val[0], ic_val[1]))
-        iv_val = data['insertion_vox'].astype(int)
-        insertion_vox = QLabel('({} {} {})'.format(iv_val[0], iv_val[1], iv_val[2]))
-
-        tc_val = np.round(data['terminus_coords'], 2)
-        terminus_coords = QLabel('ML: {}\u03BCm,  AP: {}\u03BCm'.format(tc_val[0], tc_val[1]))
-        tv_val = data['terminus_vox']
-        terminus_vox = QLabel('({} {} {})'.format(tv_val[0], tv_val[1], tv_val[2]))
+        ap_angle_value = QLabel("{} \u00B0".format(np.round(data["ap_angle"], 2)))
+        ml_angle_value = QLabel("{} \u00B0".format(np.round(data["ml_angle"], 2)))
+        probe_length = QLabel("{} \u03BCm".format(np.round(data["probe_length"], 2)))
+        dv = QLabel("{} \u03BCm".format(np.round(data["dv"], 2)))
+        ic_val = np.round(data["insertion_coords"], 2)
+        insertion_coords = QLabel(
+            "ML: {}\u03BCm,  AP: {}\u03BCm".format(ic_val[0], ic_val[1])
+        )
+        iv_val = data["insertion_vox"].astype(int)
+        insertion_vox = QLabel("({} {} {})".format(iv_val[0], iv_val[1], iv_val[2]))
+
+        tc_val = np.round(data["terminus_coords"], 2)
+        terminus_coords = QLabel(
+            "ML: {}\u03BCm,  AP: {}\u03BCm".format(tc_val[0], tc_val[1])
+        )
+        tv_val = data["terminus_vox"]
+        terminus_vox = QLabel("({} {} {})".format(tv_val[0], tv_val[1], tv_val[2]))
 
         coords_info_group = QGroupBox()
         coords_info_layout = QGridLayout(coords_info_group)
         coords_info_layout.addWidget(ap_angle_label, 0, 0, 1, 1)
         coords_info_layout.addWidget(ap_angle_value, 0, 1, 1, 1)
         coords_info_layout.addWidget(ml_angle_label, 0, 2, 1, 1)
         coords_info_layout.addWidget(ml_angle_value, 0, 3, 1, 1)
@@ -365,93 +432,125 @@
 
         coords_info_layout.addWidget(insertion_voxels_label, 3, 0, 1, 1)
         coords_info_layout.addWidget(insertion_vox, 3, 1, 1, 1)
         coords_info_layout.addWidget(terminus_voxels_label, 3, 2, 1, 1)
         coords_info_layout.addWidget(terminus_vox, 3, 3, 1, 1)
 
         # group info container
-        region_sites_num = np.ravel(data['region_sites']).astype(str)[::-1]
-        region_label = np.ravel(data['region_label']).astype(int).astype(str)[::-1]
-        region_color = np.asarray(data['label_color'])[::-1, :]
-        region_length = np.round(data['region_length'], 3).astype(str)[::-1]
-        region_name = np.ravel(data['label_name'])[::-1]
-        region_acronym = np.ravel(data['label_acronym'])[::-1]
-
-
+        region_sites_num = np.ravel(data["region_sites"]).astype(str)[::-1]
+        region_label = np.ravel(data["region_label"]).astype(int).astype(str)[::-1]
+        region_color = np.asarray(data["label_color"])[::-1, :]
+        region_length = np.round(data["region_length"], 3).astype(str)[::-1]
+        region_name = np.ravel(data["label_name"])[::-1]
+        region_acronym = np.ravel(data["label_acronym"])[::-1]
 
         sec_group = QGroupBox()
         sec_layout = QGridLayout(sec_group)
-        column_names = [QLabel('ID'), QLabel('Brain Region'), QLabel('Acronym'),
-                        QLabel('Sites (stk)'), QLabel('Length (um)'), QLabel('Color')]
+        column_names = [
+            QLabel("ID"),
+            QLabel("Brain Region"),
+            QLabel("Acronym"),
+            QLabel("Sites (stk)"),
+            QLabel("Length (um)"),
+            QLabel("Color"),
+        ]
         for i in range(len(column_names)):
             sec_layout.addWidget(column_names[i], 0, i, 1, 1)
 
         for i in range(len(region_label)):
             clb = QLabel()
-            da_color = QColor(region_color[i][0], region_color[i][1], region_color[i][2], 255).name()
-            clb.setStyleSheet('QLabel {background-color: ' + da_color + '; width: 20px; height: 20px}')
-
-            row_val = [QLabel(region_label[i]), QLabel(region_name[i]), QLabel(region_acronym[i]),
-                       QLabel(region_sites_num[i]), QLabel(region_length[i]), clb]
+            da_color = QColor(
+                region_color[i][0], region_color[i][1], region_color[i][2], 255
+            ).name()
+            clb.setStyleSheet(
+                "QLabel {background-color: " + da_color + "; width: 20px; height: 20px}"
+            )
+
+            row_val = [
+                QLabel(region_label[i]),
+                QLabel(region_name[i]),
+                QLabel(region_acronym[i]),
+                QLabel(region_sites_num[i]),
+                QLabel(region_length[i]),
+                clb,
+            ]
 
             for j in range(len(row_val)):
                 sec_layout.addWidget(row_val[j], i + 1, j, 1, 1)
 
-
         # plot container
         plot_frame = QFrame()
         plot_frame.setMaximumWidth(300)
         plot_frame.setMinimumWidth(300)
         view_layout = QHBoxLayout(plot_frame)
         view_layout.setSpacing(0)
         view_layout.setContentsMargins(0, 0, 0, 0)
 
         w = pg.GraphicsLayoutWidget()
         view = w.addViewBox()
         view.setAspectLocked()
         # view.invertY(True)
 
         # load plot data
-        vis_data = data['vis_data']
+        vis_data = data["vis_data"]
         n_column = len(vis_data)
 
-        probe_type_name = data['probe_type_name']
+        probe_type_name = data["probe_type_name"]
         # draw tips
-        if probe_type_name != 'Tetrode':
-            da_tip_loc = np.array([[0, 0], [0.5 * n_column, - 2 * n_column], [n_column, 0]])
-            tips = pg.PlotDataItem(da_tip_loc, connect='all', fillLevel=0, fillBrush=pg.mkBrush(color=(128, 128, 128)))
+        if probe_type_name != "Tetrode":
+            da_tip_loc = np.array(
+                [[0, 0], [0.5 * n_column, -2 * n_column], [n_column, 0]]
+            )
+            tips = pg.PlotDataItem(
+                da_tip_loc,
+                connect="all",
+                fillLevel=0,
+                fillBrush=pg.mkBrush(color=(128, 128, 128)),
+            )
             view.addItem(tips)
 
         # draw area
-        region_label = data['region_label']
-        region_sites = data['region_sites']
-        region_text_loc = data['text_loc']
+        region_label = data["region_label"]
+        region_sites = data["region_sites"]
+        region_text_loc = data["text_loc"]
 
-        group_color = data['label_color']
-        sites_label = data['sites_label']
+        group_color = data["label_color"]
+        sites_label = data["sites_label"]
         for i in range(n_column):
-            group_id = vis_data[i]['group_id'].astype(int)
-            start_loc = vis_data[i]['start_loc']
-            end_loc = vis_data[i]['end_loc']
-            sites_loc_column = vis_data[i]['sites']
+            group_id = vis_data[i]["group_id"].astype(int)
+            start_loc = vis_data[i]["start_loc"]
+            end_loc = vis_data[i]["end_loc"]
+            sites_loc_column = vis_data[i]["sites"]
 
             for j in range(len(group_id)):
                 area_data = np.array([[i, end_loc[j]], [i + 1, end_loc[j]]])
-                da_item = pg.PlotDataItem(area_data, fillLevel=start_loc[j],
-                                          fillBrush=group_color[group_id[j]], pen=None)
+                da_item = pg.PlotDataItem(
+                    area_data,
+                    fillLevel=start_loc[j],
+                    fillBrush=group_color[group_id[j]],
+                    pen=None,
+                )
                 view.addItem(da_item)
 
             sites_color = []
             for j in range(len(sites_label[i])):
                 color_ind = np.where(region_label == sites_label[i][j])[0][0]
                 sites_color.append(group_color[color_ind])
 
-            pnt_data = np.stack([np.repeat(i + 0.5, len(sites_loc_column)), sites_loc_column], axis=1)
-            da_item = pg.ScatterPlotItem(pos=pnt_data, pen=(128, 128, 128, 128), brush=sites_color,
-                                         symbol='s', size=3, hoverSize=8)
+            pnt_data = np.stack(
+                [np.repeat(i + 0.5, len(sites_loc_column)), sites_loc_column], axis=1
+            )
+            da_item = pg.ScatterPlotItem(
+                pos=pnt_data,
+                pen=(128, 128, 128, 128),
+                brush=sites_color,
+                symbol="s",
+                size=3,
+                hoverSize=8,
+            )
             view.addItem(da_item)
 
         # draw text
         for i in range(len(region_label)):
             region_text = pg.TextItem(str(region_sites[i]))
             region_text.setPos(n_column + 0.5, region_text_loc[i])
             view.addItem(region_text)
@@ -478,26 +577,33 @@
         layout.addWidget(ok_btn)
         self.setLayout(layout)
 
     def accept(self) -> None:
         self.close()
 
     def set_probe_color(self, color):
-        self.label.setStyleSheet('QLabel {background-color: ' + color + ';}')
+        self.label.setStyleSheet("QLabel {background-color: " + color + ";}")
 
 
 class SinglePiece(QWidget):
     sig_clicked = pyqtSignal(object)
     sig_name_changed = pyqtSignal(object)
 
-    def __init__(self, parent=None, index=0, obj_name='', obj_type='probe piece', object_icon=None):
+    def __init__(
+        self,
+        parent=None,
+        index=0,
+        obj_name="",
+        obj_type="probe piece",
+        object_icon=None,
+    ):
         QWidget.__init__(self, parent=parent)
 
-        self.inactive_style = 'QFrame{background-color:rgb(83, 83, 83); border: 1px solid rgb(128, 128, 128);}'
-        self.active_style = 'QFrame{background-color:rgb(107, 107, 107); border: 1px solid rgb(128, 128, 128);}'
+        self.inactive_style = "QFrame{background-color:rgb(83, 83, 83); border: 1px solid rgb(128, 128, 128);}"
+        self.active_style = "QFrame{background-color:rgb(107, 107, 107); border: 1px solid rgb(128, 128, 128);}"
 
         self.id = index
         self.object_name = obj_name
         self.object_type = obj_type
         self.active = True
 
         self.tbnail = QPushButton()
@@ -553,15 +659,15 @@
         self.l_line_edit.setFocus(True)
         self.set_checked(True)
         self.sig_clicked.emit(self.id)
 
     @pyqtSlot()
     def enter_pressed(self):
         da_text = self.l_line_edit.text()
-        if '-' not in da_text or 'piece' not in da_text:
+        if "-" not in da_text or "piece" not in da_text:
             return
         self.l_line_edit.setVisible(False)
         self.text_btn.setText(self.l_line_edit.text())
         self.object_name = self.l_line_edit.text()
         self.text_btn.setVisible(True)
         self.sig_name_changed.emit((self.id, self.object_name))
 
@@ -579,22 +685,31 @@
 class RegisteredObject(QWidget):
     sig_object_color_changed = pyqtSignal(object)
     eye_clicked = pyqtSignal(object)
     sig_clicked = pyqtSignal(object)
     sig_link = pyqtSignal(object)
     sig_double_clicked = pyqtSignal(object)
 
-    def __init__(self, parent=None, obj_id=0, obj_name='', obj_type='merged probe', object_icon=None):
+    def __init__(
+        self,
+        parent=None,
+        obj_id=0,
+        obj_name="",
+        obj_type="merged probe",
+        object_icon=None,
+    ):
         QWidget.__init__(self, parent=parent)
 
-        self.inactive_style = 'QFrame{background-color:rgb(83, 83, 83); border: 1px solid rgb(128, 128, 128);}'
-        self.active_style = 'QFrame{background-color:rgb(107, 107, 107); border: 1px solid rgb(128, 128, 128);}'
+        self.inactive_style = "QFrame{background-color:rgb(83, 83, 83); border: 1px solid rgb(128, 128, 128);}"
+        self.active_style = "QFrame{background-color:rgb(107, 107, 107); border: 1px solid rgb(128, 128, 128);}"
 
         self.color = QColor(randint(0, 255), randint(0, 255), randint(0, 255), 255)
-        self.icon_back = 'border:1px solid black; background-color: {}'.format(self.color.name())
+        self.icon_back = "border:1px solid black; background-color: {}".format(
+            self.color.name()
+        )
 
         self.id = obj_id
         self.object_type = obj_type
         self.object_name = obj_name
         self.active = True
         self.vis = True
 
@@ -620,15 +735,17 @@
         self.text_btn.clicked.connect(self.text_btn_on_click)
         # self.text_btn.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Ignored)
 
         self.link_button = QPushButton()
         self.link_button.setFixedSize(QSize(25, 40))
         self.link_button.setCheckable(True)
         link_icon = QIcon()
-        link_icon.addPixmap(QPixmap("icons/sidebar/link_off.svg"), QIcon.Normal, QIcon.Off)
+        link_icon.addPixmap(
+            QPixmap("icons/sidebar/link_off.svg"), QIcon.Normal, QIcon.Off
+        )
         link_icon.addPixmap(QPixmap("icons/sidebar/link.svg"), QIcon.Normal, QIcon.On)
         self.link_button.setIcon(link_icon)
         self.link_button.setIconSize(QSize(20, 20))
         self.link_button.clicked.connect(self.on_linked)
 
         self.inner_frame = QFrame()
         self.inner_frame.setStyleSheet(self.active_style)
@@ -651,15 +768,17 @@
         outer_layout.addWidget(self.inner_frame)
 
         self.setLayout(outer_layout)
         self.setFixedHeight(40)
 
     def set_icon_style(self, color):
         self.color = color
-        self.icon_back = 'border:1px solid black; background-color: {}'.format(color.name())
+        self.icon_back = "border:1px solid black; background-color: {}".format(
+            color.name()
+        )
         self.tbnail.setStyleSheet(self.icon_back)
 
     def change_object_color(self):
         self.sig_object_color_changed.emit(self.id)
 
     def eye_on_click(self):
         if self.eye_button.isChecked():
@@ -688,22 +807,21 @@
     def on_linked(self):
         self.sig_link.emit(self.id)
 
 
 class BottomButton(QPushButton):
     def __init__(self, icon_path):
         QPushButton.__init__(self)
-        btm_style = read_qss_file('qss/obj_ctrl_bottom_button.qss')
+        btm_style = read_qss_file("qss/obj_ctrl_bottom_button.qss")
         self.setFixedSize(24, 24)
         self.setStyleSheet(btm_style)
         self.setIcon(QIcon(icon_path))
         self.setIconSize(QSize(20, 20))
 
 
-
 class ObjectControl(QObject):
     """
     only pieces' name can be changed, the merged can not, so far
     """
 
     class SignalProxy(QObject):
         sigOpacityChanged = pyqtSignal(object)
@@ -711,100 +829,110 @@
         sigDeleteObject = pyqtSignal(object)
         sigAddObject = pyqtSignal(object)
         sigColorChanged = pyqtSignal(object)
         sigSizeChanged = pyqtSignal(object)
         sigBlendModeChanged = pyqtSignal(object)
 
     def __init__(self, parent=None):
-
         self._sigprox = ObjectControl.SignalProxy()
         self.sig_opacity_changed = self._sigprox.sigOpacityChanged
         self.sig_visible_changed = self._sigprox.sigVisChanged
-        self.sig_delete_object = self._sigprox.sigDeleteObject  # for delete obj 3d gl widgets
+        self.sig_delete_object = (
+            self._sigprox.sigDeleteObject
+        )  # for delete obj 3d gl widgets
         self.sig_add_object = self._sigprox.sigAddObject  # for add obj 3d gl widgets
         self.sig_color_changed = self._sigprox.sigColorChanged
         self.sig_size_changed = self._sigprox.sigSizeChanged
         self.sig_blend_mode_changed = self._sigprox.sigBlendModeChanged
 
         QObject.__init__(self)
 
         self.default_size_val = 2
         self.default_opacity_val = 100
 
-        self.valid_obj_type = ['probe piece', 'merged probe',
-                               'cells piece', 'merged cells',
-                               'virus piece', 'merged virus',
-                               'contour piece', 'merged contour',
-                               'drawing piece', 'merged drawing']
+        self.valid_obj_type = [
+            "probe piece",
+            "merged probe",
+            "cells piece",
+            "merged cells",
+            "virus piece",
+            "merged virus",
+            "contour piece",
+            "merged contour",
+            "drawing piece",
+            "merged drawing",
+        ]
 
         self.current_obj_index = None
 
         self.obj_count = 0
         self.linked_indexes = []
 
         self.obj_list = []  # widgets
         self.obj_id = []  # identity
-        self.obj_name = []  # names, initially the same as type, can be changed freely ???
+        self.obj_name = (
+            []
+        )  # names, initially the same as type, can be changed freely ???
         self.obj_type = []  # type
         self.obj_data = []  # data
         self.obj_size = []  # size
         self.obj_opacity = []
         self.obj_comp_mode = []
         self.obj_visibility = []
         self.obj_merged = []
 
-        self.probe_icon = QIcon('icons/sidebar/probe.svg')
-        self.virus_icon = QIcon('icons/sidebar/virus.svg')
-        self.drawing_icon = QIcon('icons/toolbar/pencil.svg')
-        self.cell_icon = QIcon('icons/toolbar/location.svg')
-        self.contour_icon = QIcon('icons/sidebar/contour.svg')
-        self.compare_icon = QIcon('icons/sidebar/compare.svg')
+        self.probe_icon = QIcon("icons/sidebar/probe.svg")
+        self.virus_icon = QIcon("icons/sidebar/virus.svg")
+        self.drawing_icon = QIcon("icons/toolbar/pencil.svg")
+        self.cell_icon = QIcon("icons/toolbar/location.svg")
+        self.contour_icon = QIcon("icons/sidebar/contour.svg")
+        self.compare_icon = QIcon("icons/sidebar/compare.svg")
 
-        combo_label = QLabel('Composition:')
+        combo_label = QLabel("Composition:")
         combo_label.setFixedWidth(80)
         self.obj_blend_combo = QComboBox()
         self.obj_blend_combo.setEditable(False)
-        combo_value = ['opaque', 'translucent', 'additive']
+        combo_value = ["opaque", "translucent", "additive"]
         self.obj_blend_combo.addItems(combo_value)
-        self.obj_blend_combo.setCurrentText('opaque')
+        self.obj_blend_combo.setCurrentText("opaque")
         self.obj_blend_combo.currentTextChanged.connect(self.blend_mode_changed)
         combo_wrap = QFrame()
         combo_wrap_layout = QHBoxLayout(combo_wrap)
         combo_wrap_layout.setContentsMargins(0, 0, 0, 0)
         combo_wrap_layout.setSpacing(5)
         combo_wrap_layout.addWidget(combo_label)
         combo_wrap_layout.addWidget(self.obj_blend_combo)
 
-        obj_opacity_label = QLabel('Opacity:')
+        obj_opacity_label = QLabel("Opacity:")
         obj_opacity_label.setFixedWidth(80)
         self.obj_opacity_slider = QSlider(Qt.Horizontal)
         self.obj_opacity_slider.setMaximum(100)
         self.obj_opacity_slider.setMinimum(0)
         self.obj_opacity_slider.setValue(100)
         self.obj_opacity_slider.valueChanged.connect(self.change_opacity_label_value)
         self.obj_opacity_slider.sliderMoved.connect(self.send_opacity_changed_signal)
-        self.obj_opacity_val_label = QLabel('100%')
+        self.obj_opacity_val_label = QLabel("100%")
         self.obj_opacity_val_label.setFixedWidth(40)
         opacity_wrap = QFrame()
         opacity_wrap_layout = QHBoxLayout(opacity_wrap)
         opacity_wrap_layout.setContentsMargins(0, 0, 0, 0)
         opacity_wrap_layout.setSpacing(5)
         opacity_wrap_layout.addWidget(obj_opacity_label)
         opacity_wrap_layout.addWidget(self.obj_opacity_slider)
         opacity_wrap_layout.addWidget(self.obj_opacity_val_label)
 
-        obj_size_label = QLabel('Size/Width: ')
+        obj_size_label = QLabel("Size/Width: ")
         obj_size_label.setFixedWidth(80)
         self.obj_size_slider = QSlider(Qt.Horizontal)
         self.obj_size_slider.setValue(2)
         self.obj_size_slider.setMinimum(1)
         self.obj_size_slider.setMaximum(10)
         self.obj_size_slider.valueChanged.connect(self.change_size_label_value)
         self.obj_size_slider.sliderMoved.connect(self.send_size_changed_signal)
-        self.obj_size_val_label = QLabel('2')
+        self.obj_size_val_label = QLabel("2")
         self.obj_size_val_label.setAlignment(Qt.AlignCenter)
         self.obj_size_val_label.setFixedWidth(40)
         size_wrap = QFrame()
         size_wrap_layout = QHBoxLayout(size_wrap)
         size_wrap_layout.setContentsMargins(0, 0, 0, 0)
         size_wrap_layout.setSpacing(5)
         size_wrap_layout.addWidget(obj_size_label)
@@ -819,31 +947,33 @@
         top_layout.addSpacing(10)
         top_layout.addWidget(opacity_wrap)
         top_layout.addSpacing(10)
         top_layout.addWidget(size_wrap)
         top_layout.addSpacing(10)
 
         self.layer_frame = QFrame()
-        self.layer_frame.setStyleSheet('background: transparent; border: 0px;')
+        self.layer_frame.setStyleSheet("background: transparent; border: 0px;")
         self.layer_frame.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         self.layer_layout = QBoxLayout(QBoxLayout.BottomToTop, self.layer_frame)
         self.layer_layout.setAlignment(Qt.AlignBottom)
         self.layer_layout.setContentsMargins(0, 0, 0, 0)
         self.layer_layout.setSpacing(5)
 
         self.layer_scroll = QScrollArea()
-        self.layer_scroll.setStyleSheet('background: transparent; border: 0px;')
+        self.layer_scroll.setStyleSheet("background: transparent; border: 0px;")
         self.layer_scroll.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         self.layer_scroll.setWidget(self.layer_frame)
         self.layer_scroll.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOn)
         self.layer_scroll.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.layer_scroll.setWidgetResizable(True)
 
         mid_frame = QFrame()
-        mid_frame.setStyleSheet('background: transparent; border: 1px solid rgb(128, 128, 128);')
+        mid_frame.setStyleSheet(
+            "background: transparent; border: 1px solid rgb(128, 128, 128);"
+        )
         mid_frame.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         mid_layout = QGridLayout(mid_frame)
         mid_layout.setContentsMargins(0, 0, 0, 0)
         mid_layout.setSpacing(0)
         mid_layout.setAlignment(Qt.AlignBottom)
         mid_layout.addWidget(self.layer_scroll, 0, 0, 1, 1)
 
@@ -851,81 +981,81 @@
         self.outer_frame.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         outer_layout = QVBoxLayout(self.outer_frame)
         outer_layout.setSpacing(0)
         outer_layout.addWidget(top_frame)
         outer_layout.addWidget(mid_frame)
 
         # bottom buttons
-        self.info_btn = BottomButton('icons/sidebar/info.svg')
-        self.info_btn.setToolTip('open information window')
+        self.info_btn = BottomButton("icons/sidebar/info.svg")
+        self.info_btn.setToolTip("open information window")
         self.info_btn.clicked.connect(self.info_btn_clicked)
 
-        self.vis2d_btn = BottomButton('icons/toolbar/vis2d.svg')
-        self.vis2d_btn.setToolTip('find the corresponding 2D plane')
-        self.unmerge_btn = BottomButton('icons/toolbar/unmerge.svg')
-        self.unmerge_btn.setToolTip('un-merge a merged object')
+        self.vis2d_btn = BottomButton("icons/toolbar/vis2d.svg")
+        self.vis2d_btn.setToolTip("find the corresponding 2D plane")
+        self.unmerge_btn = BottomButton("icons/toolbar/unmerge.svg")
+        self.unmerge_btn.setToolTip("un-merge a merged object")
         self.unmerge_btn.clicked.connect(self.unmerge_objects)
-        self.compare_btn = BottomButton('icons/sidebar/compare.svg')
-        self.compare_btn.setToolTip('compare multiple linked objects')
+        self.compare_btn = BottomButton("icons/sidebar/compare.svg")
+        self.compare_btn.setToolTip("compare multiple linked objects")
 
-        self.merge_probe_btn = BottomButton('icons/sidebar/probe.svg')
-        self.merge_probe_btn.setToolTip('merge probes pieces')
+        self.merge_probe_btn = BottomButton("icons/sidebar/probe.svg")
+        self.merge_probe_btn.setToolTip("merge probes pieces")
 
-        self.merge_drawing_btn = BottomButton('icons/toolbar/pencil.svg')
-        self.merge_drawing_btn.setToolTip('merge drawing pieces')
+        self.merge_drawing_btn = BottomButton("icons/toolbar/pencil.svg")
+        self.merge_drawing_btn.setToolTip("merge drawing pieces")
 
-        self.merge_cell_btn = BottomButton('icons/toolbar/location.svg')
-        self.merge_cell_btn.setToolTip('merge cells pieces')
+        self.merge_cell_btn = BottomButton("icons/toolbar/location.svg")
+        self.merge_cell_btn.setToolTip("merge cells pieces")
 
-        self.merge_virus_btn = BottomButton('icons/sidebar/virus.svg')
-        self.merge_virus_btn.setToolTip('merge virus pieces')
+        self.merge_virus_btn = BottomButton("icons/sidebar/virus.svg")
+        self.merge_virus_btn.setToolTip("merge virus pieces")
 
-        self.merge_contour_btn = BottomButton('icons/sidebar/contour.svg')
-        self.merge_contour_btn.setToolTip('merge contour pieces')
+        self.merge_contour_btn = BottomButton("icons/sidebar/contour.svg")
+        self.merge_contour_btn.setToolTip("merge contour pieces")
 
-        self.add_object_btn = BottomButton('icons/sidebar/add.png')
-        self.add_object_btn.setToolTip('add a piece')
+        self.add_object_btn = BottomButton("icons/sidebar/add.png")
+        self.add_object_btn.setToolTip("add a piece")
 
-        self.delete_object_btn = BottomButton('icons/sidebar/trash.png')
-        self.delete_object_btn.setToolTip('delete an object')
+        self.delete_object_btn = BottomButton("icons/sidebar/trash.png")
+        self.delete_object_btn.setToolTip("delete an object")
         self.delete_object_btn.clicked.connect(self.delete_object_btn_clicked)
 
     def blend_mode_changed(self):
         blend_mode = self.obj_blend_combo.currentText()
         if self.current_obj_index is None:
             return
-        if 'merged' not in self.obj_type[self.current_obj_index]:
+        if "merged" not in self.obj_type[self.current_obj_index]:
             return
         if blend_mode != self.obj_comp_mode[self.current_obj_index]:
             self.obj_comp_mode[self.current_obj_index] = blend_mode
             self.sig_blend_mode_changed.emit(blend_mode)
 
     def change_opacity_label_value(self):
         da_val = self.obj_opacity_slider.value()
-        self.obj_opacity_val_label.setText('{} %'.format(da_val))
+        self.obj_opacity_val_label.setText("{} %".format(da_val))
 
     def send_opacity_changed_signal(self):
         da_val = self.obj_opacity_slider.value()
         if self.current_obj_index is None:
             return
-        if 'merged' not in self.obj_type[self.current_obj_index]:
+        if "merged" not in self.obj_type[self.current_obj_index]:
             self.obj_opacity_slider.setValue(da_val)
             return
         self.obj_opacity[self.current_obj_index] = da_val
         self.sig_opacity_changed.emit(da_val)
 
     def change_size_label_value(self):
         da_val = self.obj_size_slider.value()
         self.obj_size_val_label.setText(str(da_val))
 
     def send_size_changed_signal(self):
         da_val = self.obj_size_slider.value()
         if self.current_obj_index is None:
             return
-        if 'merged' not in self.obj_type[self.current_obj_index]:
+        if "merged" not in self.obj_type[self.current_obj_index]:
             self.obj_size_slider.setValue(da_val)
             return
         self.obj_size[self.current_obj_index] = da_val
         self.sig_size_changed.emit((self.obj_type[self.current_obj_index], da_val))
 
     def obj_piece_name_changed(self, ev):
         clicked_id = ev[0]
@@ -936,28 +1066,28 @@
 
     def delete_object_btn_clicked(self):
         if self.current_obj_index is None:
             return
         self.delete_objects(self.current_obj_index)
 
     def info_btn_clicked(self):
-        if 'merged' in self.obj_type[self.current_obj_index]:
+        if "merged" in self.obj_type[self.current_obj_index]:
             self.obj_info_on_click()
 
     def obj_clicked(self, clicked_id):
         self.set_active_layer_to_current(clicked_id)
 
     def obj_info_on_click(self):
         da_data = self.obj_data[self.current_obj_index]
         da_name = self.obj_name[self.current_obj_index]
-        if 'probe' in self.obj_type[self.current_obj_index]:
+        if "probe" in self.obj_type[self.current_obj_index]:
             self.info_window = ProbeInfoWindow(da_name, da_data)
-        elif 'virus' in self.obj_type[self.current_obj_index]:
+        elif "virus" in self.obj_type[self.current_obj_index]:
             self.info_window = VirusInfoWindow(da_name, da_data)
-        elif 'cell' in self.obj_type[self.current_obj_index]:
+        elif "cell" in self.obj_type[self.current_obj_index]:
             self.info_window = CellsInfoWindow(da_name, da_data)
         else:
             return
         self.info_window.exec()
 
     def set_active_layer_to_current(self, clicked_id):
         previous_obj_id = self.obj_id[self.current_obj_index]
@@ -1021,63 +1151,78 @@
                 self.current_obj_index = None
         else:
             active_index = np.where(np.ravel(self.obj_id) == current_obj_id)[0][0]
             self.current_obj_index = active_index
 
     #
     def get_object_icon(self, object_type):
-        if 'probe' in object_type:
+        if "probe" in object_type:
             object_icon = self.probe_icon
-        elif 'virus' in object_type:
+        elif "virus" in object_type:
             object_icon = self.virus_icon
-        elif 'cell' in object_type:
+        elif "cell" in object_type:
             object_icon = self.cell_icon
-        elif 'contour' in object_type:
+        elif "contour" in object_type:
             object_icon = self.contour_icon
-        elif 'drawing' in object_type:
+        elif "drawing" in object_type:
             object_icon = self.drawing_icon
         else:
             object_icon = None
         return object_icon
 
     def get_group_count(self, object_type):
-        group_count = len([da_type for da_type in self.obj_type if da_type == object_type])
+        group_count = len(
+            [da_type for da_type in self.obj_type if da_type == object_type]
+        )
         return group_count
 
     def add_object(self, object_name, object_type, object_data, object_mode):
         object_icon = self.get_object_icon(object_type)
         # group_count = self.get_group_count(object_type)
         if object_icon is None:
             return
         self.obj_id.append(self.obj_count)
         self.obj_data.append(object_data)
         self.obj_name.append(object_name)
         self.obj_type.append(object_type)
-        if 'merged' in object_type:
-            new_layer = RegisteredObject(obj_id=self.obj_count, obj_name=object_name,
-                                         obj_type=object_type, object_icon=object_icon)
+        if "merged" in object_type:
+            new_layer = RegisteredObject(
+                obj_id=self.obj_count,
+                obj_name=object_name,
+                obj_type=object_type,
+                object_icon=object_icon,
+            )
             new_layer.eye_clicked.connect(self.obj_eye_clicked)
             new_layer.sig_object_color_changed.connect(self.obj_color_changed)
             new_layer.sig_link.connect(self.obj_link_changed)
             self.obj_opacity.append(self.default_opacity_val)
             self.obj_size.append(self.default_size_val)
             self.obj_comp_mode.append(object_mode)
-            da_color = (new_layer.color.red(), new_layer.color.green(), new_layer.color.blue(), 255)
-            self.obj_data[-1]['vis_color'] = da_color
+            da_color = (
+                new_layer.color.red(),
+                new_layer.color.green(),
+                new_layer.color.blue(),
+                255,
+            )
+            self.obj_data[-1]["vis_color"] = da_color
             if self.obj_size_slider.value() != self.default_size_val:
                 self.obj_size_slider.setValue(self.default_size_val)
             if self.obj_opacity_slider.value() != self.default_opacity_val:
                 self.obj_opacity_slider.setValue(self.default_opacity_val)
             if self.obj_blend_combo.currentText() != object_mode:
                 self.obj_blend_combo.blockSignals(True)
                 self.obj_blend_combo.setCurrentText(object_mode)
                 self.obj_blend_combo.blockSignals(False)
         else:
-            new_layer = SinglePiece(index=self.obj_count, obj_name=object_name,
-                                    obj_type=object_type, object_icon=object_icon)
+            new_layer = SinglePiece(
+                index=self.obj_count,
+                obj_name=object_name,
+                obj_type=object_type,
+                object_icon=object_icon,
+            )
             new_layer.sig_name_changed.connect(self.obj_piece_name_changed)
             self.obj_opacity.append([])
             self.obj_size.append([])
             self.obj_comp_mode.append([])
 
         new_layer.text_btn.setText(self.obj_name[-1])
         new_layer.set_checked(True)
@@ -1092,36 +1237,47 @@
             self.current_obj_index = active_index
 
         self.layer_layout.addWidget(self.obj_list[-1])
         self.sig_add_object.emit((object_data, object_type))
         self.obj_count += 1
 
     # merge object pieces
-    def merge_pieces(self, obj_type='probe piece'):
-        if obj_type not in ['probe piece', 'virus piece', 'contour piece', 'drawing piece', 'cells piece']:
+    def merge_pieces(self, obj_type="probe piece"):
+        if obj_type not in [
+            "probe piece",
+            "virus piece",
+            "contour piece",
+            "drawing piece",
+            "cells piece",
+        ]:
             return
         n_obj = len(self.obj_id)
         cind = [ind for ind in range(n_obj) if self.obj_type[ind] == obj_type]
+        # print("cind", cind)
         valid_pieces_names = np.ravel(self.obj_name)[np.array(cind)]
         n_pieces = len(valid_pieces_names)
         m_obj_names = []
         for i in range(n_pieces):
             da_name = valid_pieces_names[i]
             # da_name = da_name.replace(" ", "")
-            da_name_split = da_name.split('-')
+            da_name_split = da_name.split("-")
             m_obj_name = da_name_split[0]
-            if m_obj_name[-1] == ' ':
+            if m_obj_name[-1] == " ":
                 m_obj_name = m_obj_name[:-1]
             m_obj_names.append(m_obj_name)
         merging_object_names = np.unique(m_obj_names)
         n_object = len(merging_object_names)
         data = [[] for _ in range(n_object)]
         pieces_names = [[] for _ in range(n_object)]
         for i in range(n_object):
-            sub_inds = [cind[ind] for ind in range(n_pieces) if m_obj_names[ind] == merging_object_names[i]]
+            sub_inds = [
+                cind[ind]
+                for ind in range(n_pieces)
+                if m_obj_names[ind] == merging_object_names[i]
+            ]
             for j in range(len(sub_inds)):
                 data[i].append(self.obj_data[sub_inds[j]])
                 pieces_names[i].append(self.obj_name[sub_inds[j]])
             # temp = self.obj_data[da_piece_ind_in_obj_order[0]].T
             # if len(da_piece_ind_in_obj_order) > 1:
             #     for j in range(1, len(da_piece_ind_in_obj_order)):
             #         print(self.obj_data[da_piece_ind_in_obj_order[j]].T)
@@ -1129,62 +1285,74 @@
             # data[i] = temp.T
         self.delete_objects(cind)
         return data, merging_object_names, pieces_names
 
     # unmerge object pieces
     def unmerge_objects(self):
         current_type = self.obj_type[self.current_obj_index]
-        if 'merged' not in current_type:
+        if "merged" not in current_type:
             return
         current_data = self.obj_data[self.current_obj_index]
-        m_obj_type = current_type.split(' ')[1]
-        data_list = current_data['data']
-        pieces_names = current_data['pieces_names']
+        m_obj_type = current_type.split(" ")[1]
+        data_list = current_data["data"]
+        pieces_names = current_data["pieces_names"]
         self.delete_objects([self.current_obj_index])
         for i in range(len(data_list)):
-            self.add_object(pieces_names[i], '{} piece'.format(m_obj_type), data_list[i], None)
-
+            self.add_object(
+                pieces_names[i], "{} piece".format(m_obj_type), data_list[i], None
+            )
 
     # get obj data
     def get_obj_data(self):
-        data = {'obj_name': self.obj_name,
-                'obj_type': self.obj_type,
-                'obj_data': self.obj_data,
-                'obj_size': self.obj_size,
-                'obj_opacity': self.obj_opacity,
-                'obj_comp_mode': self.obj_comp_mode,
-                'current_obj_index': self.current_obj_index}
+        data = {
+            "obj_name": self.obj_name,
+            "obj_type": self.obj_type,
+            "obj_data": self.obj_data,
+            "obj_size": self.obj_size,
+            "obj_opacity": self.obj_opacity,
+            "obj_comp_mode": self.obj_comp_mode,
+            "current_obj_index": self.current_obj_index,
+        }
         return data
 
     def set_obj_data(self, data):
-        for i in range(len(data['obj_type'])):
-            self.add_object(data['obj_name'][i], data['obj_type'][i], data['obj_data'][i], data['obj_comp_mode'][i])
-
-        self.obj_size = data['obj_size']
-        self.obj_opacity = data['obj_opacity']
-        self.obj_comp_mode = data['obj_comp_mode']
-        self.current_obj_index = data['current_obj_index']
+        for i in range(len(data["obj_type"])):
+            self.add_object(
+                data["obj_name"][i],
+                data["obj_type"][i],
+                data["obj_data"][i],
+                data["obj_comp_mode"][i],
+            )
+
+        self.obj_size = data["obj_size"]
+        self.obj_opacity = data["obj_opacity"]
+        self.obj_comp_mode = data["obj_comp_mode"]
+        self.current_obj_index = data["current_obj_index"]
 
         self.obj_list[-1].set_checked(False)
         self.obj_list[self.current_obj_index].set_checked(True)
 
         # print(self.obj_type)
 
     def set_slider_combo_to_current(self):
-        if 'merged' in self.obj_type[self.current_obj_index]:
+        if "merged" in self.obj_type[self.current_obj_index]:
             size_val = self.obj_size_slider.value()
             opacity_val = self.obj_opacity_slider.value()
             compo_mode = self.obj_blend_combo.currentText()
 
             if self.obj_size[self.current_obj_index] != size_val:
                 self.obj_size_slider.setValue(self.obj_size[self.current_obj_index])
             if self.obj_opacity[self.current_obj_index] != opacity_val:
-                self.obj_opacity_slider.setValue(self.obj_opacity[self.current_obj_index])
+                self.obj_opacity_slider.setValue(
+                    self.obj_opacity[self.current_obj_index]
+                )
             if self.obj_comp_mode[self.current_obj_index] != compo_mode:
-                self.obj_blend_combo.setCurrentText(self.obj_comp_mode[self.current_obj_index])
+                self.obj_blend_combo.setCurrentText(
+                    self.obj_comp_mode[self.current_obj_index]
+                )
         else:
             return
 
     def clear_all(self):
         ind = np.arange(len(self.obj_list))[::-1]
         for i in ind:
             self.layer_layout.removeWidget(self.obj_list[i])
@@ -1201,9 +1369,7 @@
         self.current_obj_index = None
 
     def compare_obj_called(self):
         compare_names = [self.obj_name[ind] for ind in self.linked_indexes]
         compare_data = [self.obj_data[ind] for ind in self.linked_indexes]
         info_window = CompareWindow(compare_names, compare_data)
         info_window.exec()
-
-
```

### Comparing `herbs-0.2.2/herbs/probe_utiles.py` & `herbs-0.2.3/herbs/probe_utiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         direction = sp - ep
         direction = direction / np.linalg.norm(direction)
 
         valid_ind = np.where(image[:, int(sp[0])] != 0)[0]
         if len(valid_ind) > 0:
             valid_ind = valid_ind[0]
         else:
-            msg = 'Something went wrong for the probe location. Please contact maintainers.'
+            msg = "Something went wrong for the probe location. Please contact maintainers."
 
         if int(sp[1]) < valid_ind:
             sign_flag = -1
         elif int(sp[1]) > valid_ind:
             sign_flag = 1
         else:
             sign_flag = 0
@@ -52,15 +52,15 @@
         while int(temp[1]) != valid_ind:
             stop_steps += 1
             temp = sp + sign_flag * stop_steps * direction
             valid_ind = np.where(image[:, int(temp[0])] != 0)[0]
             if len(valid_ind) > 0:
                 valid_ind = valid_ind[0]
             else:
-                msg = 'Something went wrong for the probe location. Please contact maintainers.'
+                msg = "Something went wrong for the probe location. Please contact maintainers."
                 break
 
         sp = sp + sign_flag * stop_steps * direction
 
     p2 = np.array([sp, ep])
     return p2, msg
 
@@ -103,39 +103,39 @@
         ml_angle = 180 - ml_angle
 
     return ap_angle, ml_angle
 
 
 def get_tilt_info(sp, ep):
     if ep[1] < sp[1]:
-        ap_tilt = 'posterior'
+        ap_tilt = "posterior"
     elif ep[1] > sp[1]:
-        ap_tilt = 'anterior'
+        ap_tilt = "anterior"
     else:
-        ap_tilt = 'no tilt'
+        ap_tilt = "no tilt"
 
     if sp[0] > 0:
         if ep[0] < sp[0]:
-            ml_tilt = 'medial'
+            ml_tilt = "medial"
         elif ep[0] > sp[0]:
-            ml_tilt = 'lateral'
+            ml_tilt = "lateral"
         else:
-            ml_tilt = 'no tilt'
+            ml_tilt = "no tilt"
     elif sp[0] < 0:
         if ep[0] < sp[0]:
-            ml_tilt = 'lateral'
+            ml_tilt = "lateral"
         elif ep[0] > sp[0]:
-            ml_tilt = 'medial'
+            ml_tilt = "medial"
         else:
-            ml_tilt = 'no tilt'
+            ml_tilt = "no tilt"
     else:
         if ep[0] != sp[0]:
-            ml_tilt = 'lateral'
+            ml_tilt = "lateral"
         else:
-            ml_tilt = 'no tilt'
+            ml_tilt = "no tilt"
     return ap_tilt, ml_tilt
 
 
 def get_tilt_sign(sp, ep):
     if ep[1] < sp[1]:
         ap_tilt = -1
     elif ep[1] > sp[1]:
@@ -149,32 +149,36 @@
         ml_tilt = 1
     else:
         ml_tilt = 0
     return ap_tilt, ml_tilt
 
 
 def pandas_to_str(label_name, label_ano, length, channels):
-    df = pd.DataFrame({
-        'Brain Regions': label_name,
-        'Ano': label_ano,
-        'Probe Length': length,
-        'Probe Channels': channels
-    })
+    df = pd.DataFrame(
+        {
+            "Brain Regions": label_name,
+            "Ano": label_ano,
+            "Probe Length": length,
+            "Probe Channels": channels,
+        }
+    )
     return df.to_string(col_space=30, justify="justify")
 
 
-def correct_start_pnt(label_data, start_pnt, start_vox, direction, bregma, verbose=False):
+def correct_start_pnt(
+    label_data, start_pnt, start_vox, direction, bregma, verbose=False
+):
     error_index = 0
-    print('start_vox', start_vox)
+    # print('start_vox', start_vox)
     direction = direction / np.linalg.norm(direction)
     check_vec = label_data[int(start_vox[0]), int(start_vox[1]), :]
     top_vox = np.where(check_vec != 0)[0]
-    print(np.where(check_vec != 0))
+    # print(np.where(check_vec != 0))
     if len(top_vox) == 0:
-        print('wrong')
+        print("wrong")
     else:
         top_vox = top_vox[-1]
     check_vox = start_vox.astype(int)
     new_sp = start_pnt.copy()
 
     # if int(start_vox[2]) < top_vox:
     #     steps = 0
@@ -228,40 +232,46 @@
                 error_index = 12
                 break
             enter_label = label_data[check_vox[0], check_vox[1], check_vox[2]]
             enter_condition = (enter_label == 0) if z_diff >= 1 else (enter_label != 0)
         if error_index != 0:
             return new_sp, error_index
 
-        new_sp = start_pnt - sign_flag * (stop_steps - 1) * direction if z_diff < 0 else new_sp
+        new_sp = (
+            start_pnt - sign_flag * (stop_steps - 1) * direction
+            if z_diff < 0
+            else new_sp
+        )
         if verbose:
-            print('correct enter pnt with {} steps'.format(stop_steps))
-            print('old sp', start_pnt)
-            print('new pc_sp', new_sp)
+            print("correct enter pnt with {} steps".format(stop_steps))
+            # print('old sp', start_pnt)
+            # print('new pc_sp', new_sp)
 
     return new_sp, error_index
 
 
-def correct_end_point(sp, ep, direction, vox_size, tip_length, max_probe_length, verbose=False):
+def correct_end_point(
+    sp, ep, direction, vox_size, tip_length, max_probe_length, verbose=False
+):
     probe_length_with_tip = np.sqrt(np.sum((sp - ep) ** 2)) * vox_size  # in um
     probe_length_without_tip = probe_length_with_tip - tip_length  # in um
     if max_probe_length is not None:
         if probe_length_with_tip > max_probe_length:
             probe_length_with_tip = max_probe_length
             probe_length_without_tip = probe_length_with_tip - tip_length
             new_ep = sp + direction * probe_length_with_tip / vox_size
         else:
             new_ep = ep
     else:
         new_ep = ep
     if verbose:
-        print('old pc_ep', ep)
-        print('corrected pc_ep', new_ep)
-        print('old probe length with tip', probe_length_with_tip)
-        print('corrected probe length with tip', probe_length_with_tip)
+        print("old pc_ep", ep)
+        print("corrected pc_ep", new_ep)
+        print("old probe length with tip", probe_length_with_tip)
+        print("corrected probe length with tip", probe_length_with_tip)
     return new_ep, probe_length_with_tip, probe_length_without_tip
 
 
 def check_parallel_to_z(direction):
     is_parallel = False
     if abs(abs(direction[2]) - 1) < 1e-6:
         is_parallel = True
@@ -288,15 +298,14 @@
     else:
         tip_length = 0
         channel_size = None
         channel_number_in_banks = None
     return tip_length, channel_size, channel_number_in_banks
 
 
-
 def group_labels(fine_label_mat, verbose=False):
     n_row, n_column = fine_label_mat.shape
     group_mat = np.zeros(fine_label_mat.shape)
     group_mat[:] = np.nan
     group_id = 0
     group_id_label = []
 
@@ -306,169 +315,194 @@
         check_label = fine_label_mat[base_level]
         unique_label = np.unique(check_label)
         for da_label in unique_label:
             if da_label in previous_row:
                 continue
             add_row = 0
             row_index = add_row + base_level
-            label_check = (fine_label_mat[row_index] == da_label)
+            label_check = fine_label_mat[row_index] == da_label
             group_mat[row_index, label_check] = group_id
             while np.any(label_check):
                 add_row += 1
                 row_index = add_row + base_level
                 if row_index == n_row:
                     break
-                label_check = (fine_label_mat[row_index] == da_label)
+                label_check = fine_label_mat[row_index] == da_label
                 group_mat[row_index, label_check] = group_id
             group_id_label.append(da_label)
             group_id += 1
         previous_row = fine_label_mat[base_level]
 
     if verbose:
-        print('group mat nan index', np.where(np.isnan(group_mat)))
-        print('group id label', group_id_label)
-        print('group_mat')
+        print("group mat nan index", np.where(np.isnan(group_mat)))
+        print("group id label", group_id_label)
+        print("group_mat")
         indexs = np.arange(0, len(group_mat), 20)
         for i in range(len(indexs) - 1):
-            print(group_mat[indexs[i]:indexs[i + 1]])
-        print(group_mat[indexs[-1]:len(group_mat)])
+            print(group_mat[indexs[i] : indexs[i + 1]])
+        print(group_mat[indexs[-1] : len(group_mat)])
         print(len(group_mat))
 
     return group_mat, group_id_label
 
 
 def get_column_grouped_info(group_column, column_bound):
     diff_labels = np.where(np.diff(group_column) != 0)[0]
     if len(diff_labels) != 0:
         change_index = np.append(np.array([0]), diff_labels + 1)
         group_id = group_column[change_index]
         start_loc = column_bound[change_index]
-        end_loc = column_bound[np.append(change_index[1:], np.array([len(group_column)]))]
+        end_loc = column_bound[
+            np.append(change_index[1:], np.array([len(group_column)]))
+        ]
     else:
         group_id = group_column[0]
         start_loc = column_bound[0]
         end_loc = column_bound[-1]
 
     group_column_length = np.abs(end_loc - start_loc)
 
     return group_id, start_loc, end_loc, group_column_length
 
 
 def get_vis_data(group_mat, column_loc, sites_loc, sites_line_count, vox_size):
     n_column = len(column_loc)
 
     p_bounds = np.array([0])
-    p_bounds = np.append(p_bounds, column_loc[0][:-1, 0] + np.diff(column_loc[0][:, 0]) * 0.5)
+    p_bounds = np.append(
+        p_bounds, column_loc[0][:-1, 0] + np.diff(column_loc[0][:, 0]) * 0.5
+    )
     p_bounds = np.append(p_bounds, column_loc[0][-1, 0])
 
     vis_data = []
     column_group_length = []
     column_n_sites = []
     for i in range(n_column):
         sites_column = sites_loc[i][:, 0]
         # print(sites_column)
         if sites_line_count is None:
             line_counts = np.ones(len(sites_column))
         else:
             line_counts = np.ravel(sites_line_count)
         group_column = group_mat[:, i]
-        group_id, start_loc, end_loc, gc_length = get_column_grouped_info(group_column, p_bounds)
+        group_id, start_loc, end_loc, gc_length = get_column_grouped_info(
+            group_column, p_bounds
+        )
         n_sites_group = []
         for j in range(len(group_id)):
-            valid_sites_lines = np.logical_and(sites_column < end_loc[j], sites_column >= start_loc[j])
+            valid_sites_lines = np.logical_and(
+                sites_column < end_loc[j], sites_column >= start_loc[j]
+            )
             n_sites_group.append(np.sum(valid_sites_lines * line_counts))
         # print('n_sites_group', n_sites_group)
-        vis_column = {'group_id': group_id,
-                      'start_loc': start_loc / vox_size,
-                      'end_loc': end_loc / vox_size,
-                      'sites': sites_column / vox_size}
+        vis_column = {
+            "group_id": group_id,
+            "start_loc": start_loc / vox_size,
+            "end_loc": end_loc / vox_size,
+            "sites": sites_column / vox_size,
+        }
         column_group_length.append(gc_length)
         column_n_sites.append(np.ravel(n_sites_group))
         vis_data.append(vis_column)
     # print(vis_data)
     n_column = len(vis_data)
     unique_groups = np.unique(group_mat)
     group_length = []
     group_n_sites = []
     for group_ind in unique_groups:
         temp = []
         temp_sites = []
         for i in range(n_column):
-            valid_ind = np.where(vis_data[i]['group_id'] == group_ind)[0]
+            valid_ind = np.where(vis_data[i]["group_id"] == group_ind)[0]
             if len(valid_ind) != 0:
                 valid_length = np.sum(column_group_length[i][valid_ind])
                 valid_sites = np.sum(column_n_sites[i][valid_ind])
                 temp.append(valid_length)
                 temp_sites.append(valid_sites)
         group_length.append(np.sum(temp) / n_column)
         group_n_sites.append(np.sum(temp_sites))
 
     text_loc = []
     for group_ind in unique_groups:
         inds = np.where(group_mat == group_ind)[0]
         low_level = np.min(inds)
         high_level = np.max(inds)
-        text_loc.append((p_bounds[low_level] + 0.7 * (p_bounds[high_level + 1] - p_bounds[low_level])) / vox_size)
+        text_loc.append(
+            (
+                p_bounds[low_level]
+                + 0.7 * (p_bounds[high_level + 1] - p_bounds[low_level])
+            )
+            / vox_size
+        )
     return vis_data, group_length, group_n_sites, text_loc
 
 
 def get_n_sites_in_region(gr_start, gr_end, plot_sites_column):
     n_groups, n_column = gr_start.shape
 
     region_site_num = []
     for i in range(n_groups):
         n_sites = 0
         for j in range(n_column):
             if np.isnan(gr_start[i, j]):
                 continue
-            valid_ind = np.logical_and(plot_sites_column[j] >= gr_start[i, j], plot_sites_column[j] < gr_end[i, j])
+            valid_ind = np.logical_and(
+                plot_sites_column[j] >= gr_start[i, j],
+                plot_sites_column[j] < gr_end[i, j],
+            )
             n_sites += np.sum(valid_ind)
         region_site_num.append(n_sites)
 
     return region_site_num
 
 
 def get_label_name(label_info, region_label):
     label_names = []
     label_acronym = []
     label_color = []
     for i in range(len(region_label)):
         if region_label[i] == 0:
-            label_names.append(' ')
-            label_acronym.append(' ')
+            label_names.append(" ")
+            label_acronym.append(" ")
             label_color.append((128, 128, 128))
         else:
-            da_ind = np.where(np.ravel(label_info['index']) == region_label[i])[0][0]
-            label_names.append(label_info['label'][da_ind])
-            label_acronym.append(label_info['abbrev'][da_ind])
-            label_color.append(label_info['color'][da_ind])
+            da_ind = np.where(np.ravel(label_info["index"]) == region_label[i])[0][0]
+            label_names.append(label_info["label"][da_ind])
+            label_acronym.append(label_info["abbrev"][da_ind])
+            label_color.append(label_info["color"][da_ind])
 
     label_color = np.asarray(label_color)
     return label_names, label_acronym, label_color
 
 
 def get_sites_loc_related_to_base_center(probe_settings, probe_length_without_tip_um):
-    probe_type_name = probe_settings['probe_type_name']
-    probe_thickness_um = probe_settings['probe_thickness']
-    per_max_sites = probe_settings['per_max_sites']
-    sites_distance_um = probe_settings['sites_distance']
-    x_bias_um = probe_settings['x_bias']
-    y_bias_um = probe_settings['y_bias']
+    probe_type_name = probe_settings["probe_type_name"]
+    probe_thickness_um = probe_settings["probe_thickness"]
+    per_max_sites = probe_settings["per_max_sites"]
+    sites_distance_um = probe_settings["sites_distance"]
+    x_bias_um = probe_settings["x_bias"]
+    y_bias_um = probe_settings["y_bias"]
 
-    if probe_type_name == 'Tetrode':
+    if probe_type_name == "Tetrode":
         sites_loc = [np.array([[0, 0, 0]]) for _ in range(4)]
     else:
         sites_loc = []  # inverse r-vals, u-vals, n-vals
         n_val = 0.5 * probe_thickness_um
         for i in range(len(x_bias_um)):
-            possible_n_sites = int((probe_length_without_tip_um - y_bias_um[i]) / sites_distance_um[i])
+            possible_n_sites = int(
+                (probe_length_without_tip_um - y_bias_um[i]) / sites_distance_um[i]
+            )
             if possible_n_sites <= per_max_sites[i]:
-                r_vals = np.arange(possible_n_sites) * sites_distance_um[i] + y_bias_um[i]
+                r_vals = (
+                    np.arange(possible_n_sites) * sites_distance_um[i] + y_bias_um[i]
+                )
             else:
-                r_vals = np.arange(per_max_sites[i]) * sites_distance_um[i] + y_bias_um[i]
+                r_vals = (
+                    np.arange(per_max_sites[i]) * sites_distance_um[i] + y_bias_um[i]
+                )
             num_sites = len(r_vals)
             u_vals = np.repeat(x_bias_um[i], num_sites)
             n_vals = np.repeat(n_val, num_sites)
             temp = np.stack([r_vals, u_vals, n_vals], axis=1)
             sites_loc.append(temp)
     return sites_loc
 
@@ -492,65 +526,81 @@
     return sites_loc_line, sites_count
 
 
 def get_pnt_from_loc(sct, loc, n_vec, u_vec, r_vec, bregma, vox_size):
     pnt = []
     pnt_vox = []
     for i in range(len(loc)):
-        temp = [sct * vox_size + r_vec * loc[i][ind, 0] + u_vec * loc[i][ind, 1] + n_vec * loc[i][ind, 2]
-                for ind in range(len(loc[i]))]
+        temp = [
+            sct * vox_size
+            + r_vec * loc[i][ind, 0]
+            + u_vec * loc[i][ind, 1]
+            + n_vec * loc[i][ind, 2]
+            for ind in range(len(loc[i]))
+        ]
         temp = np.asarray(temp)
         temp = temp / vox_size
         pnt.append(temp)
         vox_temp = temp + bregma
         vox_temp = vox_temp.astype(int)
         pnt_vox.append(vox_temp)
 
     return pnt, pnt_vox
 
 
-def get_column_loc(sites_loc_to_base, probe_length_without_tip_um, vxsize_um, verbose=False):
+def get_column_loc(
+    sites_loc_to_base, probe_length_without_tip_um, vxsize_um, verbose=False
+):
     sites_r_vals = []
     for i in range(len(sites_loc_to_base)):
         sites_r_vals.append(sites_loc_to_base[i][:, 0])
     sites_r_vals = np.concatenate(sites_r_vals)
     uni_sites_r_vals = np.unique(sites_r_vals)
 
     if len(uni_sites_r_vals) > 1:
         if uni_sites_r_vals[0] == 0:
             vis_r_vals = np.arange(uni_sites_r_vals[0], uni_sites_r_vals[1], vxsize_um)
             for i in range(1, len(uni_sites_r_vals) - 1):
-                vis_r_vals = np.append(vis_r_vals, np.arange(uni_sites_r_vals[i], uni_sites_r_vals[i + 1], vxsize_um))
+                vis_r_vals = np.append(
+                    vis_r_vals,
+                    np.arange(uni_sites_r_vals[i], uni_sites_r_vals[i + 1], vxsize_um),
+                )
         else:
             vis_r_vals = np.arange(0, uni_sites_r_vals[0], vxsize_um)
             for i in range(len(uni_sites_r_vals) - 1):
-                vis_r_vals = np.append(vis_r_vals, np.arange(uni_sites_r_vals[i], uni_sites_r_vals[i + 1], vxsize_um))
+                vis_r_vals = np.append(
+                    vis_r_vals,
+                    np.arange(uni_sites_r_vals[i], uni_sites_r_vals[i + 1], vxsize_um),
+                )
 
         if uni_sites_r_vals[-1] != probe_length_without_tip_um:
-            vis_r_vals = np.append(vis_r_vals, np.arange(uni_sites_r_vals[-1], probe_length_without_tip_um, vxsize_um))
+            vis_r_vals = np.append(
+                vis_r_vals,
+                np.arange(uni_sites_r_vals[-1], probe_length_without_tip_um, vxsize_um),
+            )
         vis_r_vals = np.append(vis_r_vals, probe_length_without_tip_um)
     else:
         vis_r_vals = np.arange(0, probe_length_without_tip_um, vxsize_um)
 
     column_loc = []
     for i in range(len(sites_loc_to_base)):
         temp = np.zeros((len(vis_r_vals), 3))
         temp[:, 0] = vis_r_vals
         temp[:, 1] = sites_loc_to_base[i][0, 1]
         temp[:, 2] = sites_loc_to_base[i][0, 2]
         column_loc.append(temp)
 
     if verbose:
-        print('uni_sites_r_vals')
+        print("uni_sites_r_vals")
         print(uni_sites_r_vals)
 
-        print('vis_r_vals')
+        print("vis_r_vals")
         print(vis_r_vals)
 
-        print('column_loc')
+        print("column_loc")
         print(column_loc)
 
     return column_loc
 
 
 def get_loc_related_to_start(loc_to_base, probe_length_without_tip_um):
     loc_to_start = []  # inverse r-vals, u-vals, n-vals
@@ -560,29 +610,42 @@
         loc_to_start.append(temp_loc)
     return loc_to_start
 
 
 def get_fine_label_matrix(column_vox, label_data, verbose=False):
     fine_label_mat = []
     for i in range(len(column_vox)):
-        fine_label_mat.append(label_data[column_vox[i][:, 0], column_vox[i][:, 1], column_vox[i][:, 2]])
+        fine_label_mat.append(
+            label_data[column_vox[i][:, 0], column_vox[i][:, 1], column_vox[i][:, 2]]
+        )
     fine_label_mat = np.asarray(fine_label_mat).T
 
     if verbose:
         # print out fine label matrix
         indexs = np.arange(0, len(fine_label_mat), 20)
         for i in range(len(indexs) - 1):
-            print(fine_label_mat[indexs[i]:indexs[i + 1]])
-        print(fine_label_mat[indexs[-1]:len(fine_label_mat)])
+            print(fine_label_mat[indexs[i] : indexs[i + 1]])
+        print(fine_label_mat[indexs[-1] : len(fine_label_mat)])
 
     return fine_label_mat
 
 
-def calculate_probe_info(data_list, pieces_names, label_data, label_info, vxsize_um, probe_settings,
-                         merge_sites, bregma, site_face, n_hat, pre_plan):
+def calculate_probe_info(
+    data_list,
+    pieces_names,
+    label_data,
+    label_info,
+    vxsize_um,
+    probe_settings,
+    merge_sites,
+    bregma,
+    site_face,
+    n_hat,
+    pre_plan,
+):
     """
 
     :param data: 3d coordinates for all the points
     :param label_data: original brain region segmentation
     :param label_info:
     :param vxsize_um:
     :param tip_length:
@@ -591,133 +654,178 @@
     :return:
     """
 
     data_dict = None
     data = data_list[0]
     for i in range(1, len(data_list)):
         data = np.vstack([data, data_list[i]])
-    print('data', data)
+    # print('data', data)
 
     # start_pnt and end_pnt are coordinates related to the given Bregma
-    probe_type_name = probe_settings['probe_type_name']
-    probe_max_length_um = probe_settings['probe_length']
-    tip_length_um = probe_settings['tip_length']
+    probe_type_name = probe_settings["probe_type_name"]
+    probe_max_length_um = probe_settings["probe_length"]
+    tip_length_um = probe_settings["tip_length"]
 
     # get direction and probe center start and end (pc - probe center)
     pc_start_pnt, pc_end_pnt, avg, direction = line_fit(data)
     direction = pc_end_pnt - pc_start_pnt
     direction = direction / np.linalg.norm(direction)
     pc_start_vox = pc_start_pnt + bregma
     pc_end_vox = pc_end_pnt + bregma
 
-    print('direction', direction)
+    # print('direction', direction)
 
     # get angels
     ap_angle, ml_angle = get_angles(direction)
-    print('ap_angle', ap_angle)
-    print(ml_angle)
+    # print('ap_angle', ap_angle)
+    # print(ml_angle)
 
-    print('check-start_pnt', pc_start_pnt)
-    print(pc_start_vox)
+    # print('check-start_pnt', pc_start_pnt)
+    # # print(pc_start_vox)
     # correct probe center start point
-    pc_sp, error_index = correct_start_pnt(label_data, pc_start_pnt, pc_start_vox, direction, bregma, verbose=True)
+    pc_sp, error_index = correct_start_pnt(
+        label_data, pc_start_pnt, pc_start_vox, direction, bregma, verbose=True
+    )
     if error_index != 0:
         return data_dict, 15
 
     pc_ep, probe_length_with_tip_um, probe_length_without_tip_um = correct_end_point(
-        pc_sp, pc_end_pnt, direction, vxsize_um, tip_length_um, probe_max_length_um, verbose=True)
+        pc_sp,
+        pc_end_pnt,
+        direction,
+        vxsize_um,
+        tip_length_um,
+        probe_max_length_um,
+        verbose=True,
+    )
 
     pv_sp = pc_sp + bregma
     pv_sp = pv_sp.astype(int)
     pv_ep = pc_ep + bregma
     pv_ep = pv_ep.astype(int)
 
     enter_coords = pc_sp * vxsize_um
     end_coords = pc_ep * vxsize_um
 
-    print('')
+    # print('')
 
     dv = (pc_sp[2] - pc_ep[2]) * vxsize_um
     ap_tilt, ml_tilt = get_tilt_info(pc_sp, pc_ep)
 
     if pre_plan:
         r_hat = direction.copy()
         u_hat = np.cross(n_hat, r_hat)
 
         n_vec, u_vec = get_vector_according_to_site_face(n_hat, u_hat, site_face)
     else:
-        r_hat, u_vec, n_vec = calculate_vector_according_to_site_face(direction, site_face)
+        r_hat, u_vec, n_vec = calculate_vector_according_to_site_face(
+            direction, site_face
+        )
 
     # sites location, list of  [(n_sites, 3),...], in um
-    sites_loc_to_base_temp = get_sites_loc_related_to_base_center(probe_settings, probe_length_without_tip_um)
+    sites_loc_to_base_temp = get_sites_loc_related_to_base_center(
+        probe_settings, probe_length_without_tip_um
+    )
     # print('sites_loc_to_base')
     # print(sites_loc_to_base)
 
-    if merge_sites or probe_type_name == 'Tetrode':
-        sites_loc_to_base, sites_line_count = merge_sites_into_line(sites_loc_to_base_temp)
+    if merge_sites or probe_type_name == "Tetrode":
+        sites_loc_to_base, sites_line_count = merge_sites_into_line(
+            sites_loc_to_base_temp
+        )
     else:
         sites_loc_to_base = sites_loc_to_base_temp.copy()
         sites_line_count = None
 
     # column location list of [(n_locs, 3), ...], in um
-    column_loc_to_base = get_column_loc(sites_loc_to_base, probe_length_without_tip_um, vxsize_um, verbose=False)
+    column_loc_to_base = get_column_loc(
+        sites_loc_to_base, probe_length_without_tip_um, vxsize_um, verbose=False
+    )
 
     # column location relative to the start, from bottom to top, in um
-    column_loc = get_loc_related_to_start(column_loc_to_base, probe_length_without_tip_um)
+    column_loc = get_loc_related_to_start(
+        column_loc_to_base, probe_length_without_tip_um
+    )
     # print('column_loc')
     # print(column_loc)
 
     # column points (related to bregma) and column vox
-    column_pnt, column_vox = get_pnt_from_loc(pc_sp, column_loc, n_vec, u_vec, r_hat, bregma, vxsize_um)
+    column_pnt, column_vox = get_pnt_from_loc(
+        pc_sp, column_loc, n_vec, u_vec, r_hat, bregma, vxsize_um
+    )
     # print('column_pnt')
     # print(column_pnt)
     # print('column_vox')
     # print(column_vox)
 
     fine_label_mat = get_fine_label_matrix(column_vox, label_data, verbose=False)
     group_mat, group_id_label = group_labels(fine_label_mat)
     label_names, label_acronym, label_color = get_label_name(label_info, group_id_label)
 
-    if probe_type_name != 'Tetrode':
+    if probe_type_name != "Tetrode":
         # sites loc related to the start, in um
-        sites_loc = get_loc_related_to_start(sites_loc_to_base, probe_length_without_tip_um)
+        sites_loc = get_loc_related_to_start(
+            sites_loc_to_base, probe_length_without_tip_um
+        )
         # print(sites_loc)
 
-        sites_pnt, sites_vox = get_pnt_from_loc(pc_sp, sites_loc, n_vec, u_vec, r_hat, bregma, vxsize_um)
+        sites_pnt, sites_vox = get_pnt_from_loc(
+            pc_sp, sites_loc, n_vec, u_vec, r_hat, bregma, vxsize_um
+        )
         # print(sites_pnt)
         # print('sites_vox')
         # print(sites_vox)
     else:
         sites_pnt = [np.array([pc_ep])]
         sites_vox_temp = sites_pnt[0] + bregma
         sites_vox = [sites_vox_temp.astype(int)]
 
-
     sites_label = []
     for i in range(len(sites_vox)):
-        sites_label.append(label_data[sites_vox[i][:, 0], sites_vox[i][:, 1], sites_vox[i][:, 2]])
+        sites_label.append(
+            label_data[sites_vox[i][:, 0], sites_vox[i][:, 1], sites_vox[i][:, 2]]
+        )
 
     # print('sites_label')
     # print(sites_label)
 
     vis_data, region_length, region_site_num, region_text_loc = get_vis_data(
-        group_mat, column_loc_to_base, sites_loc_to_base, sites_line_count, vxsize_um)
+        group_mat, column_loc_to_base, sites_loc_to_base, sites_line_count, vxsize_um
+    )
 
-    data_dict = {'object_name': 'probe', 'probe_type_name': probe_type_name,
-                 'data': data_list, 'pieces_names': pieces_names, 'ap_tilt': ap_tilt, 'ml_tilt': ml_tilt,
-                 'insertion_coords_3d': pc_sp, 'terminus_coords_3d': pc_ep,
-                 'direction': direction, 'probe_length': probe_length_with_tip_um, 'dv': dv,
-                 'ap_angle': ap_angle, 'ml_angle': ml_angle,
-                 'insertion_coords': enter_coords, 'insertion_vox': pv_sp,
-                 'terminus_coords': end_coords, 'terminus_vox': pv_ep,
-                 'sites_label': sites_label, 'sites_loc_b': sites_pnt, 'sites_vox': sites_vox,
-                 'region_label': group_id_label,
-                 'region_length': region_length, 'region_sites': region_site_num, 'text_loc': region_text_loc,
-                 'label_name': label_names, 'label_acronym': label_acronym, 'label_color': label_color,
-                 'vis_data': vis_data}
+    data_dict = {
+        "object_name": "probe",
+        "probe_type_name": probe_type_name,
+        "data": data_list,
+        "pieces_names": pieces_names,
+        "ap_tilt": ap_tilt,
+        "ml_tilt": ml_tilt,
+        "insertion_coords_3d": pc_sp,
+        "terminus_coords_3d": pc_ep,
+        "direction": direction,
+        "probe_length": probe_length_with_tip_um,
+        "dv": dv,
+        "ap_angle": ap_angle,
+        "ml_angle": ml_angle,
+        "insertion_coords": enter_coords,
+        "insertion_vox": pv_sp,
+        "terminus_coords": end_coords,
+        "terminus_vox": pv_ep,
+        "sites_label": sites_label,
+        "sites_loc_b": sites_pnt,
+        "sites_vox": sites_vox,
+        "region_label": group_id_label,
+        "region_length": region_length,
+        "region_sites": region_site_num,
+        "text_loc": region_text_loc,
+        "label_name": label_names,
+        "label_acronym": label_acronym,
+        "label_color": label_color,
+        "vis_data": vis_data,
+    }
     return data_dict, error_index
 
 
 def get_pre_multi_shank_vis_base(x_vals, y_vals):
     x_vals = np.ravel(x_vals)
     y_vals = np.ravel(y_vals)
     valid_ind = np.where(y_vals == 0)[0]
@@ -744,29 +852,29 @@
     # for pre-plan - 2d plan
     if site_face == 0:
         # site face out, facing to you
         n_vec = n_hat.copy()
         u_vec = u_hat.copy()
     elif site_face == 1:
         # site face in, facing away from you
-        n_vec = - n_hat
-        u_vec = - u_hat
+        n_vec = -n_hat
+        u_vec = -u_hat
     elif site_face == 2:
         # site face left, facing to you left-hand side
-        n_vec = - u_hat
+        n_vec = -u_hat
         u_vec = n_hat.copy()
     elif site_face == 3:
         # site face right, facing to you right-hand side
         n_vec = u_hat.copy()
-        u_vec = - n_hat
+        u_vec = -n_hat
     else:
-        raise ValueError('no such site face, stupid!!!!!!')
+        raise ValueError("no such site face, stupid!!!!!!")
 
-    print('n_vec', n_vec)
-    print('u_vec', u_vec)
+    # print('n_vec', n_vec)
+    # print('u_vec', u_vec)
 
     return n_vec, u_vec
 
 
 def calculate_vector_according_to_site_face(direction, site_face):
     # for after surgery
     r_hat = direction.copy()
@@ -782,15 +890,15 @@
             u_hat = np.cross(n_hat, r_hat)
         elif site_face == 3:
             n_hat = np.array([1, 0, 0])
             u_hat = np.cross(n_hat, r_hat)
         else:
             n_hat = None
             u_hat = None
-            print('Site face can only be 0-Up, 1-Down, 2-Left, 3-Right.')
+            print("Site face can only be 0-Up, 1-Down, 2-Left, 3-Right.")
     else:
         if site_face == 0:
             t_hat = np.array([-r_hat[1], r_hat[0], 0])
             u_hat = t_hat / np.linalg.norm(t_hat)
             n_hat = np.cross(r_hat, u_hat)
         elif site_face == 1:
             t_hat = np.array([r_hat[1], r_hat[0], 0])
@@ -803,23 +911,24 @@
         elif site_face == 3:
             t_hat = np.array([r_hat[1], r_hat[0], 0])
             n_hat = t_hat / np.linalg.norm(t_hat)
             u_hat = np.cross(n_hat, r_hat)
         else:
             n_hat = None
             u_hat = None
-            print('Site face can only be 0-Up, 1-Down, 2-Left, 3-Right.')
+            print("Site face can only be 0-Up, 1-Down, 2-Left, 3-Right.")
         # print('t_hat', t_hat)
         # print(n_hat)
         # print(u_hat)
     return r_hat, u_hat, n_hat
 
 
-def get_center_lines(pnts, r_hat, n_hat, u_hat, x_vals, y_vals, length, site_face, vox_size):
-
+def get_center_lines(
+    pnts, r_hat, n_hat, u_hat, x_vals, y_vals, length, site_face, vox_size
+):
     n_vec, u_vec = get_vector_according_to_site_face(n_hat, u_hat, site_face)
 
     # print(x_vals)
     # print(y_vals)
 
     line_data = []
     for i in range(len(x_vals)):
@@ -828,39 +937,33 @@
         temp = [s_val, s_val + r_hat * length * vox_size]
         # print(temp)
         line_data.append(pnts[0] + np.asarray(temp) / vox_size)
 
     return line_data
 
 
-
-
-
-
-
-
 def get_pre_ms_vis_base(multi_shanks, site_face, atlas_display):
     if multi_shanks is None:
         base_loc = np.array([0])
     else:
-        if atlas_display == 'sagittal':
+        if atlas_display == "sagittal":
             if site_face not in [0, 1]:
                 base_loc = np.ravel(multi_shanks)
             else:
                 base_loc = np.array([0])
         else:
             if site_face in [0, 1]:
                 base_loc = np.ravel(multi_shanks)
             else:
                 base_loc = np.array([0])
     return base_loc
 
 
 def get_pre_mp_vis_base(base_loc, atlas_display):
-    if atlas_display == 'sagittal':
+    if atlas_display == "sagittal":
         valid_ind = np.where(base_loc[:, 1] == 0)[0]
         if len(valid_ind) == 0:
             vis_base = np.array([0])
         else:
             vis_base = base_loc[valid_ind, 1]
     else:
         valid_ind = np.where(base_loc[:, 0] == 0)[0]
@@ -893,51 +996,51 @@
 
         self.set_np1()
 
     def extend_exist_probes(self, prb):
         pass
 
     def get_exist_probes(self):
-        self.exist_probes = {'NP1.0': None, 'NP2.0': None, 'Tetrode': None}
+        self.exist_probes = {"NP1.0": None, "NP2.0": None, "Tetrode": None}
 
     def set_np2(self):
         self.probe_type = 1
-        self.probe_type_name = 'NP2.0'
+        self.probe_type_name = "NP2.0"
         self.probe_thickness = 24
         self.probe_length = 10000
         self.tip_length = 175
         self.site_width = 16
         self.site_height = 15
         self.x_bias = [-8, 16]
         self.per_max_sites = [480, 480]
         self.sites_distance = [15, 15]
         self.y_bias = [7.5, 7.5]
         self.site_number_in_banks = (384, 384, 192)
         self.multi_shanks = [-375, -125, 125, 375]
-        self.faces = 'Front'
+        self.faces = "Front"
 
     def set_np1(self):
         self.probe_type = 0
-        self.probe_type_name = 'NP1.0'
+        self.probe_type_name = "NP1.0"
         self.probe_thickness = 24
         self.probe_length = 10000
         self.tip_length = 175
         self.site_width = 16
         self.site_height = 20
         self.x_bias = [-16, -8, 8, 16]
         self.per_max_sites = [240, 240, 240, 240]
         self.sites_distance = [40, 40, 40, 40]
         self.y_bias = [30, 10, 30, 10]
         self.site_number_in_banks = (384, 384, 192)
         self.multi_shanks = None
-        self.faces = 'Front'
+        self.faces = "Front"
 
     def set_tetrode(self):
         self.probe_type = 3
-        self.probe_type_name = 'Tetrode'
+        self.probe_type_name = "Tetrode"
         self.probe_thickness = 0
         self.probe_length = None
         self.tip_length = 0
         self.site_width = None
         self.site_height = None
         self.x_bias = 0
         self.per_max_sites = 4
@@ -945,53 +1048,54 @@
         self.y_bias = 0
         self.site_number_in_banks = None
         self.multi_shanks = None
         self.faces = None
 
     def set_linear_silicon(self, pss):
         self.probe_type = 2
-        self.probe_type_name = 'Linear-Silicon'
-        self.probe_length = pss['probe_length']
-        self.probe_thickness = pss['probe_thickness']
-        self.tip_length = pss['tip_length']
-        self.site_width = pss['site_width']
-        self.site_height = pss['site_height']
-
-        self.per_max_sites = pss['per_max_sites']
-        self.sites_distance = pss['sites_distance']
-        self.x_bias = pss['x_bias']
-        self.y_bias = pss['y_bias']
+        self.probe_type_name = "Linear-Silicon"
+        self.probe_length = pss["probe_length"]
+        self.probe_thickness = pss["probe_thickness"]
+        self.tip_length = pss["tip_length"]
+        self.site_width = pss["site_width"]
+        self.site_height = pss["site_height"]
+
+        self.per_max_sites = pss["per_max_sites"]
+        self.sites_distance = pss["sites_distance"]
+        self.x_bias = pss["x_bias"]
+        self.y_bias = pss["y_bias"]
         self.site_number_in_banks = None
         self.multi_shanks = None
-        self.faces = 'Front'
-
+        self.faces = "Front"
 
     def get_settings(self):
-        data = {'probe_type': self.probe_type,
-                'probe_type_name': self.probe_type_name,
-                'probe_thickness': self.probe_thickness,
-                'probe_length': self.probe_length,
-                'tip_length': self.tip_length,
-                'site_height': self.site_height,
-                'site_width': self.site_width,
-                'per_max_sites': self.per_max_sites,
-                'sites_distance': self.sites_distance,
-                'x_bias': self.x_bias,
-                'y_bias': self.y_bias,
-                'site_number_in_banks': self.site_number_in_banks,
-                'multi_shanks': self.multi_shanks}
+        data = {
+            "probe_type": self.probe_type,
+            "probe_type_name": self.probe_type_name,
+            "probe_thickness": self.probe_thickness,
+            "probe_length": self.probe_length,
+            "tip_length": self.tip_length,
+            "site_height": self.site_height,
+            "site_width": self.site_width,
+            "per_max_sites": self.per_max_sites,
+            "sites_distance": self.sites_distance,
+            "x_bias": self.x_bias,
+            "y_bias": self.y_bias,
+            "site_number_in_banks": self.site_number_in_banks,
+            "multi_shanks": self.multi_shanks,
+        }
         return data
 
     def probe_faces_changed(self, face_direction):
         self.faces = face_direction
 
     def get_multi_shank_3d_base(self):
         if self.multi_shanks is None:
             return
-        if self.faces in ['Front', 'Back']:
+        if self.faces in ["Front", "Back"]:
             points3 = np.zeros((len(self.multi_shanks), 3))
             points3[:, 1] = self.multi_shanks
         else:
             points3 = np.zeros((len(self.multi_shanks), 3))
             points3[:, 2] = self.multi_shanks
         return points3
 
@@ -999,17 +1103,17 @@
 class MultiProbes(object):
     def __init__(self):
         self.x_vals = None
         self.y_vals = None
         self.faces = None
 
     def set_multi_probes(self, multi_settings):
-        self.x_vals = multi_settings['x_vals']
-        self.y_vals = multi_settings['y_vals']
-        self.faces = multi_settings['faces']
+        self.x_vals = multi_settings["x_vals"]
+        self.y_vals = multi_settings["y_vals"]
+        self.faces = multi_settings["faces"]
 
     def get_multi_settings(self):
         if self.x_vals is None:
             multi_settings = None
         else:
             if not isinstance(self.x_vals, list):
                 x_vals = self.x_vals.tolist()
@@ -1021,27 +1125,25 @@
             else:
                 y_vals = self.y_vals.copy()
 
             if not isinstance(self.faces, list):
                 faces = self.faces.tolist()
             else:
                 faces = self.faces.copy()
-            multi_settings = {'x_vals': x_vals,
-                              'y_vals': y_vals,
-                              'faces': faces}
+            multi_settings = {"x_vals": x_vals, "y_vals": y_vals, "faces": faces}
         return multi_settings
 
     def check_multi_settings(self):
         x_unique = np.unique(self.x_vals)
 
         for x_val in x_unique:
             v_ind = np.where(np.ravel(self.x_vals) == x_val)[0]
             if len(v_ind) > 1:
                 if len(np.unique(np.ravel(self.y_vals)[v_ind])) != len(v_ind):
-                    msg = 'There are at least 2 probes located at the same location.'
+                    msg = "There are at least 2 probes located at the same location."
                     return msg
 
         return
 
     # def get_base_loc_3d(self, multi_shank):
     #     if multi_shank is None:
     #         points3 = np.zeros((len(self.x_vals), 3))
@@ -1083,10 +1185,7 @@
     #             for i in range(len(self.x_vals)):
     #                 p2 = np.zeros((n_shank, 2))
     #                 p2[:, 0] = self.x_vals[i]
     #                 p2[:, 1] = multi_shank + self.y_vals[i]
     #                 points2.append(p2)
     #         points2 = np.concatenate(points2)
     #     return points2
-
-
-
```

### Comparing `herbs-0.2.2/herbs/qss/color_combo.qss` & `herbs-0.2.3/herbs/qss/color_combo.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/label_tree.qss` & `herbs-0.2.3/herbs/qss/label_tree.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/main_window.qss` & `herbs-0.2.3/herbs/qss/main_window.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/menu_bar.qss` & `herbs-0.2.3/herbs/qss/menu_bar.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/multi_handle_slider.qss` & `herbs-0.2.3/herbs/qss/multi_handle_slider.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/obj_ctrl_bottom_button.qss` & `herbs-0.2.3/herbs/qss/obj_ctrl_bottom_button.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/page_control.qss` & `herbs-0.2.3/herbs/qss/page_control.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/side_bar.qss` & `herbs-0.2.3/herbs/qss/side_bar.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/spinbox.qss` & `herbs-0.2.3/herbs/qss/spinbox.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/tabs.qss` & `herbs-0.2.3/herbs/qss/tabs.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/qss/tool_bar.qss` & `herbs-0.2.3/herbs/qss/tool_bar.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/slice_stacks.py` & `herbs-0.2.3/herbs/slice_stacks.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/toolbox.py` & `herbs-0.2.3/herbs/toolbox.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/triangulation_points.py` & `herbs-0.2.3/herbs/triangulation_points.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/uuuuuu.py` & `herbs-0.2.3/herbs/uuuuuu.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,70 +7,71 @@
 import colorsys
 import pyqtgraph as pg
 import pyqtgraph.opengl as gl
 import scipy.ndimage as ndi
 from scipy.interpolate import interp1d, splprep, splev
 
 
-
 def read_qss_file(qss_file_name):
-    with open(qss_file_name, 'r', encoding='UTF-8') as file:
+    with open(qss_file_name, "r", encoding="UTF-8") as file:
         return file.read()
 
 
 def check_loading_pickle_file(file_path):
     layer_dict, msg = None, None
     try:
-        infile = open(file_path, 'rb')
+        infile = open(file_path, "rb")
         layer_dict = pickle.load(infile)
         infile.close()
     except OSError:
-        msg = 'OSError: possible reason - disk full, please contact maintainers.'
+        msg = "OSError: possible reason - disk full, please contact maintainers."
         return msg
     except (pickle.PickleError, pickle.UnpicklingError):
-        msg = 'Pickling error, please check your file or contact maintainers.'
+        msg = "Pickling error, please check your file or contact maintainers."
         return msg
     except EOFError:
-        msg = 'EOFError: possible reason - suspecting loading a broken file, please contact maintainers.'
+        msg = "EOFError: possible reason - suspecting loading a broken file, please contact maintainers."
         return msg
 
     return layer_dict, msg
 
 
 def read_excel_file(file_path):
     msg = None
     file_name, file_extension = os.path.splitext(file_path)
-    if file_extension == '.csv':
+    if file_extension == ".csv":
         df = pd.read_csv(file_path)
-    elif file_extension == '.xlsx':
+    elif file_extension == ".xlsx":
         df = pd.read_excel(file_path)
     else:
         df = None
-        msg = 'Only CSV file and Excel file works.'
+        msg = "Only CSV file and Excel file works."
     return df, msg
 
 
 def read_label(file):
     lines = []
     for line in file:
         lines.append(line)
-    
+
     n_lines = len(lines)
-    label_index = np.zeros(n_lines - 14, 'i')
+    label_index = np.zeros(n_lines - 14, "i")
     label_index[:] = np.nan
-    label_colors = np.zeros((n_lines - 14, 3), 'i')
+    label_colors = np.zeros((n_lines - 14, 3), "i")
     label_colors[:] = np.nan
     label_names = []
     for i in range(n_lines - 14):
         split_lines = lines[i + 14].split()
         label_index[i] = int(split_lines[0])
-        label_colors[i] = np.array([split_lines[1], split_lines[2], split_lines[3]]).astype(int)
+        label_colors[i] = np.array(
+            [split_lines[1], split_lines[2], split_lines[3]]
+        ).astype(int)
         split_lines2 = lines[i + 14].split('"')
         label_names.append(split_lines2[1])
-    
+
     return label_index, label_names, label_colors
 
 
 def rotation_x(theta):
     ct = np.cos(theta)
     st = np.sin(theta)
     rx = np.array([[1, 0, 0], [0, ct, -st], [0, st, ct]])
@@ -110,22 +111,22 @@
     label_names = []
     label_acronym = []
     label_color = []
     region_count = []
     for i in range(len(unique_label)):
         # print(unique_label[i])
         if unique_label[i] == 0:
-            label_names.append(' ')
-            label_acronym.append(' ')
+            label_names.append(" ")
+            label_acronym.append(" ")
             label_color.append((128, 128, 128))
         else:
-            da_ind = np.where(label_info['index'] == unique_label[i])[0][0]
-            label_names.append(label_info['label'][da_ind])
-            label_acronym.append(label_info['abbrev'][da_ind])
-            label_color.append(label_info['color'][da_ind])
+            da_ind = np.where(label_info["index"] == unique_label[i])[0][0]
+            label_names.append(label_info["label"][da_ind])
+            label_acronym.append(label_info["abbrev"][da_ind])
+            label_color.append(label_info["color"][da_ind])
 
         region_count.append(len(np.where(np.ravel(region_label) == unique_label[i])[0]))
 
     return region_count, label_names, label_acronym, label_color, unique_label
 
 
 def calculate_virus_info(data_list, pieces_names, label_data, label_info, bregma):
@@ -142,54 +143,94 @@
 
     region_label = get_region_label(data, label_data, bregma)
     unique_region = np.sort(np.unique(region_label))
     region_volume = []
     for c_region in unique_region:
         region_volume.append(len(np.where(label_data == c_region)[0]))
 
-    print(region_volume)
-    region_count, label_names, label_acronym, label_color, unique_label = get_region_label_info(region_label, label_info)
-    print(region_count)
-
-    res_dict = {'object_name': 'virus', 'data': data_list, 'pieces_names': pieces_names,
-                'label_id': unique_label, 'label_name': label_names, 'label_acronym': label_acronym,
-                'label_color': label_color, 'region_volume': region_volume, 'virus_volume': region_count}
+    # print(region_volume)
+    (
+        region_count,
+        label_names,
+        label_acronym,
+        label_color,
+        unique_label,
+    ) = get_region_label_info(region_label, label_info)
+    # print(region_count)
+
+    res_dict = {
+        "object_name": "virus",
+        "data": data_list,
+        "pieces_names": pieces_names,
+        "label_id": unique_label,
+        "label_name": label_names,
+        "label_acronym": label_acronym,
+        "label_color": label_color,
+        "region_volume": region_volume,
+        "virus_volume": region_count,
+    }
 
     return res_dict
 
 
 def calculate_cells_info(data_list, pieces_names, label_data, label_info, bregma):
     data = data_list[0]
     for i in range(1, len(data_list)):
         data = np.vstack([data, data_list[i]])
 
     region_label = get_region_label(data, label_data, bregma)
-    region_count, label_names, label_acronym, label_color, unique_label = get_region_label_info(region_label, label_info)
-
-    res_dict = {'object_name': 'cell', 'pieces_names': pieces_names, 'data': data_list, 'label_name': label_names,
-                'label_acronym': label_acronym, 'label_color': label_color, 'region_count': region_count}
+    (
+        region_count,
+        label_names,
+        label_acronym,
+        label_color,
+        unique_label,
+    ) = get_region_label_info(region_label, label_info)
+
+    res_dict = {
+        "object_name": "cell",
+        "pieces_names": pieces_names,
+        "data": data_list,
+        "label_name": label_names,
+        "label_acronym": label_acronym,
+        "label_color": label_color,
+        "region_count": region_count,
+    }
     return res_dict
 
 
 def calculate_drawing_info(data_list, pieces_names, label_data, label_info, bregma):
     data = data_list[0]
     for i in range(1, len(data_list)):
         data = np.vstack([data, data_list[i]])
-    print(data)
-    if 'area' in pieces_names[0]:
-        plot_mode = 'area'
+    # print(data)
+    if "area" in pieces_names[0]:
+        plot_mode = "area"
     else:
-        plot_mode = 'line'
+        plot_mode = "line"
 
     region_label = get_region_label(data, label_data, bregma)
-    region_count, label_names, label_acronym, label_color, unique_label = get_region_label_info(region_label, label_info)
-
-    res_dict = {'object_name': 'drawing', 'pieces_names': pieces_names, 'data': data_list, 'label_name': label_names,
-                'label_acronym': label_acronym, 'label_color': label_color, 'region_count': region_count,
-                'plot_mode': plot_mode}
+    (
+        region_count,
+        label_names,
+        label_acronym,
+        label_color,
+        unique_label,
+    ) = get_region_label_info(region_label, label_info)
+
+    res_dict = {
+        "object_name": "drawing",
+        "pieces_names": pieces_names,
+        "data": data_list,
+        "label_name": label_names,
+        "label_acronym": label_acronym,
+        "label_color": label_color,
+        "region_count": region_count,
+        "plot_mode": plot_mode,
+    }
     return res_dict
 
 
 def order_contour_pnt(pnt):
     order_ind = []
     x_min = np.min(pnt[:, 0])
     left_ind = np.where(pnt[:, 0] == x_min)[0]
@@ -205,26 +246,25 @@
     data = np.asarray(data)
     res = splprep([data[:, 0], data[:, 1], data[:, 2]], s=2)
     tck = res[0]
     # x_knots, y_knots, z_knots = splev(tck[0], tck)
     u_fine = np.linspace(0, 1, len(data))
     x_fine, y_fine, z_fine = splev(u_fine, tck)
     pnts = np.stack([x_fine, y_fine, z_fine], axis=1)
-    print(pnts)
+    # print(pnts)
     return pnts
 
 
-
 def hex2rgb(hex):
-    if '#' in hex:
-        hex = hex.lstrip('#')
-        rgb_color = [int(hex[i:i + 2], 16) for i in (0, 2, 4)]
+    if "#" in hex:
+        hex = hex.lstrip("#")
+        rgb_color = [int(hex[i : i + 2], 16) for i in (0, 2, 4)]
     else:
         if len(hex) == 6:
-            rgb_color = [int(hex[i:i + 2], 16) for i in (0, 2, 4)]
+            rgb_color = [int(hex[i : i + 2], 16) for i in (0, 2, 4)]
     return rgb_color[0], rgb_color[1], rgb_color[2]
 
 
 # @jit()
 def hsv2rgb(h, s, v):
     # h [0, 1], s, v [0, 1]
     h = h * 360
@@ -256,20 +296,20 @@
     da_image = cv2.merge((r, g, b))
     return da_image
 
 
 def merge_channels_into_single_img(czi_img, channel_colors):
     merged_img = np.zeros((czi_img.shape[0], czi_img.shape[1], 3))
     frac = 1 / len(channel_colors)
-    print(frac)
+    # print(frac)
     for i in range(len(channel_colors)):
         temp_v = czi_img[:, :, i] / 65535
         temp_h = channel_colors[i][0]
         temp_s = channel_colors[i][1]
-        print(temp_h, temp_s)
+        # print(temp_h, temp_s)
         da_img = color_img(temp_h, temp_s, temp_v)
         merged_img = merged_img + frac * da_img
     return merged_img
 
 
 def make_color_lut(channel_color: tuple, bit_level: int):
     r, g, b = colorsys.hsv_to_rgb(channel_color[0], channel_color[1], channel_color[2])
@@ -293,15 +333,17 @@
     return da_color
 
 
 def gamma_line(input, lims, gamma, depth_level):
     inv_gamma = 1.0 / gamma
     y = np.zeros(len(input))
     inds = np.logical_and(input >= lims[0], input <= lims[1])
-    y[inds] = np.power((input[inds] - lims[0]) / (lims[1] - lims[0]), gamma) * depth_level
+    y[inds] = (
+        np.power((input[inds] - lims[0]) / (lims[1] - lims[0]), gamma) * depth_level
+    )
     y[input <= lims[0]] = 0
     y[input >= lims[1]] = depth_level
     return y
 
 
 def crop_landscape(image, dim):
     r = (dim[0] / image.shape[0]) / (dim[0] / dim[1])
@@ -310,40 +352,40 @@
     resized = cv2.resize(image, (nw, int(dim[1])), interpolation=cv2.INTER_AREA)
 
     half_width = int(dim[0]) / 2
     half_shape_width = int(resized.shape[1]) / 2
 
     start_x = half_shape_width - half_width
     end_x = half_width + half_shape_width
-    cropped = resized[0:dim[1], start_x:end_x]
+    cropped = resized[0 : dim[1], start_x:end_x]
 
     return cropped
 
 
 def crop_portrait(image, dim):
     r = dim[1] / image.shape[1] / (dim[1] / dim[0])
     nh = int(image.shape[0] * r)
 
     resized = cv2.resize(image, (int(dim[0]), nh), interpolation=cv2.INTER_AREA)
     half_height = int(dim[1]) / 2
     half_shape_height = int(resized.shape[0]) / 2
 
     start_y = half_shape_height - half_height
     end_y = half_height + half_shape_height
-    cropped = resized[start_y:end_y, 0:dim[0]]
+    cropped = resized[start_y:end_y, 0 : dim[0]]
 
     return cropped
 
 
 def create_other_size(image, file_name, dim, location):
     # 1 => width index, 0 => height index
     if image.shape[0] > image.shape[1]:
-      cropped = crop_portrait(image, dim)
+        cropped = crop_portrait(image, dim)
     else:
-      cropped = crop_landscape(image, dim)
+        cropped = crop_landscape(image, dim)
 
     cv2.imwrite(os.path.join(location, file_name), cropped)
 
 
 def make_hist_data(image_data, max_val):
     hist_data_list = []
     for i in range(image_data.shape[2]):
@@ -351,15 +393,15 @@
             da_bins = max_val
         else:
             da_bins = np.max(image_data[:, :, i])
         hist_y, x = np.histogram(image_data[:, :, i], bins=da_bins)
         y = np.log1p(hist_y)
         y = y / np.max(y) * max_val
         y = np.append(y, 0)
-        sfunc = interp1d(x, y, 'cubic')
+        sfunc = interp1d(x, y, "cubic")
         inter_x = np.linspace(np.min(x), np.max(x), 200)
         inter_y = sfunc(inter_x)
         inter_y[inter_y < 0] = 0
         hist_data_list.append([inter_x, inter_y])
     return hist_data_list
 
 
@@ -373,62 +415,75 @@
     elif point[1] > rect[3] + rect[1]:
         return False
     return True
 
 
 def get_warp_matrix(src_tri_pnts, dst_tri_pnts):
     # Given a pair of triangles, find the affine transform.
-    warp_mat = cv2.getAffineTransform(np.float32(src_tri_pnts), np.float32(dst_tri_pnts))
+    warp_mat = cv2.getAffineTransform(
+        np.float32(src_tri_pnts), np.float32(dst_tri_pnts)
+    )
     return warp_mat
 
 
 def apply_affine_transform(src_img, warp_mat, size_dst):
     # Apply the Affine Transform just found to the src image
-    dst = cv2.warpAffine(src_img.astype(np.float32), warp_mat, (size_dst[0], size_dst[1]), None,
-                         flags=cv2.INTER_LINEAR, borderMode=cv2.BORDER_REFLECT_101)
+    dst = cv2.warpAffine(
+        src_img.astype(np.float32),
+        warp_mat,
+        (size_dst[0], size_dst[1]),
+        None,
+        flags=cv2.INTER_LINEAR,
+        borderMode=cv2.BORDER_REFLECT_101,
+    )
     return dst
 
 
 def warp_triangle(img1, img2, t1, t2, is_rgb=False):
-
     # Find bounding rectangle for each triangle
     r1 = cv2.boundingRect(t1.astype(np.float32))
     r2 = cv2.boundingRect(t2.astype(np.float32))
 
     # Offset points by left top corner of the respective rectangles
     t1_rect = t1 - r1[:2]
     t2_rect = t2 - r2[:2]
     t2_rect_int = t2_rect.astype(int)
 
     # Get mask by filling triangle
     if is_rgb:
         mask = np.zeros((r2[3], r2[2], img1.shape[2]), dtype=np.float32)
-        cv2.fillConvexPoly(mask, np.int32(t2_rect_int), tuple(np.repeat(1.0, img1.shape[2])), 16, 0)
+        cv2.fillConvexPoly(
+            mask, np.int32(t2_rect_int), tuple(np.repeat(1.0, img1.shape[2])), 16, 0
+        )
     else:
         mask = np.zeros((r2[3], r2[2]), dtype=np.float32)
         cv2.fillConvexPoly(mask, np.int32(t2_rect_int), 1, 16, 0)
 
     # Apply warpImage to small rectangular patches
-    img1_rect = img1[r1[1]:r1[1] + r1[3], r1[0]:r1[0] + r1[2]]
+    img1_rect = img1[r1[1] : r1[1] + r1[3], r1[0] : r1[0] + r1[2]]
     # img2Rect = np.zeros((r2[3], r2[2]), dtype = img1Rect.dtype)
 
     size = (r2[2], r2[3])
 
     warp_mat = get_warp_matrix(t1_rect, t2_rect)
     img2_rect = apply_affine_transform(img1_rect, warp_mat, size)
     img2_rect = img2_rect * mask
 
     # Copy triangular region of the rectangular patch to the output image
     yr = (r2[0], r2[0] + r2[2])
     xr = (r2[1], r2[1] + r2[3])
     if is_rgb:
-        img2[xr[0]:xr[1], yr[0]:yr[1]] = img2[xr[0]:xr[1], yr[0]:yr[1]] * (tuple(np.repeat(1.0, img1.shape[2])) - mask)
+        img2[xr[0] : xr[1], yr[0] : yr[1]] = img2[xr[0] : xr[1], yr[0] : yr[1]] * (
+            tuple(np.repeat(1.0, img1.shape[2])) - mask
+        )
     else:
-        img2[xr[0]:xr[1], yr[0]:yr[1]] = img2[xr[0]:xr[1], yr[0]:yr[1]] * (1 - mask)
-    img2[xr[0]:xr[1], yr[0]:yr[1]] = img2[xr[0]:xr[1], yr[0]:yr[1]] + img2_rect
+        img2[xr[0] : xr[1], yr[0] : yr[1]] = img2[xr[0] : xr[1], yr[0] : yr[1]] * (
+            1 - mask
+        )
+    img2[xr[0] : xr[1], yr[0] : yr[1]] = img2[xr[0] : xr[1], yr[0] : yr[1]] + img2_rect
 
 
 def warp_points(pnts, t1, t2):
     # Find bounding rectangle for each triangle
     # r1 = cv2.boundingRect(t1.astype(np.float32))
     # r2 = cv2.boundingRect(t2.astype(np.float32))
     # print(r1)
@@ -443,15 +498,14 @@
 
     warp_mat = get_warp_matrix(t1, t2)
     output = np.dot(warp_mat, da_pnts.T).T
 
     return output
 
 
-
 # calculate delanauy triangle
 def calculateDelaunayTriangles(rect, points):
     # create subdiv
     subdiv = cv2.Subdiv2D(rect)
 
     # Insert points into subdiv
     for p in points:
@@ -468,19 +522,26 @@
         pt.append((t[2], t[3]))
         pt.append((t[4], t[5]))
 
         pt1 = (t[0], t[1])
         pt2 = (t[2], t[3])
         pt3 = (t[4], t[5])
 
-        if rect_contains(rect, pt1) and rect_contains(rect, pt2) and rect_contains(rect, pt3):
+        if (
+            rect_contains(rect, pt1)
+            and rect_contains(rect, pt2)
+            and rect_contains(rect, pt3)
+        ):
             ind = []
             for j in range(0, 3):
                 for k in range(0, len(points)):
-                    if (abs(pt[j][0] - points[k][0]) < 1.0 and abs(pt[j][1] - points[k][1]) < 1.0):
+                    if (
+                        abs(pt[j][0] - points[k][0]) < 1.0
+                        and abs(pt[j][1] - points[k][1]) < 1.0
+                    ):
                         ind.append(k)
             if len(ind) == 3:
                 delaunayTri.append((ind[0], ind[1], ind[2]))
 
         pt = []
 
     return delaunayTri
@@ -491,15 +552,17 @@
     n_triangles = len(triangles)
     tri_vet_inds = []
     for i in range(n_triangles):
         da_triangle = triangles[i]
         p1 = [da_triangle[0], da_triangle[1]]
         p2 = [da_triangle[2], da_triangle[3]]
         p3 = [da_triangle[4], da_triangle[5]]
-        tri_vet_inds.append([subdiv.locate(p1)[2], subdiv.locate(p2)[2], subdiv.locate(p3)[2]])
+        tri_vet_inds.append(
+            [subdiv.locate(p1)[2], subdiv.locate(p2)[2], subdiv.locate(p3)[2]]
+        )
     tri_vet_inds = np.asarray(tri_vet_inds) - 4
     return tri_vet_inds
 
 
 def get_pnts_triangle_ind(tri_vet_inds, tri_data, size, pnts):
     # import cv2
     # import numpy as np
@@ -513,18 +576,22 @@
     loc = np.zeros(n_pnts)
     loc[:] = np.nan
     da_order = []
 
     ct_list = []
     for i in range(len(tri_vet_inds)):
         da_inds = tri_vet_inds[i]
-        da_triangle = np.array([tri_data[da_inds[0]], tri_data[da_inds[1]], tri_data[da_inds[2]]])
+        da_triangle = np.array(
+            [tri_data[da_inds[0]], tri_data[da_inds[1]], tri_data[da_inds[2]]]
+        )
         mask = np.zeros(size, dtype=np.uint8)
         cv2.fillPoly(mask, pts=[da_triangle], color=255)
-        ct, hc = cv2.findContours(image=mask, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE)
+        ct, hc = cv2.findContours(
+            image=mask, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE
+        )
         ct_list.append(ct[0])
 
         # range_y = (np.min(da_triangle[:, 1]), np.max(da_triangle[:, 1]))
         # range_x = (np.min(da_triangle[:, 0]), np.max(da_triangle[:, 0]))
         #
         # valid_pnts_ind = [ind for ind in range(n_pnts) if range_x[0] <= pnts[ind][0] <= range_x[1] and range_y[0] <= pnts[ind][1] <= range_y[1]]
         # valid_pnts_ind = [ind for ind in valid_pnts_ind if ind not in da_order]
@@ -545,37 +612,42 @@
         for j in range(len(ct_list)):
             da_ct = ct_list[j]
             res = cv2.pointPolygonTest(da_ct, (int(pnts[i][0]), int(pnts[i][1])), False)
             if res >= 0:
                 loc[i] = j
                 break
 
-
     return loc
 
 
-
-
 def get_sides_points(img_size):
     size0 = img_size[1] - 1
     size1 = img_size[0] - 1
-    side_lines = np.asarray([[[0, 0], [size0, 0]], [[size0, 0], [size0, size1]],
-                             [[0, size1], [size0, size1]], [[0, 0], [0, size1]]])
+    side_lines = np.asarray(
+        [
+            [[0, 0], [size0, 0]],
+            [[size0, 0], [size0, size1]],
+            [[0, size1], [size0, size1]],
+            [[0, 0], [0, size1]],
+        ]
+    )
     corner_points = [[0, 0], [size0, 0], [size0, size1], [0, size1]]
     return side_lines, corner_points
 
 
 def num_side_pnt_changed(num_pnt, corner_points, side_lines):
     n_pnts_to_make = num_pnt - 2
     onside_data = corner_points.copy()
     if n_pnts_to_make > 0:
         for i in range(4):
             da_line = side_lines[i]
             for j in range(n_pnts_to_make):
-                inline_point = da_line[0] + (da_line[1] - da_line[0]) / (n_pnts_to_make + 1) * (j + 1)
+                inline_point = da_line[0] + (da_line[1] - da_line[0]) / (
+                    n_pnts_to_make + 1
+                ) * (j + 1)
                 onside_data.append([int(inline_point[0]), int(inline_point[1])])
     return onside_data
 
 
 def match_sides_points(rect_atlas, size_atlas, rect_image, size_image):
     x_factor = rect_atlas[2] / rect_image[2]
     y_factor = rect_atlas[3] / rect_image[3]
@@ -603,135 +675,159 @@
     if right_dist_atlas <= actual_right_dist_atlas:
         atlas_right_side = size_atlas[1] - (actual_right_dist_atlas - right_dist_atlas)
         atlas_width = int(atlas_right_side - atlas_corner_x)
         image_width = size_image[1] - image_corner_x
     else:
         atlas_width = size_atlas[1] - atlas_corner_x
         right_dist_image = actual_right_dist_atlas / x_factor
-        image_width = int(size_image[1] - image_corner_x - (actual_right_dist_image - right_dist_image))
+        image_width = int(
+            size_image[1]
+            - image_corner_x
+            - (actual_right_dist_image - right_dist_image)
+        )
 
     if top_dist_atlas <= rect_atlas[1]:
         atlas_corner_y = int(rect_atlas[1] - top_dist_atlas)
         image_corner_y = 0
     else:
         atlas_corner_y = 0
         top_dist_image = rect_atlas[1] / y_factor
         image_corner_y = int(rect_image[1] - top_dist_image)
 
     if bottom_dist_atlas <= actual_bottom_dist_atlas:
-        atlas_height = int(size_atlas[0] - atlas_corner_y - (actual_bottom_dist_atlas - bottom_dist_atlas))
+        atlas_height = int(
+            size_atlas[0]
+            - atlas_corner_y
+            - (actual_bottom_dist_atlas - bottom_dist_atlas)
+        )
         image_height = size_image[0] - image_corner_y
     else:
         atlas_height = size_atlas[0] - atlas_corner_y
         bottom_dist_image = actual_bottom_dist_atlas / y_factor
-        image_height = int(size_image[0] - image_corner_y - (actual_bottom_dist_image - bottom_dist_image))
+        image_height = int(
+            size_image[0]
+            - image_corner_y
+            - (actual_bottom_dist_image - bottom_dist_image)
+        )
 
     atlas_rect = (atlas_corner_x, atlas_corner_y, atlas_width, atlas_height)
     image_rect = (image_corner_x, image_corner_y, image_width, image_height)
 
     return atlas_rect, image_rect
 
 
 def get_corner_line_from_rect(rect):
-    corners = [[rect[0], rect[1]], [rect[0] + rect[2] - 1, rect[1]],
-               [rect[0] + rect[2] - 1, rect[1] + rect[3] - 1], [rect[0], rect[1] + rect[3] - 1]]
-
-    lines = np.asarray([[corners[0], corners[1]], [corners[1], corners[2]],
-                        [corners[3], corners[2]], [corners[0], corners[3]]])
+    corners = [
+        [rect[0], rect[1]],
+        [rect[0] + rect[2] - 1, rect[1]],
+        [rect[0] + rect[2] - 1, rect[1] + rect[3] - 1],
+        [rect[0], rect[1] + rect[3] - 1],
+    ]
+
+    lines = np.asarray(
+        [
+            [corners[0], corners[1]],
+            [corners[1], corners[2]],
+            [corners[3], corners[2]],
+            [corners[0], corners[3]],
+        ]
+    )
 
     return corners, lines
 
 
 def make_label_rgb_img(label_img, lut):
     fimg = np.dstack([label_img, label_img, label_img])
     unique_label = np.unique(label_img).astype(int)
     for ind in np.unique(unique_label):
         if ind == 0:
             continue
         loc = np.where(label_img == ind)
-        print(lut[ind])
+        # print(lut[ind])
         fimg[loc[0], loc[1], 0] = lut[ind][0]
         fimg[loc[0], loc[1], 1] = lut[ind][1]
         fimg[loc[0], loc[1], 2] = lut[ind][2]
-    return fimg.astype('uint8')
+    return fimg.astype("uint8")
 
 
 def make_contour_img(lable_img):
-    unique_label = np.unique(lable_img).astype('int')
+    unique_label = np.unique(lable_img).astype("int")
     img_size = lable_img.shape
-    contour_img = np.zeros(img_size, 'uint8')
+    contour_img = np.zeros(img_size, "uint8")
     for label_ind in unique_label:
         if label_ind == 0:
             continue
-        temp = np.zeros(img_size, 'uint8')
+        temp = np.zeros(img_size, "uint8")
         temp[lable_img == label_ind] = 1
-        ct, hc = cv2.findContours(image=temp, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE)
+        ct, hc = cv2.findContours(
+            image=temp, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_NONE
+        )
         for j in range(len(ct)):
             da_contour = ct[j].copy()
             da_shp = da_contour.shape
             da_contour = np.reshape(da_contour, (da_shp[0], da_shp[2]))
             contour_img[da_contour[:, 1], da_contour[:, 0]] = 1
     return contour_img
 
 
 def get_tri_lines(rect, pnts):
-    print(rect)
+    # print(rect)
     subdiv = cv2.Subdiv2D(rect)
     for p in pnts:
-        print(p)
+        # print(p)
         subdiv.insert((int(p[0]), int(p[1])))
     edge_list = subdiv.getEdgeList()
     lines_list = []
     # special_pnt = []
     for el in edge_list:
         pt1 = [el[0], el[1]]
         pt2 = [el[2], el[3]]
         if rect_contains(rect, pt1) and rect_contains(rect, pt2):
             lines_list.append(el)
         # else:
         #     if not rect_contains(rect, pt1) and pt1 not in special_pnt:
         #         special_pnt.append(pt1)
         #     if not rect_contains(rect, pt2) and pt2 not in special_pnt:
         #         special_pnt.append(pt2)
-    return lines_list  #, special_pnt
+    return lines_list  # , special_pnt
 
 
 # czi_img = image_file.data['scene 0'].copy()
 # channel_hsv = image_file.hsv_colors
 # temp_img = merge_channels_into_single_img(czi_img, channel_hsv)
 
+
 def gamma_correction(src, gamma):
     inv_gamma = 1 / gamma
 
     table = [((i / 255) ** inv_gamma) * 255 for i in range(256)]
     table = np.array(table, np.uint8)
 
     return cv2.LUT(src, table)
 
 
-
 def get_lower_val(val, tol, lim):
     lower_val = val - tol if tol < val else lim
     return lower_val
 
 
 def get_upper_val(val, tol, lim):
     upper_val = val + tol
     upper_val = upper_val if upper_val <= lim else lim
     return upper_val
 
 
 def get_bound_color(color, tol, level, mode):
     tol = float(tol)
-    if mode == 'gray':
+    if mode == "gray":
         lower_val = get_lower_val(color, tol, 0)
         upper_val = get_upper_val(color, tol, level)
-    elif mode == 'hsv':
-        lower_val = [get_lower_val(color[0], 1., 0)]
-        upper_val = [get_upper_val(color[0], 1., 180)]
+    elif mode == "hsv":
+        lower_val = [get_lower_val(color[0], 1.0, 0)]
+        upper_val = [get_upper_val(color[0], 1.0, 180)]
         for i in range(1, 3):
             lower_val.append(get_lower_val(color[i], tol, 0))
             upper_val.append(get_upper_val(color[i], tol, 255))
     else:
         lower_val = []
         upper_val = []
         for i in range(3):
@@ -740,19 +836,20 @@
     return lower_val, upper_val
 
 
 # ----------------------------------------------------------------------------------
 # ----------------------------------------------------------------------------------
 
 
-
 def get_statusbar_style(col):
-    style = 'background-color: #323232;' \
-            ' color: {}; border-top: 1px solid #272727; ' \
-            'padding-left: 30px;'.format(col)
+    style = (
+        "background-color: #323232;"
+        " color: {}; border-top: 1px solid #272727; "
+        "padding-left: 30px;".format(col)
+    )
     return style
 
 
 def rotate(image, angle, img_center=None, scale=1.0):
     (h, w) = image.shape[:2]
 
     if img_center is None:
@@ -792,15 +889,15 @@
     x = int(0.5 * (dim[1] - resize_dim[1]))
 
     if len(img_shape) == 3:
         center_img = np.zeros((dim[1], dim[0], img.shape[2])).astype(img.dtype)
     else:
         center_img = np.zeros((dim[1], dim[0])).astype(img.dtype)
 
-    center_img[x:(x + resize_dim[1]), y:(y + resize_dim[0])] = resize_img
+    center_img[x : (x + resize_dim[1]), y : (y + resize_dim[0])] = resize_img
 
     return center_img
 
 
 def get_tb_size(img_size):
     scale_factor = np.max(np.ravel(img_size) / 80)
     tb_size = (int(img_size[1] / scale_factor), int(img_size[0] / scale_factor))
@@ -817,19 +914,19 @@
     :param height: height of image in mm
     :param distance: distance of slice with respect to Bregma in mm
     :param origin: the coord of bregma on the current slice image
     :return:
     """
     width_factor = width / size[1] * 1000
     height_factor = height / size[0] * 1000
-    if cut == 'Coronal':
+    if cut == "Coronal":
         y_val = np.repeat(distance * 1000, len(points))
         x_val = (points[:, 0] - origin[0]) * width_factor
         z_val = (points[:, 1] - origin[1]) * height_factor
-    elif cut == 'Sagittal':
+    elif cut == "Sagittal":
         x_val = np.repeat(distance * 1000, len(points))
         y_val = (points[:, 0] - origin[0]) * width_factor
         z_val = (points[:, 1] - origin[1]) * height_factor
     else:
         z_val = np.repeat(distance * 1000, len(points))
         y_val = (points[:, 0] - origin[0]) * width_factor
         x_val = (points[:, 1] - origin[1]) * height_factor
@@ -862,48 +959,73 @@
 
     tck = splprep([points[:, 0], points[:, 1]], s=0, per=True)
 
     xi, yi = splev(np.linspace(0, 1, 1000), tck[0])
     return xi, yi
 
 
-def create_vis_img(size, point_data, color, vis_type='p', closed=False):
+def create_vis_img(size, point_data, color, vis_type="p", closed=False):
     if isinstance(point_data, list):
         point_data = np.asarray(point_data).astype(int)
     else:
         point_data = point_data.astype(int)
-    img = np.zeros((size[0], size[1], 3), 'uint8')
+    img = np.zeros((size[0], size[1], 3), "uint8")
     da_color = (int(color[0]), int(color[1]), int(color[2]))
-    if vis_type == 'p':
+    if vis_type == "p":
         for i in range(len(point_data)):
-            cv2.circle(img, (int(point_data[i][0]), int(point_data[i][1])), radius=5, color=da_color, thickness=-1)
+            cv2.circle(
+                img,
+                (int(point_data[i][0]), int(point_data[i][1])),
+                radius=5,
+                color=da_color,
+                thickness=-1,
+            )
     else:
         if closed:
             cv2.fillPoly(img, pts=[point_data], color=da_color)
         else:
             for i in range(len(point_data) - 1):
-                cv2.line(img, (int(point_data[i][0]), int(point_data[i][1])),
-                         (int(point_data[i + 1][0]), int(point_data[i + 1][1])),
-                         color=da_color, thickness=8)
+                cv2.line(
+                    img,
+                    (int(point_data[i][0]), int(point_data[i][1])),
+                    (int(point_data[i + 1][0]), int(point_data[i + 1][1])),
+                    color=da_color,
+                    thickness=8,
+                )
     return img
 
 
 def color_vis_img(img, color):
-    temp = np.zeros((img.shape[0], img.shape[1], 3), 'uint8')
+    temp = np.zeros((img.shape[0], img.shape[1], 3), "uint8")
     temp[img != 0, 0] = color[0]
     temp[img != 0, 1] = color[1]
     temp[img != 0, 2] = color[2]
     return temp
 
 
 def check_loaded_project(project_dict):
     all_keys = list(project_dict.keys())
-    valid_keys = ['atlas_path', 'current_atlas', 'num_windows', 'probe_type', 'np_onside', 'processing_slice',
-                  'processing_img', 'overlay_img', 'atlas_control', 'img_ctrl_data', 'setting_data', 'tool_data',
-                  'layer_data', 'working_img_data', 'working_atlas_data', 'object_data']
+    valid_keys = [
+        "atlas_path",
+        "current_atlas",
+        "num_windows",
+        "probe_type",
+        "np_onside",
+        "processing_slice",
+        "processing_img",
+        "overlay_img",
+        "atlas_control",
+        "img_ctrl_data",
+        "setting_data",
+        "tool_data",
+        "layer_data",
+        "working_img_data",
+        "working_atlas_data",
+        "object_data",
+    ]
     valid_project = True
     for da_key in all_keys:
         if da_key not in valid_keys:
             valid_project = False
     return valid_project
 
 
@@ -914,40 +1036,46 @@
         return True
 
 
 def obj_data_to_mesh3d(filename):
     vertices = []
     faces = []
 
-    with open(filename, 'r') as objf:
+    with open(filename, "r") as objf:
         for line in objf:
             slist = line.split()
             if slist:
-                if slist[0] == 'v':
+                if slist[0] == "v":
                     vertex = np.array(slist[1:], dtype=float)
                     vertices.append(vertex)
-                elif slist[0] == 'f':
+                elif slist[0] == "f":
                     face = []
                     for k in range(1, len(slist)):
-                        face.append([int(s) for s in slist[k].replace('//', '/').split('/')])
+                        face.append(
+                            [int(s) for s in slist[k].replace("//", "/").split("/")]
+                        )
                     if len(face) > 3:  # triangulate the n-polyonal face, n>3
                         faces.extend(
-                            [[face[0][0] - 1, face[k][0] - 1, face[k + 1][0] - 1] for k in range(1, len(face) - 1)])
+                            [
+                                [face[0][0] - 1, face[k][0] - 1, face[k + 1][0] - 1]
+                                for k in range(1, len(face) - 1)
+                            ]
+                        )
                     else:
                         faces.append([face[j][0] - 1 for j in range(len(face))])
                 else:
                     pass
 
     return np.array(vertices), np.array(faces)
 
 
 def make_atlas_label_contour(atlas_folder, segmentation_data):
-    sagital_contour_img = np.zeros(segmentation_data.shape, 'i')
-    coronal_contour_img = np.zeros(segmentation_data.shape, 'i')
-    horizontal_contour_img = np.zeros(segmentation_data.shape, 'i')
+    sagital_contour_img = np.zeros(segmentation_data.shape, "i")
+    coronal_contour_img = np.zeros(segmentation_data.shape, "i")
+    horizontal_contour_img = np.zeros(segmentation_data.shape, "i")
 
     # pre-process boundary
     for i in range(len(segmentation_data)):
         da_slice = segmentation_data[i, :, :].copy()
         contour_img = make_contour_img(da_slice)
         sagital_contour_img[i, :, :] = contour_img
 
@@ -957,21 +1085,23 @@
         coronal_contour_img[:, i, :] = contour_img
 
     for i in range(segmentation_data.shape[2]):
         da_slice = segmentation_data[:, :, i].copy()
         contour_img = make_contour_img(da_slice)
         horizontal_contour_img[:, :, i] = contour_img
 
-    boundary = {'s_contour': sagital_contour_img,
-                'c_contour': coronal_contour_img,
-                'h_contour': horizontal_contour_img}
+    boundary = {
+        "s_contour": sagital_contour_img,
+        "c_contour": coronal_contour_img,
+        "h_contour": horizontal_contour_img,
+    }
 
-    bnd = {'data': boundary}
+    bnd = {"data": boundary}
 
-    outfile_ct = open(os.path.join(atlas_folder, 'contour_pre_made.pkl'), 'wb')
+    outfile_ct = open(os.path.join(atlas_folder, "contour_pre_made.pkl"), "wb")
     pickle.dump(bnd, outfile_ct)
     outfile_ct.close()
 
     return boundary
 
 
 def get_angle_two_vector(vec1, vec2):
@@ -1012,32 +1142,39 @@
 
 def load_point_data(data_file_path):
     file_basename = os.path.basename(data_file_path)
     file_name, file_ext = os.path.splitext(file_basename)
     msg = None
     data = None
     try:
-        if file_ext == '.npy':
+        if file_ext == ".npy":
             data = np.load(data_file_path)
-        elif file_ext == '.pkl':
-            with open(data_file_path, 'rb') as f:
+        elif file_ext == ".pkl":
+            with open(data_file_path, "rb") as f:
                 data = pickle.load(f)
             # data = data_file['points']
-    except (IOError, OSError, ValueError, KeyError, IndexError, pickle.PickleError, pickle.UnpicklingError):
-        msg = 'Can not open atlas axis information file, please check the Tutorial on GitHub.'
+    except (
+        IOError,
+        OSError,
+        ValueError,
+        KeyError,
+        IndexError,
+        pickle.PickleError,
+        pickle.UnpicklingError,
+    ):
+        msg = "Can not open atlas axis information file, please check the Tutorial on GitHub."
         return data, msg
 
     if not isinstance(data, np.ndarray):
-        msg = 'Data is not numpy ndarray, please check the Tutorial on GitHub.'
+        msg = "Data is not numpy ndarray, please check the Tutorial on GitHub."
         return data, msg
 
     data_shape = data.shape
     if len(data_shape) != 2:
-        msg = 'Data has wrong size, please check the Tutorial on GitHub.'
+        msg = "Data has wrong size, please check the Tutorial on GitHub."
         return data, msg
 
     if data_shape[1] != 3:
-        msg = 'Data has wrong size, please check the Tutorial on GitHub.'
+        msg = "Data has wrong size, please check the Tutorial on GitHub."
         return data, msg
 
     return data, msg
-
```

### Comparing `herbs-0.2.2/herbs/widgets_utils.py` & `herbs-0.2.3/herbs/widgets_utils.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs/wtiles.py` & `herbs-0.2.3/herbs/wtiles.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.2/herbs.egg-info/PKG-INFO` & `herbs-0.2.3/herbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herbs
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python-based GUI for Histological E-data Registration in Brain Space
 Home-page: https://github.com/JingyiGF/HERBS
 Author: Jingyi GF
 Author-email: jingyi.g.fuglstad@gmail.com
 Project-URL: Bug Tracker, https://github.com/JingyiGF/HERBS/issues
 Keywords: brain atlas,histological image registration,probe coordinates
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `herbs-0.2.2/herbs.egg-info/SOURCES.txt` & `herbs-0.2.3/herbs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 herbs/movable_points.py
 herbs/obj_items.py
 herbs/object_control.py
 herbs/popup_message.py
 herbs/probe_utiles.py
 herbs/run_herbs.py
 herbs/slice_stacks.py
-herbs/temp.py
 herbs/toolbox.py
 herbs/triangulation_points.py
 herbs/uuuuuu.py
 herbs/version.py
 herbs/widgets_utils.py
 herbs/wtiles.py
 herbs.egg-info/PKG-INFO
```

### Comparing `herbs-0.2.2/setup.py` & `herbs-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 if sys.version_info.minor == 8 and sys.version_info.micro < 10:
     is_problematic = True
 
 if sys.version_info.minor == 9 and sys.version_info.micro == 0:
     is_problematic = True
 
-if sys.version_info.minor == 10 and sys.version_info.micro >= 5:
+if sys.version_info.minor == 10 and sys.version_info.micro > 10:
     is_problematic = True
 
 if is_problematic:
-    raise RuntimeError("Python version >= 3.8.10 < 3.10.5 / 3.9.0 required.")
+    raise RuntimeError("Python version >= 3.8.10 <= 3.10.9 / 3.9.0 required.")
+
 
 # Utility function to read the README file.
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 CLASSIFIERS = """
@@ -60,15 +61,15 @@
 numba >= 0.54.1
 numpy >= 1.20.3
 scipy >= 1.7.3
 requests >= 2.26.0
 nibabel >= 3.2.1
 pynrrd >= 0.4.3
 tifffile >= 2021.11.2
-aicspylibczi >= 3.0.3
+aicspylibczi == 3.0.3
 pandas >= 1.3.5
 natsort >= 8.0.2
 imagecodecs >= 2022.2.22
 h5py >= 3.7.0
 tables >= 3.7.0
 """
 
@@ -86,25 +87,25 @@
 icons/toolbar/*.png
 qss/*.qss
 """
 
 
 setup(
     name="herbs",
-    version="0.2.2",
+    version="0.2.3",
     author="Jingyi GF",
     author_email="jingyi.g.fuglstad@gmail.com",
     description="A Python-based GUI for Histological E-data Registration in Brain Space",
     keywords="brain atlas, histological image registration, probe coordinates",
     url="https://github.com/JingyiGF/HERBS",
     packages=find_packages(),
-    package_data={'': [_f for _f in PACKAGE_DATA.split('\n') if _f]},
+    package_data={"": [_f for _f in PACKAGE_DATA.split("\n") if _f]},
     include_package_data=True,
-    long_description=read('README.md'),
+    long_description=read("README.md"),
     long_description_content_type="text/markdown",
     project_urls={
         "Bug Tracker": "https://github.com/JingyiGF/HERBS/issues",
     },
-    classifiers=[_f for _f in CLASSIFIERS.split('\n') if _f],
+    classifiers=[_f for _f in CLASSIFIERS.split("\n") if _f],
     python_requires=">=3.8",
-    install_requires=[_f for _f in REQUIRES.split('\n') if _f]
+    install_requires=[_f for _f in REQUIRES.split("\n") if _f],
 )
```

