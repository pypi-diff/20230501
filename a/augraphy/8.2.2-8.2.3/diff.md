# Comparing `tmp/augraphy-8.2.2.tar.gz` & `tmp/augraphy-8.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augraphy-8.2.2.tar", last modified: Tue Apr 25 01:49:40 2023, max compression
+gzip compressed data, was "augraphy-8.2.3.tar", last modified: Mon May  1 10:18:14 2023, max compression
```

## Comparing `augraphy-8.2.2.tar` & `augraphy-8.2.3.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.202194 augraphy-8.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 01:49:22.000000 augraphy-8.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-25 01:49:40.202194 augraphy-8.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-04-25 01:49:22.000000 augraphy-8.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.194194 augraphy-8.2.2/augraphy/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.198194 augraphy-8.2.2/augraphy/augmentations/
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/badphotocopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/bindingsandfasteners.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/bleedthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/bookbinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/brightnesstexturize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/colorpaper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/delaunay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/dirtydrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/dirtyrollers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/dithering.py
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/faxify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/inkbleed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/jpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/letterpress.py
--rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lightinggradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/linesdegradation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lowinkline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lowinkperiodiclines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/lowinkrandomlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/noisetexturize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/pageborder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/quasicrystal.py
--rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/scribbles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/subtlenoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/voronoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/augmentations/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.198194 augraphy-8.2.2/augraphy/base/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentationpipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentationresult.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/augmentationsequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/oneof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/base/paperfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.198194 augraphy-8.2.2/augraphy/default/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32656 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/default/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.202194 augraphy-8.2.2/augraphy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/composepipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/figsharedownloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/imageoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/meshgenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/noisegenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    35472 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/overlaybuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-25 01:49:22.000000 augraphy-8.2.2/augraphy/utilities/slidingwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:49:40.194194 augraphy-8.2.2/augraphy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-25 01:49:40.000000 augraphy-8.2.2/augraphy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 01:49:39.000000 augraphy-8.2.2/augraphy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 01:49:23.000000 augraphy-8.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:49:40.202194 augraphy-8.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-25 01:49:23.000000 augraphy-8.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:18:14.654090 augraphy-8.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 10:18:00.000000 augraphy-8.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-01 10:18:14.654090 augraphy-8.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-01 10:18:00.000000 augraphy-8.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:18:14.646090 augraphy-8.2.3/augraphy/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:18:14.650090 augraphy-8.2.3/augraphy/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/badphotocopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/bindingsandfasteners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/bleedthrough.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/bookbinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/brightnesstexturize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/colorpaper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/delaunay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/dirtydrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/dirtyrollers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/dithering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/faxify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/inkbleed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/letterpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/lightinggradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/linesdegradation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/lowinkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/lowinkperiodiclines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/lowinkrandomlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/noisetexturize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/pageborder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/quasicrystal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/scribbles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/subtlenoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/augmentations/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:18:14.650090 augraphy-8.2.3/augraphy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/base/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/base/augmentationpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/base/augmentationresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/base/augmentationsequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/base/oneof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/base/paperfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:18:14.650090 augraphy-8.2.3/augraphy/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32649 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/default/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:18:14.650090 augraphy-8.2.3/augraphy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/composepipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/figsharedownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/imageoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35093 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/inkgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/meshgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/noisegenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35472 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/overlaybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/pixelbleed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-01 10:18:00.000000 augraphy-8.2.3/augraphy/utilities/slidingwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:18:14.646090 augraphy-8.2.3/augraphy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-01 10:18:14.000000 augraphy-8.2.3/augraphy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-01 10:18:14.000000 augraphy-8.2.3/augraphy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:18:14.000000 augraphy-8.2.3/augraphy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 10:18:14.000000 augraphy-8.2.3/augraphy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 10:18:14.000000 augraphy-8.2.3/augraphy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 10:18:00.000000 augraphy-8.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:18:14.654090 augraphy-8.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-01 10:18:00.000000 augraphy-8.2.3/setup.py
```

### Comparing `augraphy-8.2.2/LICENSE` & `augraphy-8.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/PKG-INFO` & `augraphy-8.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augraphy
-Version: 8.2.2
+Version: 8.2.3
 Summary: Augmentation pipeline for rendering synthetic paper printing and scanning processes
 Home-page: https://github.com/sparkfish/augraphy
 Author: Sparkfish LLC
 Author-email: packages@sparkfish.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sparkfish/augraphy/issues
 Description: <p align="center">
