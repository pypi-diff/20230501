# Comparing `tmp/herbs-0.2.3.tar.gz` & `tmp/herbs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herbs-0.2.3.tar", last modified: Mon May  1 14:27:09 2023, max compression
+gzip compressed data, was "herbs-0.2.4.tar", last modified: Mon May  1 19:52:53 2023, max compression
```

## Comparing `herbs-0.2.3.tar` & `herbs-0.2.4.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.991439 herbs-0.2.3/
--rw-r--r--   0 jingyi     (501) staff       (20)      127 2023-04-25 18:58:14.000000 herbs-0.2.3/AUTHOR.txt
--rw-r--r--   0 jingyi     (501) staff       (20)     1094 2023-04-25 18:58:15.000000 herbs-0.2.3/LICENSE.txt
--rw-r--r--   0 jingyi     (501) staff       (20)      901 2023-04-25 18:58:15.000000 herbs-0.2.3/MANIFEST.in
--rw-r--r--   0 jingyi     (501) staff       (20)     5678 2023-05-01 14:27:09.991178 herbs-0.2.3/PKG-INFO
--rw-r--r--   0 jingyi     (501) staff       (20)     4448 2023-04-25 18:58:15.000000 herbs-0.2.3/README.md
--rw-r--r--   0 jingyi     (501) staff       (20)      725 2023-04-25 18:58:15.000000 herbs-0.2.3/THANKS.txt
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.928630 herbs-0.2.3/herbs/
--rwxr-xr-x   0 jingyi     (501) staff       (20)      293 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/__init__.py
--rw-r--r--   0 jingyi     (501) staff       (20)      976 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/about_herbs.py
--rw-r--r--   0 jingyi     (501) staff       (20)    26310 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/allen_downloader.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    11325 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_downloader.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    18106 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_loader.py
--rw-r--r--   0 jingyi     (501) staff       (20)    28218 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_processor.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    58116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/atlas_view.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)     7948 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/czi_reader.py
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.932318 herbs-0.2.3/herbs/data/
--rwxr-xr-x   0 jingyi     (501) staff       (20)    26573 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/data/atlas_labels.pkl
--rw-r--r--   0 jingyi     (501) staff       (20)   227433 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/data/query.csv
--rw-r--r--   0 jingyi     (501) staff       (20)   329944 2023-05-01 14:11:36.000000 herbs-0.2.3/herbs/herbsgui.py
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.937874 herbs-0.2.3/herbs/icons/
--rw-r--r--   0 jingyi     (501) staff       (20)      760 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/backward.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      593 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/dot.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/down-arrow.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      867 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/fast_backward.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      861 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/fast_forward.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      736 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/forward.svg
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.940994 herbs-0.2.3/herbs/icons/layers/
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/add.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2322 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/ai.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2916 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/eye_off.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     3295 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/eye_on.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     3056 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/eye_white.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2193 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/hi.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2107 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/layers/trash.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1869 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/object.svg
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.952134 herbs-0.2.3/herbs/icons/sidebar/
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/add.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2731 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/atlascontrol.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1704 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/atlascontrol.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1146 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/bnd.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)    14175 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/c_section.png
--rw-r--r--   0 jingyi     (501) staff       (20)     9270 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/c_section2.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2258 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/cell.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)      517 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/check.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1539 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/compare.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      869 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/contour.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)    14191 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/h_section.png
--rw-r--r--   0 jingyi     (501) staff       (20)      691 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/info.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     3336 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/layers.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1728 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/layers.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/line.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1323 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/link.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1366 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/link_off.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)      763 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/merge.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)      994 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/object.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2584 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/probe.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1300 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/probe.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      856 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/rotation_horizontal.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      858 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/rotation_vertical.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)    14248 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/s_section.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     3741 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/tool.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1350 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/tool.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2107 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/trash.png
--rw-r--r--   0 jingyi     (501) staff       (20)      614 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/tree_checked.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     3299 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/treeview.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)      697 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/treeview.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     3211 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/treeview2.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1783 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/sidebar/virus.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      653 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/tdown.svg
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.984633 herbs-0.2.3/herbs/icons/toolbar/
--rw-r--r--   0 jingyi     (501) staff       (20)      669 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/accept.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1974 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/accept2.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     3485 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/aim.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     2108 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/aim_not.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1142 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/anchor.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      777 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/anticlockwise_rotation.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2604 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/atlas_icon.png
--rw-r--r--   0 jingyi     (501) staff       (20)     1371 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/boundary_register.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     2885 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/cancel.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1431 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/cell_select.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      868 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/cell_select_not.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)      517 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/check.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      773 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/clockwise_rotation.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1205 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/closed_path.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1060 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/closed_path2 copy.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1825 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/closed_path2.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2180 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eraser.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1275 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eraser.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      984 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eye.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1343 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/eye_closed.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      865 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/fill.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1215 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/gps.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2172 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/h_flip.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1894 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/handle.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2575 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/image_icon.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2277 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/image_icon.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      788 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/info.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1876 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/inpart.png
--rw-r--r--   0 jingyi     (501) staff       (20)      890 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/inpart.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     5945 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/lasso.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1017 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/lasso.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2913 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/left90.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/line.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      613 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/line_sites.svg
--rw-r--r--   0 jingyi     (501) staff       (20)    11865 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/linear_silicon.png
--rw-r--r--   0 jingyi     (501) staff       (20)     5202 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/linear_silicon.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      848 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/list.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)      833 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/location.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1067 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/magic-wand.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2567 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/magic_white.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)      648 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/mask.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1375 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/match.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1151 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/matchbnd.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     2402 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/matching.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)      763 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/merge.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2148 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_down.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1963 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_left.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2158 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_right.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2146 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/move_up.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     5229 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/moving.png
--rw-r--r--   0 jingyi     (501) staff       (20)     7705 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/multi-probe.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1101 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/multi_pencil.svg
--rw-r--r--   0 jingyi     (501) staff       (20)    34495 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/multi_probe.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)      994 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/object.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1893 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/open_path.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1894 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/outpart.png
--rw-r--r--   0 jingyi     (501) staff       (20)     1408 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/outpart.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2319 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/pencil.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1250 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/pencil.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2485 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/plasso.png
--rw-r--r--   0 jingyi     (501) staff       (20)     1601 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/probe.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1721 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/radar.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     4384 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/rotation.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1132 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/rotation_clockwise.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1127 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/rotation_counter_clockwise.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     1816 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/ruler.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      729 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/separate_sites.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      817 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/single_pencil.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      730 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toa.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     3165 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toa_delete.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      819 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toaa.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      740 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toh.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     3189 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/toh_delete.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      733 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/tohh.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2127 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/trans.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1028 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/trans.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      599 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/triangulation.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2339 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/two_window.png
--rw-r--r--   0 jingyi     (501) staff       (20)     1211 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/unmerge.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2144 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/v_flip.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)     1783 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/virus.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     2367 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/virus_register.svg
--rw-r--r--   0 jingyi     (501) staff       (20)     2332 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/vis2d.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2305 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/window2.png
--rw-r--r--   0 jingyi     (501) staff       (20)    15734 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/window3.png
--rwxr-xr-x   0 jingyi     (501) staff       (20)    16491 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/toolbar/window4.png
--rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/tree_close.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/tree_open.svg
--rw-r--r--   0 jingyi     (501) staff       (20)      624 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/icons/up-arrow.svg
--rwxr-xr-x   0 jingyi     (501) staff       (20)    24078 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_curves.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)     8774 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_reader.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    13631 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_stacks.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    27381 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/image_view.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)        5 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/images_reader.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)     7998 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/label_tree.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    18954 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/layers_control.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    26116 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/main_window.ui
--rw-r--r--   0 jingyi     (501) staff       (20)     7275 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/movable_points.py
--rw-r--r--   0 jingyi     (501) staff       (20)     3433 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/obj_items.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    52329 2023-05-01 14:09:27.000000 herbs-0.2.3/herbs/object_control.py
--rw-r--r--   0 jingyi     (501) staff       (20)      393 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/popup_message.py
--rw-r--r--   0 jingyi     (501) staff       (20)    38740 2023-05-01 05:23:17.000000 herbs-0.2.3/herbs/probe_utiles.py
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.990847 herbs-0.2.3/herbs/qss/
--rw-r--r--   0 jingyi     (501) staff       (20)      312 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/atlas_view_group_box.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      101 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/box_label.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      446 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/channel_selector.qss
--rw-r--r--   0 jingyi     (501) staff       (20)     2649 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/color_combo.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      166 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/decor_label.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      151 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/dialogs.qss
--rw-r--r--   0 jingyi     (501) staff       (20)       83 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/hidden_line_edit.qss
--rw-r--r--   0 jingyi     (501) staff       (20)     2586 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/label_tree.qss
--rw-r--r--   0 jingyi     (501) staff       (20)     5688 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/main_window.qss
--rw-r--r--   0 jingyi     (501) staff       (20)     1045 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/menu_bar.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      612 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/multi_handle_slider.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      543 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/obj_ctrl_bottom_button.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      359 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/object_text_button.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      950 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/page_control.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      177 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/rotation_button.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      574 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/side_bar.qss
--rw-r--r--   0 jingyi     (501) staff       (20)     2631 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/spinbox.qss
--rw-r--r--   0 jingyi     (501) staff       (20)     4366 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/tabs.qss
--rw-r--r--   0 jingyi     (501) staff       (20)     1572 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/qss/tool_bar.qss
--rw-r--r--   0 jingyi     (501) staff       (20)      247 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/run_herbs.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)     8576 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/slice_stacks.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    24452 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/toolbox.py
--rw-r--r--   0 jingyi     (501) staff       (20)     3362 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/triangulation_points.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    36300 2023-05-01 05:19:09.000000 herbs-0.2.3/herbs/uuuuuu.py
--rw-r--r--   0 jingyi     (501) staff       (20)       22 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/version.py
--rw-r--r--   0 jingyi     (501) staff       (20)     5055 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/widgets_utils.py
--rwxr-xr-x   0 jingyi     (501) staff       (20)    26611 2023-04-25 18:58:15.000000 herbs-0.2.3/herbs/wtiles.py
-drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 14:27:09.930673 herbs-0.2.3/herbs.egg-info/
--rw-r--r--   0 jingyi     (501) staff       (20)     5678 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/PKG-INFO
--rw-r--r--   0 jingyi     (501) staff       (20)     5810 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/SOURCES.txt
--rw-r--r--   0 jingyi     (501) staff       (20)        1 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/dependency_links.txt
--rw-r--r--   0 jingyi     (501) staff       (20)      411 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/requires.txt
--rw-r--r--   0 jingyi     (501) staff       (20)        6 2023-05-01 14:27:09.000000 herbs-0.2.3/herbs.egg-info/top_level.txt
--rw-r--r--   0 jingyi     (501) staff       (20)       86 2023-04-25 18:58:15.000000 herbs-0.2.3/pyproject.toml
--rw-r--r--   0 jingyi     (501) staff       (20)       38 2023-05-01 14:27:09.991508 herbs-0.2.3/setup.cfg
--rwxr-xr-x   0 jingyi     (501) staff       (20)     2857 2023-05-01 14:25:34.000000 herbs-0.2.3/setup.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.981305 herbs-0.2.4/
+-rw-r--r--   0 jingyi     (501) staff       (20)      127 2023-04-25 18:58:14.000000 herbs-0.2.4/AUTHOR.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)     1094 2023-04-25 18:58:15.000000 herbs-0.2.4/LICENSE.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)      901 2023-04-25 18:58:15.000000 herbs-0.2.4/MANIFEST.in
+-rw-r--r--   0 jingyi     (501) staff       (20)     5678 2023-05-01 19:52:53.980663 herbs-0.2.4/PKG-INFO
+-rw-r--r--   0 jingyi     (501) staff       (20)     4448 2023-04-25 18:58:15.000000 herbs-0.2.4/README.md
+-rw-r--r--   0 jingyi     (501) staff       (20)      725 2023-04-25 18:58:15.000000 herbs-0.2.4/THANKS.txt
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.833087 herbs-0.2.4/herbs/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      293 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/__init__.py
+-rw-r--r--   0 jingyi     (501) staff       (20)      976 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/about_herbs.py
+-rw-r--r--   0 jingyi     (501) staff       (20)    26310 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/allen_downloader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    11325 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/atlas_downloader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    18106 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/atlas_loader.py
+-rw-r--r--   0 jingyi     (501) staff       (20)    28218 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/atlas_processor.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    58116 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/atlas_view.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     7948 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/czi_reader.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.841715 herbs-0.2.4/herbs/data/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    26573 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/data/atlas_labels.pkl
+-rw-r--r--   0 jingyi     (501) staff       (20)   227433 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/data/query.csv
+-rw-r--r--   0 jingyi     (501) staff       (20)   329944 2023-05-01 14:11:36.000000 herbs-0.2.4/herbs/herbsgui.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.852281 herbs-0.2.4/herbs/icons/
+-rw-r--r--   0 jingyi     (501) staff       (20)      760 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/backward.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      593 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/dot.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/down-arrow.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      867 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/fast_backward.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      861 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/fast_forward.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      736 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/forward.svg
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.859334 herbs-0.2.4/herbs/icons/layers/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2116 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/layers/add.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2322 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/layers/ai.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2916 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/layers/eye_off.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3295 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/layers/eye_on.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3056 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/layers/eye_white.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2193 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/layers/hi.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2107 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/layers/trash.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1869 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/object.svg
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.888835 herbs-0.2.4/herbs/icons/sidebar/
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2116 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/add.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2731 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/atlascontrol.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1704 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/atlascontrol.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1146 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/bnd.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    14175 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/c_section.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     9270 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/c_section2.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2258 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/cell.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      517 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/check.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1539 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/compare.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      869 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/contour.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    14191 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/h_section.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      691 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/info.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3336 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/layers.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1728 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/layers.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/line.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1323 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/link.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1366 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/link_off.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      763 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/merge.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      994 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/object.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2584 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/probe.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1300 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/probe.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      856 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/rotation_horizontal.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      858 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/rotation_vertical.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    14248 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/s_section.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3741 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/tool.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1350 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/tool.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2107 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/trash.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      614 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/tree_checked.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3299 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/treeview.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      697 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/treeview.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     3211 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/treeview2.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1783 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/sidebar/virus.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      653 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/tdown.svg
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.966053 herbs-0.2.4/herbs/icons/toolbar/
+-rw-r--r--   0 jingyi     (501) staff       (20)      669 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/accept.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1974 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/accept2.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     3485 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/aim.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2108 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/aim_not.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1142 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/anchor.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      777 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/anticlockwise_rotation.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2604 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/atlas_icon.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1371 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/boundary_register.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2885 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/cancel.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1431 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/cell_select.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      868 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/cell_select_not.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      517 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/check.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      773 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/clockwise_rotation.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1205 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/closed_path.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1060 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/closed_path2 copy.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1825 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/closed_path2.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2180 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/eraser.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1275 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/eraser.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      984 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/eye.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1343 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/eye_closed.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      865 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/fill.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1215 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/gps.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2172 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/h_flip.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1894 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/handle.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2575 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/image_icon.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2277 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/image_icon.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      788 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/info.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1876 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/inpart.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      890 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/inpart.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     5945 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/lasso.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1017 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/lasso.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2913 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/left90.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/line.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      613 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/line_sites.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)    11865 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/linear_silicon.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     5202 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/linear_silicon.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      848 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/list.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      833 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/location.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1067 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/magic-wand.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2567 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/magic_white.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      648 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/mask.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1375 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/match.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1151 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/matchbnd.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2402 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/matching.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      763 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/merge.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2148 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/move_down.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1963 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/move_left.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2158 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/move_right.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2146 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/move_up.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     5229 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/moving.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     7705 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/multi-probe.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1101 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/multi_pencil.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)    34495 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/multi_probe.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)      994 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/object.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1893 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/open_path.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1894 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/outpart.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1408 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/outpart.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2319 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/pencil.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1250 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/pencil.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2485 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/plasso.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1601 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/probe.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1721 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/radar.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     4384 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/rotation.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1132 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/rotation_clockwise.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1127 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/rotation_counter_clockwise.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     1816 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/ruler.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      729 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/separate_sites.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      817 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/single_pencil.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      730 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/toa.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     3165 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/toa_delete.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      819 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/toaa.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      740 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/toh.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     3189 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/toh_delete.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      733 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/tohh.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2127 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/trans.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1028 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/trans.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      599 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/triangulation.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2339 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/two_window.png
+-rw-r--r--   0 jingyi     (501) staff       (20)     1211 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/unmerge.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2144 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/v_flip.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     1783 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/virus.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2367 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/virus_register.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)     2332 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/vis2d.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2305 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/window2.png
+-rw-r--r--   0 jingyi     (501) staff       (20)    15734 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/window3.png
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    16491 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/toolbar/window4.png
+-rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/tree_close.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      611 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/tree_open.svg
+-rw-r--r--   0 jingyi     (501) staff       (20)      624 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/icons/up-arrow.svg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    24078 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/image_curves.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     8774 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/image_reader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    13631 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/image_stacks.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    27381 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/image_view.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)        5 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/images_reader.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     7998 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/label_tree.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    18954 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/layers_control.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    26116 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/main_window.ui
+-rw-r--r--   0 jingyi     (501) staff       (20)     7275 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/movable_points.py
+-rw-r--r--   0 jingyi     (501) staff       (20)     3433 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/obj_items.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    52329 2023-05-01 14:09:27.000000 herbs-0.2.4/herbs/object_control.py
+-rw-r--r--   0 jingyi     (501) staff       (20)      393 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/popup_message.py
+-rw-r--r--   0 jingyi     (501) staff       (20)    38740 2023-05-01 05:23:17.000000 herbs-0.2.4/herbs/probe_utiles.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.979614 herbs-0.2.4/herbs/qss/
+-rw-r--r--   0 jingyi     (501) staff       (20)      312 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/atlas_view_group_box.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      101 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/box_label.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      446 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/channel_selector.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     2649 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/color_combo.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      166 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/decor_label.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      151 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/dialogs.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)       83 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/hidden_line_edit.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     2586 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/label_tree.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     5688 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/main_window.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     1045 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/menu_bar.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      612 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/multi_handle_slider.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      543 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/obj_ctrl_bottom_button.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      359 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/object_text_button.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      950 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/page_control.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      177 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/rotation_button.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      574 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/side_bar.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     2631 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/spinbox.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     4366 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/tabs.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)     1572 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/qss/tool_bar.qss
+-rw-r--r--   0 jingyi     (501) staff       (20)      247 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/run_herbs.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     8576 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/slice_stacks.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    24452 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/toolbox.py
+-rw-r--r--   0 jingyi     (501) staff       (20)     3362 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/triangulation_points.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    36300 2023-05-01 05:19:09.000000 herbs-0.2.4/herbs/uuuuuu.py
+-rw-r--r--   0 jingyi     (501) staff       (20)       22 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/version.py
+-rw-r--r--   0 jingyi     (501) staff       (20)     5055 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/widgets_utils.py
+-rwxr-xr-x   0 jingyi     (501) staff       (20)    26611 2023-04-25 18:58:15.000000 herbs-0.2.4/herbs/wtiles.py
+drwxr-xr-x   0 jingyi     (501) staff       (20)        0 2023-05-01 19:52:53.838472 herbs-0.2.4/herbs.egg-info/
+-rw-r--r--   0 jingyi     (501) staff       (20)     5678 2023-05-01 19:52:53.000000 herbs-0.2.4/herbs.egg-info/PKG-INFO
+-rw-r--r--   0 jingyi     (501) staff       (20)     5810 2023-05-01 19:52:53.000000 herbs-0.2.4/herbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)        1 2023-05-01 19:52:53.000000 herbs-0.2.4/herbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)      411 2023-05-01 19:52:53.000000 herbs-0.2.4/herbs.egg-info/requires.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)        6 2023-05-01 19:52:53.000000 herbs-0.2.4/herbs.egg-info/top_level.txt
+-rw-r--r--   0 jingyi     (501) staff       (20)       86 2023-04-25 18:58:15.000000 herbs-0.2.4/pyproject.toml
+-rw-r--r--   0 jingyi     (501) staff       (20)       38 2023-05-01 19:52:53.981469 herbs-0.2.4/setup.cfg
+-rwxr-xr-x   0 jingyi     (501) staff       (20)     2857 2023-05-01 19:45:21.000000 herbs-0.2.4/setup.py
```

### Comparing `herbs-0.2.3/LICENSE.txt` & `herbs-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/MANIFEST.in` & `herbs-0.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/PKG-INFO` & `herbs-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herbs
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python-based GUI for Histological E-data Registration in Brain Space
 Home-page: https://github.com/JingyiGF/HERBS
 Author: Jingyi GF
 Author-email: jingyi.g.fuglstad@gmail.com
 Project-URL: Bug Tracker, https://github.com/JingyiGF/HERBS/issues
 Keywords: brain atlas,histological image registration,probe coordinates
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `herbs-0.2.3/README.md` & `herbs-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/THANKS.txt` & `herbs-0.2.4/THANKS.txt`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/about_herbs.py` & `herbs-0.2.4/herbs/about_herbs.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/allen_downloader.py` & `herbs-0.2.4/herbs/allen_downloader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/atlas_downloader.py` & `herbs-0.2.4/herbs/atlas_downloader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/atlas_loader.py` & `herbs-0.2.4/herbs/atlas_loader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/atlas_processor.py` & `herbs-0.2.4/herbs/atlas_processor.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/atlas_view.py` & `herbs-0.2.4/herbs/atlas_view.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/czi_reader.py` & `herbs-0.2.4/herbs/czi_reader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/data/atlas_labels.pkl` & `herbs-0.2.4/herbs/data/atlas_labels.pkl`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/data/query.csv` & `herbs-0.2.4/herbs/data/query.csv`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/herbsgui.py` & `herbs-0.2.4/herbs/herbsgui.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/backward.svg` & `herbs-0.2.4/herbs/icons/backward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/dot.svg` & `herbs-0.2.4/herbs/icons/dot.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/down-arrow.svg` & `herbs-0.2.4/herbs/icons/down-arrow.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/fast_backward.svg` & `herbs-0.2.4/herbs/icons/fast_backward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/fast_forward.svg` & `herbs-0.2.4/herbs/icons/fast_forward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/forward.svg` & `herbs-0.2.4/herbs/icons/forward.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/layers/add.png` & `herbs-0.2.4/herbs/icons/layers/add.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/layers/ai.png` & `herbs-0.2.4/herbs/icons/layers/ai.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/layers/eye_off.png` & `herbs-0.2.4/herbs/icons/layers/eye_off.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/layers/eye_on.png` & `herbs-0.2.4/herbs/icons/layers/eye_on.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/layers/eye_white.png` & `herbs-0.2.4/herbs/icons/layers/eye_white.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/layers/hi.png` & `herbs-0.2.4/herbs/icons/layers/hi.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/layers/trash.png` & `herbs-0.2.4/herbs/icons/layers/trash.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/object.svg` & `herbs-0.2.4/herbs/icons/object.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/add.png` & `herbs-0.2.4/herbs/icons/sidebar/add.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/atlascontrol.png` & `herbs-0.2.4/herbs/icons/sidebar/atlascontrol.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/atlascontrol.svg` & `herbs-0.2.4/herbs/icons/sidebar/atlascontrol.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/bnd.svg` & `herbs-0.2.4/herbs/icons/sidebar/bnd.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/c_section.png` & `herbs-0.2.4/herbs/icons/sidebar/c_section.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/c_section2.png` & `herbs-0.2.4/herbs/icons/sidebar/c_section2.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/cell.svg` & `herbs-0.2.4/herbs/icons/sidebar/cell.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/check.svg` & `herbs-0.2.4/herbs/icons/sidebar/check.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/compare.svg` & `herbs-0.2.4/herbs/icons/sidebar/compare.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/contour.svg` & `herbs-0.2.4/herbs/icons/sidebar/contour.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/h_section.png` & `herbs-0.2.4/herbs/icons/sidebar/h_section.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/info.svg` & `herbs-0.2.4/herbs/icons/sidebar/info.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/layers.png` & `herbs-0.2.4/herbs/icons/sidebar/layers.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/layers.svg` & `herbs-0.2.4/herbs/icons/sidebar/layers.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/line.svg` & `herbs-0.2.4/herbs/icons/sidebar/line.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/link.svg` & `herbs-0.2.4/herbs/icons/sidebar/link.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/link_off.svg` & `herbs-0.2.4/herbs/icons/sidebar/link_off.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/merge.svg` & `herbs-0.2.4/herbs/icons/sidebar/merge.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/object.svg` & `herbs-0.2.4/herbs/icons/sidebar/object.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/probe.png` & `herbs-0.2.4/herbs/icons/sidebar/probe.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/probe.svg` & `herbs-0.2.4/herbs/icons/sidebar/probe.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/rotation_horizontal.svg` & `herbs-0.2.4/herbs/icons/sidebar/rotation_horizontal.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/rotation_vertical.svg` & `herbs-0.2.4/herbs/icons/sidebar/rotation_vertical.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/s_section.png` & `herbs-0.2.4/herbs/icons/sidebar/s_section.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/tool.png` & `herbs-0.2.4/herbs/icons/sidebar/tool.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/tool.svg` & `herbs-0.2.4/herbs/icons/sidebar/tool.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/trash.png` & `herbs-0.2.4/herbs/icons/sidebar/trash.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/tree_checked.svg` & `herbs-0.2.4/herbs/icons/sidebar/tree_checked.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/treeview.png` & `herbs-0.2.4/herbs/icons/sidebar/treeview.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/treeview.svg` & `herbs-0.2.4/herbs/icons/sidebar/treeview.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/treeview2.png` & `herbs-0.2.4/herbs/icons/sidebar/treeview2.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/sidebar/virus.svg` & `herbs-0.2.4/herbs/icons/sidebar/virus.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/tdown.svg` & `herbs-0.2.4/herbs/icons/tdown.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/accept.svg` & `herbs-0.2.4/herbs/icons/toolbar/accept.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/accept2.svg` & `herbs-0.2.4/herbs/icons/toolbar/accept2.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/aim.svg` & `herbs-0.2.4/herbs/icons/toolbar/aim.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/aim_not.svg` & `herbs-0.2.4/herbs/icons/toolbar/aim_not.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/anchor.svg` & `herbs-0.2.4/herbs/icons/toolbar/anchor.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/anticlockwise_rotation.svg` & `herbs-0.2.4/herbs/icons/toolbar/anticlockwise_rotation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/atlas_icon.png` & `herbs-0.2.4/herbs/icons/toolbar/atlas_icon.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/boundary_register.svg` & `herbs-0.2.4/herbs/icons/toolbar/boundary_register.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/cancel.svg` & `herbs-0.2.4/herbs/icons/toolbar/cancel.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/cell_select.svg` & `herbs-0.2.4/herbs/icons/toolbar/cell_select.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/cell_select_not.svg` & `herbs-0.2.4/herbs/icons/toolbar/cell_select_not.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/check.svg` & `herbs-0.2.4/herbs/icons/toolbar/check.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/clockwise_rotation.svg` & `herbs-0.2.4/herbs/icons/toolbar/clockwise_rotation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/closed_path.svg` & `herbs-0.2.4/herbs/icons/toolbar/closed_path.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/closed_path2 copy.svg` & `herbs-0.2.4/herbs/icons/toolbar/closed_path2 copy.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/closed_path2.svg` & `herbs-0.2.4/herbs/icons/toolbar/closed_path2.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/eraser.png` & `herbs-0.2.4/herbs/icons/toolbar/eraser.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/eraser.svg` & `herbs-0.2.4/herbs/icons/toolbar/eraser.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/eye.svg` & `herbs-0.2.4/herbs/icons/toolbar/eye.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/eye_closed.svg` & `herbs-0.2.4/herbs/icons/toolbar/eye_closed.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/fill.svg` & `herbs-0.2.4/herbs/icons/toolbar/fill.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/gps.svg` & `herbs-0.2.4/herbs/icons/toolbar/gps.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/h_flip.png` & `herbs-0.2.4/herbs/icons/toolbar/h_flip.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/handle.png` & `herbs-0.2.4/herbs/icons/toolbar/handle.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/image_icon.png` & `herbs-0.2.4/herbs/icons/toolbar/image_icon.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/image_icon.svg` & `herbs-0.2.4/herbs/icons/toolbar/image_icon.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/info.svg` & `herbs-0.2.4/herbs/icons/toolbar/info.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/inpart.png` & `herbs-0.2.4/herbs/icons/toolbar/inpart.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/inpart.svg` & `herbs-0.2.4/herbs/icons/toolbar/inpart.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/lasso.png` & `herbs-0.2.4/herbs/icons/toolbar/lasso.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/lasso.svg` & `herbs-0.2.4/herbs/icons/toolbar/lasso.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/left90.png` & `herbs-0.2.4/herbs/icons/toolbar/left90.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/line.svg` & `herbs-0.2.4/herbs/icons/toolbar/line.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/line_sites.svg` & `herbs-0.2.4/herbs/icons/toolbar/line_sites.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/linear_silicon.png` & `herbs-0.2.4/herbs/icons/toolbar/linear_silicon.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/linear_silicon.svg` & `herbs-0.2.4/herbs/icons/toolbar/linear_silicon.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/list.svg` & `herbs-0.2.4/herbs/icons/toolbar/list.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/location.svg` & `herbs-0.2.4/herbs/icons/toolbar/location.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/magic-wand.svg` & `herbs-0.2.4/herbs/icons/toolbar/magic-wand.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/magic_white.png` & `herbs-0.2.4/herbs/icons/toolbar/magic_white.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/mask.svg` & `herbs-0.2.4/herbs/icons/toolbar/mask.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/match.svg` & `herbs-0.2.4/herbs/icons/toolbar/match.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/matchbnd.svg` & `herbs-0.2.4/herbs/icons/toolbar/matchbnd.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/matching.svg` & `herbs-0.2.4/herbs/icons/toolbar/matching.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/merge.svg` & `herbs-0.2.4/herbs/icons/toolbar/merge.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/move_down.png` & `herbs-0.2.4/herbs/icons/toolbar/move_down.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/move_left.png` & `herbs-0.2.4/herbs/icons/toolbar/move_left.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/move_right.png` & `herbs-0.2.4/herbs/icons/toolbar/move_right.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/move_up.png` & `herbs-0.2.4/herbs/icons/toolbar/move_up.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/moving.png` & `herbs-0.2.4/herbs/icons/toolbar/moving.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/multi-probe.svg` & `herbs-0.2.4/herbs/icons/toolbar/multi-probe.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/multi_pencil.svg` & `herbs-0.2.4/herbs/icons/toolbar/multi_pencil.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/multi_probe.png` & `herbs-0.2.4/herbs/icons/toolbar/multi_probe.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/object.svg` & `herbs-0.2.4/herbs/icons/toolbar/object.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/open_path.svg` & `herbs-0.2.4/herbs/icons/toolbar/open_path.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/outpart.png` & `herbs-0.2.4/herbs/icons/toolbar/outpart.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/outpart.svg` & `herbs-0.2.4/herbs/icons/toolbar/outpart.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/pencil.png` & `herbs-0.2.4/herbs/icons/toolbar/pencil.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/pencil.svg` & `herbs-0.2.4/herbs/icons/toolbar/pencil.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/plasso.png` & `herbs-0.2.4/herbs/icons/toolbar/plasso.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/probe.svg` & `herbs-0.2.4/herbs/icons/toolbar/probe.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/radar.svg` & `herbs-0.2.4/herbs/icons/toolbar/radar.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/rotation.svg` & `herbs-0.2.4/herbs/icons/toolbar/rotation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/rotation_clockwise.svg` & `herbs-0.2.4/herbs/icons/toolbar/rotation_clockwise.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/rotation_counter_clockwise.svg` & `herbs-0.2.4/herbs/icons/toolbar/rotation_counter_clockwise.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/ruler.svg` & `herbs-0.2.4/herbs/icons/toolbar/ruler.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/separate_sites.svg` & `herbs-0.2.4/herbs/icons/toolbar/separate_sites.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/single_pencil.svg` & `herbs-0.2.4/herbs/icons/toolbar/single_pencil.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/toa.svg` & `herbs-0.2.4/herbs/icons/toolbar/toa.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/toa_delete.svg` & `herbs-0.2.4/herbs/icons/toolbar/toa_delete.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/toaa.svg` & `herbs-0.2.4/herbs/icons/toolbar/toaa.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/toh.svg` & `herbs-0.2.4/herbs/icons/toolbar/toh.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/toh_delete.svg` & `herbs-0.2.4/herbs/icons/toolbar/toh_delete.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/tohh.svg` & `herbs-0.2.4/herbs/icons/toolbar/tohh.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/trans.png` & `herbs-0.2.4/herbs/icons/toolbar/trans.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/trans.svg` & `herbs-0.2.4/herbs/icons/toolbar/trans.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/triangulation.svg` & `herbs-0.2.4/herbs/icons/toolbar/triangulation.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/two_window.png` & `herbs-0.2.4/herbs/icons/toolbar/two_window.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/unmerge.svg` & `herbs-0.2.4/herbs/icons/toolbar/unmerge.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/v_flip.png` & `herbs-0.2.4/herbs/icons/toolbar/v_flip.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/virus.svg` & `herbs-0.2.4/herbs/icons/toolbar/virus.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/virus_register.svg` & `herbs-0.2.4/herbs/icons/toolbar/virus_register.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/vis2d.svg` & `herbs-0.2.4/herbs/icons/toolbar/vis2d.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/window2.png` & `herbs-0.2.4/herbs/icons/toolbar/window2.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/window3.png` & `herbs-0.2.4/herbs/icons/toolbar/window3.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/toolbar/window4.png` & `herbs-0.2.4/herbs/icons/toolbar/window4.png`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/tree_close.svg` & `herbs-0.2.4/herbs/icons/tree_close.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/tree_open.svg` & `herbs-0.2.4/herbs/icons/tree_open.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/icons/up-arrow.svg` & `herbs-0.2.4/herbs/icons/up-arrow.svg`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/image_curves.py` & `herbs-0.2.4/herbs/image_curves.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/image_reader.py` & `herbs-0.2.4/herbs/image_reader.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/image_stacks.py` & `herbs-0.2.4/herbs/image_stacks.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/image_view.py` & `herbs-0.2.4/herbs/image_view.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/label_tree.py` & `herbs-0.2.4/herbs/label_tree.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/layers_control.py` & `herbs-0.2.4/herbs/layers_control.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/main_window.ui` & `herbs-0.2.4/herbs/main_window.ui`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/movable_points.py` & `herbs-0.2.4/herbs/movable_points.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/obj_items.py` & `herbs-0.2.4/herbs/obj_items.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/object_control.py` & `herbs-0.2.4/herbs/object_control.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/probe_utiles.py` & `herbs-0.2.4/herbs/probe_utiles.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/color_combo.qss` & `herbs-0.2.4/herbs/qss/color_combo.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/label_tree.qss` & `herbs-0.2.4/herbs/qss/label_tree.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/main_window.qss` & `herbs-0.2.4/herbs/qss/main_window.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/menu_bar.qss` & `herbs-0.2.4/herbs/qss/menu_bar.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/multi_handle_slider.qss` & `herbs-0.2.4/herbs/qss/multi_handle_slider.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/obj_ctrl_bottom_button.qss` & `herbs-0.2.4/herbs/qss/obj_ctrl_bottom_button.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/page_control.qss` & `herbs-0.2.4/herbs/qss/page_control.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/side_bar.qss` & `herbs-0.2.4/herbs/qss/side_bar.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/spinbox.qss` & `herbs-0.2.4/herbs/qss/spinbox.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/tabs.qss` & `herbs-0.2.4/herbs/qss/tabs.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/qss/tool_bar.qss` & `herbs-0.2.4/herbs/qss/tool_bar.qss`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/slice_stacks.py` & `herbs-0.2.4/herbs/slice_stacks.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/toolbox.py` & `herbs-0.2.4/herbs/toolbox.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/triangulation_points.py` & `herbs-0.2.4/herbs/triangulation_points.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/uuuuuu.py` & `herbs-0.2.4/herbs/uuuuuu.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/widgets_utils.py` & `herbs-0.2.4/herbs/widgets_utils.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs/wtiles.py` & `herbs-0.2.4/herbs/wtiles.py`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/herbs.egg-info/PKG-INFO` & `herbs-0.2.4/herbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herbs
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python-based GUI for Histological E-data Registration in Brain Space
 Home-page: https://github.com/JingyiGF/HERBS
 Author: Jingyi GF
 Author-email: jingyi.g.fuglstad@gmail.com
 Project-URL: Bug Tracker, https://github.com/JingyiGF/HERBS/issues
 Keywords: brain atlas,histological image registration,probe coordinates
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `herbs-0.2.3/herbs.egg-info/SOURCES.txt` & `herbs-0.2.4/herbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `herbs-0.2.3/setup.py` & `herbs-0.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,26 +50,26 @@
 Operating System :: MacOS
 """
 
 REQUIRES = """
 PyQt5 >= 5.14.2; python_version == "3.8"
 PyQt5 >= 5.15.1; python_version == "3.9"
 PyQt5 >= 5.15.5; python_version == "3.10"
+aicspylibczi >= 3.0.3
 pyqtgraph == 0.12.3
 PyOpenGL >= 3.1.5
 QtRangeSlider == 0.1.5
 opencv-python >= 4.5.4.60
-numba >= 0.54.1
+numba == 0.54.1
 numpy >= 1.20.3
 scipy >= 1.7.3
 requests >= 2.26.0
 nibabel >= 3.2.1
 pynrrd >= 0.4.3
 tifffile >= 2021.11.2
-aicspylibczi == 3.0.3
 pandas >= 1.3.5
 natsort >= 8.0.2
 imagecodecs >= 2022.2.22
 h5py >= 3.7.0
 tables >= 3.7.0
 """
 
@@ -87,15 +87,15 @@
 icons/toolbar/*.png
 qss/*.qss
 """
 
 
 setup(
     name="herbs",
-    version="0.2.3",
+    version="0.2.4",
     author="Jingyi GF",
     author_email="jingyi.g.fuglstad@gmail.com",
     description="A Python-based GUI for Histological E-data Registration in Brain Space",
     keywords="brain atlas, histological image registration, probe coordinates",
     url="https://github.com/JingyiGF/HERBS",
     packages=find_packages(),
     package_data={"": [_f for _f in PACKAGE_DATA.split("\n") if _f]},
```

