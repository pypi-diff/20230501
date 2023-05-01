# Comparing `tmp/paraphase-2.2.1.tar.gz` & `tmp/paraphase-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paraphase-2.2.1.tar", last modified: Sat Apr 29 00:53:47 2023, max compression
+gzip compressed data, was "paraphase-2.2.2.tar", last modified: Mon May  1 19:34:36 2023, max compression
```

## Comparing `paraphase-2.2.1.tar` & `paraphase-2.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:47.119403 paraphase-2.2.1/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-2.2.1/LICENSE
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-04-29 00:53:47.088419 paraphase-2.2.1/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     6974 2023-04-28 20:10:14.000000 paraphase-2.2.1/README.md
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:46.954860 paraphase-2.2.1/paraphase/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2023-04-29 00:53:26.000000 paraphase-2.2.1/paraphase/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2023-04-29 00:41:34.000000 paraphase-2.2.1/paraphase/__main__.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:46.981713 paraphase-2.2.1/paraphase/data/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     3457 2023-04-28 17:55:07.000000 paraphase-2.2.1/paraphase/data/config.yaml
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      104 2023-04-28 22:46:44.000000 paraphase-2.2.1/paraphase/data/genes.yaml
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2022-10-20 17:37:49.000000 paraphase-2.2.1/paraphase/data/genome_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:46.997128 paraphase-2.2.1/paraphase/data/rccx/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2023-03-11 03:44:27.000000 paraphase-2.2.1/paraphase/data/rccx/cyp21_diff_sites.txt
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:47.015118 paraphase-2.2.1/paraphase/data/smn1/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2023-04-27 16:23:00.000000 paraphase-2.2.1/paraphase/data/smn1/known_haplotypes.json
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    48846 2023-03-11 03:44:27.000000 paraphase-2.2.1/paraphase/data/smn1/ref_smn2.fa
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-03-11 03:44:27.000000 paraphase-2.2.1/paraphase/data/smn1/ref_smn2.fa.fai
--rw-r--r--   0 xchen    (71795) Domain Users (10513)  1584900 2022-10-20 17:37:49.000000 paraphase-2.2.1/paraphase/data/smn1/smn_matching_pos.txt
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:47.079111 paraphase-2.2.1/paraphase/genes/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      320 2023-04-28 18:45:59.000000 paraphase-2.2.1/paraphase/genes/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2719 2023-04-27 21:36:41.000000 paraphase-2.2.1/paraphase/genes/cfc1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     6307 2023-04-27 21:36:33.000000 paraphase-2.2.1/paraphase/genes/f8_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     6693 2023-04-28 17:26:02.000000 paraphase-2.2.1/paraphase/genes/ikbkg_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4435 2023-04-27 21:36:20.000000 paraphase-2.2.1/paraphase/genes/ncf1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5462 2023-04-28 17:25:14.000000 paraphase-2.2.1/paraphase/genes/neb_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2887 2023-04-27 21:35:54.000000 paraphase-2.2.1/paraphase/genes/pms2_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    23326 2023-04-28 18:12:50.000000 paraphase-2.2.1/paraphase/genes/rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25529 2023-04-27 21:35:43.000000 paraphase-2.2.1/paraphase/genes/smn1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5590 2023-04-27 21:35:43.000000 paraphase-2.2.1/paraphase/genes/strc_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1836 2023-04-14 17:02:02.000000 paraphase-2.2.1/paraphase/genome_depth.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    47878 2023-04-27 17:58:27.000000 paraphase-2.2.1/paraphase/haplotype_assembler.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    18069 2023-04-28 20:38:13.000000 paraphase-2.2.1/paraphase/paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    55195 2023-04-28 23:15:37.000000 paraphase-2.2.1/paraphase/phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    30200 2023-04-28 23:18:26.000000 paraphase-2.2.1/paraphase/prepare_bam_and_vcf.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:46.985810 paraphase-2.2.1/paraphase.egg-info/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-04-29 00:53:46.000000 paraphase-2.2.1/paraphase.egg-info/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1153 2023-04-29 00:53:46.000000 paraphase-2.2.1/paraphase.egg-info/SOURCES.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2023-04-29 00:53:46.000000 paraphase-2.2.1/paraphase.egg-info/dependency_links.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2023-04-29 00:53:46.000000 paraphase-2.2.1/paraphase.egg-info/entry_points.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2023-04-29 00:53:46.000000 paraphase-2.2.1/paraphase.egg-info/requires.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2023-04-29 00:53:46.000000 paraphase-2.2.1/paraphase.egg-info/top_level.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-04-29 00:53:47.119423 paraphase-2.2.1/setup.cfg
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      815 2023-04-29 00:53:22.000000 paraphase-2.2.1/setup.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-04-29 00:53:47.086403 paraphase-2.2.1/tests/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2023-03-11 01:37:24.000000 paraphase-2.2.1/tests/test_haplotype_assembler.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2023-04-28 19:00:08.000000 paraphase-2.2.1/tests/test_paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8332 2023-04-28 18:20:08.000000 paraphase-2.2.1/tests/test_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1793 2023-04-28 20:49:34.000000 paraphase-2.2.1/tests/test_prepare_bam_and_vcf.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2023-04-28 20:18:11.000000 paraphase-2.2.1/tests/test_rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8582 2023-04-27 16:50:03.000000 paraphase-2.2.1/tests/test_smn1_phaser.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:36.061583 paraphase-2.2.2/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-2.2.2/LICENSE
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-05-01 19:34:36.060574 paraphase-2.2.2/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     6974 2023-04-29 00:59:55.000000 paraphase-2.2.2/README.md
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.658566 paraphase-2.2.2/paraphase/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2023-05-01 19:10:23.000000 paraphase-2.2.2/paraphase/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2023-05-01 16:34:08.000000 paraphase-2.2.2/paraphase/__main__.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.701833 paraphase-2.2.2/paraphase/data/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     3457 2023-05-01 19:05:53.000000 paraphase-2.2.2/paraphase/data/config.yaml
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      104 2023-05-01 19:05:53.000000 paraphase-2.2.2/paraphase/data/genes.yaml
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2022-10-20 17:37:49.000000 paraphase-2.2.2/paraphase/data/genome_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.704834 paraphase-2.2.2/paraphase/data/rccx/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2023-03-11 03:44:27.000000 paraphase-2.2.2/paraphase/data/rccx/cyp21_diff_sites.txt
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.729842 paraphase-2.2.2/paraphase/data/smn1/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/data/smn1/known_haplotypes.json
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    48846 2023-03-11 03:44:27.000000 paraphase-2.2.2/paraphase/data/smn1/ref_smn2.fa
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-03-11 03:44:27.000000 paraphase-2.2.2/paraphase/data/smn1/ref_smn2.fa.fai
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)  1584900 2022-10-20 17:37:49.000000 paraphase-2.2.2/paraphase/data/smn1/smn_matching_pos.txt
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.956567 paraphase-2.2.2/paraphase/genes/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      320 2023-05-01 19:05:53.000000 paraphase-2.2.2/paraphase/genes/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2719 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/cfc1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     6307 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/f8_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     6693 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/ikbkg_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4435 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/ncf1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5462 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/neb_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2887 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/pms2_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    23326 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25529 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/smn1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5590 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/strc_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1836 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genome_depth.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    47878 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/haplotype_assembler.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    18442 2023-05-01 19:09:17.000000 paraphase-2.2.2/paraphase/paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    55195 2023-05-01 16:34:08.000000 paraphase-2.2.2/paraphase/phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    30069 2023-05-01 19:08:38.000000 paraphase-2.2.2/paraphase/prepare_bam_and_vcf.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.687569 paraphase-2.2.2/paraphase.egg-info/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1153 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/entry_points.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/requires.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/top_level.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-05-01 19:34:36.062567 paraphase-2.2.2/setup.cfg
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      846 2023-05-01 19:31:14.000000 paraphase-2.2.2/setup.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:36.056576 paraphase-2.2.2/tests/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2023-03-11 01:37:24.000000 paraphase-2.2.2/tests/test_haplotype_assembler.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8332 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1793 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_prepare_bam_and_vcf.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8582 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_smn1_phaser.py
```

### Comparing `paraphase-2.2.1/LICENSE` & `paraphase-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/PKG-INFO` & `paraphase-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paraphase
-Version: 2.2.1
+Version: 2.2.2
 Summary: paraphase: HiFi-based caller for highly homologous genes
 Home-page: https://github.com/PacificBiosciences/paraphase
 Author: Xiao Chen
 Author-email: xchen@pacificbiosciences.com
 License: BSD-3-Clause-Clear
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paraphase-2.2.1/README.md` & `paraphase-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/data/config.yaml` & `paraphase-2.2.2/paraphase/data/config.yaml`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/data/genome_region.bed` & `paraphase-2.2.2/paraphase/data/genome_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/data/smn1/known_haplotypes.json` & `paraphase-2.2.2/paraphase/data/smn1/known_haplotypes.json`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/data/smn1/ref_smn2.fa` & `paraphase-2.2.2/paraphase/data/smn1/ref_smn2.fa`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/data/smn1/smn_matching_pos.txt` & `paraphase-2.2.2/paraphase/data/smn1/smn_matching_pos.txt`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/cfc1_phaser.py` & `paraphase-2.2.2/paraphase/genes/cfc1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/f8_phaser.py` & `paraphase-2.2.2/paraphase/genes/f8_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/ikbkg_phaser.py` & `paraphase-2.2.2/paraphase/genes/ikbkg_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/ncf1_phaser.py` & `paraphase-2.2.2/paraphase/genes/ncf1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/neb_phaser.py` & `paraphase-2.2.2/paraphase/genes/neb_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/pms2_phaser.py` & `paraphase-2.2.2/paraphase/genes/pms2_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/rccx_phaser.py` & `paraphase-2.2.2/paraphase/genes/rccx_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/smn1_phaser.py` & `paraphase-2.2.2/paraphase/genes/smn1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genes/strc_phaser.py` & `paraphase-2.2.2/paraphase/genes/strc_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/genome_depth.py` & `paraphase-2.2.2/paraphase/genome_depth.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/haplotype_assembler.py` & `paraphase-2.2.2/paraphase/haplotype_assembler.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/paraphase.py` & `paraphase-2.2.2/paraphase/paraphase.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
 
 class Paraphase:
     def __init__(self):
         self.samtools = None
         self.minimap2 = None
 