@@ -36,15 +36,17 @@
         The end result is an image that mimics real documents.
         
         <p align="center" width="100%">
             <img src="https://github.com/sparkfish/augraphy/blob/dev/images/Pipeline.png?raw=true">
         </p>
         
         ## Example Before / After Images
-        ![examples](https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png)
+        <p align="center" width="100%">
+            <img src="https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png?raw=true">
+        </p>
         
         
         # Example Usage
         To use the default pipeline which contains all available augmentations and sensible defaults:
         
         ```python
         from augraphy import *
@@ -85,15 +87,15 @@
         |Letterpress         |             0.23|           158.60|
         |LightingGradient    |             0.34|           638.31|
         |LowInkPeriodicLines |             2.94|            12.74|
         |LowInkRandomLines   |            71.05|            12.74|
         |Markup              |             0.71|           533.16|
         |NoiseTexturize      |             0.53|           249.36|
         |PageBorder          |             0.52|           465.19|
-        |PencilScribbles     |             1.15|           138.13|
+        |Scribbles           |             1.15|           138.13|
         |SubtleNoise         |             1.03|           202.87|
         |WaterMark           |             1.19|           373.41|
         |VoronoiTessellation |             0.47|            15.90|
         |DelaunayTessellation|             0.76|            36.33|
         |Quasi Crystals      |             0.25|              7.5|
         
         # Alternative Augmentation Libraries
@@ -107,15 +109,15 @@
         
         BibTeX:
         ```
         @software{augraphy_library,
             author = {The Augraphy Project},
             title = {Augraphy: an augmentation pipeline for rendering synthetic paper printing, faxing, scanning and copy machine processes},
             url = {https://github.com/sparkfish/augraphy},
-            version = {8.2.2}
+            version = {8.2.3}
         }
         ```
         
         # License
         Copyright 2023 Sparkfish LLC
         
         Augraphy is free and open-source software distributed under the terms of the [**MIT**](https://github.com/sparkfish/augraphy/blob/dev/LICENSE) license.
```

### Comparing `augraphy-8.2.2/README.md` & `augraphy-8.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 The end result is an image that mimics real documents.
 
 <p align="center" width="100%">
     <img src="https://github.com/sparkfish/augraphy/blob/dev/images/Pipeline.png?raw=true">
 </p>
 
 ## Example Before / After Images
-![examples](https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png)
+<p align="center" width="100%">
+    <img src="https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png?raw=true">
+</p>
 
 
 # Example Usage
 To use the default pipeline which contains all available augmentations and sensible defaults:
 
 ```python
 from augraphy import *
@@ -76,15 +78,15 @@
 |Letterpress         |             0.23|           158.60|
 |LightingGradient    |             0.34|           638.31|
 |LowInkPeriodicLines |             2.94|            12.74|
 |LowInkRandomLines   |            71.05|            12.74|
 |Markup              |             0.71|           533.16|
 |NoiseTexturize      |             0.53|           249.36|
 |PageBorder          |             0.52|           465.19|
-|PencilScribbles     |             1.15|           138.13|
+|Scribbles           |             1.15|           138.13|
 |SubtleNoise         |             1.03|           202.87|
 |WaterMark           |             1.19|           373.41|
 |VoronoiTessellation |             0.47|            15.90|
 |DelaunayTessellation|             0.76|            36.33|
 |Quasi Crystals      |             0.25|              7.5|
 
 # Alternative Augmentation Libraries
@@ -98,15 +100,15 @@
 
 BibTeX:
 ```
 @software{augraphy_library,
     author = {The Augraphy Project},
     title = {Augraphy: an augmentation pipeline for rendering synthetic paper printing, faxing, scanning and copy machine processes},
     url = {https://github.com/sparkfish/augraphy},
-    version = {8.2.2}
+    version = {8.2.3}
 }
 ```
 
 # License
 Copyright 2023 Sparkfish LLC
 
 Augraphy is free and open-source software distributed under the terms of the [**MIT**](https://github.com/sparkfish/augraphy/blob/dev/LICENSE) license.
```

### Comparing `augraphy-8.2.2/augraphy/augmentations/__init__.py` & `augraphy-8.2.3/augraphy/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/badphotocopy.py` & `augraphy-8.2.3/augraphy/augmentations/badphotocopy.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/bindingsandfasteners.py` & `augraphy-8.2.3/augraphy/augmentations/bindingsandfasteners.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/bleedthrough.py` & `augraphy-8.2.3/augraphy/augmentations/bleedthrough.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/bookbinding.py` & `augraphy-8.2.3/augraphy/augmentations/bookbinding.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/brightness.py` & `augraphy-8.2.3/augraphy/augmentations/brightness.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/brightnesstexturize.py` & `augraphy-8.2.3/augraphy/augmentations/brightnesstexturize.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/colorpaper.py` & `augraphy-8.2.3/augraphy/augmentations/colorpaper.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/delaunay.py` & `augraphy-8.2.3/augraphy/augmentations/delaunay.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/dirtydrum.py` & `augraphy-8.2.3/augraphy/augmentations/dirtydrum.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/dirtyrollers.py` & `augraphy-8.2.3/augraphy/augmentations/dirtyrollers.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/dithering.py` & `augraphy-8.2.3/augraphy/augmentations/dithering.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/faxify.py` & `augraphy-8.2.3/augraphy/augmentations/faxify.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/folding.py` & `augraphy-8.2.3/augraphy/augmentations/folding.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/gamma.py` & `augraphy-8.2.3/augraphy/augmentations/gamma.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/geometric.py` & `augraphy-8.2.3/augraphy/augmentations/geometric.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/inkbleed.py` & `augraphy-8.2.3/augraphy/augmentations/inkbleed.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/jpeg.py` & `augraphy-8.2.3/augraphy/augmentations/jpeg.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/letterpress.py` & `augraphy-8.2.3/augraphy/augmentations/letterpress.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/lib.py` & `augraphy-8.2.3/augraphy/augmentations/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,16 @@
     # find indices where sobelized image value == 255 and random value < intensity
     if noise_condition == 0:
         condition_evaluation = checking_image == 0
     elif noise_condition == 1:
         condition_evaluation = checking_image == 255
     elif noise_condition == 2:
         condition_evaluation = checking_image > 255
+    elif noise_condition == 4:
+        condition_evaluation = checking_image < 255
 
     condition_evaluation2 = random_value < intensity
     indices = np.logical_and(condition_evaluation, condition_evaluation2)
 
     # output
     image_noise = image.copy()
```

### Comparing `augraphy-8.2.2/augraphy/augmentations/lightinggradient.py` & `augraphy-8.2.3/augraphy/augmentations/lightinggradient.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/linesdegradation.py` & `augraphy-8.2.3/augraphy/augmentations/linesdegradation.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/lowinkline.py` & `augraphy-8.2.3/augraphy/augmentations/lowinkline.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/lowinkperiodiclines.py` & `augraphy-8.2.3/augraphy/augmentations/lowinkperiodiclines.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/lowinkrandomlines.py` & `augraphy-8.2.3/augraphy/augmentations/lowinkrandomlines.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/markup.py` & `augraphy-8.2.3/augraphy/augmentations/markup.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/noisetexturize.py` & `augraphy-8.2.3/augraphy/augmentations/noisetexturize.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/pageborder.py` & `augraphy-8.2.3/augraphy/augmentations/pageborder.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/quasicrystal.py` & `augraphy-8.2.3/augraphy/augmentations/quasicrystal.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/subtlenoise.py` & `augraphy-8.2.3/augraphy/augmentations/subtlenoise.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/voronoi.py` & `augraphy-8.2.3/augraphy/augmentations/voronoi.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/augmentations/watermark.py` & `augraphy-8.2.3/augraphy/augmentations/watermark.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/base/augmentation.py` & `augraphy-8.2.3/augraphy/base/augmentation.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/base/augmentationpipeline.py` & `augraphy-8.2.3/augraphy/base/augmentationpipeline.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/base/augmentationresult.py` & `augraphy-8.2.3/augraphy/base/augmentationresult.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/base/augmentationsequence.py` & `augraphy-8.2.3/augraphy/base/augmentationsequence.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/base/oneof.py` & `augraphy-8.2.3/augraphy/base/oneof.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/base/paperfactory.py` & `augraphy-8.2.3/augraphy/base/paperfactory.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/default/pipeline.py` & `augraphy-8.2.3/augraphy/default/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,19 +360,19 @@
             scribbles_type="text",
             scribbles_ink="pencil",
             scribbles_location=(0.5, 0.95),
             scribbles_size_range=(700, 700),
             scribbles_count_range=(1, 1),
             scribbles_thickness_range=(1, 1),
             scribbles_brightness_change=[0],
+            scribbles_skeletonize=0,
             scribbles_color=(0, 0, 0),
             scribbles_text="P·142",
             scribbles_text_font="random",
             scribbles_text_rotate_range=(3, 3),
-            scribbles_pencil_skeletonize=0,
         ),
         BadPhotoCopy(
             noise_type=1,
             noise_side="bottom",
             noise_iteration=(1, 1),
             noise_size=(5, 7),
             noise_value=(0, 64),
@@ -740,15 +740,15 @@
             kernel_size=(3, 3),
             severity=(1.0, 1.0),
         ),
         Scribbles(
             scribbles_type="text",
             scribbles_ink="pen",
             scribbles_location=(0.8, 0.8),
-            scribbles_size_range=(650, 650),
+            scribbles_size_range=(320, 320),
             scribbles_count_range=(1, 1),
             scribbles_thickness_range=(2, 2),
             scribbles_brightness_change=[0],
             scribbles_color=(0, 0, 0),
             scribbles_text="Dr Architg \n \n  Dr Lynn added that \n me to Dereene etan \n with you . He feel that \n we should stay away \n from the mystery that could \n help to .FTC on  \n In attend the president \n of the committee \n       Cloude ",
             scribbles_text_font="https://www.fontsquirrel.com/fonts/download/Windsong",
             scribbles_text_rotate_range=(15, 15),
```

### Comparing `augraphy-8.2.2/augraphy/utilities/__init__.py` & `augraphy-8.2.3/augraphy/utilities/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from augraphy.utilities.composepipelines import ComposePipelines
 from augraphy.utilities.figsharedownloader import FigshareDownloader
 from augraphy.utilities.function import Function
 from augraphy.utilities.imageoverlay import ImageOverlay
+from augraphy.utilities.inkgenerator import InkGenerator
 from augraphy.utilities.interop import Interop
 from augraphy.utilities.meshgenerator import Noise
 from augraphy.utilities.noisegenerator import NoiseGenerator
 from augraphy.utilities.overlaybuilder import OverlayBuilder
+from augraphy.utilities.pixelbleed import PixelBleed
 from augraphy.utilities.slidingwindow import PatternMaker
 
 __all__ = [
     "ComposePipelines",
     "FigshareDownloader",
     "Function",
     "ImageOverlay",
+    "InkGenerator",
     "Interop",
     "OverlayBuilder",
     "Noise",
     "NoiseGenerator",
     "PatternMaker",
+    "PixelBleed",
 ]
```

### Comparing `augraphy-8.2.2/augraphy/utilities/composepipelines.py` & `augraphy-8.2.3/augraphy/utilities/composepipelines.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/figsharedownloader.py` & `augraphy-8.2.3/augraphy/utilities/figsharedownloader.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/function.py` & `augraphy-8.2.3/augraphy/utilities/function.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/imageoverlay.py` & `augraphy-8.2.3/augraphy/utilities/imageoverlay.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/interop.py` & `augraphy-8.2.3/augraphy/utilities/interop.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/meshgenerator.py` & `augraphy-8.2.3/augraphy/utilities/meshgenerator.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/noisegenerator.py` & `augraphy-8.2.3/augraphy/utilities/noisegenerator.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/overlaybuilder.py` & `augraphy-8.2.3/augraphy/utilities/overlaybuilder.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy/utilities/slidingwindow.py` & `augraphy-8.2.3/augraphy/utilities/slidingwindow.py`

 * *Files identical despite different names*

### Comparing `augraphy-8.2.2/augraphy.egg-info/PKG-INFO` & `augraphy-8.2.3/augraphy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augraphy
-Version: 8.2.2
+Version: 8.2.3
 Summary: Augmentation pipeline for rendering synthetic paper printing and scanning processes
 Home-page: https://github.com/sparkfish/augraphy
 Author: Sparkfish LLC
 Author-email: packages@sparkfish.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sparkfish/augraphy/issues
 Description: <p align="center">
@@ -36,15 +36,17 @@
         The end result is an image that mimics real documents.
         
         <p align="center" width="100%">
             <img src="https://github.com/sparkfish/augraphy/blob/dev/images/Pipeline.png?raw=true">
         </p>
         
         ## Example Before / After Images
-        ![examples](https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png)
+        <p align="center" width="100%">
+            <img src="https://github.com/sparkfish/augraphy/blob/dev/images/basic_examples.png?raw=true">
+        </p>
         
         
         # Example Usage
         To use the default pipeline which contains all available augmentations and sensible defaults:
         
         ```python
         from augraphy import *
@@ -85,15 +87,15 @@
         |Letterpress         |             0.23|           158.60|
         |LightingGradient    |             0.34|           638.31|
         |LowInkPeriodicLines |             2.94|            12.74|
         |LowInkRandomLines   |            71.05|            12.74|
         |Markup              |             0.71|           533.16|
         |NoiseTexturize      |             0.53|           249.36|
         |PageBorder          |             0.52|           465.19|
-        |PencilScribbles     |             1.15|           138.13|
+        |Scribbles           |             1.15|           138.13|
         |SubtleNoise         |             1.03|           202.87|
         |WaterMark           |             1.19|           373.41|
         |VoronoiTessellation |             0.47|            15.90|
         |DelaunayTessellation|             0.76|            36.33|
         |Quasi Crystals      |             0.25|              7.5|
         
         # Alternative Augmentation Libraries
@@ -107,15 +109,15 @@
         
         BibTeX:
         ```
         @software{augraphy_library,
             author = {The Augraphy Project},
             title = {Augraphy: an augmentation pipeline for rendering synthetic paper printing, faxing, scanning and copy machine processes},
             url = {https://github.com/sparkfish/augraphy},
-            version = {8.2.2}
+            version = {8.2.3}
         }
         ```
         
         # License
         Copyright 2023 Sparkfish LLC
         
         Augraphy is free and open-source software distributed under the terms of the [**MIT**](https://github.com/sparkfish/augraphy/blob/dev/LICENSE) license.
```

### Comparing `augraphy-8.2.2/augraphy.egg-info/SOURCES.txt` & `augraphy-8.2.3/augraphy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -51,12 +51,14 @@
 augraphy/default/__init__.py
 augraphy/default/pipeline.py
 augraphy/utilities/__init__.py
 augraphy/utilities/composepipelines.py
 augraphy/utilities/figsharedownloader.py
 augraphy/utilities/function.py
 augraphy/utilities/imageoverlay.py
+augraphy/utilities/inkgenerator.py
 augraphy/utilities/interop.py
 augraphy/utilities/meshgenerator.py
 augraphy/utilities/noisegenerator.py
 augraphy/utilities/overlaybuilder.py
+augraphy/utilities/pixelbleed.py
 augraphy/utilities/slidingwindow.py
```

### Comparing `augraphy-8.2.2/setup.py` & `augraphy-8.2.3/setup.py`

 * *Files identical despite different names*

