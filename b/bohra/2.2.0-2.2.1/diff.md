# Comparing `tmp/bohra-2.2.0.tar.gz` & `tmp/bohra-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bohra-2.2.0.tar", last modified: Mon Apr 24 04:09:57 2023, max compression
+gzip compressed data, was "dist/bohra-2.2.1.tar", last modified: Mon May  1 07:21:22 2023, max compression
```

## Comparing `bohra-2.2.0.tar` & `bohra-2.2.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35149 2019-07-28 01:44:48.000000 bohra-2.2.0/LICENSE.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      202 2021-08-27 05:57:12.000000 bohra-2.2.0/MANIFEST.in
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    16293 2023-04-24 04:09:57.000000 bohra-2.2.0/PKG-INFO
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    13280 2023-03-31 02:22:29.000000 bohra-2.2.0/README.md
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      769 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/CustomLog.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    30708 2023-04-24 03:55:45.000000 bohra-2.2.0/bohra/SnpDetection.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     8434 2020-03-12 06:16:45.000000 bohra-2.2.0/bohra/Utils.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      216 2019-08-07 06:34:59.000000 bohra-2.2.0/bohra/__init__.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9065 2023-04-24 03:56:33.000000 bohra-2.2.0/bohra/bohra.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     5409 2023-04-04 03:44:06.000000 bohra-2.2.0/bohra/main.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/collation/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/collation/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      710 2021-11-18 03:36:53.000000 bohra-2.2.0/bohra/modules/collation/bin/add_header_mlst.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1480 2021-12-19 02:04:48.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_asm.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      664 2021-11-09 04:29:51.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_kraken2.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      343 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_plasmids.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     2517 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_stats.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    13486 2022-03-05 01:26:46.000000 bohra-2.2.0/bohra/modules/collation/bin/compile.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1405 2021-10-05 07:55:10.000000 bohra-2.2.0/bohra/modules/collation/bin/snippy_qc.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      598 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/bin/wrangle_mobsuite.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     7114 2023-03-31 02:12:30.000000 bohra-2.2.0/bohra/modules/collation/main.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/csvtk/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/csvtk/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1140 2023-03-31 01:20:40.000000 bohra-2.2.0/bohra/modules/csvtk/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/csvtk/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/gubbins/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/gubbins/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1020 2023-03-31 01:20:31.000000 bohra-2.2.0/bohra/modules/gubbins/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/gubbins/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/iqtree/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/iqtree/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1212 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/iqtree/bin/iqtree_generator.sh
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/iqtree/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1229 2023-03-31 01:20:24.000000 bohra-2.2.0/bohra/modules/iqtree/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/iqtree/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/kraken2/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/kraken2/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1282 2023-03-31 01:20:15.000000 bohra-2.2.0/bohra/modules/kraken2/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/kraken2/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mash/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mash/sketch/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/sketch/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1415 2023-03-31 01:20:11.000000 bohra-2.2.0/bohra/modules/mash/sketch/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/sketch/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mash/triangle/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/triangle/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1069 2023-03-31 01:20:06.000000 bohra-2.2.0/bohra/modules/mash/triangle/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/triangle/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mlst/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mlst/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1427 2023-03-31 06:32:25.000000 bohra-2.2.0/bohra/modules/mlst/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1721 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mlst/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mobsuite/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mobsuite/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1349 2023-03-31 01:19:55.000000 bohra-2.2.0/bohra/modules/mobsuite/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mobsuite/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/panaroo/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-09-03 10:18:11.000000 bohra-2.2.0/bohra/modules/panaroo/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1414 2023-04-24 03:58:15.000000 bohra-2.2.0/bohra/modules/panaroo/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-09-03 10:18:11.000000 bohra-2.2.0/bohra/modules/panaroo/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/prokka/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/prokka/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1285 2023-03-31 01:19:42.000000 bohra-2.2.0/bohra/modules/prokka/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/prokka/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/quicktree/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/quicktree/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1090 2023-03-31 01:19:37.000000 bohra-2.2.0/bohra/modules/quicktree/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/quicktree/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/resistome/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/resistome/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1118 2021-11-11 03:19:28.000000 bohra-2.2.0/bohra/modules/resistome/bin/combine.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/bin/concat.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1789 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/bin/meta.yaml
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2940 2023-03-31 01:19:31.000000 bohra-2.2.0/bohra/modules/resistome/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1834 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/roary2svg/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/roary2svg/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     5179 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/bin/roary2svg.pl
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      712 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqkit/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1461 2023-03-31 01:19:19.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqkit/stats/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/stats/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1570 2023-03-31 01:19:14.000000 bohra-2.2.0/bohra/modules/seqkit/stats/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/stats/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqtk/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqtk/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1132 2023-03-31 01:21:08.000000 bohra-2.2.0/bohra/modules/seqtk/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqtk/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/shovill/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/shovill/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1295 2023-03-31 01:21:34.000000 bohra-2.2.0/bohra/modules/shovill/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/shovill/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/skesa/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/skesa/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1277 2023-03-31 01:21:53.000000 bohra-2.2.0/bohra/modules/skesa/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/skesa/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snippy/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-28 02:54:18.000000 bohra-2.2.0/bohra/modules/snippy/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1663 2023-04-13 00:09:28.000000 bohra-2.2.0/bohra/modules/snippy/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snippy/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snippy_clean/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-03-31 00:49:55.000000 bohra-2.2.0/bohra/modules/snippy_clean/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      944 2023-03-31 01:22:37.000000 bohra-2.2.0/bohra/modules/snippy_clean/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2023-03-31 00:49:55.000000 bohra-2.2.0/bohra/modules/snippy_clean/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snippy_core/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snippy_core/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1350 2023-03-31 01:22:43.000000 bohra-2.2.0/bohra/modules/snippy_core/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snippy_core/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snp_dists/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snp_dists/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1095 2023-03-31 01:23:35.000000 bohra-2.2.0/bohra/modules/snp_dists/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snp_dists/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/spades/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/spades/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1406 2023-03-31 01:23:33.000000 bohra-2.2.0/bohra/modules/spades/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/spades/meta.yml
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1963 2023-03-31 01:27:18.000000 bohra-2.2.0/bohra/nextflow.config
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/templates/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      932 2019-09-21 05:50:22.000000 bohra-2.2.0/bohra/templates/cluster.tmpl
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      806 2021-02-23 06:36:40.000000 bohra-2.2.0/bohra/templates/config_snippy.yaml
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    17031 2021-11-23 01:23:44.000000 bohra-2.2.0/bohra/templates/index.html
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    17104 2021-11-22 01:20:59.000000 bohra-2.2.0/bohra/templates/report_analysis.json
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/tests/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test.bed
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)  7163607 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test.gbk
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      788 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test.tab
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2172 2021-08-29 03:00:41.000000 bohra-2.2.0/bohra/tests/test_bohra.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test_file.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       17 2023-04-24 04:02:07.000000 bohra-2.2.0/bohra/version.py
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/workflows/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2577 2023-03-31 06:22:16.000000 bohra-2.2.0/bohra/workflows/assemble_typing.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/workflows/collation.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1519 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/workflows/common.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4714 2023-03-31 06:22:16.000000 bohra-2.2.0/bohra/workflows/default.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      375 2021-10-05 08:04:23.000000 bohra-2.2.0/bohra/workflows/pangenome.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      402 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/workflows/preview.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    16293 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/PKG-INFO
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3728 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/SOURCES.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/dependency_links.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       44 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/entry_points.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2019-08-07 06:36:45.000000 bohra-2.2.0/bohra.egg-info/not-zip-safe
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      117 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/requires.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        6 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/top_level.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1131 2023-04-24 04:09:57.000000 bohra-2.2.0/setup.cfg
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       69 2020-03-06 03:52:01.000000 bohra-2.2.0/setup.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35149 2019-07-28 01:44:48.000000 bohra-2.2.1/LICENSE.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      202 2021-08-27 05:57:12.000000 bohra-2.2.1/MANIFEST.in
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    12805 2023-05-01 07:21:22.000000 bohra-2.2.1/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    10272 2023-04-24 05:05:44.000000 bohra-2.2.1/README.md
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      769 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/CustomLog.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    30708 2023-04-24 03:55:45.000000 bohra-2.2.1/bohra/SnpDetection.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     8434 2020-03-12 06:16:45.000000 bohra-2.2.1/bohra/Utils.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      216 2019-08-07 06:34:59.000000 bohra-2.2.1/bohra/__init__.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9065 2023-04-24 05:09:25.000000 bohra-2.2.1/bohra/bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     5409 2023-04-04 03:44:06.000000 bohra-2.2.1/bohra/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/collation/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/collation/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      710 2021-11-18 03:36:53.000000 bohra-2.2.1/bohra/modules/collation/bin/add_header_mlst.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1480 2021-12-19 02:04:48.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_asm.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      664 2021-11-09 04:29:51.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_kraken2.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      343 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_plasmids.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     2517 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_stats.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    13486 2022-03-05 01:26:46.000000 bohra-2.2.1/bohra/modules/collation/bin/compile.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1405 2021-10-05 07:55:10.000000 bohra-2.2.1/bohra/modules/collation/bin/snippy_qc.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      598 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/bin/wrangle_mobsuite.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     7114 2023-03-31 02:12:30.000000 bohra-2.2.1/bohra/modules/collation/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/csvtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/csvtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1140 2023-03-31 01:20:40.000000 bohra-2.2.1/bohra/modules/csvtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/csvtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/gubbins/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/gubbins/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1021 2023-05-01 06:55:31.000000 bohra-2.2.1/bohra/modules/gubbins/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/gubbins/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/iqtree/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/iqtree/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1212 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/iqtree/bin/iqtree_generator.sh
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/iqtree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1229 2023-03-31 01:20:24.000000 bohra-2.2.1/bohra/modules/iqtree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/iqtree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/kraken2/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/kraken2/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1282 2023-03-31 01:20:15.000000 bohra-2.2.1/bohra/modules/kraken2/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/kraken2/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mash/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mash/sketch/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/sketch/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1415 2023-03-31 01:20:11.000000 bohra-2.2.1/bohra/modules/mash/sketch/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/sketch/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mash/triangle/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/triangle/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1069 2023-03-31 01:20:06.000000 bohra-2.2.1/bohra/modules/mash/triangle/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/triangle/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mlst/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mlst/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1427 2023-03-31 06:32:25.000000 bohra-2.2.1/bohra/modules/mlst/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1721 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mlst/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mobsuite/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mobsuite/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1349 2023-03-31 01:19:55.000000 bohra-2.2.1/bohra/modules/mobsuite/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mobsuite/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/panaroo/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-09-03 10:18:11.000000 bohra-2.2.1/bohra/modules/panaroo/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1414 2023-04-24 03:58:15.000000 bohra-2.2.1/bohra/modules/panaroo/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-09-03 10:18:11.000000 bohra-2.2.1/bohra/modules/panaroo/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/prokka/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/prokka/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1285 2023-03-31 01:19:42.000000 bohra-2.2.1/bohra/modules/prokka/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/prokka/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/quicktree/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/quicktree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1090 2023-03-31 01:19:37.000000 bohra-2.2.1/bohra/modules/quicktree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/quicktree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/resistome/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/resistome/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1118 2021-11-11 03:19:28.000000 bohra-2.2.1/bohra/modules/resistome/bin/combine.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/bin/concat.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1789 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/bin/meta.yaml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2940 2023-03-31 01:19:31.000000 bohra-2.2.1/bohra/modules/resistome/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1834 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/roary2svg/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/roary2svg/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     5179 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/bin/roary2svg.pl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      712 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqkit/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1461 2023-03-31 01:19:19.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqkit/stats/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/stats/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1570 2023-03-31 01:19:14.000000 bohra-2.2.1/bohra/modules/seqkit/stats/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/stats/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1132 2023-03-31 01:21:08.000000 bohra-2.2.1/bohra/modules/seqtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/shovill/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/shovill/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1295 2023-03-31 01:21:34.000000 bohra-2.2.1/bohra/modules/shovill/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/shovill/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/skesa/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/skesa/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1277 2023-03-31 01:21:53.000000 bohra-2.2.1/bohra/modules/skesa/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/skesa/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snippy/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-28 02:54:18.000000 bohra-2.2.1/bohra/modules/snippy/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1663 2023-04-13 00:09:28.000000 bohra-2.2.1/bohra/modules/snippy/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snippy/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snippy_clean/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-03-31 00:49:55.000000 bohra-2.2.1/bohra/modules/snippy_clean/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      944 2023-03-31 01:22:37.000000 bohra-2.2.1/bohra/modules/snippy_clean/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2023-03-31 00:49:55.000000 bohra-2.2.1/bohra/modules/snippy_clean/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snippy_core/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snippy_core/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1350 2023-03-31 01:22:43.000000 bohra-2.2.1/bohra/modules/snippy_core/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snippy_core/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snp_dists/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snp_dists/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1095 2023-03-31 01:23:35.000000 bohra-2.2.1/bohra/modules/snp_dists/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snp_dists/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/spades/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/spades/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1406 2023-03-31 01:23:33.000000 bohra-2.2.1/bohra/modules/spades/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/spades/meta.yml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1963 2023-03-31 01:27:18.000000 bohra-2.2.1/bohra/nextflow.config
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/templates/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      932 2019-09-21 05:50:22.000000 bohra-2.2.1/bohra/templates/cluster.tmpl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      806 2021-02-23 06:36:40.000000 bohra-2.2.1/bohra/templates/config_snippy.yaml
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    17031 2021-11-23 01:23:44.000000 bohra-2.2.1/bohra/templates/index.html
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    17104 2021-11-22 01:20:59.000000 bohra-2.2.1/bohra/templates/report_analysis.json
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/tests/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test.bed
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)  7163607 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test.gbk
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      788 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test.tab
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2172 2021-08-29 03:00:41.000000 bohra-2.2.1/bohra/tests/test_bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test_file.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       17 2023-05-01 07:12:48.000000 bohra-2.2.1/bohra/version.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/workflows/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2577 2023-03-31 06:22:16.000000 bohra-2.2.1/bohra/workflows/assemble_typing.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/workflows/collation.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1519 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/workflows/common.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4714 2023-03-31 06:22:16.000000 bohra-2.2.1/bohra/workflows/default.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      375 2021-10-05 08:04:23.000000 bohra-2.2.1/bohra/workflows/pangenome.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      402 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/workflows/preview.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    12805 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3728 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/SOURCES.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/dependency_links.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       44 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/entry_points.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2019-08-07 06:36:45.000000 bohra-2.2.1/bohra.egg-info/not-zip-safe
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      108 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/requires.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        6 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/top_level.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1122 2023-05-01 07:21:22.000000 bohra-2.2.1/setup.cfg
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       69 2020-03-06 03:52:01.000000 bohra-2.2.1/setup.py
```

### Comparing `bohra-2.2.0/LICENSE.txt` & `bohra-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/PKG-INFO` & `bohra-2.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: bohra
-Version: 2.2.0
+Version: 2.2.1
 Summary: A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
 Home-page: https://github.com/kristyhoran/bohra
 Author: Kristy Horan
 Author-email: kristyhoran15@gmail.com
 License: UNKNOWN