+    @staticmethod
+    def get_version():
+        with open(os.path.join(os.path.dirname(__file__), "__init__.py")) as f:
+            for line in f:
+                if "version" in line:
+                    return line.split('"')[1]
+        return None
+
     def parse_configs(self, region_config=None):
         """
         Parse config files
         region_config: parameters for each region of interest
         gene_config: specifies some additional analyses triggered with some genes
         """
         data_path = os.path.join(os.path.dirname(__file__), "data")
@@ -361,14 +369,17 @@
             required=False,
         )
         parser.add_argument(
             "--minimap2",
             help="Optional path to minimap2",
             required=False,
         )
+        parser.add_argument(
+            "-v", "--version", action="version", version=f"{self.get_version()}"
+        )
         return parser
 
     def run(self):
         parser = self.load_parameters()
         args = parser.parse_args()
         outdir = args.out
         if os.path.exists(outdir) is False:
```

### Comparing `paraphase-2.2.1/paraphase/phaser.py` & `paraphase-2.2.2/paraphase/phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/paraphase/prepare_bam_and_vcf.py` & `paraphase-2.2.2/paraphase/prepare_bam_and_vcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,16 +279,14 @@
 
         self.tmpdir = tmpdir
         if self.tmpdir is None:
             self.tmpdir = self.outdir
         self.bam = os.path.join(
             tmpdir, self.sample_id + f"_{self.gene}_realigned_tagged.bam"
         )
-        if os.path.exists(self.bam) is False:
-            raise Exception(f"{self.bam} does not exist. VCFs are not generated...")
         self.vcf_dir = os.path.join(self.outdir, f"{self.sample_id}_vcfs")
         if os.path.exists(self.vcf_dir) is False:
             os.makedirs(self.vcf_dir)
 
     def get_range_in_other_gene(self, pos):
         """
         Find the correponding coordinates in the other gene
```

### Comparing `paraphase-2.2.1/paraphase.egg-info/PKG-INFO` & `paraphase-2.2.2/paraphase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paraphase
-Version: 2.2.1
+Version: 2.2.2
 Summary: paraphase: HiFi-based caller for highly homologous genes
 Home-page: https://github.com/PacificBiosciences/paraphase
 Author: Xiao Chen
 Author-email: xchen@pacificbiosciences.com
 License: BSD-3-Clause-Clear
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paraphase-2.2.1/paraphase.egg-info/SOURCES.txt` & `paraphase-2.2.2/paraphase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/setup.py` & `paraphase-2.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup
+import paraphase
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="paraphase",
-    version="2.2.1",
+    version=paraphase.__version__,
     description="paraphase: HiFi-based caller for highly homologous genes",
     long_description=readme(),
     url="https://github.com/PacificBiosciences/paraphase",
     author="Xiao Chen",
     author_email="xchen@pacificbiosciences.com",
     license="BSD-3-Clause-Clear",
     packages=["paraphase", "paraphase.genes"],
```

### Comparing `paraphase-2.2.1/tests/test_haplotype_assembler.py` & `paraphase-2.2.2/tests/test_haplotype_assembler.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/tests/test_paraphase.py` & `paraphase-2.2.2/tests/test_paraphase.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/tests/test_phaser.py` & `paraphase-2.2.2/tests/test_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/tests/test_prepare_bam_and_vcf.py` & `paraphase-2.2.2/tests/test_prepare_bam_and_vcf.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/tests/test_rccx_phaser.py` & `paraphase-2.2.2/tests/test_rccx_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.1/tests/test_smn1_phaser.py` & `paraphase-2.2.2/tests/test_smn1_phaser.py`

 * *Files identical despite different names*