-Description: [![CircleCI](https://circleci.com/gh/MDU-PHL/bohra.svg?style=svg&circle-token=530799cb0764519fc65966ab48bac7e0d02f3688)](https://circleci.com/gh/MDU-PHL/bohra)
-        [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-        
+Description: <!-- [![CircleCI](https://circleci.com/gh/MDU-PHL/bohra.svg?style=svg&circle-token=530799cb0764519fc65966ab48bac7e0d02f3688)](https://circleci.com/gh/MDU-PHL/bohra) -->
+        [![Python 3.7](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-370/)
         
         
         # Bohra
         
         Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. At a minimum the pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
         
-        ## Bohra has a new look! Welcome to Bohra-NF
-        
-        **New features**
-        
         * Pipeline written in [Nextflow](https://www.nextflow.io)
         * Default mode
             * Can be run on a single isolate (phylogenetic tree will not be generated if fewer than three sequences included in dataset)
             * MobSuite integration.
             * Updated [abriTAMR](https://github.com/MDU-PHL/abritamr) with support for point mutations and virulence factors (beta).
         * Panaroo with visualisation of pan-genome.
         * Improved support for different computing environments.
         
+        ## Recent changes to bohra
+        * Each bohra process is now run in its own conda environment. These will by default be included in your working directory.
+        * Alternatively you can install your own conda environments and provide the path to where these can be found (see help below).
+        * If you wish you can maintain the existing structure - where all the dependencies are installed in a single environment. BEWARE this can cause unexpected behaviour and even cause the pipeline to fail. If you wish to run bohra in this way please contact us for advice.
+        
         **Comming soon**
         
         * Improved report structure
-        * Option to add your own modules
+        * Baby kraken
+        * Typing (_Salmonella_ spp., _Listeria monocytogenes_, _Neiserria_)
+        * Mtb AMR
         
         
         **Accreditation**
         
         * _snippy and snippy-core version 4.4.5 are NATA accredited for accurate detection of SNPs for reporting of genomic relationships at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
         * _abritamr is accredited for detection of AMR genes at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
         
@@ -77,43 +79,53 @@
         * MLST
         * Resistome
         * Annotate
         * Plasmid prediction
         * Species identification
         * Pan Genome
         
-        ### Installation
-        
-        **New installation instructions comming soon**
-        
-        Bohra requires >=python3.7
+        ### Installation (with conda)
         
-        #### Conda (Highly recomended)
+        Bohra requires >=python3.9 and conda
         
-        Installing bohra with conda will ensure that all dependencies are present. See below for instructions on how to configure the databases for kraken2.
+        See below for instructions on how to configure the databases for kraken2.
         
-        Set up conda - documentation for conda installation can be found [here](https://conda.io/en/latest/miniconda.html)
+        1. Set up conda - documentation for conda installation can be found [here](https://conda.io/en/latest/miniconda.html)
         ```
         conda config --add channels defaults
         conda config --add channels bioconda
         conda config --add channels conda-forge
         ```
-        It is recomended that you set up a `bohra` environment
-        ```
-        conda create -n <bohra_env_name> bohra
-        ```
-        To use bohra
+        
+        2. Create the conda environment
         ```
+        conda create -n <bohra_env_name> bohra python=3.9
         conda activate <bohra_env_name>
         ```
-        #### PyPi
-        If installing with `pip` you will need to ensure other dependencies are also installed.
+        You can also install `bohra` with 
         ```
         pip3 install bohra
         ```
+        
+        3. Ensure that you have a kraken2 database. Minikraken can obtained as follows
+        ```
+        wget ftp://ftp.ccb.jhu.edu/pub/data/kraken2_dbs/minikraken2_v2_8GB_201904_UPDATE.tgz
+        tar -C $HOME -zxvf minikraken2_v2_8GB_201904_UPDATE.tgz
+        ```
+        This will download and unzip the kraken2 DB. Other kraken2 DB are also available, you can find more information [here](https://ccb.jhu.edu/software/kraken2/index.shtml?t=downloads)
+        
+        Once you have the DB downloaded you will have to create an environment variable called `KRAKEN2_DEFAULT_DB`. This can be done by adding the following to your `$HOME/.bashrc`
+        ```
+        export KRAKEN_DEFAULT_DB=$HOME/minikraken2_v2_8GB_201904_UPDATE
+        ```
+        
+        #### Recommended conda environments (for the brave)
+        
+        If you would like to use pre-installed conda envs - the following are suggested. You may also attempt to install all these dependencies into a single conda environment - however it is not recomended as there may be significant dependency clashes.
+        
         * [Snippy (v4.4.5 recommended)](https://github.com/tseemann/snippy)
         * [Shovill (skesa and spades.py)](https://github.com/tseemann/shovill)
         * [Panaroo](https://github.com/gtonkinhill/panaroo)
         * [Prokka](https://github.com/tseemann/prokka)
         * [kraken2](https://ccb.jhu.edu/software/kraken/)
         * [abritamr](https://github.com/MDU-PHL/abritamr)
         * [mlst](https://github.com/tseemann/mlst)
@@ -121,122 +133,35 @@
         * [seqtk](https://github.com/lh3/seqtk)
         * [snp-dists](https://github.com/tseemann/snp-dists)
         * [mash](https://github.com/lskatz/mashtree)
         * [mob_suite](https://github.com/phac-nml/mob-suite)
         * [csvtk](https://github.com/shenwei356/csvtk)
         
         
-        #### Check installation
-        
-        Check that all dependencies are installed.
-        
-        ```
-        bohra check
-        ```
-        
-        *IMPORTANT*
-        
-        In addition to installing kraken ensure that you have a kraken2 database. Minikraken can obtained as follows
-        ```
-        wget ftp://ftp.ccb.jhu.edu/pub/data/kraken2_dbs/minikraken2_v2_8GB_201904_UPDATE.tgz
-        tar -C $HOME -zxvf minikraken2_v2_8GB_201904_UPDATE.tgz
-        ```
-        This will download and unzip the kraken2 DB. Other kraken2 DB are also available, you can find more information [here](https://ccb.jhu.edu/software/kraken2/index.shtml?t=downloads)
-        
-        Once you have the DB downloaded you will have to create an environment variable called `KRAKEN2_DEFAULT_DB`. This can be done by adding the following to your `$HOME/.bashrc`
-        ```
-        export KRAKEN_DEFAULT_DB=$HOME/minikraken2_v2_8GB_201904_UPDATE
-        ```
         
         ### Running bohra
         
         **A word on resources**
         
         * A minimum of 8 cpus is required for running `bohra`
         * `bohra` has default settings for running at MDU (both on research and service systems). These ensure optimal running on these systems.
         * Whether you are running `bohra` on MDU systems or not, you can override the default max cpus, by providing an upper limit for your job using the `--cpus` flag.
         * If you are running on a queue or in the cloud you will need to provide an additional config file with details of your profile requirements.
         
         #### Using CLI
         
-        ```
-        $ bohra run -h
-        
-        Bohra - a bacterial genomics pipeline - version 2.0.0
+        **`bohra generate_input`**
         
-         -h, --help            show this help message and exit
-          -v, --version         show program's version number and exit
-          --check               Check that dependencies are installed correctly.
-                                (default: False)
-          --input_file INPUT_FILE, -i INPUT_FILE
-                                Path to reads file, which is a tab-delimited with 3
-                                columns <isolatename> <path_to_read1> <path_to_read2>.
-                                REQUIRED (default: )
-          --contigs CONTIGS, -c CONTIGS
-                                Path to contigs file, which is a tab-delimited with 3
-                                columns <isolatename> <path_to_contigs>. OPTIONAL if
-                                you already have assemblies. (default: )
-          --job_id JOB_ID, -j JOB_ID
-                                Job ID, will be the name of the output directory
-                                (default: )
-          --reference REFERENCE, -r REFERENCE
-                                Path to reference (.gbk or .fa) (default: )
-          --mask MASK, -m MASK  Path to mask file if used (.bed) (default: )
-          --abritamr_args {Acinetobacter_baumannii,Campylobacter,Enterococcus_faecalis,Enterococcus_faecium,Escherichia,Klebsiella,Salmonella,Staphylococcus_aureus,Staphylococcus_pseudintermedius,Streptococcus_agalactiae,Streptococcus_pneumoniae,Streptococcus_pyogenes,Vibrio_cholerae}
-                                Set if you would like to use point mutations, please
-                                provide a valid species. (default: )
-          --kraken_db KRAKEN_DB, -k KRAKEN_DB
-                                Path to DB for use with kraken2, if no DB present
-                                speciation will not be performed. (default:
-                                KRAKEN2_DEFAULT_DB)
-          --pipeline {preview,default,all}, -p {preview,default,all}
-                                The pipeline to run. `preview` - generates a rapid
-                                tree using mash distances | `default` - runs snippy,
-                                phylogenetic tree (if > 3 sequences), assemblies, mlst
-                                and amr gene detection | `all` - same as default but
-                                includes roary pangenome analysis (default: preview)
-          --assembler {shovill,skesa,spades}, -a {shovill,skesa,spades}
-                                Assembler to use. (default: spades)
-          --cpus CPUS           Number of max CPU cores to run, will define how many
-                                rules are run at a time (default: 72)
-          --minaln MINALN, -ma MINALN
-                                Minimum percent alignment. Isolates which do not align
-                                to reference at this threshold will not be included in
-                                core phylogeny. (default: 0)
-          --minqual MINQUAL, -mq MINQUAL
-                                Minimum Avg quality of reads (default: 0)
-          --mincov MINCOV, -mc MINCOV
-                                Minimum percent alignment. Isolates which do not have
-                                average read coverage above this threshold will not be
-                                included further analysis. (default: 0)
-          --workdir WORKDIR, -w WORKDIR
-                                The directory where Bohra will be run, default is
-                                current directory (default:
-                                /home/khhor/sandbox/bohra/weird_bugs)
-          --force, -f           Add if you would like to force a complete restart of
-                                the pipeline. All previous logs will be lost.
-                                (default: False)
-          --no_phylo            Set if you do NOT want to generate a phylogentic tree.
-                                (default: False)
-          --config CONFIG       An additional config file, required if running on a
-                                non-local machine, ie slurm, cloud. For help see
-                                documentation at https://github.com/MDU-PHL/bohra or
-                                https://www.nextflow.io/docs/latest/executor.html
-                                (default: )
-          --profile PROFILE     The resource profile to use. Defaults to local, if
-                                using an alternative config file, this calue should
-                                represent the name of a profile provided (default:
-                                lcl)
-          --gubbins             Set to use gubbins for recombination correction.
-                                (default: False)
-          --keep {Y,N}          If you are rerunning bohra over an exisiting directory
-                                set --keep to 'Y' to archive report files - otherwise
-                                previous reprot files will be removed. (default: N)
+        `bohra` will generate an input file for you with the path to reads in the correct format, you will need to supply a path to where the reads can be found. You may also want to supply a file with a list of sample IDs (especially if there are more reads in the path provided than you wish to use). Please note `generate_input` assumes that the files are named as `<sample_ID_someother_stuff_{R1,R2}.f*q.gz>` and will output a file called `isolates.tab`
         
         ```
+        bohra generate_input -r path_to_reads
+        ```
+        
+        **`bohra run`**
         
         
         **Input file**
         
         The input file needs to be a tab-delimited file with three columns IsolateID, path to R1 and path to R2. 
         ```
         Isolate-ID    /path/to/reads/R1.fq.gz    /path/to/reads/R2.fq.gz
@@ -256,30 +181,45 @@
         
         **Mask**
         
         Phage masking is important for to prevent the inflation of SNPs that can be introduced by horizontal transfer as opposed to vertical transfer. For closed genomes or those that are publicly available `phaster-query.pl` can be used to identify regions for masking. If a denovo assembly is used the website `phaster.ca` can be used. Regions for masking should be provided in `.bed` format.
         
         
         
-        ### Preview mode
+        ### Preview mode (default)
         
         `bohra` preview mode uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
         
         ```
         bohra run -i input.tab -r ref.fa -p preview -j job_id
         ```
         
         ### Default
         
         Default mode will perform SNP detection, assemblies (if contigs file not provided), mlst, abritamr and phylogeny (unless `--no_phylo` or < 4 samples used as input).
         
         ```
         bohra run -i input.tab -c contigs.tab -r ref.fa -p default -j job_id
         ```
-        
+        In addition, if you would like `bohra` to output point mutations for AMR (based on `abritAMR` and AMRFinderplus), you can also add the `--abritamr_args` flag with one of the following species:
+        ```
+        Neisseria
+        Acinetobacter_baumannii
+        Campylobacter
+        Enterococcus_faecalis
+        Enterococcus_faecium
+        Escherichia
+        Klebsiella
+        Salmonella
+        Staphylococcus_aureus
+        Staphylococcus_pseudintermedius
+        Streptococcus_agalactiae
+        Streptococcus_pneumoniae
+        Streptococcus_pyogenes,Vibrio_cholerae
+        ```
         
         ### Plus pangenome
         
         In addition to the default mode above, `all` will also run `panaroo` . If less than 4 samples are provided, `panaroo` will not be run and pipeline will revert to `default`
         
         ```
         bohra run -i input.tab -c contigs.tab -r ref.fa -p pluspan -j job_id
@@ -296,10 +236,10 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `bohra-2.2.0/README.md` & `bohra-2.2.1/bohra.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,286 +1,245 @@
-[![CircleCI](https://circleci.com/gh/MDU-PHL/bohra.svg?style=svg&circle-token=530799cb0764519fc65966ab48bac7e0d02f3688)](https://circleci.com/gh/MDU-PHL/bohra)
-[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-
-
-
-# Bohra
-
-Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. At a minimum the pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
-
-## Bohra has a new look! Welcome to Bohra-NF
-
-**New features**
-
-* Pipeline written in [Nextflow](https://www.nextflow.io)
-* Default mode
-    * Can be run on a single isolate (phylogenetic tree will not be generated if fewer than three sequences included in dataset)
-    * MobSuite integration.
-    * Updated [abriTAMR](https://github.com/MDU-PHL/abritamr) with support for point mutations and virulence factors (beta).
-* Panaroo with visualisation of pan-genome.
-* Improved support for different computing environments.
-
-**Comming soon**
-
-* Improved report structure
-* Option to add your own modules
-
-
-**Accreditation**
-
-* _snippy and snippy-core version 4.4.5 are NATA accredited for accurate detection of SNPs for reporting of genomic relationships at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
-* _abritamr is accredited for detection of AMR genes at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
-
-### Motivation
-
-Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Nextflow](https://www.nextflow.io).
-
-### Etymology
-
-Bohra the name of an exinct species of tree kangaroo that lived on the Nullarbor plain in Australia. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on [*snippy*](https://github.com/tseemann/snippy) (named for a very famous kangaroo) and was inspired by [*nullarbor*](https://github.com/tseemann/nullarbor). 
-
-
-## Pipeline
-
-Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports. An addtional file can be porvided with the paths to any assemblies that have already been generated. This is a helpful saver of time.
-
-![Image](https://github.com/MDU-PHL/bohra/blob/master/workflow.png)
-
-Bohra can be run in three modes
-1. Preview
-* Calculate mash-distances
-* Build a mash-tree
-* Report sequencing statistics
-* Species identification (providing you have kraken2 database setup properly ;) )
-
-2. Default SNPs, species ID, assemly, MLST, Resistome and annotation)
-* Call variants
-* Generate a phylogenetic tree
-* Assemble 
-* MLST
-* Resistome
-* Annotate
-* Plasmid prediction
-* Species identification
-
-3. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
-* Call variants
-* Generate a phylogenetic tree
-* Assemble 
-* MLST
-* Resistome
-* Annotate
-* Plasmid prediction
-* Species identification
-* Pan Genome
-
-### Installation
-
-**New installation instructions comming soon**
-
-Bohra requires >=python3.7
-
-#### Conda (Highly recomended)
-
-Installing bohra with conda will ensure that all dependencies are present. See below for instructions on how to configure the databases for kraken2.
-
-Set up conda - documentation for conda installation can be found [here](https://conda.io/en/latest/miniconda.html)
-```
-conda config --add channels defaults
-conda config --add channels bioconda
-conda config --add channels conda-forge
-```
-It is recomended that you set up a `bohra` environment
-```
-conda create -n <bohra_env_name> bohra
-```
-To use bohra
-```
-conda activate <bohra_env_name>
-```
-#### PyPi
-If installing with `pip` you will need to ensure other dependencies are also installed.
-```
-pip3 install bohra
-```
-* [Snippy (v4.4.5 recommended)](https://github.com/tseemann/snippy)
-* [Shovill (skesa and spades.py)](https://github.com/tseemann/shovill)
-* [Panaroo](https://github.com/gtonkinhill/panaroo)
-* [Prokka](https://github.com/tseemann/prokka)
-* [kraken2](https://ccb.jhu.edu/software/kraken/)
-* [abritamr](https://github.com/MDU-PHL/abritamr)
-* [mlst](https://github.com/tseemann/mlst)
-* [iqtree](http://www.iqtree.org/)
-* [seqtk](https://github.com/lh3/seqtk)
-* [snp-dists](https://github.com/tseemann/snp-dists)
-* [mash](https://github.com/lskatz/mashtree)
-* [mob_suite](https://github.com/phac-nml/mob-suite)
-* [csvtk](https://github.com/shenwei356/csvtk)
-
-
-#### Check installation
-
-Check that all dependencies are installed.
-
-```
-bohra check
-```
-
-*IMPORTANT*
-
-In addition to installing kraken ensure that you have a kraken2 database. Minikraken can obtained as follows
-```
-wget ftp://ftp.ccb.jhu.edu/pub/data/kraken2_dbs/minikraken2_v2_8GB_201904_UPDATE.tgz
-tar -C $HOME -zxvf minikraken2_v2_8GB_201904_UPDATE.tgz
-```
-This will download and unzip the kraken2 DB. Other kraken2 DB are also available, you can find more information [here](https://ccb.jhu.edu/software/kraken2/index.shtml?t=downloads)
-
-Once you have the DB downloaded you will have to create an environment variable called `KRAKEN2_DEFAULT_DB`. This can be done by adding the following to your `$HOME/.bashrc`
-```
-export KRAKEN_DEFAULT_DB=$HOME/minikraken2_v2_8GB_201904_UPDATE
-```
-
-### Running bohra
-
-**A word on resources**
-
-* A minimum of 8 cpus is required for running `bohra`
-* `bohra` has default settings for running at MDU (both on research and service systems). These ensure optimal running on these systems.
-* Whether you are running `bohra` on MDU systems or not, you can override the default max cpus, by providing an upper limit for your job using the `--cpus` flag.
-* If you are running on a queue or in the cloud you will need to provide an additional config file with details of your profile requirements.
-
-#### Using CLI
-
-```
-$ bohra run -h
-
-Bohra - a bacterial genomics pipeline - version 2.0.0
-
- -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  --check               Check that dependencies are installed correctly.
-                        (default: False)
-  --input_file INPUT_FILE, -i INPUT_FILE
-                        Path to reads file, which is a tab-delimited with 3
-                        columns <isolatename> <path_to_read1> <path_to_read2>.
-                        REQUIRED (default: )
-  --contigs CONTIGS, -c CONTIGS
-                        Path to contigs file, which is a tab-delimited with 3
-                        columns <isolatename> <path_to_contigs>. OPTIONAL if
-                        you already have assemblies. (default: )
-  --job_id JOB_ID, -j JOB_ID
-                        Job ID, will be the name of the output directory
-                        (default: )
-  --reference REFERENCE, -r REFERENCE
-                        Path to reference (.gbk or .fa) (default: )
-  --mask MASK, -m MASK  Path to mask file if used (.bed) (default: )
-  --abritamr_args {Acinetobacter_baumannii,Campylobacter,Enterococcus_faecalis,Enterococcus_faecium,Escherichia,Klebsiella,Salmonella,Staphylococcus_aureus,Staphylococcus_pseudintermedius,Streptococcus_agalactiae,Streptococcus_pneumoniae,Streptococcus_pyogenes,Vibrio_cholerae}
-                        Set if you would like to use point mutations, please
-                        provide a valid species. (default: )
-  --kraken_db KRAKEN_DB, -k KRAKEN_DB
-                        Path to DB for use with kraken2, if no DB present
-                        speciation will not be performed. (default:
-                        KRAKEN2_DEFAULT_DB)
-  --pipeline {preview,default,all}, -p {preview,default,all}
-                        The pipeline to run. `preview` - generates a rapid
-                        tree using mash distances | `default` - runs snippy,
-                        phylogenetic tree (if > 3 sequences), assemblies, mlst
-                        and amr gene detection | `all` - same as default but
-                        includes roary pangenome analysis (default: preview)
-  --assembler {shovill,skesa,spades}, -a {shovill,skesa,spades}
-                        Assembler to use. (default: spades)
-  --cpus CPUS           Number of max CPU cores to run, will define how many
-                        rules are run at a time (default: 72)
-  --minaln MINALN, -ma MINALN
-                        Minimum percent alignment. Isolates which do not align
-                        to reference at this threshold will not be included in
-                        core phylogeny. (default: 0)
-  --minqual MINQUAL, -mq MINQUAL
-                        Minimum Avg quality of reads (default: 0)
-  --mincov MINCOV, -mc MINCOV
-                        Minimum percent alignment. Isolates which do not have
-                        average read coverage above this threshold will not be
-                        included further analysis. (default: 0)
-  --workdir WORKDIR, -w WORKDIR
-                        The directory where Bohra will be run, default is
-                        current directory (default:
-                        /home/khhor/sandbox/bohra/weird_bugs)
-  --force, -f           Add if you would like to force a complete restart of
-                        the pipeline. All previous logs will be lost.
-                        (default: False)
-  --no_phylo            Set if you do NOT want to generate a phylogentic tree.
-                        (default: False)
-  --config CONFIG       An additional config file, required if running on a
-                        non-local machine, ie slurm, cloud. For help see
-                        documentation at https://github.com/MDU-PHL/bohra or
-                        https://www.nextflow.io/docs/latest/executor.html
-                        (default: )
-  --profile PROFILE     The resource profile to use. Defaults to local, if
-                        using an alternative config file, this calue should
-                        represent the name of a profile provided (default:
-                        lcl)
-  --gubbins             Set to use gubbins for recombination correction.
-                        (default: False)
-  --keep {Y,N}          If you are rerunning bohra over an exisiting directory
-                        set --keep to 'Y' to archive report files - otherwise
-                        previous reprot files will be removed. (default: N)
-
-```
-
-
-**Input file**
-
-The input file needs to be a tab-delimited file with three columns IsolateID, path to R1 and path to R2. 
-```
-Isolate-ID    /path/to/reads/R1.fq.gz    /path/to/reads/R2.fq.gz
-```
-
-In addition a file of contigs may also be provided if you have already generated assemblies you wish to use. This is also a tab-delimited file. 
-
-```
-Isolate-ID    /path/to/asm.fasta
-```
-**Reference**
-
-The choice of reference is important for the accuracy of SNP detection and therefore the investigation of genomic relatedness. Appropriate references should be chosen following the guidelines below.
-1. A closed reference from the same ST (where applicable) or a gold-standard reference (as may be used in M. tuberculosis).
-2. A pacbio or nanopore assembly from MDU that is of the same type as the query dataset
-3. A high quality de novo assembly of either an isolate in the dataset or an isolate of the same ST or type.
-
-**Mask**
-
-Phage masking is important for to prevent the inflation of SNPs that can be introduced by horizontal transfer as opposed to vertical transfer. For closed genomes or those that are publicly available `phaster-query.pl` can be used to identify regions for masking. If a denovo assembly is used the website `phaster.ca` can be used. Regions for masking should be provided in `.bed` format.
-
-
-
-### Preview mode
-
-`bohra` preview mode uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
-
-```
-bohra run -i input.tab -r ref.fa -p preview -j job_id
-```
-
-### Default
-
-Default mode will perform SNP detection, assemblies (if contigs file not provided), mlst, abritamr and phylogeny (unless `--no_phylo` or < 4 samples used as input).
-
-```
-bohra run -i input.tab -c contigs.tab -r ref.fa -p default -j job_id
-```
-
-
-### Plus pangenome
-
-In addition to the default mode above, `all` will also run `panaroo` . If less than 4 samples are provided, `panaroo` will not be run and pipeline will revert to `default`
-
-```
-bohra run -i input.tab -c contigs.tab -r ref.fa -p pluspan -j job_id
-```
-
-### Profile
-
-You can provide a specific profile for running `bohra` on various computing platforms (see https://www.nextflow.io/docs/latest/executor.html for available platforms). You will need to specify a `--profile`, which MUST be the same as the name of the profile in your `--config` file. An example structure is provided in `example.config` 
-
-
-
-
+Metadata-Version: 2.1
+Name: bohra
+Version: 2.2.1
+Summary: A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
+Home-page: https://github.com/kristyhoran/bohra
+Author: Kristy Horan
+Author-email: kristyhoran15@gmail.com
+License: UNKNOWN
+Description: <!-- [![CircleCI](https://circleci.com/gh/MDU-PHL/bohra.svg?style=svg&circle-token=530799cb0764519fc65966ab48bac7e0d02f3688)](https://circleci.com/gh/MDU-PHL/bohra) -->
+        [![Python 3.7](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-370/)
+        
+        
+        # Bohra
+        
+        Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. At a minimum the pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
+        
+        * Pipeline written in [Nextflow](https://www.nextflow.io)
+        * Default mode
+            * Can be run on a single isolate (phylogenetic tree will not be generated if fewer than three sequences included in dataset)
+            * MobSuite integration.
+            * Updated [abriTAMR](https://github.com/MDU-PHL/abritamr) with support for point mutations and virulence factors (beta).
+        * Panaroo with visualisation of pan-genome.
+        * Improved support for different computing environments.
+        
+        ## Recent changes to bohra
+        * Each bohra process is now run in its own conda environment. These will by default be included in your working directory.
+        * Alternatively you can install your own conda environments and provide the path to where these can be found (see help below).
+        * If you wish you can maintain the existing structure - where all the dependencies are installed in a single environment. BEWARE this can cause unexpected behaviour and even cause the pipeline to fail. If you wish to run bohra in this way please contact us for advice.
+        
+        **Comming soon**
+        
+        * Improved report structure
+        * Baby kraken
+        * Typing (_Salmonella_ spp., _Listeria monocytogenes_, _Neiserria_)
+        * Mtb AMR
+        
+        
+        **Accreditation**
+        
+        * _snippy and snippy-core version 4.4.5 are NATA accredited for accurate detection of SNPs for reporting of genomic relationships at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
+        * _abritamr is accredited for detection of AMR genes at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
+        
+        ### Motivation
+        
+        Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Nextflow](https://www.nextflow.io).
+        
+        ### Etymology
+        
+        Bohra the name of an exinct species of tree kangaroo that lived on the Nullarbor plain in Australia. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on [*snippy*](https://github.com/tseemann/snippy) (named for a very famous kangaroo) and was inspired by [*nullarbor*](https://github.com/tseemann/nullarbor). 
+        
+        
+        ## Pipeline
+        
+        Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports. An addtional file can be porvided with the paths to any assemblies that have already been generated. This is a helpful saver of time.
+        
+        ![Image](https://github.com/MDU-PHL/bohra/blob/master/workflow.png)
+        
+        Bohra can be run in three modes
+        1. Preview
+        * Calculate mash-distances
+        * Build a mash-tree
+        * Report sequencing statistics
+        * Species identification (providing you have kraken2 database setup properly ;) )
+        
+        2. Default SNPs, species ID, assemly, MLST, Resistome and annotation)
+        * Call variants
+        * Generate a phylogenetic tree
+        * Assemble 
+        * MLST
+        * Resistome
+        * Annotate
+        * Plasmid prediction
+        * Species identification
+        
+        3. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
+        * Call variants
+        * Generate a phylogenetic tree
+        * Assemble 
+        * MLST
+        * Resistome
+        * Annotate
+        * Plasmid prediction
+        * Species identification
+        * Pan Genome
+        
+        ### Installation (with conda)
+        
+        Bohra requires >=python3.9 and conda
+        
+        See below for instructions on how to configure the databases for kraken2.
+        
+        1. Set up conda - documentation for conda installation can be found [here](https://conda.io/en/latest/miniconda.html)
+        ```
+        conda config --add channels defaults
+        conda config --add channels bioconda
+        conda config --add channels conda-forge
+        ```
+        
+        2. Create the conda environment
+        ```
+        conda create -n <bohra_env_name> bohra python=3.9
+        conda activate <bohra_env_name>
+        ```
+        You can also install `bohra` with 
+        ```
+        pip3 install bohra
+        ```
+        
+        3. Ensure that you have a kraken2 database. Minikraken can obtained as follows
+        ```
+        wget ftp://ftp.ccb.jhu.edu/pub/data/kraken2_dbs/minikraken2_v2_8GB_201904_UPDATE.tgz
+        tar -C $HOME -zxvf minikraken2_v2_8GB_201904_UPDATE.tgz
+        ```
+        This will download and unzip the kraken2 DB. Other kraken2 DB are also available, you can find more information [here](https://ccb.jhu.edu/software/kraken2/index.shtml?t=downloads)
+        
+        Once you have the DB downloaded you will have to create an environment variable called `KRAKEN2_DEFAULT_DB`. This can be done by adding the following to your `$HOME/.bashrc`
+        ```
+        export KRAKEN_DEFAULT_DB=$HOME/minikraken2_v2_8GB_201904_UPDATE
+        ```
+        
+        #### Recommended conda environments (for the brave)
+        
+        If you would like to use pre-installed conda envs - the following are suggested. You may also attempt to install all these dependencies into a single conda environment - however it is not recomended as there may be significant dependency clashes.
+        
+        * [Snippy (v4.4.5 recommended)](https://github.com/tseemann/snippy)
+        * [Shovill (skesa and spades.py)](https://github.com/tseemann/shovill)
+        * [Panaroo](https://github.com/gtonkinhill/panaroo)
+        * [Prokka](https://github.com/tseemann/prokka)
+        * [kraken2](https://ccb.jhu.edu/software/kraken/)
+        * [abritamr](https://github.com/MDU-PHL/abritamr)
+        * [mlst](https://github.com/tseemann/mlst)
+        * [iqtree](http://www.iqtree.org/)
+        * [seqtk](https://github.com/lh3/seqtk)
+        * [snp-dists](https://github.com/tseemann/snp-dists)
+        * [mash](https://github.com/lskatz/mashtree)
+        * [mob_suite](https://github.com/phac-nml/mob-suite)
+        * [csvtk](https://github.com/shenwei356/csvtk)
+        
+        
+        
+        ### Running bohra
+        
+        **A word on resources**
+        
+        * A minimum of 8 cpus is required for running `bohra`
+        * `bohra` has default settings for running at MDU (both on research and service systems). These ensure optimal running on these systems.
+        * Whether you are running `bohra` on MDU systems or not, you can override the default max cpus, by providing an upper limit for your job using the `--cpus` flag.
+        * If you are running on a queue or in the cloud you will need to provide an additional config file with details of your profile requirements.
+        
+        #### Using CLI
+        
+        **`bohra generate_input`**
+        
+        `bohra` will generate an input file for you with the path to reads in the correct format, you will need to supply a path to where the reads can be found. You may also want to supply a file with a list of sample IDs (especially if there are more reads in the path provided than you wish to use). Please note `generate_input` assumes that the files are named as `<sample_ID_someother_stuff_{R1,R2}.f*q.gz>` and will output a file called `isolates.tab`
+        
+        ```
+        bohra generate_input -r path_to_reads
+        ```
+        
+        **`bohra run`**
+        
+        
+        **Input file**
+        
+        The input file needs to be a tab-delimited file with three columns IsolateID, path to R1 and path to R2. 
+        ```
+        Isolate-ID    /path/to/reads/R1.fq.gz    /path/to/reads/R2.fq.gz
+        ```
+        
+        In addition a file of contigs may also be provided if you have already generated assemblies you wish to use. This is also a tab-delimited file. 
+        
+        ```
+        Isolate-ID    /path/to/asm.fasta
+        ```
+        **Reference**
+        
+        The choice of reference is important for the accuracy of SNP detection and therefore the investigation of genomic relatedness. Appropriate references should be chosen following the guidelines below.
+        1. A closed reference from the same ST (where applicable) or a gold-standard reference (as may be used in M. tuberculosis).
+        2. A pacbio or nanopore assembly from MDU that is of the same type as the query dataset
+        3. A high quality de novo assembly of either an isolate in the dataset or an isolate of the same ST or type.
+        
+        **Mask**
+        
+        Phage masking is important for to prevent the inflation of SNPs that can be introduced by horizontal transfer as opposed to vertical transfer. For closed genomes or those that are publicly available `phaster-query.pl` can be used to identify regions for masking. If a denovo assembly is used the website `phaster.ca` can be used. Regions for masking should be provided in `.bed` format.
+        
+        
+        
+        ### Preview mode (default)
+        
+        `bohra` preview mode uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
+        
+        ```
+        bohra run -i input.tab -r ref.fa -p preview -j job_id
+        ```
+        
+        ### Default
+        
+        Default mode will perform SNP detection, assemblies (if contigs file not provided), mlst, abritamr and phylogeny (unless `--no_phylo` or < 4 samples used as input).
+        
+        ```
+        bohra run -i input.tab -c contigs.tab -r ref.fa -p default -j job_id
+        ```
+        In addition, if you would like `bohra` to output point mutations for AMR (based on `abritAMR` and AMRFinderplus), you can also add the `--abritamr_args` flag with one of the following species:
+        ```
+        Neisseria
+        Acinetobacter_baumannii
+        Campylobacter
+        Enterococcus_faecalis
+        Enterococcus_faecium
+        Escherichia
+        Klebsiella
+        Salmonella
+        Staphylococcus_aureus
+        Staphylococcus_pseudintermedius
+        Streptococcus_agalactiae
+        Streptococcus_pneumoniae
+        Streptococcus_pyogenes,Vibrio_cholerae
+        ```
+        
+        ### Plus pangenome
+        
+        In addition to the default mode above, `all` will also run `panaroo` . If less than 4 samples are provided, `panaroo` will not be run and pipeline will revert to `default`
+        
+        ```
+        bohra run -i input.tab -c contigs.tab -r ref.fa -p pluspan -j job_id
+        ```
+        
+        ### Profile
+        
+        You can provide a specific profile for running `bohra` on various computing platforms (see https://www.nextflow.io/docs/latest/executor.html for available platforms). You will need to specify a `--profile`, which MUST be the same as the name of the profile in your `--config` file. An example structure is provided in `example.config` 
+        
+        
+        
+        
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
```

### Comparing `bohra-2.2.0/bohra/CustomLog.py` & `bohra-2.2.1/bohra/CustomLog.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/SnpDetection.py` & `bohra-2.2.1/bohra/SnpDetection.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/Utils.py` & `bohra-2.2.1/bohra/Utils.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/bohra.py` & `bohra-2.2.1/bohra/bohra.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/main.nf` & `bohra-2.2.1/bohra/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/bin/add_header_mlst.py` & `bohra-2.2.1/bohra/modules/collation/bin/add_header_mlst.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/bin/collate_asm.py` & `bohra-2.2.1/bohra/modules/collation/bin/collate_asm.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/bin/collate_kraken2.py` & `bohra-2.2.1/bohra/modules/collation/bin/collate_kraken2.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/bin/collate_stats.py` & `bohra-2.2.1/bohra/modules/collation/bin/collate_stats.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/bin/compile.py` & `bohra-2.2.1/bohra/modules/collation/bin/compile.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/bin/snippy_qc.py` & `bohra-2.2.1/bohra/modules/collation/bin/snippy_qc.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/bin/wrangle_mobsuite.py` & `bohra-2.2.1/bohra/modules/collation/bin/wrangle_mobsuite.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/functions.nf` & `bohra-2.2.1/bohra/modules/collation/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/collation/main.nf` & `bohra-2.2.1/bohra/modules/collation/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/csvtk/functions.nf` & `bohra-2.2.1/bohra/modules/csvtk/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/csvtk/main.nf` & `bohra-2.2.1/bohra/modules/csvtk/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/csvtk/meta.yml` & `bohra-2.2.1/bohra/modules/csvtk/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/gubbins/functions.nf` & `bohra-2.2.1/bohra/modules/gubbins/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/gubbins/main.nf` & `bohra-2.2.1/bohra/modules/gubbins/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     output:
     path('gubbins.aln'), emit: gubbins
 
     // tuple val(meta), path('spades.log'), emit: log
 
     script:
     """
-    run_gubbins.py -c $task.cpus  --prefix clean cleaned
+    run_gubbins.py -c $task.cpus  --prefix clean $cleaned
     snp-sites -c clean.filtered_polymorphic_sites.fasta > gubbins.aln
     """
     
 }
```

### Comparing `bohra-2.2.0/bohra/modules/gubbins/meta.yml` & `bohra-2.2.1/bohra/modules/gubbins/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/iqtree/bin/iqtree_generator.sh` & `bohra-2.2.1/bohra/modules/iqtree/bin/iqtree_generator.sh`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/iqtree/functions.nf` & `bohra-2.2.1/bohra/modules/iqtree/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/iqtree/main.nf` & `bohra-2.2.1/bohra/modules/iqtree/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/iqtree/meta.yml` & `bohra-2.2.1/bohra/modules/iqtree/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/kraken2/functions.nf` & `bohra-2.2.1/bohra/modules/kraken2/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/kraken2/main.nf` & `bohra-2.2.1/bohra/modules/kraken2/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/kraken2/meta.yml` & `bohra-2.2.1/bohra/modules/kraken2/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mash/sketch/functions.nf` & `bohra-2.2.1/bohra/modules/mash/sketch/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mash/sketch/main.nf` & `bohra-2.2.1/bohra/modules/mash/sketch/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mash/sketch/meta.yml` & `bohra-2.2.1/bohra/modules/mash/sketch/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mash/triangle/functions.nf` & `bohra-2.2.1/bohra/modules/mash/triangle/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mash/triangle/main.nf` & `bohra-2.2.1/bohra/modules/mash/triangle/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mash/triangle/meta.yml` & `bohra-2.2.1/bohra/modules/mash/triangle/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mlst/functions.nf` & `bohra-2.2.1/bohra/modules/mlst/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mlst/main.nf` & `bohra-2.2.1/bohra/modules/mlst/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mlst/meta.yml` & `bohra-2.2.1/bohra/modules/mlst/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mobsuite/functions.nf` & `bohra-2.2.1/bohra/modules/mobsuite/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mobsuite/main.nf` & `bohra-2.2.1/bohra/modules/mobsuite/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/mobsuite/meta.yml` & `bohra-2.2.1/bohra/modules/mobsuite/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/panaroo/functions.nf` & `bohra-2.2.1/bohra/modules/panaroo/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/panaroo/main.nf` & `bohra-2.2.1/bohra/modules/panaroo/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/panaroo/meta.yml` & `bohra-2.2.1/bohra/modules/panaroo/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/prokka/functions.nf` & `bohra-2.2.1/bohra/modules/prokka/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/prokka/main.nf` & `bohra-2.2.1/bohra/modules/prokka/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/prokka/meta.yml` & `bohra-2.2.1/bohra/modules/prokka/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/quicktree/functions.nf` & `bohra-2.2.1/bohra/modules/quicktree/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/quicktree/main.nf` & `bohra-2.2.1/bohra/modules/quicktree/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/quicktree/meta.yml` & `bohra-2.2.1/bohra/modules/quicktree/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/resistome/bin/combine.py` & `bohra-2.2.1/bohra/modules/resistome/bin/combine.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/resistome/bin/concat.py` & `bohra-2.2.1/bohra/modules/resistome/bin/concat.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/resistome/bin/meta.yaml` & `bohra-2.2.1/bohra/modules/resistome/bin/meta.yaml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/resistome/functions.nf` & `bohra-2.2.1/bohra/modules/resistome/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/resistome/main.nf` & `bohra-2.2.1/bohra/modules/resistome/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/resistome/meta.yml` & `bohra-2.2.1/bohra/modules/resistome/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/roary2svg/bin/roary2svg.pl` & `bohra-2.2.1/bohra/modules/roary2svg/bin/roary2svg.pl`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/roary2svg/functions.nf` & `bohra-2.2.1/bohra/modules/roary2svg/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/roary2svg/main.nf` & `bohra-2.2.1/bohra/modules/roary2svg/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/roary2svg/meta.yml` & `bohra-2.2.1/bohra/modules/roary2svg/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqkit/fx2tab/functions.nf` & `bohra-2.2.1/bohra/modules/seqkit/fx2tab/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqkit/fx2tab/main.nf` & `bohra-2.2.1/bohra/modules/seqkit/fx2tab/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqkit/fx2tab/meta.yml` & `bohra-2.2.1/bohra/modules/seqkit/fx2tab/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqkit/stats/functions.nf` & `bohra-2.2.1/bohra/modules/seqkit/stats/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqkit/stats/main.nf` & `bohra-2.2.1/bohra/modules/seqkit/stats/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqkit/stats/meta.yml` & `bohra-2.2.1/bohra/modules/seqkit/stats/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqtk/functions.nf` & `bohra-2.2.1/bohra/modules/seqtk/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqtk/main.nf` & `bohra-2.2.1/bohra/modules/seqtk/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/seqtk/meta.yml` & `bohra-2.2.1/bohra/modules/seqtk/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/shovill/functions.nf` & `bohra-2.2.1/bohra/modules/shovill/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/shovill/main.nf` & `bohra-2.2.1/bohra/modules/shovill/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/shovill/meta.yml` & `bohra-2.2.1/bohra/modules/shovill/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/skesa/functions.nf` & `bohra-2.2.1/bohra/modules/skesa/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/skesa/main.nf` & `bohra-2.2.1/bohra/modules/skesa/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/skesa/meta.yml` & `bohra-2.2.1/bohra/modules/skesa/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy/functions.nf` & `bohra-2.2.1/bohra/modules/snippy/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy/main.nf` & `bohra-2.2.1/bohra/modules/snippy/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy/meta.yml` & `bohra-2.2.1/bohra/modules/snippy/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy_clean/functions.nf` & `bohra-2.2.1/bohra/modules/snippy_clean/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy_clean/main.nf` & `bohra-2.2.1/bohra/modules/snippy_clean/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy_clean/meta.yml` & `bohra-2.2.1/bohra/modules/snippy_clean/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy_core/functions.nf` & `bohra-2.2.1/bohra/modules/snippy_core/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy_core/main.nf` & `bohra-2.2.1/bohra/modules/snippy_core/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snippy_core/meta.yml` & `bohra-2.2.1/bohra/modules/snippy_core/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snp_dists/functions.nf` & `bohra-2.2.1/bohra/modules/snp_dists/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snp_dists/main.nf` & `bohra-2.2.1/bohra/modules/snp_dists/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/snp_dists/meta.yml` & `bohra-2.2.1/bohra/modules/snp_dists/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/spades/functions.nf` & `bohra-2.2.1/bohra/modules/spades/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/spades/main.nf` & `bohra-2.2.1/bohra/modules/spades/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/modules/spades/meta.yml` & `bohra-2.2.1/bohra/modules/spades/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/nextflow.config` & `bohra-2.2.1/bohra/nextflow.config`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/templates/cluster.tmpl` & `bohra-2.2.1/bohra/templates/cluster.tmpl`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/templates/config_snippy.yaml` & `bohra-2.2.1/bohra/templates/config_snippy.yaml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/templates/index.html` & `bohra-2.2.1/bohra/templates/index.html`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/templates/report_analysis.json` & `bohra-2.2.1/bohra/templates/report_analysis.json`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/tests/test.gbk` & `bohra-2.2.1/bohra/tests/test.gbk`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/tests/test.tab` & `bohra-2.2.1/bohra/tests/test.tab`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/tests/test_bohra.py` & `bohra-2.2.1/bohra/tests/test_bohra.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/workflows/assemble_typing.nf` & `bohra-2.2.1/bohra/workflows/assemble_typing.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/workflows/collation.nf` & `bohra-2.2.1/bohra/workflows/collation.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/workflows/common.nf` & `bohra-2.2.1/bohra/workflows/common.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra/workflows/default.nf` & `bohra-2.2.1/bohra/workflows/default.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/bohra.egg-info/SOURCES.txt` & `bohra-2.2.1/bohra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bohra-2.2.0/setup.cfg` & `bohra-2.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [metadata]
 name = bohra
 author = Kristy Horan
 author_email = kristyhoran15@gmail.com
 description = A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
-version = 2.2.0
+version = 2.2.1
 url = https://github.com/kristyhoran/bohra
 classifiers = 
 	Programming Language :: Python :: 3.9
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = 
 	LICENSE.txt
 
 [options]
-python_requires = >= 3.9
+python_requires = >= 3.8
 packages = find:
 zip_safe = False
 install_requires = 
 	pytest
 	altair
 	jinja2
 	biopython>=1.70
-	pandas>=0.25.0,<=1.0.5
+	pandas==1.0.5
 	numpy==1.23.1
 	psutil
 	sh
 	packaging
 include_package_data = True
 
 [options.extras_require]
```

