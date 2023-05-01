# Comparing `tmp/haplotyping-0.0.5.tar.gz` & `tmp/haplotyping-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haplotyping-0.0.5.tar", last modified: Tue Dec  6 09:39:49 2022, max compression
+gzip compressed data, was "haplotyping-0.0.6.tar", last modified: Mon May  1 11:52:34 2023, max compression
```

## Comparing `haplotyping-0.0.5.tar` & `haplotyping-0.0.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.504773 haplotyping-0.0.5/
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2021-06-02 10:04:29.000000 haplotyping-0.0.5/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)      425 2022-12-06 09:39:49.504486 haplotyping-0.0.5/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)       14 2021-06-02 10:04:29.000000 haplotyping-0.0.5/README.md
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.474789 haplotyping-0.0.5/haplotyping/
--rw-r--r--   0 matthijs   (501) staff       (20)      101 2022-11-24 12:53:25.000000 haplotyping-0.0.5/haplotyping/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)       22 2022-12-06 09:39:37.000000 haplotyping-0.0.5/haplotyping/_version.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.477566 haplotyping-0.0.5/haplotyping/api/
--rw-r--r--   0 matthijs   (501) staff       (20)      112 2022-11-24 12:55:52.000000 haplotyping-0.0.5/haplotyping/api/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    22089 2022-12-01 07:46:47.000000 haplotyping-0.0.5/haplotyping/api/api.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.480174 haplotyping-0.0.5/haplotyping/data/
--rw-r--r--   0 matthijs   (501) staff       (20)      212 2022-11-24 09:50:44.000000 haplotyping-0.0.5/haplotyping/data/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     8014 2022-09-20 07:55:39.000000 haplotyping-0.0.5/haplotyping/data/checkDatabase.py
--rw-r--r--   0 matthijs   (501) staff       (20)    28658 2022-10-15 13:11:33.000000 haplotyping-0.0.5/haplotyping/data/constructDatabase.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.486372 haplotyping-0.0.5/haplotyping/data/schema/
--rw-r--r--   0 matthijs   (501) staff       (20)      401 2022-09-07 12:28:45.000000 haplotyping-0.0.5/haplotyping/data/schema/data_default_experiments.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      454 2022-09-08 08:58:46.000000 haplotyping-0.0.5/haplotyping/data/schema/data_default_mappings.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)     1097 2022-09-08 07:45:58.000000 haplotyping-0.0.5/haplotyping/data/schema/data_default_markers.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      306 2022-09-06 17:27:01.000000 haplotyping-0.0.5/haplotyping/data/schema/data_default_metadata.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      517 2022-09-06 08:11:34.000000 haplotyping-0.0.5/haplotyping/data/schema/data_default_scores.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      992 2022-09-06 08:15:21.000000 haplotyping-0.0.5/haplotyping/data/schema/data_default_sequences.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)     1029 2022-09-02 06:57:46.000000 haplotyping-0.0.5/haplotyping/data/schema/data_default_varieties.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)     1050 2022-05-23 16:46:35.000000 haplotyping-0.0.5/haplotyping/data/schema/pedigree_ancestors.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      598 2022-09-02 06:47:09.000000 haplotyping-0.0.5/haplotyping/data/schema/pedigree_breeders.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      341 2022-09-02 06:53:51.000000 haplotyping-0.0.5/haplotyping/data/schema/pedigree_countries.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      529 2022-05-23 16:46:59.000000 haplotyping-0.0.5/haplotyping/data/schema/pedigree_synonyms.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)      903 2022-09-02 06:46:07.000000 haplotyping-0.0.5/haplotyping/data/schema/pedigree_varieties.schema.json
--rw-r--r--   0 matthijs   (501) staff       (20)    40843 2022-09-21 09:37:06.000000 haplotyping-0.0.5/haplotyping/data/validator.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1775 2022-06-01 07:52:46.000000 haplotyping-0.0.5/haplotyping/general.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.489840 haplotyping-0.0.5/haplotyping/graph/
--rw-r--r--   0 matthijs   (501) staff       (20)      196 2022-11-24 09:50:11.000000 haplotyping-0.0.5/haplotyping/graph/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     7098 2022-12-06 09:24:46.000000 haplotyping-0.0.5/haplotyping/graph/api.py
--rw-r--r--   0 matthijs   (501) staff       (20)    58189 2022-11-30 18:52:13.000000 haplotyping-0.0.5/haplotyping/graph/baseGraph.py
--rw-r--r--   0 matthijs   (501) staff       (20)    36540 2022-11-30 19:46:10.000000 haplotyping-0.0.5/haplotyping/graph/sections.py
--rw-r--r--   0 matthijs   (501) staff       (20)    62285 2022-11-27 09:28:18.000000 haplotyping-0.0.5/haplotyping/graph/sequence.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.493205 haplotyping-0.0.5/haplotyping/index/
--rw-r--r--   0 matthijs   (501) staff       (20)      119 2022-11-24 09:50:24.000000 haplotyping-0.0.5/haplotyping/index/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    15333 2022-09-29 07:28:32.000000 haplotyping-0.0.5/haplotyping/index/database.py
--rw-r--r--   0 matthijs   (501) staff       (20)    27142 2022-10-25 07:46:20.000000 haplotyping-0.0.5/haplotyping/index/reads.py
--rw-r--r--   0 matthijs   (501) staff       (20)    29940 2022-10-17 18:01:44.000000 haplotyping-0.0.5/haplotyping/index/splits.py
--rw-r--r--   0 matthijs   (501) staff       (20)   115233 2022-10-15 12:24:57.000000 haplotyping-0.0.5/haplotyping/index/storage.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.500504 haplotyping-0.0.5/haplotyping/service/
--rw-r--r--   0 matthijs   (501) staff       (20)      116 2022-11-24 09:50:34.000000 haplotyping-0.0.5/haplotyping/service/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     9239 2022-11-23 10:25:41.000000 haplotyping-0.0.5/haplotyping/service/api.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-09-23 16:27:38.000000 haplotyping-0.0.5/haplotyping/service/api_collection.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1663 2022-09-08 16:36:20.000000 haplotyping-0.0.5/haplotyping/service/api_country.py
--rw-r--r--   0 matthijs   (501) staff       (20)    11956 2022-11-28 17:11:58.000000 haplotyping-0.0.5/haplotyping/service/api_dataset.py
--rw-r--r--   0 matthijs   (501) staff       (20)    19780 2022-11-23 14:46:20.000000 haplotyping-0.0.5/haplotyping/service/api_kmer.py
--rw-r--r--   0 matthijs   (501) staff       (20)     4831 2022-09-30 09:36:03.000000 haplotyping-0.0.5/haplotyping/service/api_marker.py
--rw-r--r--   0 matthijs   (501) staff       (20)    15776 2022-11-23 12:57:26.000000 haplotyping-0.0.5/haplotyping/service/api_split.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1093 2021-09-17 12:29:55.000000 haplotyping-0.0.5/haplotyping/service/api_tools.py
--rw-r--r--   0 matthijs   (501) staff       (20)    20630 2022-11-28 18:02:44.000000 haplotyping-0.0.5/haplotyping/service/api_variety.py
--rw-r--r--   0 matthijs   (501) staff       (20)     7177 2022-09-23 18:28:20.000000 haplotyping-0.0.5/haplotyping/service/kmer_kmc.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2956 2022-09-30 09:22:50.000000 haplotyping-0.0.5/haplotyping/service/marker.py
--rw-r--r--   0 matthijs   (501) staff       (20)    18632 2022-11-25 07:51:41.000000 haplotyping-0.0.5/haplotyping/service/split.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.476535 haplotyping-0.0.5/haplotyping.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)      425 2022-12-06 09:39:48.000000 haplotyping-0.0.5/haplotyping.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     1994 2022-12-06 09:39:49.000000 haplotyping-0.0.5/haplotyping.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2022-12-06 09:39:48.000000 haplotyping-0.0.5/haplotyping.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)      201 2022-12-06 09:39:49.000000 haplotyping-0.0.5/haplotyping.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       18 2022-12-06 09:39:49.000000 haplotyping-0.0.5/haplotyping.egg-info/top_level.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2022-12-06 09:39:49.504857 haplotyping-0.0.5/setup.cfg
--rw-r--r--   0 matthijs   (501) staff       (20)     1152 2022-11-28 11:01:06.000000 haplotyping-0.0.5/setup.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.501883 haplotyping-0.0.5/tests/
--rw-r--r--   0 matthijs   (501) staff       (20)       33 2021-06-02 10:04:29.000000 haplotyping-0.0.5/tests/__init__.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.502776 haplotyping-0.0.5/tests/index/
--rw-r--r--   0 matthijs   (501) staff       (20)       40 2021-06-02 10:04:29.000000 haplotyping-0.0.5/tests/index/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    11079 2021-06-02 10:04:29.000000 haplotyping-0.0.5/tests/index/test_database.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2022-12-06 09:39:49.503621 haplotyping-0.0.5/tests/service/
--rw-r--r--   0 matthijs   (501) staff       (20)       36 2021-06-11 12:14:36.000000 haplotyping-0.0.5/tests/service/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    26188 2021-07-23 07:42:21.000000 haplotyping-0.0.5/tests/service/test_api.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1337 2021-06-02 10:04:29.000000 haplotyping-0.0.5/tests/test_general.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2021-06-16 07:44:07.000000 haplotyping-0.0.6/LICENSE
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      389 2023-05-01 11:52:34.121224 haplotyping-0.0.6/PKG-INFO
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       14 2021-06-16 07:44:07.000000 haplotyping-0.0.6/README.md
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      101 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       22 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/_version.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping/api/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      112 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/api/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    22089 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/api/api.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping/data/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      212 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/data/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9180 2023-05-01 11:45:58.000000 haplotyping-0.0.6/haplotyping/data/checkDatabase.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    29485 2023-05-01 11:45:04.000000 haplotyping-0.0.6/haplotyping/data/constructDatabase.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.117224 haplotyping-0.0.6/haplotyping/data/schema/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      401 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_experiments.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      454 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_mappings.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1097 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_markers.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      327 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_metadata.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      517 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_scores.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      993 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_sequences.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1029 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_varieties.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1050 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_ancestors.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      598 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_breeders.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      341 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_countries.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      529 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_synonyms.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      903 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_varieties.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    42098 2023-05-01 08:56:45.000000 haplotyping-0.0.6/haplotyping/data/validator.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1775 2022-03-10 19:41:20.000000 haplotyping-0.0.6/haplotyping/general.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.117224 haplotyping-0.0.6/haplotyping/graph/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      196 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     7206 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/api.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    58189 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/baseGraph.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    38481 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/sections.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    62285 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/sequence.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.117224 haplotyping-0.0.6/haplotyping/index/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      119 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/index/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    13104 2023-04-29 07:03:33.000000 haplotyping-0.0.6/haplotyping/index/database.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    41641 2023-05-01 09:11:12.000000 haplotyping-0.0.6/haplotyping/index/direct.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    34252 2023-05-01 09:13:06.000000 haplotyping-0.0.6/haplotyping/index/splits.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)   128031 2023-04-28 18:59:52.000000 haplotyping-0.0.6/haplotyping/index/storage.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/haplotyping/service/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      116 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9887 2023-05-01 08:05:15.000000 haplotyping-0.0.6/haplotyping/service/api.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4244 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/api_collection.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1663 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/service/api_country.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12310 2023-04-30 09:20:00.000000 haplotyping-0.0.6/haplotyping/service/api_dataset.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    20805 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/api_kmer.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4917 2023-04-30 09:20:57.000000 haplotyping-0.0.6/haplotyping/service/api_marker.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12952 2023-04-30 09:20:34.000000 haplotyping-0.0.6/haplotyping/service/api_split.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1093 2021-06-30 08:50:36.000000 haplotyping-0.0.6/haplotyping/service/api_tools.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    20951 2023-04-30 09:17:00.000000 haplotyping-0.0.6/haplotyping/service/api_variety.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     7177 2022-11-16 14:08:23.000000 haplotyping-0.0.6/haplotyping/service/kmer_kmc.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     2956 2022-11-16 14:08:23.000000 haplotyping-0.0.6/haplotyping/service/marker.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    18632 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/split.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping.egg-info/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      389 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/PKG-INFO
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1995 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        1 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      228 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/requires.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       18 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/top_level.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       38 2023-05-01 11:52:34.121224 haplotyping-0.0.6/setup.cfg
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1202 2023-05-01 11:15:54.000000 haplotyping-0.0.6/setup.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/tests/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       33 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/__init__.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/tests/index/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       40 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/index/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11079 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/index/test_database.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/tests/service/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       36 2021-06-29 16:25:06.000000 haplotyping-0.0.6/tests/service/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    26188 2021-10-09 11:28:48.000000 haplotyping-0.0.6/tests/service/test_api.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1337 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/test_general.py
```

### Comparing `haplotyping-0.0.5/haplotyping/api/api.py` & `haplotyping-0.0.6/haplotyping/api/api.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/checkDatabase.py` & `haplotyping-0.0.6/haplotyping/data/checkDatabase.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                         self._cursor.execute(query, (dataset["id"], collection["id"],))  
                     else:
                         self._logger.error("marker collection {}: markers for {} not found in database {}".format(
                             collection["name"], dataset["variety"], dataset["location"]))
             self._connection.commit()
             
     def _check_kmers(self):
-        query = """SELECT * FROM `collection` WHERE `type` = 'kmer' ORDER BY `id`"""
+        query = """SELECT * FROM `collection` WHERE `type` = 'wgs' OR `type` = 'baits' ORDER BY `id`"""
         self._cursor.execute(query)
         collections = self._cursor.fetchall()        
         for row in collections:
             collection = dict(zip(row.keys(), row))
             if collection["location"]!=None:
                 if not os.path.exists(os.path.join(self._kmerDir,collection["location"])):
                     self._logger.error("kmer collection {}: location {} not found".format(
@@ -134,20 +134,36 @@
                     else:
                         if not os.path.exists(os.path.join(kmerLocation,"kmer.kmc.kmc_pre")):  
                             kmerNotFound+=1
                         elif not os.path.exists(os.path.join(kmerLocation,"kmer.kmc.kmc_suf")):  
                             kmerNotFound+=1
                         else:
                             datasetType = "kmer"
-                            if not os.path.exists(os.path.join(kmerLocation,"kmer.data.h5")): 
+                            datasetSubType = None
+                            datasetVersion = None
+                            dbLocation = os.path.join(kmerLocation,"kmer.data.h5")
+                            if not os.path.exists(dbLocation): 
                                 splitNotFound+=1
                             else:
-                                datasetType = "split"
-                            query = """UPDATE `dataset` SET `type` = ? WHERE `id` = ? AND `collection_id` = ?"""
-                            self._cursor.execute(query, (datasetType, dataset["id"], collection["id"],))  
+                                try:
+                                    with h5py.File(dbLocation, "r") as h5file:                                        
+                                        datasetVersion = h5file["/config"].attrs["version"]
+                                        if not ("/relations" in h5file and "/relations/direct" in h5file):
+                                            datasetSubType = "split"
+                                        elif not ("/relations/readData" in h5file):
+                                            datasetSubType = "direct"
+                                        else:
+                                            datasetSubType = "read"
+                                        datasetType = "split"
+                                except:
+                                    self._logger.error("couldn't parse {}".format(dbLocation))
+                            query = """UPDATE `dataset` SET `type` = ?, `subtype` = ?, `version` = ?
+                                        WHERE `id` = ? AND `collection_id` = ?"""
+                            self._cursor.execute(query, (datasetType, datasetSubType, datasetVersion, 
+                                                         dataset["id"], collection["id"],))  
             self._connection.commit()            
             if locationsNotFound>0:
                 self._logger.error("kmer collection {}: {} location(s) not found".format(
                                 collection["name"], locationsNotFound))
             if kmerNotFound>0:
                 self._logger.error("kmer collection {}: {} k-mer databases not found".format(
                                 collection["name"], locationsNotFound))
```

### Comparing `haplotyping-0.0.5/haplotyping/data/constructDatabase.py` & `haplotyping-0.0.6/haplotyping/data/constructDatabase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!python
 
 import os,logging,tempfile
-from frictionless import Package, extract
+from frictionless import Package
 import gzip,csv,pandas as pd, numpy as np
 import sqlite3, json, time
 from sqlite3 import Error
 import h5py, random, shutil
 
 class ConstructDatabase:
     
@@ -133,15 +133,15 @@
                             );
                             CREATE INDEX "breeder_country" ON "breeder" ("country");
                             CREATE TABLE IF NOT EXISTS "collection" (
                                 "id" INTEGER NOT NULL,
                                 "uid" VARCHAR(13) NULL,
                                 "resource" VARCHAR(255) NULL,
                                 "internal_id" INTEGER NOT NULL,
-                                "type" VARCHAR(6) CHECK("type" IN ("marker","kmer") ) NOT NULL,
+                                "type" VARCHAR(6) CHECK("type" IN ("marker","wgs","baits") ) NOT NULL,
                                 "name" VARCHAR(255) NULL,
                                 "experiment" VARCHAR(255) NULL,
                                 "location" VARCHAR(255) NULL,
                                 PRIMARY KEY ("id")
                             );
                             CREATE UNIQUE INDEX "collection_resource_internal_type" 
                                 ON "collection" ("resource","internal_id","type");
@@ -150,46 +150,48 @@
                                 "id" INTEGER NOT NULL,
                                 "uid" VARCHAR(13) NULL,
                                 "variety" VARCHAR(13) NULL,
                                 "collection_id" INTEGER NOT NULL,
                                 "internal_id" INTEGER NOT NULL,
                                 "location" VARCHAR(255) NULL,
                                 "type" VARCHAR(6) CHECK("type" IN ("marker","kmer","split") ) NULL,
+                                "subtype" VARCHAR(6) CHECK("subtype" IN ("split","direct","read") ) NULL,
+                                "version" VARCHAR(8) NULL,
                                 PRIMARY KEY ("id")
                             );
                             CREATE INDEX "dataset_collection_id" ON "dataset" ("collection_id");
                             CREATE UNIQUE INDEX "dataset_collection_internal" 
                                 ON "dataset" ("collection_id","internal_id");
                             CREATE UNIQUE INDEX "dataset_uid" ON "dataset" ("uid");
                             CREATE INDEX "dataset_variety" ON "dataset" ("variety");"""
                     self._connection.executescript(sql)
                     #countries
-                    countries = pd.DataFrame(extract(package.get_resource("pedigree_countries")))
+                    countries = pd.DataFrame(package.get_resource("pedigree_countries").read_rows())
                     countries = countries[["code","name"]]
                     countries.columns = ["uid","name"]
                     countries.to_sql("country", con=self._connection, index=False, if_exists="append")
                     self._logger.info("add {} countries".format(len(countries)))
                     #breeders
-                    breeders = pd.DataFrame(extract(package.get_resource("pedigree_breeders")))
+                    breeders = pd.DataFrame(package.get_resource("pedigree_breeders").read_rows())
                     breeders = breeders[["id","name","country"]]
                     breeders.to_sql("breeder", con=self._connection, index=False, if_exists="append")
                     self._logger.info("add {} breeders".format(len(breeders)))
                     #varieties
-                    varieties = pd.DataFrame(extract(package.get_resource("pedigree_varieties")))
+                    varieties = pd.DataFrame(package.get_resource("pedigree_varieties").read_rows())
                     varieties = varieties[["uid", "name", "yearMin", "yearMax", "origin", "breederId"]]
                     varieties.columns = ["uid", "name", "year_min", "year_max", "origin", "breeder_id"]
                     varieties.to_sql("variety", con=self._connection, index=False, if_exists="append")
                     self._logger.info("add {} varieties".format(len(varieties)))
                     #ancestors
-                    ancestors = pd.DataFrame(extract(package.get_resource("pedigree_ancestors")))
+                    ancestors = pd.DataFrame(package.get_resource("pedigree_ancestors").read_rows())
                     ancestors = ancestors[["id","variety", "ancestor", "type", "offspring"]]
                     ancestors.to_sql("variety_ancestor", con=self._connection, index=False, if_exists="append")
                     self._logger.info("add {} ancestors".format(len(ancestors)))
                     #synonyms
-                    synonyms = pd.DataFrame(extract(package.get_resource("pedigree_synonyms")))
+                    synonyms = pd.DataFrame(package.get_resource("pedigree_synonyms").read_rows())
                     synonyms = synonyms[["uid","synonym"]]
                     synonyms.to_sql("variety_synonym", con=self._connection, index=False, if_exists="append")
                     self._logger.info("add {} synonyms".format(len(synonyms)))
                     return
         self._logger.error("no pedigree found in {}".format(self._baseDir))
                     
                     
@@ -254,19 +256,20 @@
         self._cursor.execute(query, (resource, int(internal_id),collection_type,))  
         collection = self._cursor.fetchone()
         if collection:
             return (collection[0],uid,)
         else:
             raise Exception("could not create collection")
         
-    def _createDataset(self,variety,collection_id,collection_uid,internal_id,location,type=None):
+    def _createDataset(self,variety,collection_id,collection_uid,internal_id,location,type=None,subtype=None,version=None):
         uid = self._newDatasetUid(collection_uid, internal_id)
-        query = """INSERT OR IGNORE INTO `dataset` (`uid`,`variety`,`collection_id`,`internal_id`,`location`,`type`) 
-        VALUES (?,?,?,?,?,?)"""
-        self._connection.execute(query, (uid,variety, int(collection_id), int(internal_id), location, type, ))
+        query = """INSERT OR IGNORE INTO `dataset` (`uid`,`variety`,`collection_id`,`internal_id`,
+                            `location`,`type`,`subtype`,`version`) 
+        VALUES (?,?,?,?,?,?,?,?)"""
+        self._connection.execute(query, (uid,variety, int(collection_id), int(internal_id), location, type, subtype, version))
         self._connection.commit()
         
     def _getUint(maximumValue):
         if maximumValue<=np.iinfo(np.uint8).max:
             return "uint8"
         elif maximumValue<=np.iinfo(np.uint16).max:
             return "uint16"
@@ -282,53 +285,59 @@
         package = Package(fileName)        
         if package.has_resource("varieties") and package.has_resource("metadata") and package.has_resource("experiments"):
             if (package.has_resource("sequences") or 
                     (package.has_resource("scores") 
                      and package.has_resource("markers") 
                      and package.has_resource("mappings"))):
                 #get shared data
-                metadata = pd.DataFrame(extract(package.get_resource("metadata")))
+                metadata = pd.DataFrame(package.get_resource("metadata").read_rows())
                 metadata = {x:y for (x,y,) in zip(metadata["label"],metadata["value"])}
-                varieties = pd.DataFrame(extract(package.get_resource("varieties")))
-                experiments = pd.DataFrame(extract(package.get_resource("experiments")))
+                varieties = pd.DataFrame(package.get_resource("varieties").read_rows())
+                experiments = pd.DataFrame(package.get_resource("experiments").read_rows())
                 if len(varieties)>0 and len(experiments)>0:
                     varieties = varieties.set_index("id")
                     experiments = experiments.set_index("id")
                     self._logger.info("store data for '{}'".format(metadata.get("name",resourceName)))
                 else:
                     return
                 #process sequence data
                 if package.has_resource("sequences"):
-                    sequences = pd.DataFrame(extract(package.get_resource("sequences")))                    
+                    collectionList = {}
+                    sequences = pd.DataFrame(package.get_resource("sequences").read_rows())
                     if len(sequences)>0:
                         for experiment_id in set(sequences["experiment_id"]):
                             collectionId=None
                             for id,row in sequences[sequences["experiment_id"]==experiment_id].iterrows():
                                 variety = varieties.loc[row["variety_id"]]
                                 if variety["uid"]:
-                                    if collectionId==None:
+                                    #use seperate collection for each sequence type
+                                    if (len(collectionList)==0) or not row["type"] in collectionList:
                                         experiment_name = experiments.loc[experiment_id]["name"]
                                         locationResource = metadata.get("location","")
                                         locationResource = "" if locationResource==None else locationResource
                                         locationExperiment = experiments.loc[experiment_id]["location"]
                                         locationExperiment = "" if locationExperiment==None else locationExperiment
                                         location = os.path.join(locationResource,locationExperiment)
                                         (collectionId,collectionUid) = self._createCollection(
-                                             resourceName, experiment_id, "kmer",
+                                             resourceName, experiment_id, row["type"],
                                              metadata.get("name",resourceName), experiment_name, location)
-                                    self._createDataset(variety["uid"],collectionId,collectionUid,
+                                        collectionList[row["type"]] = {"collectionId": collectionId, 
+                                                                       "collectionUid": collectionUid}
+                                    self._createDataset(variety["uid"],
+                                                        collectionList[row["type"]]["collectionId"],
+                                                        collectionList[row["type"]]["collectionUid"],
                                                         row["variety_id"],row["location"])
 
                 #process marker data
                 if (package.has_resource("scores") and package.has_resource("markers") and package.has_resource("mappings")):
-                    scores = pd.DataFrame(extract(package.get_resource("scores")))
-                    markers = pd.DataFrame(extract(package.get_resource("markers")))
+                    scores = pd.DataFrame(package.get_resource("scores").read_rows())
+                    markers = pd.DataFrame(package.get_resource("markers").read_rows())
                     if len(markers)>0:
                         markers = markers.set_index("id")
-                    mappings = pd.DataFrame(extract(package.get_resource("mappings")))
+                    mappings = pd.DataFrame(package.get_resource("mappings").read_rows())
                     #process scores
                     for score_id,row in scores.iterrows():
                         varietyList = []
                         markerList = []
                         resourceData = {"data":[],"lg":[],"marker":[],"variety":[], "varietyIndex": {}}
                         with tempfile.NamedTemporaryFile() as tmpMarkerFile:
                             sourceFilename = os.path.join(package.basepath,row["source"])
```

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/data_default_markers.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/data_default_markers.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/data_default_scores.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/data_default_scores.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/data_default_sequences.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/data_default_sequences.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990740740740741%*

 * *Differences: {"'fields'": "{2: {'constraints': {'enum': {insert: [(1, 'baits')], delete: [1]}}}}"}*

```diff
@@ -14,15 +14,15 @@
             "name": "experiment_id",
             "type": "integer"
         },
         {
             "constraints": {
                 "enum": [
                     "wgs",
-                    "bait"
+                    "baits"
                 ],
                 "required": true
             },
             "name": "type",
             "type": "string"
         },
         {
```

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/data_default_varieties.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/data_default_varieties.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/pedigree_ancestors.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/pedigree_ancestors.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/pedigree_breeders.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/pedigree_breeders.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/pedigree_synonyms.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/pedigree_synonyms.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/schema/pedigree_varieties.schema.json` & `haplotyping-0.0.6/haplotyping/data/schema/pedigree_varieties.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/data/validator.py` & `haplotyping-0.0.6/haplotyping/data/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os, logging, tempfile
-import gzip,csv
+import gzip,csv,json
 from openpyxl import load_workbook
-from frictionless import Resource, Schema, Field, Package, Layout
-from frictionless.plugins.excel import ExcelDialect
-from frictionless import validate, extract
+from frictionless import Resource, Schema, Package, Dialect, formats, errors
+from frictionless import validate
 import pandas as pd, numpy as np, textwrap
 from shutil import copyfile
 
 class ValidateReport:
     
     def __init__(self, logger:logging.Logger):
         self._logger = logger
@@ -165,15 +164,16 @@
         if isinstance(schema, Schema):
             self._report.addReportDebug(resourceName,"use provided schema") 
             resourceSchema = schema
         elif isinstance(schema, str):
             schemaFilename = os.path.join(self._schemaPath,schema)
             if os.access(schemaFilename, os.R_OK):
                 self._report.addReportDebug(resourceName,"validate using schema '{}'".format(schema)) 
-                resourceSchema = Schema(schemaFilename)
+                with open(schemaFilename, "r") as f:                 
+                    resourceSchema = Schema.from_descriptor(json.load(f))
             else:
                 self._report.addReportError(resourceName,"could not read schema '{}'".format(schemaFilename))
         else:
             self._report.addReportError(resourceName,"no recognized schema format")
         resource = Resource([[field.name for field in resourceSchema.fields]])
         resource.schema = resourceSchema
         if layout:
@@ -189,40 +189,39 @@
         #define resource
         self._allowedSheets.add(sheetName)
         self._report.addReport(resourceName, True)
         if not sheetName in self._availableSheets:
             self._report.addReportError(resourceName,"sheet '{}' not available".format(sheetName))
         else:
             self._report.addReportDebug(resourceName,"define resource '{}'".format(sheetName))
-            resource = Resource(basepath=self._dataPath, path=self._resourceFilename, hashing="", 
-                                                dialect=ExcelDialect(sheet=sheetName, preserve_formatting=False))  
-            if headerRows>1:
-                resource.layout=Layout(header_rows=[headerRows])
+            dialect = Dialect(header_rows=[headerRows])
+            dialect.add_control(formats.ExcelControl(sheet=sheetName, preserve_formatting=False))
+            resource = Resource(basepath=self._dataPath, path=self._resourceFilename, dialect=dialect)  
             #set name and remove if exists
             if self._package.has_resource(resourceName):
                 self._package.remove_resource(resourceName)
             resource.name = resourceName
             #try to get schema
             if isinstance(schema, Schema):
                 self._report.addReportDebug(resourceName,"use provided schema") 
                 resource.schema = schema
             elif isinstance(schema, str):
                 schemaFilename = os.path.join(self._schemaPath,schema)
                 if os.access(schemaFilename, os.R_OK):
                     self._report.addReportDebug(resourceName,"validate using schema '{}'".format(schema)) 
-                    resource.schema = Schema(schemaFilename)
+                    with open(schemaFilename, "r") as f:       
+                        resource.schema = Schema.from_descriptor(json.load(f))
                 else:
                     self._report.addReportError(resourceName,"could not read schema '{}'".format(schemaFilename))
             else:
                 self._report.addReportDebug(resourceName,"no recognized schema format")
             #check string types, empty rows and columns
             if (self._adjustTypeForStringColumns and not 
                 validate(resource, pick_errors=["type-error"], skip_errors=skip_errors).valid):
-                
-                stringColumnNames = [field["name"] for field in resource.schema.fields if (field.get("type",None)=="string")]
+                stringColumnNames = [field.name for field in resource.schema.fields if (field.type=="string")]
                 self._updateTypeForStringColumns(sheetName, stringColumnNames, headerRows, resourceName)                
             if self._removeEmptyRows and not validate(resource, pick_errors=["blank-row"], skip_errors=skip_errors).valid:
                 self._removeEmptyRowsForSheet(sheetName,resourceName)
             if self._removeEmptyColumns and not validate(resource, pick_errors=["extra-label"], skip_errors=skip_errors).valid:
                 self._removeEmptyColumnsForSheet(sheetName,resourceName)
             self._report.addReportDebug(resourceName,"validate using schema")    
             if not skip_errors==None:
@@ -240,20 +239,20 @@
             #check missing columns for normal run
             if skip_errors==None and not resource_validation.valid:
                 self._checkMissingColumns(sheetName,resourceName,headerRows-1)
     
     def _validatePackage(self):
         self._report.addReport("package", False)
         self._report.addReportDebug("package","validate package") 
-        package_validation = validate(self._package)
+        package_validation = self._package.validate()
+        self._report.setReportFrictionless("package", package_validation)
         if not package_validation.valid:
-            self._report.addReportError("package","frictionless validation package failed")            
+            self._report.addReportError("package","frictionless validation package failed")   
         else:
             self._report.addReportInfo("package","succesfull frictionless validation package")
-        self._report.setReportFrictionless("package",package_validation)
         #return package and validation report
         return package_validation
     
     def _validateLogic(self):
         self._report.addReport("logic", False)
         try:
             if not self._allowAdditionalSheets:
@@ -435,23 +434,41 @@
     
     def createReport(self):
         """
         Create JSON object with report
         """
         def createFrictionlessData(fdata):
             list = []
-            for task in fdata["tasks"]:
-                for error in task["errors"]:
-                    list.append({"resource": task["resource"]["name"],
-                                 "rowPosition": error.get("rowPosition",None), 
-                                 "fieldPosition": error.get("fieldPosition",None),
-                                 "code": error.get("code",None),
-                                 "description": error.get("description",None)})
+            for task in fdata.tasks:
+                for error in task.errors:
+                    list.append({"resource": task.name,
+                                 "rowPosition": error.get_defined("row_number"), 
+                                 "rowPositions": error.get_defined("row_numbers"), 
+                                 "fieldPosition": error.get_defined("field_number"),
+                                 "fieldPositions": error.get_defined("field_numbers"),
+                                 "type": error.__class__.__name__,
+                                 "message": error.get_defined("message"),
+                                 "description": error.get_defined("description")})
             return pd.DataFrame(list)
-        def excelCoordinates(row, col):
+        def excelCoordinates(row, col, rows, cols):
+            if row and col:
+                return excelCoordinate(row,col)
+            elif row and cols:
+                locations = [excelCoordinate(row,col) for col in cols]
+                locations.remove(None)
+                return(",".join(locations))
+            elif rows and col:
+                locations = [excelCoordinate(row,col) for row in rows]
+                locations.remove(None)
+                return(",".join(locations))
+            elif row or col:
+                return excelCoordinate(row,col)
+            else:
+                return None
+        def excelCoordinate(row, col):
             try:
                 LETTERS = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
                 if not col==None and not np.isnan(col):
                     result = []
                     while col:
                         col, rem = divmod(col-1, 26)
                         result[:0] = LETTERS[int(rem)]
@@ -462,63 +479,66 @@
                 elif not row ==None and not np.isnan(row):
                     return "row "+str(int(row))
                 else:
                     return None
             except:
                 return None
         reportObject = {"name": os.path.basename(self._name), "valid": self.valid, "reports": []}
-        previousFrictionlessCodes = set()
+        previousFrictionlessTypes = set()
         for report in self._report.reports:
             isNotValid=((not self._report[report]["valid"]) or 
                         ("frictionless" in self._report[report].keys() and 
-                         (not self._report[report]["frictionless"]["valid"])))
+                         (not self._report[report]["frictionless"].valid)))
             reportDetails = {"name": report, 
                              "valid": False if isNotValid else True,
                              "warnings": [], "errors": [], "frictionless": []}  
             if isNotValid or len(self._report[report]["warnings"])>0:
                 if len(self._report[report]["warnings"])>0:
                     for warning in self._report[report]["warnings"]:
                         reportDetails["warnings"].append(warning)
                 if len(self._report[report]["errors"])>0:
                     for error in self._report[report]["errors"]:
                         reportDetails["errors"].append(error)
                 if "frictionless" in self._report[report].keys():
                     frictionlessData = createFrictionlessData(self._report[report]["frictionless"])
                     if len(frictionlessData)>0:
-                        frictionlessCodes = frictionlessData.code.value_counts()
+                        frictionlessTypes = frictionlessData.type.value_counts()
                         if report=="package":
                             #don't repeat frictionless entries from separate sheets
-                            frictionlessCodeList = set(frictionlessCodes.index).difference(previousFrictionlessCodes)
-                            if len(frictionlessCodeList)==0:
+                            frictionlessTypeList = set(frictionlessTypes.index).difference(previousFrictionlessTypes)
+                            if len(frictionlessTypeList)==0:
                                 continue
                         else:
-                            frictionlessCodeList = frictionlessCodes.index
-                            previousFrictionlessCodes.update(frictionlessCodes.index)
-                        for code in frictionlessCodeList:
-                            frictionlessDetails = {"name": code, "details": []}
-                            for id,row in frictionlessData[frictionlessData.code==code].iterrows():
-                                location = excelCoordinates(row["rowPosition"],row["fieldPosition"])
+                            frictionlessTypeList = frictionlessTypes.index
+                            previousFrictionlessTypes.update(frictionlessTypes.index)
+                        for type in frictionlessTypeList:
+                            frictionlessDetails = {"name": type, "details": []}
+                            for id,row in frictionlessData[frictionlessData.type==type].iterrows():
+                                location = excelCoordinates(row["rowPosition"],row["fieldPosition"],
+                                                            row["rowPositions"],row["fieldPositions"])
                                 frictionlessDetails["details"].append({"resource": row["resource"], 
                                                                        "location": location,
                                                                        "row": row["rowPosition"],
+                                                                       "rows": row["rowPositions"],
                                                                        "column": row["fieldPosition"],
+                                                                       "columns": row["fieldPositions"],
+                                                                       "message": row["message"],
                                                                        "description": row["description"]})   
                             reportDetails["frictionless"].append(frictionlessDetails)
             reportObject["reports"].append(reportDetails)
         return reportObject
         
     def createTextReport(self, textWidth=100, examples=3):
         """
         Create text version report
         """
         #create report
         reportObject = self.createReport()
         #create text    
         reportText = "=== {} '{}' ===".format(("VALID" if reportObject["valid"] else "INVALID"),reportObject["name"])
-        previousFrictionlessCodes = set()
         for reportDetails in reportObject["reports"]:
             if (not reportDetails["valid"]) or len(reportDetails["warnings"])>0:
                 reportText = reportText + "\n** problem with '{}' **".format(reportDetails["name"])
                 if len(reportDetails["warnings"])>0:
                     reportText = reportText + "\n- warnings:"
                     for warning in reportDetails["warnings"]:
                         reportText = reportText + "\n" + textwrap.fill(warning,textWidth-4,
@@ -535,15 +555,15 @@
                                                                                       len(frictionlessItem["details"]))
                         rowCounter = 0
                         for row in frictionlessItem["details"]:
                             if rowCounter>=examples:
                                 reportText = reportText + "\n    - ..."
                                 break
                             reportText = reportText + "\n" + textwrap.fill("{}{}: {}".format(row["resource"],
-                                     ((" ["+row["location"]+"]") if not row["location"]==None else ""),row["description"])
+                                     ((" ["+row["location"]+"]") if not row["location"]==None else ""),row["message"])
                                      ,textWidth-6,initial_indent="    - ",subsequent_indent="      ")
                             rowCounter+=1
         return reportText
         
     @property
     def valid(self):        
         return self._report.valid
@@ -719,19 +739,19 @@
                     assert os.access(os.path.join(self._schemaPath,item["schema"]), os.R_OK)
                     self._createEmptyResource(item["sheet"], item["schema"], item.get("name", item["sheet"]))
                     
                     
             #check marker scores
             if (self._package.has_resource("scores") and self._package.has_resource("markers") 
                 and self._package.has_resource("varieties")):
-                scores = pd.DataFrame(extract(self._package.get_resource("scores")))
-                markers = pd.DataFrame(extract(self._package.get_resource("markers")))
+                scores = pd.DataFrame(self._package.get_resource("scores").read_rows())
+                markers = pd.DataFrame(self._package.get_resource("markers").read_rows())
                 if len(markers)>0:
                     markers = markers.set_index("id")
-                varieties = pd.DataFrame(extract(self._package.get_resource("varieties")))
+                varieties = pd.DataFrame(self._package.get_resource("varieties").read_rows())
                 if len(varieties)>0:
                     varieties = varieties.set_index("id")        
                 for score_id,score_row in scores.iterrows():
                     scoreFilename = score_row["source"]
                     self._report.addReport(score_row["source"], False)
                     fullScoreFilename = os.path.join(self._dataPath, scoreFilename)
                     if not os.access(fullScoreFilename, os.R_OK):
```

### Comparing `haplotyping-0.0.5/haplotyping/general.py` & `haplotyping-0.0.6/haplotyping/general.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/graph/api.py` & `haplotyping-0.0.6/haplotyping/graph/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         #call parent constructor
         super(haplotyping.graph.api.APIGraph, self).__init__()
         #logger
         self._api_logger = logging.getLogger(__name__)
         #store call parameters
         self._baseUrl : str = str(url)
         self._uid : str = str(uid)
+        self._varietyUid : str = None
         self._username : str = username
         self._password : str = password
         #initialise
         self._variety : str = None
         self._collection : str = None
         self._datasetFrequencyCkmers = set()
         self._datasetFrequencies = {}
@@ -52,14 +53,15 @@
                 dataset = data["list"][0]
                 if not (dataset["type"]=="kmer" or dataset["type"]=="split"):
                     self._api_logger.error("dataset {} has no k-mer database".format(self._uid))
                 if not (dataset["type"]=="split"):
                     self._api_logger.error("dataset {} has no splitting k-mer database".format(self._uid))   
                 if dataset["variety"]:
                     self._variety = str(dataset["variety"]["name"])
+                    self._varietyUid = str(dataset["variety"]["uid"])
                     self._api_logger.debug("set variety to '{}'".format(self._variety))
                 if dataset["collection"]:
                     self._collection = str(dataset["collection"]["name"])
                     self._api_logger.debug("set collection to '{}'".format(self._collection))
                 if self._variety:
                     self._name = "'{}'".format(self._variety)
                     if self._collection:
```

### Comparing `haplotyping-0.0.5/haplotyping/graph/baseGraph.py` & `haplotyping-0.0.6/haplotyping/graph/baseGraph.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/graph/sections.py` & `haplotyping-0.0.6/haplotyping/graph/sections.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging,requests,re, html
 import haplotyping.graph.baseGraph as baseGraph
+from haplotyping.graph.api import APIGraph
 from haplotyping.general import General
 from graphviz import Digraph
 
 class Sections():
     """constructing linear ordered sections from candidates in the De Bruijn graph"""
     
     def __init__(self, graph: baseGraph.Graph):
@@ -13,14 +14,17 @@
         assert isinstance(graph, baseGraph.Graph)
         #logger
         self._logger = logging.getLogger(__name__)
         
         self._graph = graph
         self._parts = []
         
+        self._datasetFrequencies = None
+        self._datasetVarieties = None
+        
         #create sections
         for baseConnectedCandidates in self._graph.getConnectedCandidates(True):
             self._createSections(baseConnectedCandidates)
             
             
     def getOrientatedCkmers(self):
         orientatedCkmers = set()
@@ -30,14 +34,23 @@
         
     def getCandidates(self):
         candidates = []
         for orientatedCkmer in self.getOrientatedCkmers():
             if self._graph._orientatedCkmers[orientatedCkmer].candidate():
                 candidates.append(orientatedCkmer)
         return set(candidates)
+    
+    def processDatasetFrequencies(self):
+        if isinstance(self._graph, APIGraph):
+            self._datasetFrequencies = self._graph.getDatasetFrequencies()
+            self._datasetVarieties = self._graph.getDatasetVarieties()      
+            for part in self._parts:
+                part._processDatasetFrequencies()                
+        else:
+            self._logger.warning("unsupported for this graph type")
         
     def _createSections(self, connectedCandidates):
         #compute section start entries (not every connected start is necessarily a section start)
         shortestDistances = self._graph.getShortestDistances()
         startEntries = connectedCandidates["start"]
         problematicStartEntries = set()
         for orientatedCkmer in startEntries:
@@ -54,15 +67,15 @@
             if len(problematicStartEntries)==len(startEntries):
                 self._logger.warning("all {} start entries sections problematic".format(len(startEntries)))
             else:
                 startEntries = startEntries.difference(problematicStartEntries)
                 self._logger.debug("ignore {} start entries, continue with {} for sections".format(
                     len(problematicStartEntries),len(startEntries)))
         #now try to create sections       
-        part = self.Part(self._graph)   
+        part = self.Part(self)   
         partOrientatedCkmers = set()
         sectionItem = self.SectionItem(startEntries, connectedCandidates["start"], connectedCandidates["end"],
                                        connectedCandidates["connected"],self._graph)
         part._append(sectionItem)
         partOrientatedCkmers.update(sectionItem._orientatedCkmers)
         while(len(sectionItem._end["ckmers"].difference(connectedCandidates["end"]))>0):
             newStartCkmers = (sectionItem._end["ckmers"]
@@ -111,26 +124,30 @@
             kwargs["label"] = "Part {}".format(i+1)
             self._parts[i].visualize(*args, **kwargs)
         return g
                        
     
     class Part():
         
-        def __init__(self, graph):
+        def __init__(self, sections):
             """
             construct part
             """
             #logger
             self._logger = logging.getLogger(__name__)
             
-            self._graph = graph
+            self._sections = sections
+            self._graph = sections._graph
             self._sectionItems = []
             self._order : int = None
             self._pathNumber : int = None
                 
+            self._datasets = set()
+            self._varieties = set()
+                
         def __repr__(self):
             text = "Part graph"
             if self._graph._name:
                 text = "{} {}".format(text,self._graph._name)
             text = "{}; containing {} section{} with {} path{}".format(text,len(self._sectionItems),
                    "s" if len(self._sectionItems)>1 else "", self._pathNumber, "s" if self._pathNumber>1 else "")
             return text
@@ -154,19 +171,33 @@
                     if not orientatedCkmer in sectionItem._end["ckmers"]:
                         self._pathNumber += numbers[orientatedCkmer]
             #add all remaining   
             for orientatedCkmer in numbers:
                 if orientatedCkmer in sectionItem._end["ckmers"]:
                     self._pathNumber += numbers[orientatedCkmer]            
             
-        def number(self):
+        def _processDatasetFrequencies(self, ignoreDatasets=[]):
+            for sectionItem in self._sectionItems:
+                for sectionItemPath in sectionItem._paths:
+                    orientatedCkmers = sectionItemPath.getOrientatedCkmers()
+                    sectionItemPath._datasets = set(self._sections._datasetFrequencies.index)
+                    for orientatedCkmer in orientatedCkmers:
+                        ckmerDatasets=self._sections._datasetFrequencies.index[
+                            self._sections._datasetFrequencies[orientatedCkmer[0]]>0]
+                        sectionItemPath._datasets = sectionItemPath._datasets.intersection(ckmerDatasets)
+                    sectionItemPath._varieties = set([self._sections._datasetVarieties[ds]["uid"] 
+                                                      for ds in sectionItemPath._datasets 
+                                                      if ds in self._sections._datasetVarieties])
+                    print(len(sectionItemPath._datasets))
+        
+        def sectionNumber(self):
             return len(self._sectionItems)
         
         def section(self, i):
-            if i>0 and i<=self.number():
+            if i>0 and i<=self.sectionNumber():
                 return self._sectionItems[i-1]
         
         def getOrientatedCkmers(self):
             orientatedCkmers = set()
             for sectionItem in self._sectionItems:
                 orientatedCkmers.update(sectionItem._orientatedCkmers)
             return orientatedCkmers
@@ -209,19 +240,19 @@
                 g = Digraph()
             
             partGraph=g.subgraph(name="cluster_{}".format(config["prefix"]))      
             
             with partGraph as pg:
                 if config["label"]:
                     graph_label = config["label"]
-                    graph_label = "{} with {} section{}".format(graph_label, self.number(), 
-                                                                "s" if self.number()>1 else "")
+                    graph_label = "{} with {} section{}".format(graph_label, self.sectionNumber(), 
+                                                                "s" if self.sectionNumber()>1 else "")
                 else:
-                    graph_label = "{} section{}".format(self.number(),
-                                                                "s" if self.number()>1 else "")
+                    graph_label = "{} section{}".format(self.sectionNumber(),
+                                                                "s" if self.sectionNumber()>1 else "")
                     if self._graph._name:
                         graph_label = "{} for Graph {}".format(graph_label,self._graph._name)
                 graph_label = ("<" + 
                                   "<font point-size=\"12\" color=\"grey\">{}</font><br/>".format(graph_label) +
                                   "<font point-size=\"10\">{:,} paths</font><br/>".format(self._pathNumber) +
                                   ">")
                 graph_style = config["baseStylePart"]
@@ -272,22 +303,22 @@
                             ag.attr(label=arm_label, style=arm_style, fillcolor=arm_fillcolor, 
                                 color=arm_color, penwidth=str(arm_penwidth), labelloc="t", nodesep="0", ranksep="0")
 
                             ag.node("arm_{}_{}".format(self._graph._arms[j].armType(),
                                                        self._graph._arms[j].key()), shape="point")
                 #sections
                 previousPrefix = ""
-                for j in range(self.number()):
+                for j in range(self.sectionNumber()):
                     sectionItem = self.section(j+1)
                     section_prefix = "graph_section_{}".format(j)
-                    section_label = "Section {} of {}".format(j+1,self.number())
+                    section_label = "Section {} of {}".format(j+1,self.sectionNumber())
                     sharedStart = (self._sectionItems[j-1]._orientatedCkmers.intersection(sectionItem._orientatedCkmers) 
                                    if j>0 else set())
                     sharedEnd = (self._sectionItems[j+1]._orientatedCkmers.intersection(sectionItem._orientatedCkmers) 
-                                   if j<(self.number()-1) else set())
+                                   if j<(self.sectionNumber()-1) else set())
                     kwargs["containerGraph"] = pg
                     kwargs["prefix"] = section_prefix
                     kwargs["label"] = section_label
                     kwargs["hideDeadEndBefore"] = sharedStart
                     kwargs["hideDeadEndAfter"] = sharedEnd
                     #create section graph
                     self._sectionItems[j].visualize(*args, **kwargs)
@@ -378,15 +409,18 @@
             self._order : int = None
             self._paths : None
             self._pathNumber : int = None
             self._optionalPathNumber : int = None
             self._requiredPathNumber : int = None            
             
             self._checkBackwardList = set()
-            self._checkForwardList = {}           
+            self._checkForwardList = {} 
+            
+            self._datasets = set()
+            self._varieties = set()
             
             #compute connected bases
             for connectedCkmer in connectedCkmers:
                 self._connectedBases.update(self._graph._orientatedCkmers[connectedCkmer]._orientatedBases.values())
 
             self._logger.debug("create section with {} starting k-mers".format(len(startCkmers)))
             for initialCkmer in initialCkmers:
@@ -614,14 +648,16 @@
             def __init__(self, orientatedCkmerList, pathSequence, distance, graph):                
                 self._orientatedCkmerList = orientatedCkmerList
                 self._pathSequence = pathSequence
                 self._distance = distance
                 self._required = False
                 self._optional = False
                 self._graph = graph
+                self._datasets = set()
+                self._varieties = set()
                 
             def distance(self):
                 return self._distance
             
             def sequence(self):
                 return self._pathSequence
```

### Comparing `haplotyping-0.0.5/haplotyping/graph/sequence.py` & `haplotyping-0.0.6/haplotyping/graph/sequence.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/index/database.py` & `haplotyping-0.0.6/haplotyping/index/database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging, h5py, os, sys, glob, re, math, shutil
 import numpy as np, tables, gzip, csv
 import multiprocessing as mp
 
 import haplotyping
 import haplotyping.index.splits
-import haplotyping.index.reads
+import haplotyping.index.direct
 
 class Database:
     
     """
     Constructing splitting k-mer database
     
     Parameters
@@ -35,70 +35,51 @@
         Optional, but at least readFiles or pairedReadFiles should be defined and non-empty
 
     minimumFrequency: int, optional, default is 2
         The minimum frequency for a splitting k-mer.
         Adjusting this number will change the amount of read error based results but 
         can also introduce gaps; With higher read depth or lower error rate, this number can possibly be increased
         
-    maximumProcesses: int, optional, default is 5
-        The maximum number of processes including main process, should be at least 5
+    maximumMemory: int, default is 0 (for no maximum)
+        Maximum memory size, reduces the number of processes if too much memory is needed
         
-    maximumProcessesAutomaton: int, optional, default is 1
-        The maximum number of processes used for direct parsing of reads using the automaton
-        Because shared memory can't be used, multiple copies of the automaton have to be in memory
-        Be carefull if available memory is limited
-    
-    maximumProcessesIndex: int, optional
-        The maximum number of processes used for creating a (partial) index from the matches
-        Making use of shared memory to load index
-        
-    maximumProcessesMatches: int, optional
-        The maximum number of processes used for creating a (partial) index from the matches
-        Collecting and organising data is done mostly in memory
-        Be carefull if available memory is limited
-    
-    maximumProcessesConnections: int, optional
-        The maximum number of processes used for creating a (partial) index from the matches
-        Collecting and organising data is done mostly in memory
-        Be carefull if available memory is limited
-    
-    maximumProcessesMerges: int, optional
-        The maximum number of processes used for merging operations
-    
-    automatonKmerSize: int optional, default is None
-        The used reduced k-mer size, if undefined automatically set to just above half the k-mer size
+    maximumProcesses: int, default is 0 (for no maximum)
+        The maximum number of processes including main process, should be at least 4
+        
+    automatonKmerSize: int optional, default is 0 (for automatically)
+        The used reduced k-mer size, maximum is the k-mer size
         
     onlySplittingKmers: bool, optional, default is False
         Only the first step will be executed, using a single process.
+        
+    onlyDirectConnections: bool, optional, default is False
+        Only direct connections are extracted from the reads
     
     debug: bool, optional, default is False
         Only use this when debugging or extending the code.      
         
     keepTemporaryFiles: bool, optional, default is False
         Only use this when debugging or extending the code.      
         
     """
 
-    version = "20220916"
+    version = "20230429"
     
     def __init__(self,
                  k: int, 
                  name: str, 
                  filenameBase: str,
                  sortedIndexFile: str,
                  readFiles=[], pairedReadFiles=[],
                  minimumFrequency: int = 2,
-                 maximumProcesses: int = 5,
-                 maximumProcessesAutomaton: int = 1,
-                 maximumProcessesIndex: int = None,
-                 maximumProcessesMatches: int = None,
-                 maximumProcessesConnections: int = None,
-                 maximumProcessesMerges: int = None,
-                 automatonKmerSize: int = None,
+                 maximumMemory: int = 0,
+                 maximumProcesses: int = 0,
+                 automatonKmerSize: int = 0,
                  onlySplittingKmers: bool = False,
+                 onlyDirectConnections: bool = False,
                  debug: bool = False,
                  keepTemporaryFiles: bool=False):  
         
         
         
         """
         Internal use only: initialize
@@ -115,84 +96,69 @@
         
         #logger
         self._logger = logging.getLogger(__name__)
         self._logger.info("create data storage for "+str(name)+" in "+filenameBase)
         
         #store variables
         self.k=k
-        self.automatonKmerSize=math.ceil((self.k+1)/2) if automatonKmerSize==None else math.min(self.k,automatonKmerSize)
         self.name=name
-        self.minimumFrequency = minimumFrequency
         self.debug = debug
+        self.onlySplittingKmers = onlySplittingKmers
+        self.onlyDirectConnections = onlyDirectConnections
+        self.automatonKmerSize = automatonKmerSize
+        self.minimumFrequency = minimumFrequency
         self.keepTemporaryFiles = keepTemporaryFiles
         self.filenameBase = filenameBase
+        self.maximumMemory = maximumMemory
         self.maximumProcesses = maximumProcesses
-        self.maximumProcessesAutomaton = (maximumProcesses if maximumProcessesAutomaton==None 
-                                          else maximumProcessesAutomaton)
-        self.maximumProcessesIndex = (maximumProcesses if maximumProcessesIndex==None 
-                                      else maximumProcessesIndex)
-        self.maximumProcessesMatches = (maximumProcesses if maximumProcessesMatches==None 
-                                        else maximumProcessesMatches)
-        self.maximumProcessesConnections = (maximumProcesses if maximumProcessesConnections==None 
-                                            else maximumProcessesConnections)
-        self.maximumProcessesMerges = (maximumProcesses if maximumProcessesMerges==None 
-                                       else maximumProcessesMerges)
-        
+                
         #check boundaries number of processes
-        assert self.maximumProcesses>=5
-        assert self.maximumProcessesAutomaton>=1
-        assert self.maximumProcessesMatches>=1
-        assert self.maximumProcessesIndex>=1
-        assert self.maximumProcessesConnections>=1
-        assert self.maximumProcessesMerges>=1
-        
-        if (not onlySplittingKmers) and (len(readFiles)==0) and (len(pairedReadFiles)==0):
+        assert self.automatonKmerSize>=0 and self.automatonKmerSize<=self.k
+        assert self.maximumMemory>=0
+        assert self.maximumProcesses>=0
+                
+        if (not self.onlySplittingKmers) and (len(readFiles)==0) and (len(pairedReadFiles)==0):
             self._logger.error("no read files provided")
         else:                
             #define filenames
-            filename = filenameBase+".h5"            
+            filename = "{}.h5".format(filenameBase)
             
             #skip finished steps
             if self.debug:
-                filename_splits = filenameBase+".splits.h5"
-                filename_distances = filenameBase+".distances.h5"
+                filename_splits = "{}.splits.h5".format(filenameBase)
+                filename_distances = "{}.distances.h5".format(filenameBase)
                 if os.path.exists(filename_distances):
                     shutil.copyfile(filename_distances, filename)
                 elif os.path.exists(filename_splits):
                     shutil.copyfile(filename_splits, filename)
 
             #use tables for temporary file, and h5py for final
+            #don't use libver="latest" before checking other tools!
             with h5py.File(filename,"a") as h5file:
 
                 #set or check config
                 if not "/config" in h5file:
                     h5file.create_group("/config")
                     h5file["/config"].attrs["k"] = self.k
                     h5file["/config"].attrs["version"] = self.version
                     h5file["/config"].attrs["automatonKmerSize"] = self.automatonKmerSize
-                    h5file["/config"].attrs["name"] = self.name
-                    h5file["/config"].attrs["debug"] = self.debug
-                    h5file["/config"].attrs["minimumFrequency"] = self.minimumFrequency
+                    h5file["/config"].attrs["minimumCanonicalSplitFrequency"] = self.minimumFrequency
                     h5file.flush()
                 else:
                     assert h5file["/config"].attrs["k"] == self.k
                     assert h5file["/config"].attrs["version"] == self.version
                     assert h5file["/config"].attrs["automatonKmerSize"] == self.automatonKmerSize
-                    assert h5file["/config"].attrs["name"] == self.name
-                    assert h5file["/config"].attrs["debug"] == self.debug
-                    assert h5file["/config"].attrs["minimumFrequency"] == self.minimumFrequency
+                    assert h5file["/config"].attrs["minimumCanonicalSplitFrequency"] == self.minimumFrequency
                     
                 #these settings are allowed to change in secondary runs
+                h5file["/config"].attrs["name"] = self.name
+                h5file["/config"].attrs["debug"] = self.debug
+                h5file["/config"].attrs["maximumMemory"] = self.maximumMemory
                 h5file["/config"].attrs["maximumProcesses"] = self.maximumProcesses
-                h5file["/config"].attrs["maximumProcessesAutomaton"] = self.maximumProcessesAutomaton
-                h5file["/config"].attrs["maximumProcessesIndex"] = self.maximumProcessesIndex
-                h5file["/config"].attrs["maximumProcessesMatches"] = self.maximumProcessesMatches
-                h5file["/config"].attrs["maximumProcessesConnections"] = self.maximumProcessesConnections
-                h5file["/config"].attrs["maximumProcessesMerges"] = self.maximumProcessesMerges
-
+                
                 #get splitting k-mers from index   
                 if not ("/split" in h5file and "/histogram" in h5file):
                     if not os.path.exists(sortedIndexFile):
                         self._logger.error("no sorted k-mer list provided")
                     else:
                         self._logger.debug("get splitting k-mers from the provided index")
                         haplotyping.index.splits.Splits(sortedIndexFile, h5file, 
@@ -201,19 +167,20 @@
                         #backup
                         if self.debug:
                             shutil.copyfile(filename, filename_splits)
                 else:
                     self._logger.debug("detected splitting k-mers from previous run")
                     
                 #parse read files and store distances
-                if (not onlySplittingKmers) and ("/split" in h5file) and ("/histogram" in h5file):
+                if (not self.onlySplittingKmers) and ("/split" in h5file) and ("/histogram" in h5file):
                     if not ("/relations" in h5file and "/connections" in h5file):
                         self._logger.debug("parse read files and store distances in database")
-                        haplotyping.index.reads.Reads(readFiles,pairedReadFiles, h5file, 
-                                                      self.filenameBase, self.debug, self.keepTemporaryFiles)
+                        haplotyping.index.direct.Direct(readFiles,pairedReadFiles, h5file, 
+                                                      self.filenameBase, self.onlyDirectConnections, 
+                                                      self.debug, self.keepTemporaryFiles)
                         h5file.flush()
                         #backup
                         if self.debug:
                             shutil.copyfile(filename, filename_distances)
                     else:
                         self._logger.debug("detected distances from previous run")
```

### Comparing `haplotyping-0.0.5/haplotyping/index/reads.py` & `haplotyping-0.0.6/haplotyping/index/direct.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,354 +1,440 @@
 import logging, h5py, tables, gzip, time
-import os, sys, math, signal
+import os, sys, math, signal, psutil
 import re, haplotyping
 import numpy as np
 import haplotyping.index.storage
 import haplotyping.index.splits
 import multiprocessing as mp
+from threading import Event
 from queue import Empty
 
-class Reads:
+class Direct:
     
     """
     Internal use, parse read files and store results in database
     """
     
-    def __init__(self, unpairedReadFiles, pairedReadFiles, h5file, filenameBase, debug=False, keepTemporaryFiles=False):
+    def __init__(self, unpairedReadFiles, pairedReadFiles, h5file, filenameBase, 
+                 onlyDirectConnections=False, debug=False, keepTemporaryFiles=False):
         
         """
         Internal use only: initialize
         """
         
         #logger
         self._logger = logging.getLogger(__name__)
         if len(unpairedReadFiles)>0:
             self._logger.info("parse "+str(len(unpairedReadFiles))+" unpaired readfile(s)")
         if len(pairedReadFiles)>0:
-            self._logger.info("parse "+str(2*len(pairedReadFiles))+" paired readfile(s)")
-        
+            self._logger.info("parse "+str(2*len(pairedReadFiles))+" paired readfile(s)")                
+                    
         self.debug = debug
         self.keepTemporaryFiles = keepTemporaryFiles
+        self.onlyDirectConnections = onlyDirectConnections
         self.filenameBase = filenameBase
         
         #set variables
         self.k = h5file["/config"].attrs["k"]
         self.automatonKmerSize = h5file["/config"].attrs["automatonKmerSize"]
-        self.maximumFrequency = h5file["/config"].attrs["maximumFrequency"]
+        self.maximumFrequency = h5file["/config"].attrs["maximumCanonicalSplitFrequency"]
+        self.minimumFrequency = h5file["/config"].attrs["minimumCanonicalSplitFrequency"]
+        self.maximumMemory = h5file["/config"].attrs["maximumMemory"]
         self.maximumProcesses = h5file["/config"].attrs["maximumProcesses"]
-        self.maximumProcessesAutomaton = h5file["/config"].attrs["maximumProcessesAutomaton"]
-        self.maximumProcessesIndex = h5file["/config"].attrs["maximumProcessesIndex"]
-        self.maximumProcessesMatches = h5file["/config"].attrs["maximumProcessesMatches"]
-        self.maximumProcessesConnections = h5file["/config"].attrs["maximumProcessesConnections"]
-        self.maximumProcessesMerges = h5file["/config"].attrs["maximumProcessesMerges"]
         self.numberOfKmers = h5file["/split/ckmer"].shape[0]
-        self.totalNumberOfKmers = h5file["/config"].attrs["totalNumberOfKmers"]
+        self.totalNumberOfKmers = h5file["/config"].attrs["numberKmers"]
         self.h5file = h5file
         self.unpairedReadFiles = unpairedReadFiles
         self.pairedReadFiles = pairedReadFiles
         self.temporaryMergedRelationsFile = None
         
         #statistics
         self.readLengthMinimum=None
         self.readLengthMaximum=None
         self.readPairedTotal=0
         self.readUnpairedTotal=0
         self.readTotal=0
+        self.totalReadLength=0
         self.processReadsTime=0
         
         #estimated size
         self.estimatedMaximumReadLength = 0
         
-        #get config
-        self.minimumFrequency = h5file["/config"].attrs["minimumFrequency"]
-        
         #check existence group
         if not "/relations" in h5file:
             h5file.create_group("/relations")
-        if not "/connections" in h5file:
-            h5file.create_group("/connections")    
         
-        #create relations and connections datasets
+        #create relations datasets
         if "/relations/direct" in h5file:
             self._logger.warning("direct relation dataset already exists in hdf5 storage")
         elif "/relations/cycle" in h5file:
             self._logger.warning("cycle relation dataset already exists in hdf5 storage")
         elif "/relations/reversal" in h5file:
             self._logger.warning("reversal relation dataset already exists in hdf5 storage")
-        elif "/connections/list" in h5file:
-            self._logger.warning("connections list dataset already exists in hdf5 storage")
         else:
-            #estimate number of splitting k-mers in the read
-            self.estimatedMaximumReadLength = self._quickEstimateReadLength()
             #theoretical maximum is 2 * #letters, however read-errors will introduce additional connections
             #partly they will be pre-filtered, but a buffer seems sensible (?)
-            self.arrayNumberDirect = 2*len(haplotyping.index.Database.letters)
-            h5file["/config/"].attrs["arrayNumberDirect"] = self.arrayNumberDirect
-            #estimate number of connections as two times the estimated number of splitting k-mers in a read
-            #this estimation is the splitting k-mer fraction times the estimated number of k-mers in a read
-            #the factor two is used for paired reads that did partly overlap
-            #keep this number within reason, therefore in the interval between arrayNumberDirect and 
-            #the number of letters to the power 4 (256)
-            self.arrayNumberConnection = math.ceil(2*(self.numberOfKmers/self.totalNumberOfKmers)*
-                                          (1+self.estimatedMaximumReadLength-self.k))
-            self.arrayNumberConnection = max(self.arrayNumberDirect,self.arrayNumberConnection)
-            self.arrayNumberConnection = min(self.arrayNumberConnection,len(haplotyping.index.Database.letters)**4)
-            h5file["/config/"].attrs["arrayNumberConnection"] = self.arrayNumberConnection
+            self.numberDirectArray = 2*len(haplotyping.index.Database.letters)
+            h5file["/config/"].attrs["numberDirectArray"] = self.numberDirectArray
+                                    
             #process
             try:                                                
                 #create automaton and index
-                automatonFile = filenameBase+".automaton.splits"
-                indexFile = filenameBase+".index.splits"
-                haplotyping.index.splits.Splits.createAutomatonWithIndex(
-                    self.h5file, indexFile, automatonFile, self.automatonKmerSize)
+                automatonKmerSize = (math.ceil((self.k+1)/2) 
+                                     if self.automatonKmerSize==0 else min(self.k,self.automatonKmerSize))  
+                self.automatonKmerSize = automatonKmerSize
+                (automatonMemory,indexFile, automatonFile) = haplotyping.index.splits.Splits.createAutomatonWithIndex(
+                    self.h5file, filenameBase, automatonKmerSize)
                 #process
-                pytablesFile = filenameBase+"_tmp_direct_connections_merge.h5"
+                pytablesFile = filenameBase+"_tmp_connections_merge.h5"
                 if os.path.exists(pytablesFile):
                     os.remove(pytablesFile)
                 self._logger.debug("store temporary in "+pytablesFile)    
                 #create datasets
                 with tables.open_file(pytablesFile, mode="w", title="Temporary storage") as self.pytablesStorage:
-                    self._processReadFiles(indexFile, automatonFile)
-                    self._store()
+                    self._processReadFiles(indexFile, automatonFile, automatonMemory)
+                    self._storeDirect()
+                    if not self.onlyDirectConnections:
+                        self._processReads()
+                        self._storeReads()
                     self.h5file.flush()     
             except Exception as e:
-                self._logger.error("problem occurred while processing reads: "+str(e))
+               self._logger.error("problem occurred while processing reads: "+str(e))
             finally:
                 try:
                     if not self.keepTemporaryFiles:
                         os.remove(pytablesFile)
-                        os.remove(automatonFile)
-                        os.remove(indexFile)
+                        haplotyping.index.splits.Splits.deleteAutomatonWithIndex(filenameBase, automatonKmerSize)
                 except:
-                    self._logger.error("problem removing files")    
+                    self._logger.error("problem removing files")   
+                    
+                    
+    def _collect_queue(queue_entry):
+        time.sleep(0.1)
+        while True:
+            try:
+                item = queue_entry.get(block=True, timeout=1)
+            except Empty:
+                break
 
-    def _processReadFiles(self, indexFile, automatonFile):
-        
-        def close_queue(queue_entry):
-            time.sleep(0.1)
-            queue_entry.close()
-            queue_entry.join_thread()
-            
-        def collect_and_close_queue(queue_entry):
-            entries = []
-            queue_entry.put(None)
-            time.sleep(0.1)
-            while True:
-                try:
-                    item = queue_entry.get(block=True, timeout=1)
-                    if item==None:
-                        break
-                    else:
-                        entries.append(item)
-                except Empty:
-                    break 
-            #now also close this queue
-            close_queue(queue_entry)
-            return entries
-            
+    def _close_queue(queue_entry):
+        time.sleep(0.1)
+        queue_entry.close()
+        queue_entry.join_thread()
+
+    def _collect_and_close_queue(queue_entry):
+        entries = []
+        queue_entry.put(None)
+        time.sleep(0.1)
+        while True:
+            try:
+                item = queue_entry.get(block=True, timeout=1)
+                if item==None:
+                    break
+                else:
+                    entries.append(item)
+            except Empty:
+                break 
+        #now also close this queue
+        Direct._close_queue(queue_entry)
+        return entries
+
+    def _processMemory():
+        process = psutil.Process(os.getpid())
+        memory = process.memory_info().rss
+        for child in process.children(recursive=True):
+            memory += child.memory_info().rss
+        return memory
+
+    def _processReadFiles(self, indexFile, automatonFile, automatonMemory):
+          
+        def estimateIndexMemory(nWorkersAutomaton,workerAutomatonMemory,nWorkersMatches,
+                           workerMatchesMemory,nWorkersIndex,workerIndexMemory):
+            return ((nWorkersAutomaton*workerAutomatonMemory) + 
+                    (nWorkersMatches*workerMatchesMemory) + 
+                    (nWorkersIndex*workerIndexMemory))
+                
         #get method
         self._logger.debug("using method '{}' for multiprocessing".format(mp.get_start_method()))
+        process = psutil.Process(os.getpid())
+        self._logger.debug("initially used memory {} MB".format(math.ceil(Direct._processMemory()/1048576)))
         
-        #create shared memory k-mer index (to confirm results from automaton)
+        self._logger.debug("memory info: {}".format(psutil.Process(os.getpid()).memory_info()))
+        
+        #compute size shared memory k-mer index (to confirm results from automaton)
         shm_index_size = os.path.getsize(indexFile)
-        shm_index = mp.shared_memory.SharedMemory(create=True, size=shm_index_size)
-        with open(indexFile, "r") as f:
-            shm_index.buf[0:shm_index_size] = bytes(f.read(),"utf-8")
-        self._logger.debug("created shared memory {} MB k-mer index".format(round(shm_index_size/1048576)))
-            
-        #create shared memory k-mer type, number and bases
+        self._logger.debug("size shared memory {} MB k-mer index".format(math.ceil(shm_index_size/1048576)))
+                    
+        #compute size shared memory k-mer type, number and bases
         shm_kmer_link = np.dtype(haplotyping.index.Database.getUint(self.numberOfKmers)).type
         shm_kmer_number = np.dtype(haplotyping.index.Database.getUint(self.maximumFrequency)).type
         shm_kmer_size = self.numberOfKmers*(1+shm_kmer_number(0).nbytes+(2*shm_kmer_link(0).nbytes))
-        shm_kmer = mp.shared_memory.SharedMemory(create=True, size=shm_kmer_size)
-        kmer_properties = np.ndarray((self.numberOfKmers,), dtype=[("type","S1"),("number",shm_kmer_number),
-                           ("left",shm_kmer_link),("right",shm_kmer_link)], buffer=shm_kmer.buf)
-        ckmerLink = 0
-        stepSizeStorage=1000000
-        for i in range(0,self.numberOfKmers,stepSizeStorage):
-            ckmers = self.h5file["/split/ckmer"][i:min(self.numberOfKmers,i+stepSizeStorage)]
-            for row in ckmers:
-                kmer_properties[ckmerLink] = (row[1],row[2],row[3][0],row[3][1],)
-                ckmerLink+=1
-        self._logger.debug("created shared memory {} MB k-mer properties".format(round(shm_kmer_size/1048576)))
-
+        self._logger.debug("size shared memory {} MB k-mer properties".format(math.ceil(shm_kmer_size/1048576)))
+        
+        #shutdown
         shutdown_event = mp.Event()
         
         qsize = 10000
+        queue_start = mp.Queue(qsize)
         queue_automaton = mp.Queue(qsize)
         queue_index = mp.Queue(qsize)
         queue_matches = mp.Queue(qsize)
-        queue_connections = mp.Queue(qsize)
         queue_finished = mp.Queue()
         queue_storageDirect = mp.Queue()
-        queue_storageConnections = mp.Queue()
+        queue_storageReads = mp.Queue()
         
-        #auto distribute within limits
-        nWorkers = self.maximumProcesses - 1
-        nWorkersAutomaton = min(self.maximumProcessesAutomaton,math.floor(nWorkers/4))
-        nWorkersMatches = min(self.maximumProcessesMatches,math.floor((nWorkers - nWorkersAutomaton)/3))
-        nWorkersIndex = min(self.maximumProcessesIndex,math.floor((nWorkers - nWorkersAutomaton - nWorkersMatches)/2))
-        nWorkersConnections = min(self.maximumProcessesConnections,
-                                  (nWorkers - nWorkersAutomaton - nWorkersMatches - nWorkersIndex))
-        
-        nWorkersLeft = nWorkers - nWorkersAutomaton - nWorkersMatches - nWorkersIndex - nWorkersConnections
+        #estimate worker automaton memory
+        workerAutomatonMemory = automatonMemory
+        #estimate worker matches memory
+        workerMatchesDtypeEntry = haplotyping.index.storage.Storage.worker_matches_dtype(
+            self.numberOfKmers,self.maximumFrequency,self.estimatedMaximumReadLength,self.numberDirectArray)
+        workerMatchesMemory = self.numberOfKmers * np.dtype(workerMatchesDtypeEntry).itemsize
+        #estimate worker index memory (shared)
+        workerIndexMemory = 0
+        workerSharedMemory = (shm_kmer_size+shm_index_size)
+        
+        self._logger.debug("estimated shared memory: {} MB".format(math.ceil(workerSharedMemory/1048576)))
+        self._logger.debug("estimated memory automaton worker: {} MB".format(math.ceil(workerAutomatonMemory/1048576)))
+        self._logger.debug("estimated memory index worker: {} MB".format(math.ceil(workerIndexMemory/1048576)))
+        self._logger.debug("estimated memory matches worker: {} MB".format(math.ceil(workerMatchesMemory/1048576)))
+        
+        #worker requirements
+        nWorkers = max(3,mp.cpu_count()-1) if self.maximumProcesses==0 else self.maximumProcesses - 1
+        
+        #memory requirements
+        if self.maximumMemory>0:
+            maximumMemory = min(psutil.virtual_memory().available + process.memory_info().rss, self.maximumMemory)
+        else:
+            maximumMemory = round(0.95*psutil.virtual_memory().available) + process.memory_info().rss    
+            
+            
+        #compute maximum number of automaton workers (high memory usage)
+        #assume that ideal ratio workers is 1:2:4 (to be verified/computed?)
+        nWorkersAutomaton = max(1,min(math.floor(nWorkers/3),
+                                      math.floor((maximumMemory-workerSharedMemory)/
+                                             estimateIndexMemory(1,workerAutomatonMemory,
+                                                                 2,workerMatchesMemory,
+                                                                 4,workerIndexMemory))))
+        #auto distribute other workers within limits
+        nWorkersMatches = math.floor((nWorkers - nWorkersAutomaton)/2)
+        nWorkersIndex = nWorkers - nWorkersAutomaton - nWorkersMatches        
+        #increment if processes available
+        nWorkersLeft = nWorkers - nWorkersAutomaton - nWorkersMatches - nWorkersIndex
         while(nWorkersLeft>0):
-            if(nWorkersLeft>0 and nWorkersMatches<self.maximumProcessesMatches):
+            if(nWorkersLeft>0):
                 nWorkersMatches+=1
-            if(nWorkersLeft>0 and nWorkersIndex<self.maximumProcessesIndex):
+                nWorkersLeft-=1
+            if(nWorkersLeft>0):
                 nWorkersIndex+=1
-            newWorkersLeft = nWorkers - nWorkersAutomaton - nWorkersMatches - nWorkersIndex - nWorkersConnections
-            if nWorkersLeft<newWorkersLeft:
-                nWorkersLeft=newWorkersLeft
+                nWorkersLeft-=1                                         
+        #reduce to fit memory requirements   
+        while (estimatedMemory := estimateIndexMemory(nWorkersAutomaton,workerAutomatonMemory,
+                             nWorkersMatches,workerMatchesMemory,
+                             nWorkersIndex,workerIndexMemory)) + workerSharedMemory > maximumMemory:
+            if (nWorkersAutomaton==1) and (nWorkersMatches==1) and (nWorkersIndex==1):
+                raise Exception("not enough memory available, required: {} MB".format(round(estimatedMemory/1048576)))
+            elif (nWorkersAutomaton==1) and (nWorkersMatches==1):
+                nWorkersIndex -= 1
+            elif (nWorkersMatches>nWorkersAutomaton):
+                nWorkersMatches -= 1
+                nWorkersIndex = nWorkersIndex+1
             else:
-                break
-
+                nWorkersAutomaton-=1
+                nWorkersIndex = nWorkersIndex+1
+        #don't oversize the index workers, maximum two times matches workers
+        nWorkersIndex = min(nWorkersIndex,2*nWorkersMatches)
+        #final calculation memory estimation
+        estimatedMemory = estimateIndexMemory(nWorkersAutomaton,workerAutomatonMemory,
+                             nWorkersMatches,workerMatchesMemory,nWorkersIndex,workerIndexMemory) + workerSharedMemory
+        
         self._logger.debug("start {} processes to parse reads with reduced automaton".format(nWorkersAutomaton))
-        self._logger.debug("start {} processes to check matches with index".format(nWorkersIndex))
+        self._logger.debug("start {} processes to check index".format(nWorkersIndex))
         self._logger.debug("start {} processes to process matches".format(nWorkersMatches))
-        self._logger.debug("start {} processes to process connections".format(nWorkersConnections))
-        
+        self._logger.debug("estimated total memory usage: {} MB".format(math.ceil(estimatedMemory/1048576)))
+                
         original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
         pool_automaton = mp.Pool(nWorkersAutomaton, haplotyping.index.storage.Storage.worker_automaton, 
-                             (shutdown_event,queue_automaton,queue_index,queue_finished,
+                             (shutdown_event,queue_start,queue_automaton,queue_index,queue_finished,
                               self.k,self.automatonKmerSize,automatonFile,))
+        #first start automatonss, one at a time, because of memory peak
+        startedAutomaton = 0
+        queue_start.put("automaton")
+        while not (startedAutomaton==nWorkersAutomaton):
+            try:
+                item = queue_finished.get(block=True, timeout=1)
+                if item=="automaton:started":
+                    startedAutomaton+=1
+                    self._logger.debug("{} of {} automatons started".format(startedAutomaton,nWorkersAutomaton))
+                    if startedAutomaton<nWorkersAutomaton:
+                        queue_start.put("automaton")
+                else:
+                    self._logger.error("unexpected start value in finished queue: {}".format(item))
+            except:
+                pass
+            time.sleep(1)
+            
+        #create shared memory k-mer index (to confirm results from automaton)
+        shm_index = mp.shared_memory.SharedMemory(create=True, size=shm_index_size)
+        with open(indexFile, "r") as f:
+            shm_index.buf[0:shm_index_size] = bytes(f.read(),"utf-8")
+        self._logger.debug("created shared memory {} MB k-mer index".format(math.ceil(shm_index_size/1048576)))
+        
+        #create shared memory k-mer type, number and bases
+        shm_kmer = mp.shared_memory.SharedMemory(create=True, size=shm_kmer_size)
+        kmer_properties = np.ndarray((self.numberOfKmers,), dtype=[("type","S1"),("number",shm_kmer_number),
+                           ("left",shm_kmer_link),("right",shm_kmer_link)], buffer=shm_kmer.buf)
+        ckmerLink = 0
+        stepSizeStorage=1000000
+        for i in range(0,self.numberOfKmers,stepSizeStorage):
+            ckmers = self.h5file["/split/ckmer"][i:min(self.numberOfKmers,i+stepSizeStorage)]
+            stepData = [(row[1],row[2],row[3][0],row[3][1],) for row in ckmers]
+            kmer_properties[ckmerLink:ckmerLink+len(stepData)] = stepData
+            ckmerLink+=len(stepData)
+            del stepData
+        self._logger.debug("created shared memory {} MB k-mer properties".format(math.ceil(shm_kmer_size/1048576)))
+
+        #now start other workers
         pool_index = mp.Pool(nWorkersIndex, haplotyping.index.storage.Storage.worker_index, 
-                             (shutdown_event,queue_index,queue_matches,queue_finished,
-                              self.k,shm_index.name))
+                             (shutdown_event,queue_index,queue_matches,queue_storageReads,queue_finished,
+                              self.filenameBase,self.numberOfKmers,self.k,
+                              self.onlyDirectConnections,shm_index.name))
         pool_matches = mp.Pool(nWorkersMatches, haplotyping.index.storage.Storage.worker_matches, 
-                               (shutdown_event,queue_matches,queue_connections,queue_storageDirect,queue_finished,
+                               (shutdown_event,queue_matches,queue_storageDirect,queue_finished,
                                 self.filenameBase,self.numberOfKmers,self.maximumFrequency,
-                                self.estimatedMaximumReadLength,self.arrayNumberDirect))
-        pool_connections = mp.Pool(nWorkersConnections, haplotyping.index.storage.Storage.worker_connections, 
-                               (shutdown_event,queue_connections,queue_storageConnections,queue_finished,
-                                self.filenameBase,self.numberOfKmers,
-                                self.arrayNumberConnection,self.maximumFrequency,shm_kmer.name))
+                                self.estimatedMaximumReadLength,self.numberDirectArray,
+                                self.onlyDirectConnections,shm_kmer.name))
         signal.signal(signal.SIGINT, original_sigint_handler)
 
         try:
             #process and register unpaired read files
             if not "unpairedReads" in self.h5file["/config/"].keys():
                 dtypeList = [("file","S255"),("readLength","uint64"),
-                     ("readNumber","uint64"),("processTime","uint32")]
+                     ("readNumber","uint64"),("totalReadLength","uint64"),("processTime","uint32")]
             
                 ds = self.h5file["/config/"].create_dataset("unpairedReads",(len(self.unpairedReadFiles),),
-                                                  dtype=np.dtype(dtypeList),chunks=None)
+                                                  dtype=np.dtype(dtypeList),chunks=None, 
+                                                  compression="gzip", compression_opts=9)
                 for i in range(len(self.unpairedReadFiles)):
-                    (readLength,readNumber,processTime) = self._processReadFile(self.unpairedReadFiles[i], 
+                    self._logger.debug("process {}".format(os.path.basename(self.unpairedReadFiles[i])))
+                    (readLength,readNumber,totalReadLength,processTime) = self._processReadFile(
+                                                                   self.unpairedReadFiles[i], 
                                                                    queue_automaton, queue_index, queue_matches)
                     ds[i] = (self.unpairedReadFiles[i],
-                             readLength,readNumber,int(processTime))
+                             readLength,readNumber,totalReadLength,int(processTime))
             else:
                 self._logger.error("unpairedReads already (partly) processed")
 
             #process and register paired read files
             if not "pairedReads" in self.h5file["/config/"].keys():
                 dtypeList = [("file0","S255"),("file1","S255"),("readLength","uint64"),
-                         ("readNumber","uint64"),("processTime","uint32")]
+                         ("readNumber","uint64"),("totalReadLength","uint64"),("processTime","uint32")]
                 ds = self.h5file["/config/"].create_dataset("pairedReads",(len(self.pairedReadFiles),),
-                                                  dtype=np.dtype(dtypeList),chunks=None)
+                                                  dtype=np.dtype(dtypeList),chunks=None, 
+                                                  compression="gzip", compression_opts=9)
                 for i in range(len(self.pairedReadFiles)):
-                    (readLength,readNumber,processTime) = self._processPairedReadFiles(self.pairedReadFiles[i][0],
+                    self._logger.debug("process {} and {}".format(os.path.basename(self.pairedReadFiles[i][0]),
+                                                           os.path.basename(self.pairedReadFiles[i][1])))
+                    (readLength,readNumber,totalReadLength,processTime) = self._processPairedReadFiles(
+                                                                     self.pairedReadFiles[i][0],
                                                                      self.pairedReadFiles[i][1], 
                                                                      queue_automaton, queue_index, queue_matches)
                     ds[i] = (self.pairedReadFiles[i][0],self.pairedReadFiles[i][1],
-                             readLength,readNumber,int(processTime))
+                             readLength,readNumber,totalReadLength,int(processTime))
             else:
                 self._logger.error("pairedReads already (partly) processed")                    
             
             #now wait until queues are empty
-            while not (queue_automaton.empty() and queue_index.empty() and queue_matches.empty() 
-                       and queue_connections.empty()):
+            while not (queue_automaton.empty() and queue_index.empty() and queue_matches.empty()):
                 time.sleep(1)
                 
             #then trigger stopping by sending enough Nones
             for i in range(pool_automaton._processes):
                 queue_automaton.put(None)
             for i in range(pool_index._processes):
                 queue_index.put(None)
             for i in range(pool_matches._processes):
                 queue_matches.put(None)
-            for i in range(pool_connections._processes):
-                queue_connections.put(None)
                 
             #now wait until everyone is finished
             finishedAutomaton=0
             finishedIndex=0
             finishedMatches=0
-            finishedConnections=0
+            totalCanonicalSplitFrequencies=0
             while not (finishedAutomaton==nWorkersAutomaton and finishedIndex==nWorkersIndex
-                       and finishedMatches==nWorkersMatches and finishedConnections==nWorkersConnections):
+                       and finishedMatches==nWorkersMatches):
                 try:
                     item = queue_finished.get(block=True, timeout=1)
-                    if item=="automaton":
+                    if item.startswith("automaton:ended"):
                         finishedAutomaton+=1
-                    elif item=="index":
+                    elif item.startswith("index:ended"):
                         finishedIndex+=1
-                    elif item=="matches":
+                        totalCanonicalSplitFrequencies+=int(item.split(":")[3])
+                    elif item.startswith("matches:ended"):
                         finishedMatches+=1
-                    elif item=="connections":
-                        finishedConnections+=1
                     else:
                         self._logger.error("unexpected value in finished queue: {}".format(item))
                 except:
                     pass
                 time.sleep(1)
+            #store total found canonical k-mers (doesn't fully match results from kmc because of overlapping sequences)
+            self.h5file["/config/"].attrs["totalCanonicalSplitFrequencies"] = totalCanonicalSplitFrequencies
                 
         except KeyboardInterrupt:
-            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
             self._logger.debug("caught KeyboardInterrupt")
+            #collect from queue
+            Direct._collect_queue(queue_automaton)
+            Direct._collect_queue(queue_index)
+            Direct._collect_queue(queue_matches)
             #shutdown directly
             shutdown_event.set()
             #release memory
             shm_index.close()
             shm_index.unlink()
-            signal.signal(signal.SIGINT, original_sigint_handler)
+            os.exit()
         finally:
             #terminate pools
             pool_automaton.terminate()
             pool_index.terminate()
             pool_matches.terminate()
-            pool_connections.terminate()
             #close queus workers
-            close_queue(queue_automaton)
-            close_queue(queue_index)
-            close_queue(queue_matches)
-            close_queue(queue_connections)
+            Direct._close_queue(queue_automaton)
+            Direct._close_queue(queue_index)
+            Direct._close_queue(queue_matches)
             #shutdown
             shutdown_event.set()
             #join pools
             pool_automaton.join()
             pool_index.join()
             pool_matches.join()
             #release memory
             shm_index.close()
             shm_index.unlink()
             #collect created files 
-            storageDirectFiles = collect_and_close_queue(queue_storageDirect)
-            storageConnectionsFiles = collect_and_close_queue(queue_storageConnections)
-
+            storageDirectFiles = Direct._collect_and_close_queue(queue_storageDirect)
+            self.storageReadFiles = Direct._collect_and_close_queue(queue_storageReads)            
+            
         #now all files are created, so merging can start
         self._logger.debug("merge {} files with direct connections".format(len(storageDirectFiles)))
-        self._logger.debug("merge {} files with additional connections".format(len(storageConnectionsFiles)))
             
         #reset shutdown event
         shutdown_event.clear()
         
-        nWorkersMerges = min(self.maximumProcessesMerges,self.maximumProcesses - 1)
+        #assume memory is no problem
+        nWorkersMerges = max(1,mp.cpu_count()-1) if self.maximumProcesses==0 else self.maximumProcesses - 1
         self._logger.debug("start {} processes to merge stored data".format(nWorkersMerges))
         
         queue_ranges = mp.Queue(nWorkersMerges)
         queue_merges = mp.Queue(nWorkersMerges)
         original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-        pool_merges = mp.Pool(nWorkersMerges, haplotyping.index.storage.Storage.worker_merges, 
+        pool_merges = mp.Pool(nWorkersMerges, haplotyping.index.storage.Storage.worker_mergeDirect, 
                                (shutdown_event,queue_ranges,queue_merges,
-                                storageDirectFiles,storageConnectionsFiles,
+                                storageDirectFiles,
                                 self.filenameBase,self.numberOfKmers,
                                 self.maximumFrequency,self.minimumFrequency,
-                                self.arrayNumberConnection,shm_kmer.name))
+                                shm_kmer.name))
         signal.signal(signal.SIGINT, original_sigint_handler)
         
         try:
             #fill queue
             mergeNumber = math.ceil(self.numberOfKmers/nWorkersMerges)
             for mergeStart in range(0,self.numberOfKmers,mergeNumber):
                 queue_ranges.put((mergeStart,mergeNumber,))
@@ -361,107 +447,109 @@
             while not (queue_ranges.empty()):
                 time.sleep(1)
                 
             #clean
             if not self.keepTemporaryFiles:
                 for item in storageDirectFiles:
                     os.remove(item)
-                for item in storageConnectionsFiles:
-                    os.remove(item)
-                
+                                
             #collect created merges
             mergeFiles = []
             while True:
                 try:
                     item = queue_merges.get(block=True, timeout=1)
                     if item==None:
                         break
                     elif isinstance(item,str):
                         mergeFiles.append(item)
                 except Empty:
                     break 
             #now also close this queue
-            close_queue(queue_merges)
+            Direct._close_queue(queue_merges)
             
             self._logger.debug("combine {} merged files".format(len(mergeFiles)))
             
             #combine
-            haplotyping.index.storage.Storage.combine_merges(
-                mergeFiles, self.pytablesStorage, self.numberOfKmers,self.maximumFrequency, 
-                self.arrayNumberConnection)
+            haplotyping.index.storage.Storage.combine_direct_merges(
+                mergeFiles, self.pytablesStorage, self.numberOfKmers,self.maximumFrequency)                        
             
             #clean
             if not self.keepTemporaryFiles:
                 for item in mergeFiles:
                     os.remove(item)
                 
         except KeyboardInterrupt:
-            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
             self._logger.debug("caught KeyboardInterrupt")
             shutdown_event.set()
             #release memory
             shm_kmer.close()
             shm_kmer.unlink()
-            signal.signal(signal.SIGINT, original_sigint_handler)
+            os.exit()
         finally:
             #terminate pool
             pool_merges.terminate()
             #close queus workers
-            close_queue(queue_ranges)
-            close_queue(queue_merges)
+            Direct._close_queue(queue_ranges)
+            Direct._close_queue(queue_merges)
             #shutdown
             shutdown_event.set()
             #join pool
             pool_merges.join()
             #release memory
             shm_kmer.close()
             shm_kmer.unlink()
             
         self._logger.debug("created merged file")
+        
+        self._logger.debug("process {} files with read information".format(len(self.storageReadFiles)))        
             
     def _processReadFile(self, filename: str, queue_automaton, queue_index, queue_matches):
         startTime = time.time()
         with gzip.open(filename, "rt") as f:
             readLengthMinimum=None
             readLengthMaximum=None
             readNumber=0
+            totalReadLength=0
             while True:               
                 f.readline()
                 sequence = f.readline().rstrip()  
                 f.readline()
                 f.readline()
                 if sequence:
                     readLengthMinimum=(len(sequence) if readLengthMinimum==None 
                                        else min(readLengthMinimum,len(sequence)))
                     readLengthMaximum=(len(sequence) if readLengthMaximum==None 
                                        else max(readLengthMaximum,len(sequence)))
                     readNumber+=1
+                    totalReadLength+=len(sequence)
                     queue_automaton.put(sequence)
                     if readNumber%1000000==0:
                         self._logger.debug("- processed {} reads".format(readNumber)) 
                 else:
                     break
             endTime = time.time()
             if readLengthMinimum>0:
                 self.readLengthMinimum=(readLengthMinimum if self.readLengthMinimum==None 
                                         else min(self.readLengthMinimum,readLengthMinimum))
             self.readLengthMaximum=(readLengthMaximum if self.readLengthMaximum==None 
                                     else max(self.readLengthMaximum,readLengthMaximum))
             self.readUnpairedTotal+=readNumber
             self.readTotal+=readNumber
+            self.totalReadLength+=totalReadLength
             self.processReadsTime+=endTime-startTime
         self._logger.info("processed {} reads".format(readNumber)) 
-        return (readLengthMaximum,readNumber,endTime-startTime)
+        return (readLengthMaximum,readNumber,totalReadLength,endTime-startTime)
 
     def _processPairedReadFiles(self, filename0: str, filename1: str, queue_automaton, queue_index, queue_matches):
         startTime = time.time()
         with gzip.open(filename0, "rt") as f0, gzip.open(filename1, "rt") as f1:
             readLengthMinimum=None
             readLengthMaximum=None
             readNumber=0
+            totalReadLength=0
             while True:
                 #first of pair
                 f0.readline()
                 sequence0 = f0.readline().rstrip()  
                 f0.readline()
                 f0.readline()
                 #second of pair
@@ -472,43 +560,45 @@
                 #process
                 if sequence0 and sequence1:
                     readLengthMinimum=(min(len(sequence0),len(sequence1)) if readLengthMinimum==None 
                                            else min(readLengthMinimum,len(sequence0),len(sequence1)))
                     readLengthMaximum=(max(len(sequence0),len(sequence1)) if readLengthMaximum==None 
                                        else max(readLengthMaximum,len(sequence0),len(sequence1)))
                     readNumber+=2  
-                    if sequence1[0:31] in sequence0:
+                    totalReadLength+=(len(sequence0)+len(sequence1))
+                    if sequence1[0:self.k] in sequence0:
                         pos = sequence0.find(sequence1[0:self.k])
                         rpos = sequence0.rfind(sequence1[0:self.k])
                         if pos==rpos:
                             match = sequence0[pos:]
                             if sequence1[0:len(match)]==match:
                                 #process as single read because of minimal glue match of size k
-                                queue_automaton.put((sequence0[0:pos]+sequence1,))
+                                queue_automaton.put(sequence0[0:pos]+sequence1) 
                             else:
-                                queue_automaton.put((sequence0,sequence1,))
+                                queue_automaton.put((sequence0,sequence1,))                                
                         else:
-                            queue_automaton.put((sequence0,sequence1,))
+                            queue_automaton.put((sequence0,sequence1,))                            
                     else:
-                        queue_automaton.put((sequence0,sequence1,))
+                        queue_automaton.put((sequence0,sequence1,))                        
                     if readNumber%1000000==0:
-                        self._logger.debug("- processed {} paired reads".format(readNumber)) 
+                        self._logger.debug("- processed {} paired reads".format(readNumber))                     
                 else:
                     break
             endTime = time.time()
             if readLengthMinimum>0:
                 self.readLengthMinimum=(readLengthMinimum if self.readLengthMinimum==None 
                                         else min(self.readLengthMinimum,readLengthMinimum))
             self.readLengthMaximum=(readLengthMaximum if self.readLengthMaximum==None 
                                     else max(self.readLengthMaximum,readLengthMaximum))
             self.readPairedTotal+=readNumber
             self.readTotal+=readNumber
+            self.totalReadLength+=totalReadLength
             self._logger.info("processed {} paired reads".format(readNumber)) 
             self.processReadsTime+=endTime-startTime
-        return (readLengthMaximum,readNumber,endTime-startTime)
+        return (readLengthMaximum,readNumber,totalReadLength,endTime-startTime)
         
         
     def _quickEstimateReadLength(self):
         readLengthMaximum=None
         #collect resources
         filenames = set()
         filenames.update(self.unpairedReadFiles)
@@ -522,22 +612,222 @@
                 sequence = f.readline().rstrip()  
                 if sequence:
                    readLengthMaximum=(len(sequence) if readLengthMaximum==None else max(readLengthMaximum,len(sequence)))
         #return result based on first lines of each file
         return readLengthMaximum
         
         
-    def _store(self):
-        self.h5file["/config/"].attrs["readLengthMinimum"]=self.readLengthMinimum
-        self.h5file["/config/"].attrs["readLengthMaximum"]=self.readLengthMaximum
-        self.h5file["/config/"].attrs["readPairedTotal"]=self.readPairedTotal
-        self.h5file["/config/"].attrs["readUnpairedTotal"]=self.readUnpairedTotal
-        self.h5file["/config/"].attrs["readTotal"]=self.readTotal
-        self.h5file["/config/"].attrs["processReadsTime"]=int(np.ceil(self.processReadsTime))        
+    def _storeDirect(self):
+        self.h5file["/config/"].attrs["minimumReadLength"]=self.readLengthMinimum
+        self.h5file["/config/"].attrs["maximumReadLength"]=self.readLengthMaximum
+        self.h5file["/config/"].attrs["numberReadsPaired"]=self.readPairedTotal
+        self.h5file["/config/"].attrs["numberReadsUnpaired"]=self.readUnpairedTotal
+        self.h5file["/config/"].attrs["numberReads"]=self.readTotal
+        self.h5file["/config/"].attrs["totalReadLength"]=self.totalReadLength
+        self.h5file["/config/"].attrs["timeProcessReads"]=int(np.ceil(self.processReadsTime))        
         
         #store merged data
-        haplotyping.index.storage.Storage.store_merged_connections(
+        haplotyping.index.storage.Storage.store_merged_direct(
             self.h5file, self.pytablesStorage, 
-            self.numberOfKmers, self.minimumFrequency)        
+            self.numberOfKmers, self.minimumFrequency)
+        
+    def _storeReads(self):
+        #store merged data
+        haplotyping.index.storage.Storage.store_merged_reads(
+            self.h5file, self.pytablesStorage, 
+            self.numberOfKmers,self.numberOfPartitions)
+        
+    def _processReads(self):   
+        
+        if len(self.storageReadFiles)>0:
+            
+            #shutdown
+            shutdown_event = mp.Event()
+        
+            #partition k-mers based on direct connections
+            maxNumberOfPartitions = int(self.numberOfKmers ** (2/3))
+            self.numberOfPartitions = haplotyping.index.storage.Storage.partition_kmers(self.h5file, self.pytablesStorage,
+                                                              maxNumberOfPartitions)
+            #prepare shared memory with k-mer properties
+            shm_kmer_partition = np.dtype(haplotyping.index.Database.getUint(self.numberOfPartitions)).type
+            shm_kmer_number = np.dtype(haplotyping.index.Database.getUint(self.maximumFrequency)).type
+            shm_kmer_disconnected = np.dtype("uint8").type
+            shm_kmer_size = self.numberOfKmers*(shm_kmer_partition(0).nbytes+shm_kmer_number(0).nbytes+
+                                                shm_kmer_disconnected(0).nbytes)
+            self._logger.debug("size shared memory {} MB k-mer properties".format(math.ceil(shm_kmer_size/1048576)))
 
-    
-    
+            shm_kmer = mp.shared_memory.SharedMemory(create=True, size=shm_kmer_size)
+            kmer_properties = np.ndarray((self.numberOfKmers,), 
+                                         dtype=[("partition",shm_kmer_partition),
+                                                ("number",shm_kmer_number),
+                                                ("disconnected","uint8")], 
+                                         buffer=shm_kmer.buf)
+            ckmerLink = 0
+            stepSizeStorage=1000000
+            for i in range(0,self.numberOfKmers,stepSizeStorage):
+                ckmers = self.h5file["/split/ckmer"][i:min(self.numberOfKmers,i+stepSizeStorage)]
+                stepData = [(row[5],row[2],row[4][1][1]+row[4][2][1]==0) for row in ckmers]
+                kmer_properties[ckmerLink:ckmerLink+len(stepData)] = stepData
+                ckmerLink+=len(stepData)
+                del stepData
+            self._logger.debug("created shared memory {} MB k-mer properties".format(math.ceil(shm_kmer_size/1048576)))
+            
+            #worker requirements
+            nWorkers = max(3,mp.cpu_count()-1) if self.maximumProcesses==0 else self.maximumProcesses - 1
+            nWorkersReads = min(len(self.storageReadFiles),nWorkers)            
+            self._logger.debug("start {} processes to process reads".format(nWorkersReads))
+            
+            #queues
+            queue_rawReads = mp.Queue(len(self.storageReadFiles))
+            queue_filteredReads = mp.Queue()
+            queue_finished = mp.Queue()            
+            
+            #maximum number of splitting k-mers in read
+            maximumReadLength = self.h5file["/config/"].attrs["maximumReadLength"] - self.k + 1
+            
+            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+            pool_reads = mp.Pool(nWorkersReads, haplotyping.index.storage.Storage.worker_processReads, 
+                                 (shutdown_event,queue_rawReads,queue_filteredReads,queue_finished,
+                                  self.filenameBase,self.numberOfKmers,
+                                  self.numberOfPartitions,self.maximumFrequency,maximumReadLength,shm_kmer.name))
+            signal.signal(signal.SIGINT, original_sigint_handler)
+            
+            try:
+                #fill queue
+                for item in self.storageReadFiles:
+                    queue_rawReads.put(item)
+                #trigger stopping by sending enough Nones
+                for i in range(pool_reads._processes):
+                    queue_rawReads.put(None)
+
+                #now wait    
+                while not (queue_rawReads.empty()):
+                    time.sleep(1)
+
+                #clean
+                if not self.keepTemporaryFiles:
+                   for item in self.storageReadFiles:
+                       os.remove(item)
+                del self.storageReadFiles
+
+            except KeyboardInterrupt:
+                self._logger.debug("caught KeyboardInterrupt")
+                shutdown_event.set()
+                #release memory
+                shm_kmer.close()
+                shm_kmer.unlink()
+                os.exit()
+            finally:
+                #terminate pool
+                pool_reads.terminate()
+                #close queus workers
+                Direct._close_queue(queue_rawReads)
+                Direct._close_queue(queue_finished)
+                #shutdown
+                shutdown_event.set()
+                #join pool
+                pool_reads.join()
+                #release memory
+                shm_kmer.close()
+                shm_kmer.unlink()
+                #get filtered readfiles
+                storageFilteredReadFiles = Direct._collect_and_close_queue(queue_filteredReads)   
+                
+            #compute merged paired from storageFilteredReadFiles
+            haplotyping.index.storage.Storage.combine_filtered_pairs(
+                storageFilteredReadFiles, self.pytablesStorage, self.numberOfKmers)
+
+            #get sizes for partitions
+            partitionSizes = [[0,0] for i in range(self.numberOfPartitions)]
+            for item in storageFilteredReadFiles:
+                with tables.open_file(item, mode="r") as pytablesStorageFiltered:
+                    nReads = pytablesStorageFiltered.root.readPartitionInfo.shape[0]
+                    stepSize = 1000000
+                    for i in range(0,nReads,stepSize):
+                        stepData = pytablesStorageFiltered.root.readPartitionInfo[i:i+stepSize]
+                        for row in stepData:
+                            partitionSizes[row[1]][0]+=1
+                            partitionSizes[row[1]][1]+=row[0]   
+            
+            #shutdown
+            shutdown_event = mp.Event()
+        
+            #worker requirements
+            nWorkers = max(3,mp.cpu_count()-1) if self.maximumProcesses==0 else self.maximumProcesses - 1
+            nWorkersMerges = min(len(storageFilteredReadFiles),nWorkers)     
+            self._logger.debug("start {} processes to merge reads".format(nWorkersMerges))
+            
+            queue_ranges = mp.Queue(nWorkersMerges)
+            queue_merges = mp.Queue(nWorkersMerges)
+            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+            pool_merges = mp.Pool(nWorkersMerges, haplotyping.index.storage.Storage.worker_mergeReads, 
+                                   (shutdown_event,queue_ranges,queue_merges,
+                                    storageFilteredReadFiles,partitionSizes,self.filenameBase,
+                                    self.numberOfKmers,self.numberOfPartitions,maximumReadLength))
+            signal.signal(signal.SIGINT, original_sigint_handler)
+        
+            try:
+                #fill queue
+                mergeNumber = math.ceil(self.numberOfPartitions/nWorkersMerges)
+                for mergeStart in range(0,self.numberOfPartitions,mergeNumber):
+                    queue_ranges.put((mergeStart,mergeNumber,))
+                    
+                #then trigger stopping by sending enough Nones
+                for i in range(pool_merges._processes):
+                    queue_ranges.put(None)
+
+                #now wait    
+                while not (queue_ranges.empty()):
+                    time.sleep(1)
+
+                #collect created merges
+                mergeFiles = []
+                while True:
+                    try:
+                        item = queue_merges.get(block=True, timeout=1)
+                        if item==None:
+                            break
+                        elif isinstance(item,str):
+                            mergeFiles.append(item)
+                    except Empty:
+                        if len(mergeFiles)==nWorkersMerges:
+                            break
+                        else:
+                            time.sleep(1)
+                #now also close this queue
+                Direct._close_queue(queue_merges)
+
+                self._logger.debug("combine {} merged files".format(len(mergeFiles)))
+
+                #combine
+                haplotyping.index.storage.Storage.combine_read_merges(
+                    sorted(mergeFiles), self.pytablesStorage, 
+                    self.numberOfKmers,self.numberOfPartitions,maximumReadLength)
+
+                #clean mergeFiles
+                if not self.keepTemporaryFiles:
+                    for item in mergeFiles:
+                        os.remove(item)
+                        
+            except KeyboardInterrupt:
+                self._logger.debug("caught KeyboardInterrupt")
+                shutdown_event.set()
+                os.exit()
+            finally:
+                #terminate pool
+                pool_merges.terminate()
+                #close queus workers
+                Direct._close_queue(queue_ranges)
+                #shutdown
+                shutdown_event.set()
+                #join pool
+                pool_merges.join()
+                
+            #clean storageFilteredReadFiles
+            if not self.keepTemporaryFiles:
+                for item in storageFilteredReadFiles:
+                    os.remove(item)
+                
+            
+            
+            
+
```

### Comparing `haplotyping-0.0.5/haplotyping/index/splits.py` & `haplotyping-0.0.6/haplotyping/index/splits.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import logging, h5py, tables, gzip, csv
-import os, sys, numpy as np
-import re, haplotyping, ahocorasick, pickle
+import logging, h5py, tables, gzip, time
+import os, sys, shutil, psutil, numpy as np
+import re, haplotyping, ahocorasick, pickle, signal
 import haplotyping.index.database
+import multiprocessing as mp
+from queue import Empty
 
 class Splits:
     
     """
     Internal use, get splitting k-mers from index
     """
     
@@ -17,20 +19,18 @@
         Internal use only: initialize
         """
         
         #logger
         self._logger = logging.getLogger(__name__)
         self._logger.info("parse k-mers to find right splitting k-mers")
         
-        self.matchPattern = re.compile(r"^["+"".join(haplotyping.index.Database.letters)+"]+$")
-        
         #set variables
         self.k = h5file["/config"].attrs["k"]
         self.automatonKmerSize = h5file["/config"].attrs["automatonKmerSize"]
-        self.minimumFrequency = h5file["/config"].attrs["minimumFrequency"]
+        self.minimumFrequency = h5file["/config"].attrs["minimumCanonicalSplitFrequency"]
         self.h5file = h5file
         self.maximumNumber = 0
         self.debug = debug
         self.keepTemporaryFiles = keepTemporaryFiles
         
         
         #check existence group
@@ -69,155 +69,184 @@
                 self._logger.error("problem occurred while constructing splits: "+str(e))
             finally:
                 try:
                     if not self.keepTemporaryFiles:
                         os.remove(pytablesFile)
                 except:
                     self._logger.error("problem removing "+pytablesFile)    
-
+                    
+                    
     def _parseIndex(self, filename: str):
         
+        
+        def close_queue(queue_entry):
+            time.sleep(0.1)
+            queue_entry.close()
+            queue_entry.join_thread()
+            
+        
         #create temporary storage
         tableCkmerDef = {
             "ckmer": tables.StringCol(self.k,pos=0),
             "type": tables.StringCol(1,pos=1),
             "number": tables.UInt64Col(pos=2),
         }
         self.tableDumpKmers = self.pytablesStorage.create_table(self.pytablesStorage.root,
-                                                                   "dumpCkmer",tableCkmerDef, 
-                                                "Temporary to store dump canonical k-mers")
+                                    "dumpCkmer",tableCkmerDef, "Temporary to store dump canonical k-mers")
         
-        #administration
-        rightSplitBases = 0
-        rightSplitKmers = 0
-        
-        def saveToDumpStorage(base, stored, rightSplitBases,rightSplitKmers):   
-            rightSplitBases+=1
-            for key,value in stored.items():
-                kmer = base+key
-                ckmer = haplotyping.General.canonical(kmer)
-                #assume right splitting if k-mer equals rc
-                #todo: can this (in theory) cause problematic situations?
-                ckmerType = "r" if kmer==ckmer else "l"
-                ckmerRow = self.tableDumpKmers.row            
-                ckmerRow["ckmer"] = ckmer
-                ckmerRow["type"] = ckmerType
-                ckmerRow["number"] = value
-                ckmerRow.append()
-                rightSplitKmers+=1
-                self.frequencyHistogram["ckmer"][value] = (
-                                self.frequencyHistogram["ckmer"].get(value,0)+1)
-            return (rightSplitBases,rightSplitKmers)
+        #multiprocessing
+        with mp.Manager() as manager:
+            shutdown_event = mp.Event()
+            qsize = 10000
+            queue_splits = mp.Queue(qsize)
+            totalNumberOfKmers = mp.Value("L",0)
+            totalSumOfKmerFrequencies = mp.Value("L",0)
+            minimumAllKmerFrequencies = mp.Value("L",2**32)
+            maximumAllKmerFrequencies = mp.Value("L",0)
+            histogramKmer = manager.dict()
+            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+            process_list = mp.Process(target=haplotyping.index.splits.Splits.worker_list, 
+                                      args=(shutdown_event,filename,self.k,self.minimumFrequency,
+                                            totalNumberOfKmers,totalSumOfKmerFrequencies,
+                                            minimumAllKmerFrequencies,maximumAllKmerFrequencies,histogramKmer,
+                                            queue_splits, ))
+            signal.signal(signal.SIGINT, original_sigint_handler)
 
-        #loop over sorted list with k-mers, detect right splitting k-mers
+            try:
+                #start
+                process_list.start()
+                #init
+                rightSplitBases = 0
+                rightSplitKmers = 0
+                self.frequencyHistogram = {"kmer": {}, "ckmer": {}, "base": {}}
+                #process queue
+                while True:
+                    try:
+                        item = queue_splits.get(block=True, timeout=1)
+                        if item==None:
+                            break
+                        else:
+                            rightSplitBases+=1
+                            for key,value in item[1].items():
+                                kmer = item[0]+key
+                                ckmer = haplotyping.General.canonical(kmer)
+                                #assume right splitting if k-mer equals rc
+                                #todo: can this (in theory) cause problematic situations?
+                                ckmerType = "r" if kmer==ckmer else "l"
+                                ckmerRow = self.tableDumpKmers.row            
+                                ckmerRow["ckmer"] = ckmer
+                                ckmerRow["type"] = ckmerType
+                                ckmerRow["number"] = value
+                                ckmerRow.append()
+                                rightSplitKmers+=1 
+                                self.frequencyHistogram["ckmer"][value] = (
+                                    self.frequencyHistogram["ckmer"].get(value,0)+1)
+                            if (rightSplitBases%1000000)==0:
+                                self._logger.debug("processed {} bases and {} k-mers".format(
+                                    rightSplitBases,rightSplitKmers))
+                    except Empty:
+                        continue
+                self.tableDumpKmers.flush()
+                self._logger.debug("found {} rightSplitBases and {} rightSplitKmers".format(
+                    rightSplitBases,rightSplitKmers))
+                self.h5file["/config/"].attrs["numberRightSplitBases"]=rightSplitBases
+                self.h5file["/config/"].attrs["numberRightSplitKmers"]=rightSplitKmers
+
+            except KeyboardInterrupt:
+                self._logger.debug("caught KeyboardInterrupt")
+                #shutdown directly
+                shutdown_event.set()
+                self._logger.debug("forced exit")
+                os.exit()
+            finally:
+                #close queus workers
+                close_queue(queue_splits)
+                #shutdown
+                shutdown_event.set()
+                #join
+                process_list.join() 
+
+            #store stats
+            self.frequencyHistogram["kmer"] = dict(histogramKmer)
+            self.h5file["/config/"].attrs["numberKmers"]=totalNumberOfKmers.value
+            self.h5file["/config/"].attrs["totalKmerFrequencies"]=totalSumOfKmerFrequencies.value
+            self.h5file["/config/"].attrs["minimumKmerFrequencies"]=minimumAllKmerFrequencies.value
+            self.h5file["/config/"].attrs["maximumKmerFrequencies"]=maximumAllKmerFrequencies.value
+            
+    def worker_list(shutdown_event,filename,k,minimumFrequency,totalNumberOfKmers,totalSumOfKmerFrequencies,
+                                        minimumAllKmerFrequencies,maximumAllKmerFrequencies,histogramKmer,
+                                        queue_splits):
+        logger = logging.getLogger("{}.worker.list".format(__name__))
         try:
             with gzip.open(filename, "rt") as f: 
-                self._logger.debug("parse sorted list to detect right splitting k-mers")
-                reader = csv.reader(f, delimiter="\t")
+                logger.debug("parse sorted list to detect right splitting k-mers")
                 previousBase = ""
                 previousBranch = ""
                 previousKmer = ""
-                previousNumber = 0 
-                totalNumberOfKmers = 0
-                totalSumOfKmerFrequencies = 0
-                minimumAllKmerFrequencies = 2**32
-                maximumAllKmerFrequencies = 0
-                self.frequencyHistogram = {"kmer": {}, "ckmer": {}, "base": {}}
+                previousNumber = 0                 
+                #administration
+                rightSplitBases = 0
+                rightSplitKmers = 0
                 stored={}
                 errorNumber = 0
-                for line in reader:
-                    if len(line)<2:
-                        if errorNumber==0:
-                            self._logger.warning("unexpected item in sorted list: "+str(line))
-                        errorNumber+=1
+                _totalNumberOfKmers=0
+                _totalSumOfKmerFrequencies=0
+                _minimumAllKmerFrequencies=2**32
+                _maximumAllKmerFrequencies=0
+                _histogramKmer = {}
+                while (row := f.readline()):
+                    line = row.strip().split("\t") 
+                    currentBase = line[0][:-1]
+                    currentBranch = line[0][-1]
+                    currentKmer = line[0]
+                    _totalNumberOfKmers+=1
+                    if (_totalNumberOfKmers%10000000)==0 and (_totalNumberOfKmers>0):
+                        logger.debug("processed {} k-mers".format(_totalNumberOfKmers))
+                    currentNumber = int(line[1])
+                    _totalSumOfKmerFrequencies += currentNumber
+                    _minimumAllKmerFrequencies = min(_minimumAllKmerFrequencies,currentNumber)
+                    _maximumAllKmerFrequencies = max(_maximumAllKmerFrequencies,currentNumber)
+                    _histogramKmer[currentNumber] = (_histogramKmer.get(currentNumber,0)+1)
+                    if currentNumber < minimumFrequency:
+                        pass
                     else:
-                        currentBase = line[0][:-1]
-                        currentBranch = line[0][-1]
-                        currentKmer = line[0]
-                        totalNumberOfKmers+=1
-                        #always get number
-                        try:
-                            currentNumber = int(line[1])
-                            totalSumOfKmerFrequencies += currentNumber
-                            minimumAllKmerFrequencies = min(minimumAllKmerFrequencies,currentNumber)
-                            maximumAllKmerFrequencies = max(minimumAllKmerFrequencies,currentNumber)
-                            self.frequencyHistogram["kmer"][currentNumber] = (
-                                self.frequencyHistogram["kmer"].get(currentNumber,0)+1)
-                        except ValueError:
-                            currentNumber = 0
-                        #check k-mer size
-                        if not len(currentKmer)==self.k:
-                            if errorNumber==0:
-                                self._logger.warning("different k-mer size in sorted list ("+
-                                                   str(len(currentKmer))+" instead of "+str(self.k)+")")
-                            errorNumber+=1
-                        #check pattern    
-                        elif not self.matchPattern.match(currentKmer):    
-                            if errorNumber==0:
-                                self._logger.warning("k-mer didn't match pattern")
-                            errorNumber+=1
-                            pass
-                        #check sorted
-                        elif not (previousKmer=="") and not (previousKmer<currentKmer):
-                            if errorNumber==0:
-                                self._logger.warning("provided list not properly sorted")
-                            errorNumber+=1
-                        #check frequency
-                        elif currentNumber<1:
-                            if errorNumber==0:
-                                self._logger.warning("unexpected frequency for "+str(currentKmer))
-                            errorNumber+=1
+                        if currentBase==previousBase:
+                            stored[previousBranch]=previousNumber
+                            stored[currentBranch]=currentNumber
                         else:
-                            if currentNumber < self.minimumFrequency:
-                                pass
-                            else:
-                                if currentBase==previousBase:
-                                    if currentBranch==previousBranch:
-                                        self._logger.warning("detected reoccurrence of same k-mer ("+currentKmer+")")
-                                    else:
-                                        if not previousBranch in stored.keys():
-                                            stored[previousBranch]=previousNumber
-                                        stored[currentBranch]=currentNumber
-                                else:
-                                    if len(stored)>0:
-                                        (rightSplitBases,rightSplitKmers) = saveToDumpStorage(previousBase,stored,
-                                                                                              rightSplitBases,rightSplitKmers)
-                                        stored={}
-                                        if (rightSplitBases%1000000)==0:
-                                            self._logger.debug("processed "+str(rightSplitBases)
-                                                               +" bases and "+str(rightSplitKmers)+" k-mers")
-                                previousBase = currentBase
-                                previousBranch = currentBranch
-                                previousKmer = currentKmer
-                                previousNumber = currentNumber
-                        
-                if len(stored)>0:
-                    (rightSplitBases,rightSplitKmers) = saveToDumpStorage(previousBase,stored,
-                                                                          rightSplitBases,rightSplitKmers)  
-                self.tableDumpKmers.flush()
+                            if len(stored)>1:
+                                queue_splits.put((previousBase,stored,))
+                                stored={}                                        
+                        previousBase = currentBase
+                        previousBranch = currentBranch
+                        previousKmer = currentKmer
+                        previousNumber = currentNumber
+                if len(stored)>1:
+                    queue_splits.put((previousBase,stored,)) 
+                #store stats
+                totalNumberOfKmers.value=_totalNumberOfKmers
+                totalSumOfKmerFrequencies.value=_totalSumOfKmerFrequencies
+                minimumAllKmerFrequencies.value=_minimumAllKmerFrequencies
+                maximumAllKmerFrequencies.value=_maximumAllKmerFrequencies
+                for key in _histogramKmer.keys():
+                    histogramKmer[key] = _histogramKmer[key]
+                #close queue
+                queue_splits.put(None)
                 #warning
                 if errorNumber>0:
-                    self._logger.warning("skipped {} items in sorted list".format(errorNumber))
+                    logger.warning("skipped {} items in sorted list".format(errorNumber))
                 #stats
-                minimumAllKmerFrequencies=min(minimumAllKmerFrequencies,maximumAllKmerFrequencies)
-                self._logger.debug("checked {} k-mers with {} total frequency".format(
-                    totalNumberOfKmers,totalSumOfKmerFrequencies))
-                self._logger.debug("found {} rightSplitBases and {} rightSplitKmers".format(
-                    rightSplitBases,rightSplitKmers))
-                self._logger.debug("frequency k-mers between {} and {}".format(
-                    minimumAllKmerFrequencies,maximumAllKmerFrequencies))
-                self.h5file["/config/"].attrs["rightSplitBases"]=rightSplitBases
-                self.h5file["/config/"].attrs["rightSplitKmers"]=rightSplitKmers
-                self.h5file["/config/"].attrs["totalNumberOfKmers"]=totalNumberOfKmers
-                self.h5file["/config/"].attrs["totalSumOfKmerFrequencies"]=totalSumOfKmerFrequencies
-                self.h5file["/config/"].attrs["minimumAllKmerFrequencies"]=minimumAllKmerFrequencies
-                self.h5file["/config/"].attrs["maximumAllKmerFrequencies"]=maximumAllKmerFrequencies
-        except OSError as ex:
-            self._logger.error("problem with sorted list: "+str(ex))
-
+                minimumAllKmerFrequencies.value=min(minimumAllKmerFrequencies.value,maximumAllKmerFrequencies.value)
+                logger.debug("checked {} k-mers with {} total frequency".format(
+                    totalNumberOfKmers.value,totalSumOfKmerFrequencies.value))
+                logger.debug("frequency k-mers between {} and {}".format(
+                    minimumAllKmerFrequencies.value,maximumAllKmerFrequencies.value))
+        except Exception as ex:
+            logger.error("problem with sorted list: "+str(ex))
+    
 
     def _sort(self):                        
         
         def saveToSortedCkmerStorage(ckmer,ckmerType,number,numberOfCkmers):
             ckmerRow = self.tableSortedKmers.row            
             ckmerRow["ckmer"] = ckmer
             ckmerRow["type"] = ckmerType
@@ -233,29 +262,23 @@
         def saveToSortedBaseStorage(base,branches,number,numberOfBases):
             baseRow = self.tableSortedBases.row    
             baseRow["base"] = base
             baseRow["number"] = number
             self.frequencyHistogram["base"][number] = (
                                 self.frequencyHistogram["base"].get(number,0)+1)
             for letter in branches.keys():
-                baseRow["branches/"+str(letter)+"/number"] = branches[letter]["number"]
-                baseRow["branches/"+str(letter)+"/ckmerLink"] = branches[letter]["ckmerLink"]
-                ckmerRow = self.tableSortedKmers[branches[letter]["ckmerLink"]]
+                baseRow["branches/"+str(letter)+"/number"] = branches[letter][0]
+                baseRow["branches/"+str(letter)+"/ckmerLink"] = branches[letter][1]
+                ckmerRow = self.tableSortedKmers[branches[letter][1]]
                 ckmer = ckmerRow["ckmer"].decode()
                 rkmer=haplotyping.General.reverse_complement(ckmer)
                 if ckmer == base+letter:
-                    self.tableSortedKmers.modify_column(branches[letter]["ckmerLink"],
-                                                        branches[letter]["ckmerLink"]+1,
-                                                        column=[numberOfBases],
-                                                        colname="rightSplitBaseLink/rightSplit")   
+                    baseReferences[branches[letter][1]][1] = numberOfBases
                 if rkmer == base+letter:
-                    self.tableSortedKmers.modify_column(branches[letter]["ckmerLink"],
-                                                        branches[letter]["ckmerLink"]+1,
-                                                        column=[numberOfBases],
-                                                        colname="rightSplitBaseLink/leftSplit")   
+                    baseReferences[branches[letter][1]][0] = numberOfBases
             baseRow.append()
             return numberOfBases+1
             
         def saveToDumpBaseStorage(base,branch,number,ckmerLink):   
             baseRow = self.tableDumpRightSplitBases.row
             baseRow["base"] = base
             baseRow["branch"] = branch
@@ -275,17 +298,16 @@
                 "rightSplitBaseLink": {
                     "leftSplit": haplotyping.index.Database.getTablesUint(numberOfSplittingKmers,0),
                     "rightSplit": haplotyping.index.Database.getTablesUint(numberOfSplittingKmers,1),
                 },
                 "number": tables.UInt32Col(pos=3,dflt=0),
             }
             self.tableSortedKmers = self.pytablesStorage.create_table(self.pytablesStorage.root,
-                                                                       "sortedCkmer",tableCkmerDef, 
-                                                    "Temporary to store sorted canonical k-mers",
-                                                                      expectedrows=numberOfSplittingKmers)  
+                                        "sortedCkmer",tableCkmerDef, "Temporary to store sorted canonical k-mers",
+                                        expectedrows=numberOfSplittingKmers)  
             
             #create dump table for bases
             tableDumpBaseDef = {
                 "base": tables.StringCol(self.k-1,pos=0),
                 "branch": tables.StringCol(1,pos=1),
                 "number": tables.UInt32Col(pos=2,dflt=0),
                 "ckmerLink": haplotyping.index.Database.getTablesUint(numberOfSplittingKmers,3),
@@ -295,14 +317,15 @@
                                                                    "Temporary to store dump bases",
                                                                        expectedrows=numberOfSplittingKmers)
             
             #store sorted k-mers
             self._logger.debug("sort and group "+str(numberOfSplittingKmers)+" splitting k-mers")
             self.tableDumpKmers.cols.ckmer.create_csindex()
             self.tableDumpKmers.flush()
+            self._logger.debug("created index to sort k-mers")
             previousCkmer=None
             previousType=None
             previousN=None
             self.maximumNumber = 0
             numberOfCkmers = 0
             for row in self.tableDumpKmers.itersorted("ckmer",checkCSI=True):
                 currentCkmer=row["ckmer"]
@@ -315,19 +338,22 @@
                     previousType=currentType.decode()
                 elif previousCkmer and not previousType==currentType:
                     previousType="b"
                 else:
                     previousType=currentType.decode()
                 previousCkmer=currentCkmer
                 previousN=currentN
+                if (numberOfCkmers%1000000)==0 and (numberOfCkmers>0):
+                    self._logger.debug("processed {} k-mers".format(numberOfCkmers))
             if previousCkmer:        
                 numberOfCkmers = saveToSortedCkmerStorage(previousCkmer.decode(),previousType,
                                                      previousN,numberOfCkmers) 
                 self.maximumNumber=max(self.maximumNumber,previousN)
-                
+            self._logger.debug("in total processed {} k-mers".format(numberOfCkmers))
+            
             self.tableDumpRightSplitBases.flush()                
             numberOfBases=self.tableDumpRightSplitBases.shape[0]
                 
             #store sorted bases
             self.tableSortedKmers.flush()
             numberOfKmers=self.tableSortedKmers.shape[0]
             tableBaseDef = {
@@ -342,38 +368,48 @@
                 }
             self.tableSortedBases = self.pytablesStorage.create_table(self.pytablesStorage.root,
                                                                    "sortedBase",tableBaseDef, 
                                                                    "Temporary to store dump bases",
                                                                        expectedrows=numberOfKmers)
             
             #store sorted bases
-            self._logger.debug("sort and group "+str(numberOfBases)+" bases")
+            self._logger.debug("sort and group {} bases".format(numberOfBases))
             self.tableDumpRightSplitBases.cols.base.create_csindex()
             self.tableDumpRightSplitBases.flush()
+            self._logger.debug("created index to sort bases")
             previousBase=None
             previousBranches={}
             previousNumber=0
             numberOfBases = 0
+            #reserve memory for links in ckmer table
+            ckmerLinkType = np.dtype(haplotyping.index.Database.getUint(numberOfKmers)).type
+            baseReferences = np.full((numberOfKmers,2), 0, dtype=ckmerLinkType)
             for row in self.tableDumpRightSplitBases.itersorted("base",checkCSI=True):
-                currentBase=row["base"]
-                currentBranch=row["branch"]
-                currentNumber=row["number"]
-                currentCkmerLink=row["ckmerLink"]
+                currentBase=row[0]
+                currentBranch=row[1]
+                currentNumber=row[2]
+                currentCkmerLink=row[3]
                 if previousBase and not previousBase==currentBase:
                     numberOfBases = saveToSortedBaseStorage(previousBase.decode(),previousBranches,
                                                             previousNumber,numberOfBases)
                     previousBase=None
                     previousBranches={}
                     previousNumber=0
+                    if (numberOfBases%1000000)==0 and (numberOfBases>0):
+                        self._logger.debug("processed {} bases".format(numberOfBases))
                 previousBase=currentBase
-                previousBranches[row["branch"].decode()] = {"number": currentNumber, "ckmerLink": currentCkmerLink}
-                previousNumber+=currentNumber
+                previousBranches[currentBranch.decode()] = (currentNumber, currentCkmerLink,)
+                previousNumber+=currentNumber                    
             if previousBase:
                     numberOfBases = saveToSortedBaseStorage(previousBase.decode(),previousBranches,
-                                                            previousNumber,numberOfBases)    
+                                                            previousNumber,numberOfBases)  
+            self._logger.debug("in total processed {} bases".format(numberOfBases))
+            #update ckmers
+            self.tableSortedKmers.modify_columns(columns=baseReferences,
+                             names=["rightSplitBaseLink/leftSplit","rightSplitBaseLink/rightSplit"])   
                 
         else:
             self._logger.warning("no splitting k-mers to sort and group")
             
     def _store(self):
         canonicalSplitKmers = 0
         canonicalSplitKmersLeft = 0
@@ -394,139 +430,192 @@
                               ("left",
                                [("distinct","uint8"),
                                 ("number",haplotyping.index.Database.getUint(self.maximumNumber))]),
                               ("right",
                                [("distinct","uint8"),
                                 ("number",haplotyping.index.Database.getUint(self.maximumNumber))])
                              ]),
-                   ("connected",[("link",haplotyping.index.Database.getUint(numberOfKmers)),
-                                 ("number",haplotyping.index.Database.getUint(len(haplotyping.index.Database.letters)**4)),
-                                 ("connected",
-                                      haplotyping.index.Database.getUint(len(haplotyping.index.Database.letters)**4))]),
-                   ("paired",[("link",haplotyping.index.Database.getUint(numberOfKmers)),
-                              ("number",haplotyping.index.Database.getUint(len(haplotyping.index.Database.letters)**4))]),
+                   ("partition",haplotyping.index.Database.getUint(numberOfKmers)),
                    ("cycle",[("number",haplotyping.index.Database.getUint(self.maximumNumber))]),
-                   ("reversal",[("number",haplotyping.index.Database.getUint(self.maximumNumber))])]
+                   ("reversal",[("number",haplotyping.index.Database.getUint(self.maximumNumber))]),
+                   ("paired",[("link",haplotyping.index.Database.getUint(numberOfKmers)),
+                              ("number",haplotyping.index.Database.getUint(self.maximumNumber))])]
         dtCkmer=np.dtype(dtypeCkmerList)
-        dsCkmer=self.h5file["/split/"].create_dataset("ckmer",(numberOfKmers,), dtype=dtCkmer, chunks=None)
+        dsCkmer=self.h5file["/split/"].create_dataset("ckmer",(numberOfKmers,), dtype=dtCkmer, chunks=None, 
+                                                      compression="gzip", compression_opts=9)
         self._logger.info("store {} splitting k-mers".format(numberOfKmers))
         #add stored and grouped kmers to the final unchunked storage
         for i in range(0,numberOfKmers,Splits.stepSizeStorage):
             stepData = self.tableSortedKmers[i:i+Splits.stepSizeStorage]
             dsCkmer[i:i+Splits.stepSizeStorage] = stepData
             for row in stepData:
                 canonicalSplitKmers+=1
                 if row[1].decode()=="l":
                     canonicalSplitKmersLeft+=1
                 elif row[1].decode()=="b":
                     canonicalSplitKmersBoth+=1
                 elif row[1].decode()=="r":
                     canonicalSplitKmersRight+=1
+        dsCkmer.flush()
         # BASE STORAGE - don't make the structure unnecessary big
         dtypeBaseList=[("base","S"+str(self.k-1)),
                    ("number",haplotyping.index.Database.getUint(self.maximumNumber)),
                    ("branches",[])]
         for i in range(len(haplotyping.index.Database.letters)):
             letter = haplotyping.index.Database.letters[i]
             dtypeBaseList[2][1].append((letter,[("number",haplotyping.index.Database.getUint(self.maximumNumber)),
                                                 ("ckmerLink",numberOfKmers)]))
         dtBase=np.dtype(dtypeBaseList)
-        dsBase=self.h5file["/split/"].create_dataset("base",(numberOfBases,), dtype=dtBase, chunks=None)
+        dsBase=self.h5file["/split/"].create_dataset("base",(numberOfBases,), dtype=dtBase, chunks=None,
+                                                     compression="gzip", compression_opts=9)
         self._logger.info("store {} bases".format(numberOfBases))
         #add stored and grouped bases to the final unchunked storage
         for i in range(0,numberOfBases,Splits.stepSizeStorage):
             stepData = self.tableSortedBases[i:i+Splits.stepSizeStorage]
             dsBase[i:i+Splits.stepSizeStorage] = stepData
         # HISTOGRAM K-MER STORAGE - don't make the structure unnecessary big
         maximumFrequency = max(self.frequencyHistogram["kmer"].keys())
         maximumNumber = max(self.frequencyHistogram["kmer"].values())
         dtypeFrequencyHistogramKmerList=[
                     ("frequency",haplotyping.index.Database.getUint(maximumFrequency)),
                     ("number",haplotyping.index.Database.getUint(maximumNumber)),]
         dtFrequencyHistogramKmer=np.dtype(dtypeFrequencyHistogramKmerList)
         dsFrequencyHistogramKmer=self.h5file["/histogram/"].create_dataset("kmer",(len(self.frequencyHistogram["kmer"]),), 
-                                                                  dtype=dtFrequencyHistogramKmer, chunks=None)
+                                                                  dtype=dtFrequencyHistogramKmer, chunks=None, 
+                                                                  compression="gzip", compression_opts=9)
         self._logger.info("store {} entries k-mer histogram".format(len(self.frequencyHistogram["kmer"])))
         #store histogram
         dsFrequencyHistogramKmer[0:len(self.frequencyHistogram["kmer"])] = list(
             sorted(self.frequencyHistogram["kmer"].items()))
         # HISTOGRAM SPLITTING K-MER STORAGE - don't make the structure unnecessary big
         maximumFrequency = max(self.frequencyHistogram["ckmer"].keys())
         maximumNumber = max(self.frequencyHistogram["ckmer"].values())
         dtypeFrequencyHistogramCkmerList=[
                     ("frequency",haplotyping.index.Database.getUint(maximumFrequency)),
                     ("number",haplotyping.index.Database.getUint(maximumNumber)),]
         dtFrequencyHistogramCkmer=np.dtype(dtypeFrequencyHistogramCkmerList)
         dsFrequencyHistogramCkmer=self.h5file["/histogram/"].create_dataset("ckmer",(len(self.frequencyHistogram["ckmer"]),), 
-                                                                  dtype=dtFrequencyHistogramCkmer, chunks=None)
+                                                                  dtype=dtFrequencyHistogramCkmer, chunks=None, 
+                                                                  compression="gzip", compression_opts=9)
         self._logger.info("store {} entries splitting k-mer histogram".format(len(self.frequencyHistogram["ckmer"])))
         #store histogram
         dsFrequencyHistogramCkmer[0:len(self.frequencyHistogram["ckmer"])] = list(
             sorted(self.frequencyHistogram["ckmer"].items()))
         # HISTOGRAM SPLITTING K-MER BASES STORAGE - don't make the structure unnecessary big
         maximumFrequency = max(self.frequencyHistogram["base"].keys())
         maximumNumber = max(self.frequencyHistogram["base"].values())
         dtypeFrequencyHistogramBaseList=[
                     ("frequency",haplotyping.index.Database.getUint(maximumFrequency)),
                     ("number",haplotyping.index.Database.getUint(maximumNumber)),]
         dtFrequencyHistogramBase=np.dtype(dtypeFrequencyHistogramBaseList)
         dsFrequencyHistogramBase=self.h5file["/histogram/"].create_dataset("base",(len(self.frequencyHistogram["base"]),), 
-                                                                  dtype=dtFrequencyHistogramBase, chunks=None)
+                                                                  dtype=dtFrequencyHistogramBase, chunks=None, 
+                                                                  compression="gzip", compression_opts=9)
         self._logger.info("store {} entries splitting k-mer bases histogram".format(len(self.frequencyHistogram["base"])))
         #store histogram
         dsFrequencyHistogramBase[0:len(self.frequencyHistogram["base"])] = list(
             sorted(self.frequencyHistogram["base"].items()))
         #store the stats
         self._logger.debug("found {} canonicalSplitKmersLeft".format(canonicalSplitKmersLeft))
         self._logger.debug("found {} canonicalSplitKmersRight".format(canonicalSplitKmersRight))
         self._logger.debug("found {} canonicalSplitKmersBoth".format(canonicalSplitKmersBoth))
-        self.h5file["/config/"].attrs["maximumFrequency"]=self.maximumNumber
-        self.h5file["/config/"].attrs["canonicalSplitKmers"]=canonicalSplitKmers
-        self.h5file["/config/"].attrs["canonicalSplitKmersLeft"]=canonicalSplitKmersLeft
-        self.h5file["/config/"].attrs["canonicalSplitKmersBoth"]=canonicalSplitKmersBoth
-        self.h5file["/config/"].attrs["canonicalSplitKmersRight"]=canonicalSplitKmersRight 
+        self.h5file["/config/"].attrs["maximumCanonicalSplitFrequency"]=self.maximumNumber
+        self.h5file["/config/"].attrs["numberCanonicalSplit"]=canonicalSplitKmers
+        self.h5file["/config/"].attrs["numberCanonicalSplitLeft"]=canonicalSplitKmersLeft
+        self.h5file["/config/"].attrs["numberCanonicalSplitBoth"]=canonicalSplitKmersBoth
+        self.h5file["/config/"].attrs["numberCanonicalSplitRight"]=canonicalSplitKmersRight 
+        
+    def deleteAutomatonWithIndex(filenameBase, k):
+        indexFile = "{}_{}.index.splits".format(filenameBase,k)
+        automatonFile = "{}_{}.automaton.splits".format(filenameBase,k)
+        automatonStatsFile = "{}_{}.automaton.splits.stats".format(filenameBase,k)
+        if os.path.exists(indexFile):
+            os.remove(indexFile)
+        if os.path.exists(automatonFile):
+            os.remove(automatonFile)
+        if os.path.exists(automatonStatsFile):
+            os.remove(automatonStatsFile)
         
-    def createAutomatonWithIndex(h5file, indexFile, automatonFile, k):
+    def createAutomatonWithIndex(h5file, filenameBase, k):
         k = min(h5file["/config"].attrs["k"],k)
         logger = logging.getLogger(__name__)
         logger.info("create automaton with k' = {}".format(k))
-        automatonSplits = ahocorasick.Automaton()
-        numberOfKmers = h5file["/split/ckmer"].shape[0]
-        kmers = h5file["/split/ckmer"]
-        with open(indexFile, "w") as f:
-            for i in range(0,numberOfKmers,Splits.stepSizeStorage):
-                kmerSubset = kmers[i:i+Splits.stepSizeStorage]
-                for j in range(len(kmerSubset)):
-                    id = i + j
-                    row = kmerSubset[j]                
-                    kmer = row[0].decode()
-                    #store in index
-                    f.write(kmer)
-                    #build automaton for k'-mers with k'<=k describing:
-                    #- number of canonical k-mers to check starting from the provided index-location
-                    #- index-location of the first matching canonical k-mer
-                    rkmer = haplotyping.General.reverse_complement(kmer[-k:])
-                    kmer = kmer[:k]
-                    if (not automatonSplits.exists(kmer)):
-                        automatonSplits.add_word(kmer,(1,id))
-                    else:
-                        value=list(automatonSplits.get(kmer))
-                        if value[0]==0:
-                            value[1]=id
-                            value[0]=1
-                        else:
-                            value[0]=id-value[1]+1
-                        automatonSplits.add_word(kmer,tuple(value))
-                    if not kmer==rkmer:
-                        if (not automatonSplits.exists(rkmer)):
-                            automatonSplits.add_word(rkmer,(0,id))
-        #create and store automaton
-        automatonSplits.make_automaton()
-        stats = automatonSplits.get_stats()
-        logger.debug("automaton with {} words, size {} MB".format(stats["words_count"],
-                                                                  round(stats["total_size"]/1048576)))
-        with open(automatonFile, "wb") as f:
-            pickle.dump(automatonSplits, f)
+        indexFile = "{}_{}.index.splits".format(filenameBase,k)
+        automatonFile = "{}_{}.automaton.splits".format(filenameBase,k)
+        automatonStatsFile = "{}_{}.automaton.splits.stats".format(filenameBase,k)
+        if os.path.exists(indexFile) and os.path.exists(automatonFile)and os.path.exists(automatonStatsFile):
+            logger.debug("detected previously generated automaton and index")
+            with open(automatonStatsFile, "rb") as f:
+                stats = pickle.load(f)
+            logger.debug("automaton with {} words, size {} MB".format(stats["words_count"],
+                                                                          round(stats["real_size"]/1048576)))
+            logger.debug("associated index filesize {} MB".format(round(os.stat(indexFile).st_size/1048576)))
+            return (max(stats["real_size"],stats["total_size"]),indexFile, automatonFile)
+        else:
+            logger.debug("generate automaton and index")
+            tmpAutomatonFile = "{}.tmp".format(automatonFile)
+            tmpIndexFile = "{}.tmp".format(indexFile)
+            try:
+                process = psutil.Process(os.getpid())
+                memoryBefore = process.memory_info().rss
+                automatonSplits = ahocorasick.Automaton()
+                numberOfKmers = h5file["/split/ckmer"].shape[0]
+                kmers = h5file["/split/ckmer"]
+                with open(tmpIndexFile, "w") as f:
+                    for i in range(0,numberOfKmers,Splits.stepSizeStorage):
+                        kmerSubset = kmers[i:i+Splits.stepSizeStorage]
+                        for j in range(len(kmerSubset)):
+                            id = i + j
+                            row = kmerSubset[j]                
+                            kmer = row[0].decode()
+                            #store in index
+                            f.write(kmer)
+                            #build automaton for k'-mers with k'<=k describing:
+                            #- number of canonical k-mers to check starting from the provided index-location
+                            #- index-location of the first matching canonical k-mer
+                            rkmer = haplotyping.General.reverse_complement(kmer[-k:])
+                            kmer = kmer[:k]
+                            if (not automatonSplits.exists(kmer)):
+                                automatonSplits.add_word(kmer,(1,id))
+                            else:
+                                value=list(automatonSplits.get(kmer))
+                                if value[0]==0:
+                                    value[1]=id
+                                    value[0]=1
+                                else:
+                                    value[0]=id-value[1]+1
+                                automatonSplits.add_word(kmer,tuple(value))
+                            if not kmer==rkmer:
+                                if (not automatonSplits.exists(rkmer)):
+                                    automatonSplits.add_word(rkmer,(0,id))
+                #create and store automaton
+                automatonSplits.make_automaton()
+                memoryAfter = process.memory_info().rss
+                stats = automatonSplits.get_stats()
+                stats["real_size"] = memoryAfter - memoryBefore
+                logger.debug("automaton with {} words, size {} MB".format(stats["words_count"],
+                                                                          round(stats["real_size"]/1048576)))
+                logger.debug("associated index filesize {} MB".format(round(os.stat(tmpIndexFile).st_size/1048576)))
+                automatonSplits.save(tmpAutomatonFile, pickle.dumps)
+                #clear
+                automatonSplits.clear()
+                del automatonSplits
+                #copy all
+                shutil.copyfile(tmpAutomatonFile, automatonFile)
+                shutil.copyfile(tmpIndexFile, indexFile)
+                #also store stats
+                with open(automatonStatsFile, "wb") as f:
+                    pickle.dump(stats, f)
+            except Exception as ex:
+                logger.debug("problem while creating automaton: {}".format(ex))
+            finally:
+                if os.path.exists(tmpIndexFile):
+                    os.remove(tmpIndexFile)
+                if os.path.exists(tmpAutomatonFile):
+                    os.remove(tmpAutomatonFile)
+                    
+                
+        return (max(stats["real_size"],stats["total_size"]),indexFile, automatonFile)
```

### Comparing `haplotyping-0.0.5/haplotyping/index/storage.py` & `haplotyping-0.0.6/haplotyping/index/storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import haplotyping.index.database
 from multiprocessing import shared_memory, current_process
+from statistics import multimode
 from queue import Empty
-import os, re, pickle, tables, statistics, logging
+import ahocorasick, metis
+import os, re, pickle, tables, statistics, logging, time, psutil
 import numpy as np, math
 from contextlib import ExitStack
 
 class Storage:
     
     """
     Internal use, storage and processing
     """
     
-    def create_merge_storage(pytablesStorage, numberOfKmers, maximumFrequency, maximumConnectionLength,
-                             nCycle=None, nReversal=None, nDirect=None, 
-                             nConnections=None, nPaired=None):
+    stepSizeStorage = 1000000
+    
+    def create_mergeDirect_storage(pytablesStorage, numberOfKmers, maximumFrequency,
+                             nCycle=None, nReversal=None, nDirect=None, nPaired=None):
+        pytablesStorage.create_table(pytablesStorage.root, 
+            "tmpPaired",{
+            "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
+            "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1),
+        }, "Temporary Paired", expectedrows=nPaired)
         pytablesStorage.create_table(pytablesStorage.root, 
             "cycle",{
             "ckmerLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
             "minimumLength": tables.UInt16Col(pos=1),
             "number": haplotyping.index.Database.getTablesUint(maximumFrequency,2),
         }, "Cycles", expectedrows=nCycle)
         pytablesStorage.create_table(pytablesStorage.root, 
@@ -42,133 +50,199 @@
         pytablesStorage.create_table(pytablesStorage.root, 
             "deleteDirect",{
             "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
             "fromDirection": tables.StringCol(itemsize=1,pos=1),
             "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,2),
             "toDirection": tables.StringCol(itemsize=1,pos=3),
         }, "Incorrect direct relations", expectedrows=nDirect)
-        pytablesStorage.create_table(pytablesStorage.root, 
-            "connections",{
-            "ckmerLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
-            "dataLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1),
-            "length": haplotyping.index.Database.getTablesUint(maximumConnectionLength,2),
-            "number": haplotyping.index.Database.getTablesUint(maximumFrequency,3),
-            "direct": tables.UInt8Col(pos=4),
-        }, "Indirect relations", expectedrows=nConnections)
-        pytablesStorage.create_earray(pytablesStorage.root, 
-            "data",haplotyping.index.Database.getTablesUintAtom(numberOfKmers),(0,), 
-            "Data", expectedrows=nConnections)
-        pytablesStorage.create_table(pytablesStorage.root, 
-            "paired",{
-            "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
-            "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1),
-            "number": haplotyping.index.Database.getTablesUint(maximumFrequency,2),
-        }, "Paired relations", expectedrows=nPaired)
-        pytablesStorage.create_table(pytablesStorage.root, 
-            "deletePaired",{
-            "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
-            "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1),
-        }, "Incorrect paired relations", expectedrows=nPaired)
         
-    def worker_automaton(shutdown_event,queue_automaton,queue_index,queue_finished,k,automatonKmerSize,automatonFile):
+    def create_filteredReads_storage(pytablesStorage,numberOfReads,numberOfData,numberOfKmers,
+                                  numberOfPartitions,maximumReadLength,numberOfPaired):
+        filters = tables.Filters(complevel=9, complib="blosc")
+        pytablesStorage.create_earray(
+                      pytablesStorage.root, "readPartitionData",
+                      haplotyping.index.Database.getTablesUintAtom(numberOfKmers), 
+                      shape=(0,), filters=filters, 
+                      expectedrows=numberOfData)
+        pytablesStorage.create_table(
+                      pytablesStorage.root, "readPartitionInfo", {
+                        "length": haplotyping.index.Database.getTablesUint(maximumReadLength,0),
+                        "partition": haplotyping.index.Database.getTablesUint(numberOfPartitions,1)
+                      }, "Read size and partition",
+                      expectedrows=numberOfReads)
+        pytablesStorage.create_table(
+                      pytablesStorage.root, "readPaired", {
+                        "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
+                        "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1),
+                      }, "Paired Reads",
+                      expectedrows=numberOfPaired)
+        
+    def create_filteredMergedReads_storage(pytablesStorage,numberOfReads,numberOfData,numberOfKmers,
+                                            numberOfPartitions,maximumReadLength):
+        filters = tables.Filters(complevel=9, complib="blosc")
+        pytablesStorage.create_earray(
+                      pytablesStorage.root, "readPartitionData",
+                      haplotyping.index.Database.getTablesUintAtom(numberOfKmers), 
+                      shape=(0,), filters=filters, 
+                      expectedrows=numberOfData)
+        pytablesStorage.create_table(
+                      pytablesStorage.root, "readPartitionInfo", {
+                        "length": haplotyping.index.Database.getTablesUint(maximumReadLength,0),
+                        "number": haplotyping.index.Database.getTablesUint(numberOfReads,1)
+                      }, "Read size and number",
+                      expectedrows=numberOfReads)
+        pytablesStorage.create_table(
+                      pytablesStorage.root, "readPartition", {
+                        "readPartitionDataLink": haplotyping.index.Database.getTablesUint(numberOfData,0),
+                        "readPartitionDataNumber": haplotyping.index.Database.getTablesUint(numberOfData,1),
+                        "readPartitionInfoLink": haplotyping.index.Database.getTablesUint(numberOfReads,2),
+                        "readPartitionInfoNumber": haplotyping.index.Database.getTablesUint(numberOfReads,3)
+                      }, "Index data and info readPartitions",
+                      expectedrows=numberOfPartitions)
         
-        logger = logging.getLogger(__name__)
+    def create_mergeReads_storage(pytablesStorage,numberOfReads,numberOfData,numberOfKmers,
+                                  numberOfPartitions,maximumReadLength):
+        filters = tables.Filters(complevel=9, complib="blosc")
+        pytablesStorage.create_carray(
+                      pytablesStorage.root, "readPartitionData",
+                      haplotyping.index.Database.getTablesUintAtom(numberOfKmers), 
+                      shape=(numberOfData,), filters=filters)
+        pytablesStorage.create_carray(
+                      pytablesStorage.root, "readPartitionLength",
+                      haplotyping.index.Database.getTablesUintAtom(maximumReadLength), 
+                      shape=(numberOfReads,), filters=filters)
+        pytablesStorage.create_carray(
+                      pytablesStorage.root, "readPartitionInfo",
+                      haplotyping.index.Database.getTablesUintAtom(numberOfPartitions), 
+                      shape=(numberOfReads,), filters=filters)        
+    
+    def worker_automaton(shutdown_event,queue_start,queue_automaton,queue_index,
+                         queue_finished,k,automatonKmerSize,automatonFile):
         
+        logger = logging.getLogger("{}.worker.automaton".format(__name__))
+                
         def compute_matches(sequence,automatonSplits):
             rsequence = haplotyping.General.reverse_complement(sequence)
-            boundary = (len(sequence)-k+automatonKmerSize-1)
-            correction_reverse = len(sequence) + automatonKmerSize - 1 - k
+            boundary = len(sequence)-k+automatonKmerSize
+            correction_reverse = boundary - 1
             correction_forward = automatonKmerSize - 1
             #use automaton to check reverse complement sequence
-            rdict = {correction_reverse - end_index: (number, startLinks,)
-                     for (end_index, (number,startLinks)) in automatonSplits.iter(rsequence) 
-                     if end_index <= boundary}
-            if len(rdict.keys())>0:
-                #use automaton to check sequence
-                flist = [(end_index - correction_forward, number, startLinks)
-                         for (end_index, (number,startLinks)) in automatonSplits.iter(sequence)
-                         if end_index <= boundary]
+            rdict = {(correction_reverse - end_index): (number, startLinks,)
+                     for (end_index, (number,startLinks)) in automatonSplits.iter(rsequence,0,boundary)}
+            if len(rdict)>0:
+                flist = [(end_index - correction_forward, number, startLinks,)
+                         for (end_index, (number,startLinks)) in automatonSplits.iter(sequence,0,boundary)]
                 #combine results
                 clist = [(pos, (number, startLinks,) ,rdict[pos]) 
                          for (pos, number, startLinks) in flist 
                          if pos in rdict.keys()]
             else:
                 clist = []
             return clist
         
-        #load automaton into memory
-        with open(automatonFile, "rb") as f:
-            automatonSplits = pickle.load(f)
-        logger.debug("automaton: fsm loaded from {} MB".format(round(os.stat(automatonFile).st_size/1048576)))
+        try:
             
-        while not shutdown_event.is_set():
-            try:
-                item = queue_automaton.get(block=True, timeout=1)
-                if item==None:
-                    break
-                elif isinstance(item,tuple) and len(item)==2:
-                    queue_index.put((
-                        (item[0],compute_matches(item[0],automatonSplits),),
-                        (item[1],compute_matches(item[1],automatonSplits),),
-                    ))
+            #wait for permission to start loading automaton
+            while True:
+                try:
+                    item = queue_start.get(block=True, timeout=1)
+                    if item=="automaton":
+                        break
+                    else:
+                        logger.error("automaton ({}): unexpected start value in queue: {}".format(os.getpid(),item))
+                except:
                     pass
-                elif isinstance(item,str):
-                    queue_index.put((
-                        (item,compute_matches(item,automatonSplits),),
-                    ))
-            except Empty:
-                continue
-        del automatonSplits
-        logger.debug("automaton: fsm released")
-        queue_finished.put("automaton")
+                time.sleep(1)
+            
+            logger.debug("automaton ({}): load automaton from {}".format(os.getpid(),automatonFile))
+            
+            #load automaton into memory
+            automatonSplits = ahocorasick.load(automatonFile,pickle.loads)
+            logger.debug("automaton ({}): fsm loaded from {} MB".format(
+                os.getpid(),math.ceil(os.stat(automatonFile).st_size/1048576)))
+
+            process = psutil.Process(os.getpid())
+            logger.debug("automaton ({}): used memory {} MB".format(
+                os.getpid(),math.ceil(process.memory_info().rss/1048576)))
+            
+            #finished loading automaton
+            queue_finished.put("automaton:started")
+
+            while not shutdown_event.is_set():
+                try:
+                    item = queue_automaton.get(block=True, timeout=1)
+                    if item==None:
+                        logger.debug("autmaton ({}): none item".format(os.getpid()))
+                        break
+                    elif isinstance(item,tuple) and len(item)==2:
+                        queue_index.put((
+                            (item[0],compute_matches(item[0],automatonSplits),),
+                            (item[1],compute_matches(item[1],automatonSplits),),
+                        ))
+                    elif isinstance(item,str):
+                        queue_index.put((
+                            (item,compute_matches(item,automatonSplits),),
+                        ))
+                except Empty:
+                    logger.debug("automaton ({}): empty".format(os.getpid()))
+                    time.sleep(5)
+                    continue
+        except Exception as ex:
+            logger.error("automaton ({}): problem with worker: {}".format(os.getpid(),ex))
+        finally:
+            del automatonSplits
+            logger.debug("automaton ({}): fsm released".format(os.getpid()))
+        queue_finished.put("automaton:ended")
             
                 
     
-    def worker_index(shutdown_event,queue_index,queue_matches,queue_finished,k,shm_name):
+    def worker_index(shutdown_event,queue_index,queue_matches,queue_storage,queue_finished,
+                     filenameBase,numberOfKmers,k,onlyDirectConnections,shm_name):
 
-        logger = logging.getLogger(__name__)
+        logger = logging.getLogger("{}.worker.index".format(__name__))
         problemPattern = re.compile(r"["+"".join(haplotyping.index.Database.letters)+
-                                         "][^"+"".join(haplotyping.index.Database.letters)+"]+")
+                                         "][^"+"".join(haplotyping.index.Database.letters)+"]+")   
         
         def problemStartPositions(sequence):
             problemStartPositions = []        
             for m in re.finditer(problemPattern, sequence):
                 problemStartPositions.append(m.span()[0]+1)
             return problemStartPositions
 
-        def compute_matches(sequence,clist):
+        def compute_matches(sequence,clist):            
             history = {}
             matchesList = []
             problems = problemStartPositions(sequence)
             relevantProblem = None if len(problems)==0 else problems[0]
             matches = []
-            
             previousLink = -1
             previousPos = -1
-            
             positions = []
+            totalChecks=len(clist)
+            totalMatches = 0
             for pos, (forward_number,forward_startLinks), (reverse_number,reverse_startLinks) in clist:
                 positions.append(pos)
                 #check if really match
-                kmer = sequence[pos:pos+k]            
+                kmer = sequence[pos:pos+k]  
                 #only possible if is reversed
                 if forward_number==0:  
                     if reverse_number==0:
                         continue
                     else:
                         rkmer = haplotyping.General.reverse_complement(kmer)
                         if rkmer>kmer:
                             continue
                         else:
                             startLinks = max(forward_startLinks,reverse_startLinks)
                             endLinks = reverse_startLinks+reverse_number
                             foundMatch = False
                             for i in range(startLinks,endLinks):
                                 indexLink = i*k
-                                if rkmer==shm.buf[indexLink:indexLink+k].tobytes().decode():
+                                nkmer = shm.buf[indexLink:indexLink+k].tobytes().decode()
+                                if rkmer==nkmer:
                                     link = i
                                     orientation = "r"
                                     foundMatch = True
                                     break
                             if not foundMatch:
                                 continue
                 else:
@@ -179,160 +253,270 @@
                             continue
                         else:
                             startLinks = max(forward_startLinks,reverse_startLinks)
                             endLinks = forward_startLinks+forward_number
                             foundMatch = False
                             for i in range(startLinks,endLinks):
                                 indexLink = i*k
-                                if kmer==shm.buf[indexLink:indexLink+k].tobytes().decode():
+                                nkmer = shm.buf[indexLink:indexLink+k].tobytes().decode()
+                                if kmer==nkmer:
                                     link = i
                                     orientation = "c"
                                     foundMatch = True
                                     break
                             if not foundMatch:
                                 continue
                     else:
                         foundMatch = False
                         #if forward
                         if kmer<rkmer:
                             startLinks = forward_startLinks
                             endLinks = forward_startLinks+forward_number
                             for i in range(startLinks,endLinks):
                                 indexLink = i*k
-                                if kmer==shm.buf[indexLink:indexLink+k].tobytes().decode():
+                                nkmer = shm.buf[indexLink:indexLink+k].tobytes().decode()
+                                if kmer==nkmer:
                                     link = i
                                     orientation = "c"
                                     foundMatch = True
                                     break
                             if not foundMatch:
                                 #no match
                                 continue
                         #if reverse
                         else:
                             startLinks = reverse_startLinks
                             endLinks = reverse_startLinks+reverse_number
                             foundMatch = False
                             for i in range(startLinks,endLinks):
                                 indexLink = i*k
-                                if rkmer==shm.buf[indexLink:indexLink+k].tobytes().decode():
+                                nkmer = shm.buf[indexLink:indexLink+k].tobytes().decode()
+                                if rkmer==nkmer:
                                     link = i
                                     orientation = "r"
                                     foundMatch = True
                                     break
                             if not foundMatch:
                                 continue
 
                 history[link]=[orientation,pos]
                 #check if a problem did occur between last match and current
                 if relevantProblem and len(matches)>0 and pos>relevantProblem:
                     matchesList.append(matches)
-                    matches=[]  
+                    totalMatches+=len(matches)
+                    matches=[]                  
                 matches.append([pos,link,orientation])
                 previousPos = pos
                 previousLink = link
                 #compute where the next problem will occur
                 if relevantProblem and pos>relevantProblem:
                     relevantProblem = None
                     for problem in problems:
                         if problem>pos:
                             relevantProblem=problem
                             break                   
             if len(matches)>0:
                 matchesList.append(matches)
-            return (matchesList, len(matchesList)==1)
+                totalMatches+=len(matches)
+            return (matchesList, len(matchesList)==1, totalChecks, totalMatches)
+        
+        def normalised_matchesList(matches):
+            matchesList = []
+            for item in matches:
+                matchesList.extend([s[1] for s in item])
+            if len(matchesList)==0:
+                return matchesList
+            elif matchesList[0]<matchesList[-1]:
+                return matchesList
+            elif matchesList[0]>matchesList[-1]:
+                return matchesList[::-1]
+            elif hash(tuple(matchesList))<hash(tuple(matchesList[::-1])):
+                return matchesList
+            else:
+                return matchesList[::-1]
+            
+        def store_matches(matches,readData,readInfo):
+            matchesList = normalised_matchesList(matches)
+            if len(matchesList)>0:
+                readData.append(tuple(matchesList))
+                readInfo.append([(len(matchesList),0,)])
+            
+        def store_paired_matches(matches0,matches1,readData,readInfo):
+            matches0List = normalised_matchesList(matches0)
+            matches1List = normalised_matchesList(matches1)
+            if len(matches0List)==0 and len(matches1List)==0:
+                pass
+            elif len(matches0List)==0:
+                store_matches(matches1,readData,readInfo)
+            elif len(matches1List)==0:
+                store_matches(matches0,readData,readInfo)
+            else:
+                readData.append(tuple(matches0List))
+                readData.append(tuple(matches1List))
+                readInfo.append([(len(matches0List),1,)])
+                readInfo.append([(len(matches1List),2,)])
+            
+                    
+        #stats
+        totalChecks = 0
+        totalMatches = 0
         
         shm = shared_memory.SharedMemory(shm_name)
-        logger.debug("index: shared memory of {} MB used".format(round(shm.size/1048576)))
+        logger.debug("index ({}): shared memory of {} MB used".format(
+            os.getpid(),math.ceil(shm.size/1048576)))
+        
+        process = psutil.Process(os.getpid())
+        logger.debug("index ({}): used memory {} MB".format(
+            os.getpid(),math.ceil(process.memory_info().rss/1048576)))
+        
         try:
-            while not shutdown_event.is_set():
-                try:
-                    item = queue_index.get(block=True, timeout=1)
-                    if item==None:
-                        break
-                    elif isinstance(item,tuple):
-                        if len(item)==1:
-                            (matches, direct, ) = compute_matches(item[0][0],item[0][1])
-                            if len(matches)==0 or (len(matches)==1 and len(matches[0])==1):
-                                pass
-                            else:
-                                queue_matches.put(((matches, direct,),))
-                        elif len(item)==2:
-                            sequence0 = item[0][0]
-                            sequence1 = item[1][0]
-                            (matches0, direct0, ) = compute_matches(item[0][0],item[0][1])
-                            (matches1, direct1, ) = compute_matches(item[1][0],item[1][1])
-                            if len(matches0)==0 and len(matches1)==0:
-                                pass
-                            elif len(matches0)==0:
-                                if len(matches1)==1 and len(matches1[0])==1:
+            curr_proc = current_process()
+            pytablesFileWorker = filenameBase+"_tmp_reads_{}.process.h5".format(curr_proc.name)
+            if os.path.exists(pytablesFileWorker):
+                os.remove(pytablesFileWorker)
+
+            with (open(os.devnull,"w") if onlyDirectConnections 
+                      else tables.open_file(pytablesFileWorker, mode="w")) as pytablesStorageWorker:
+                
+                if not onlyDirectConnections:
+                    filters = tables.Filters(complevel=9, complib="blosc")
+                    readData = pytablesStorageWorker.create_earray(pytablesStorageWorker.root, "readRawData",
+                                      haplotyping.index.Database.getTablesUintAtom(numberOfKmers), 
+                                      shape=(0,), filters=filters)
+                    readInfo = pytablesStorageWorker.create_table(
+                                      pytablesStorageWorker.root, "readRawInfo", {
+                                        "length": tables.UInt32Col(pos=0),
+                                        "paired": tables.UInt8Col(pos=1)
+                                      }, "Read size and paired")
+                    
+                while not shutdown_event.is_set():
+                    try:
+                        item = queue_index.get(block=True, timeout=1)
+                        if item==None:
+                            logger.debug("index ({}): none item".format(os.getpid()))
+                            break
+                        elif isinstance(item,tuple):
+                            if len(item)==1:
+                                (matches,direct,tmpTotalChecks,tmpTotalMatches,) = compute_matches(item[0][0],item[0][1])
+                                totalChecks+=tmpTotalChecks
+                                totalMatches+=tmpTotalMatches
+                                if tmpTotalMatches<=1:
                                     pass
                                 else:
-                                    queue_matches.put(((matches1, direct1,),))
-                            elif len(matches1)==0:
-                                if len(matches0)==1 and len(matches0[0])==1:
+                                    queue_matches.put(((matches, direct,),))
+                                    if not onlyDirectConnections and tmpTotalMatches>2:
+                                        store_matches(matches,readData,readInfo)
+                            elif len(item)==2:
+                                (matches0,direct0,tmpTotalChecks0,tmpTotalMatches0,) = compute_matches(item[0][0],item[0][1])
+                                (matches1,direct1,tmpTotalChecks1,tmpTotalMatches1,) = compute_matches(item[1][0],item[1][1])
+                                totalChecks+=tmpTotalChecks0+tmpTotalChecks1
+                                totalMatches+=tmpTotalMatches0+tmpTotalMatches1
+                                if tmpTotalChecks0==0 and tmpTotalChecks1==0:
                                     pass
+                                elif tmpTotalChecks0==0:
+                                    if tmpTotalChecks1>1:
+                                        queue_matches.put(((matches1, direct1,),))
+                                        if not onlyDirectConnections and tmpTotalChecks1>2:
+                                            store_matches(matches1,readData,readInfo)
+                                elif tmpTotalChecks1==0:
+                                    if tmpTotalChecks0>1:
+                                        queue_matches.put(((matches0, direct0,),))
+                                        if not onlyDirectConnections and tmpTotalChecks0>2:
+                                            store_matches(matches0,readData,readInfo)
                                 else:
-                                    queue_matches.put(((matches0, direct0, ), ))
-                            else:
-                                queue_matches.put(((matches0, direct0, ),
-                                                   (matches1, direct1, )))
-                except Empty:
-                    continue
+                                    queue_matches.put(((matches0, direct0, ),
+                                                       (matches1, direct1, )))
+                                    if not onlyDirectConnections:
+                                        store_paired_matches(matches0,matches1,readData,readInfo)
+                    except Empty:
+                        logger.debug("index ({}): empty".format(os.getpid()))
+                        time.sleep(5)
+                        continue
+            #now the file can be released for later processing
+            if not onlyDirectConnections:
+                queue_storage.put(pytablesFileWorker) 
+        except Exception as ex:
+           logger.error("index  ({}): problem with worker: {}".format(os.getpid(),ex))
         finally:
             shm.close()
-        logger.debug("index: shared memory released")
-        queue_finished.put("index")
+        logger.debug("index ({}): found {} matches in {} checks".format(os.getpid(),totalMatches,totalChecks))
+        queue_finished.put("index:ended:{}:{}".format(totalChecks,totalMatches))
             
     
     """
     Process matches into direct connections and queue full list of matches for indirect connections
     """
-    def worker_matches(shutdown_event,queue_matches,queue_connections,queue_storage,queue_finished,
-                       filenameBase,numberOfKmers,maximumFrequency,estimatedMaximumReadLength,arrayNumberDirect):
+    def worker_matches_dtype(numberOfKmers,maximumFrequency,estimatedMaximumReadLength,numberDirectArray):
+        dtype = [("cycle", [("number", haplotyping.index.Database.getUint(maximumFrequency)),
+                                    ("minimum", haplotyping.index.Database.getUint(
+                                                      2*estimatedMaximumReadLength))]),
+                         ("reversal", [("number", haplotyping.index.Database.getUint(maximumFrequency)),
+                                       ("minimum", haplotyping.index.Database.getUint(
+                                                      2*estimatedMaximumReadLength))]),
+                         ("direct", [("d"+str(i),[("type","uint8"),
+                                                  ("link",haplotyping.index.Database.getUint(numberOfKmers)),
+                                                  ("distance",haplotyping.index.Database.getUint(
+                                                      2*estimatedMaximumReadLength)),
+                                                  ("number",haplotyping.index.Database.getUint(maximumFrequency))]) 
+                                     for i in range(numberDirectArray)]),]
+        return dtype
+    
+    def worker_matches(shutdown_event,queue_matches,queue_storage,queue_finished,
+                       filenameBase,numberOfKmers,maximumFrequency,estimatedMaximumReadLength,
+                       numberDirectArray,onlyDirectConnections,shm_name):
         
-        logger = logging.getLogger(__name__)
+        logger = logging.getLogger("{}.worker.matches".format(__name__))
         try:
             curr_proc = current_process()
             pytablesFileWorker = filenameBase+"_tmp_direct_{}.process.h5".format(curr_proc.name)
             if os.path.exists(pytablesFileWorker):
                 os.remove(pytablesFileWorker)
 
             with tables.open_file(pytablesFileWorker, mode="a") as pytablesStorageWorker:
                 
-                logger.debug("matches: store direct connections (dimension: {})".format(arrayNumberDirect))
+                logger.debug("matches ({}): store direct connections (dimension: {})".format(
+                    os.getpid(),numberDirectArray))
+                
+                #stats
+                totalChecks = 0
+                totalDirect = 0
+                totalCycle = 0
+                totalReversal = 0
                 
                 #define correct maxValues based on previous results             
-                dtype = [("cycle", [("number", haplotyping.index.Database.getUint(maximumFrequency)),
-                                    ("minimum", haplotyping.index.Database.getUint(
-                                                      2*estimatedMaximumReadLength))]),
-                         ("reversal", [("number", haplotyping.index.Database.getUint(maximumFrequency)),
-                                       ("minimum", haplotyping.index.Database.getUint(
-                                                      2*estimatedMaximumReadLength))]),
-                         ("direct", [("d"+str(i),[("type","uint8"),
-                                                  ("link",haplotyping.index.Database.getUint(numberOfKmers)),
-                                                  ("distance",haplotyping.index.Database.getUint(
-                                                      2*estimatedMaximumReadLength)),
-                                                  ("number",haplotyping.index.Database.getUint(maximumFrequency))]) 
-                                     for i in range(arrayNumberDirect)]),]
+                dtype = haplotyping.index.storage.Storage.worker_matches_dtype(
+                    numberOfKmers,maximumFrequency,estimatedMaximumReadLength,numberDirectArray)
                 connections = np.ndarray((numberOfKmers,), dtype=dtype, order="C")
-                connections.fill(((0,0,),(0,0,),tuple((0,0,0,0,) for i in range(arrayNumberDirect))))
+                connections.fill(((0,0,),(0,0,),tuple((0,0,0,0,) for i in range(numberDirectArray))))
                 
-                logger.debug("created memory storage for direct connections: {} MB".format(round(connections.nbytes/1048576)))
+                logger.debug("matches ({}): created memory storage for direct connections: {} MB".format(
+                    os.getpid(), math.ceil(connections.nbytes/1048576)))
+                
+                #store paired connections for partition graph
+                tablePaired = pytablesStorageWorker.create_table(pytablesStorageWorker.root, 
+                    "tmpPaired",{
+                    "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
+                    "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1),
+                }, "Temporary to dump paired relations", track_times=False)
                 
                 #define correct maxValues based on previous results
                 tableDirectOther = pytablesStorageWorker.create_table(pytablesStorageWorker.root, 
                     "directOther",{
                     "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
                     "fromDirection": tables.UInt8Col(pos=1),
                     "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,2),
                     "toDirection": tables.UInt8Col(pos=3),
                     "number": haplotyping.index.Database.getTablesUint(maximumFrequency,4),
                     "distance": haplotyping.index.Database.getTablesUint(2*estimatedMaximumReadLength,5),
                 }, "Temporary to dump other direct relations", track_times=False)
 
+                def store_paired(linkFrom, linkTo):
+                    if not linkFrom==linkTo:
+                        tablePaired.append([(linkFrom,linkTo,)])
+
                 def store_cycle(fromLink, distance):
                     (previousNumber,previousDistance,) = connections[fromLink][0]
                     if (previousDistance==0) or (distance<previousDistance):
                         connections[fromLink][0] = (previousNumber+1,distance,)
                     else:
                         connections[fromLink][0] = (previousNumber+1,previousDistance,)
 
@@ -340,26 +524,26 @@
                     (previousNumber,previousDistance,) = connections[fromLink][1]
                     if (previousDistance==0) or (distance<previousDistance):
                         connections[fromLink][1] = (previousNumber+1,distance,)
                     else:
                         connections[fromLink][1] = (previousNumber+1,previousDistance,)
 
                 def store_direct(fromLink, fromDirection, toLink, toDirection, distance):
-                    numberFilled = arrayNumberDirect
+                    numberFilled = numberDirectArray
                     connectionType = 1 + fromDirection + (2*toDirection)
                     directRow = connections[fromLink][2]
-                    for i in range(arrayNumberDirect):
+                    for i in range(numberDirectArray):
                         if directRow[i][0]==0:
                             numberFilled = i
                             break
                         elif (directRow[i][1]==toLink and directRow[i][0]==connectionType 
                               and directRow[i][2]==distance):
                             directRow[i][3]+=1 
                             return
-                    if numberFilled<arrayNumberDirect:
+                    if numberFilled<numberDirectArray:
                         directRow[numberFilled] = (connectionType,toLink,distance,1,)
                     else:
                         #try to smartly swap with other direct link
                         #doing this will increase the probability that only valid connections are stored
                         #in these arrays, and mainly invalid connections end up in the additional table
                         sameFromDirectionTypes = [1 + fromDirection + (2*x) for x in range(2)]
                         sameFromDirectionDistances = []
@@ -374,29 +558,29 @@
                                 sameFromDirectionEntries.append(i)
                             elif directRow[i][0]>0:
                                 otherFromDirectionDistances.append(directRow[i][2])
                                 otherFromDirectionEntries.append(i)
                             else:
                                 break
                         #too much in same direction
-                        if 2*len(sameFromDirectionDistances)>=arrayNumberDirect:
+                        if 2*len(sameFromDirectionDistances)>=numberDirectArray:
                             sameFromDirectionDistance = sorted(statistics.multimode(sameFromDirectionDistances))[0]
                             if distance==sameFromDirectionDistance:
                                 candidates=[]
                                 for i,d in zip(sameFromDirectionEntries,sameFromDirectionDistances):
                                     if not d==sameFromDirectionDistance:
                                         candidates.append(i)
                                 if len(candidates)>0:
                                     minimum = min([directRow[i][3] for i in candidates])
                                     for i in candidates:
                                         if directRow[i][3]==minimum:
                                             swapEntry = i
                                             break
                         #too much in other direction
-                        elif 2*len(otherFromDirectionDistances)>arrayNumberDirect:
+                        elif 2*len(otherFromDirectionDistances)>numberDirectArray:
                             otherFromDirectionDistance = sorted(statistics.multimode(otherFromDirectionDistances))[0]
                             candidates=[]
                             for i,d in zip(otherFromDirectionEntries,otherFromDirectionDistances):
                                 if not d==otherFromDirectionDistance:
                                     candidates.append(i)
                             if len(candidates)>0:
                                 minimum = min([directRow[i][3] for i in candidates])
@@ -418,20 +602,21 @@
                             dumpDirectRow["fromDirection"] = fromDirection
                             dumpDirectRow["toLink"] = toLink
                             dumpDirectRow["toDirection"] = toDirection
                             dumpDirectRow["number"] = 1
                             dumpDirectRow["distance"] = distance
                         dumpDirectRow.append()
 
-                def process_matches(matchesList):
+                def process_matches(matchesList,totalDirect,totalReversal,totalCycle,totalChecks):
                     history = {}
                     links = []
                     startPos = 0
                     endPos = 0
                     for matches in matchesList:
+                        totalChecks+=len(matches)
                         if len(matches)>0:
                             previousPos = matches[0][0]
                             previousLink = matches[0][1]
                             startPos = previousPos
                             #0: left, 1:right
                             previousDirection = (1 if matches[0][2]=="c" else 0)
                             links.append((previousLink,previousDirection))
@@ -446,405 +631,136 @@
                             for i in range(1,len(matches)):
                                 currentPos = matches[i][0]
                                 currentLink = matches[i][1]
                                 endPos = currentPos
                                 #0: left, 1:right
                                 currentDirection = (0 if matches[i][2]=="c" else 1)
                                 links.append((currentLink,currentDirection))
+                                totalDirect+=1
                                 store_direct(previousLink, previousDirection, 
                                              currentLink, currentDirection, currentPos-previousPos)
                                 store_direct(currentLink, currentDirection, 
                                              previousLink, previousDirection, currentPos-previousPos)
                                 previousPos = currentPos
                                 previousLink = currentLink
                                 previousDirection = (currentDirection+1)%2
                                 #cycles and reversals
                                 if currentLink in history.keys():
                                     if history[currentLink][0]==previousDirection:
+                                        totalCycle+=1
                                         store_cycle(currentLink,currentPos-history[currentLink][1])
                                     else:
+                                        totalReversal+=1
                                         store_reversal(currentLink,currentPos-history[currentLink][1])
                                 history[previousLink]=(previousDirection,previousPos,)
-                    return (links,max(0,endPos-startPos),)
+                    return (links,max(0,endPos-startPos),totalDirect,totalReversal,totalCycle,totalChecks,)
 
+                process = psutil.Process(os.getpid())
+                logger.debug("matches ({}): used memory {} MB".format(
+                    os.getpid(),math.ceil(process.memory_info().rss/1048576)))
+                
+                shm = shared_memory.SharedMemory(shm_name)
+                logger.debug("matches ({}): shared memory of {} MB used".format(os.getpid(),math.ceil(shm.size/1048576)))
+                
+                #get shared memory
+                shm_kmer_link = np.dtype(haplotyping.index.Database.getUint(numberOfKmers)).type
+                shm_kmer_number = np.dtype(haplotyping.index.Database.getUint(maximumFrequency)).type
+                kmer_properties = np.ndarray((numberOfKmers,), dtype=[("type","S1"),("number",shm_kmer_number),
+                                       ("left",shm_kmer_link),("right",shm_kmer_link)], buffer=shm.buf)
+        
                 while not shutdown_event.is_set():
                     try:
                         item = queue_matches.get(block=True, timeout=1)
                         if item==None:
+                            logger.debug("matches ({}): none".format(os.getpid()))
                             break
                         elif isinstance(item,tuple):
                             if len(item)==1:
                                 matchesList = item[0][0]
                                 directConnected = item[0][1]
-                                (links,length,) = process_matches(matchesList)
-                                if len(links)>2:
-                                    queue_connections.put(((links,length,directConnected,)))
+                                (links,length,totalDirect,totalReversal,totalCycle,totalChecks,) = process_matches(
+                                    matchesList,totalDirect,totalReversal,totalCycle,totalChecks)
                             elif len(item)==2:
                                 matchesList0 = item[0][0]
                                 directConnected0 = item[0][1]
                                 matchesList1 = item[1][0]
                                 directConnected1 = item[1][1]
-                                (links0,length0,) = process_matches(matchesList0)
-                                (links1,length1,) = process_matches(matchesList1)
-                                if len(links0)==0:
-                                    if len(links1)>2:
-                                        queue_connections.put(((links1,length1,directConnected1,)))
-                                elif len(links1)==0:
-                                    if len(links0)>2:
-                                        queue_connections.put(((links0,length0,directConnected0,)))
-                                else:
-                                    queue_connections.put((
-                                        (links0,length0,directConnected0,),
-                                        (links1,length1,directConnected1,),
-                                    ))
+                                (links0,length0,totalDirect,totalReversal,totalCycle,totalChecks,) = process_matches(
+                                    matchesList0,totalDirect,totalReversal,totalCycle,totalChecks)
+                                (links1,length1,totalDirect,totalReversal,totalCycle,totalChecks,) = process_matches(
+                                    matchesList1,totalDirect,totalReversal,totalCycle,totalChecks)
+                                #register pair data for single matches
+                                if (len(links0)==1) and (len(links1)>0):
+                                    pairFrom = links0[0][0]
+                                    minFreq = 0
+                                    for link in links1:
+                                        freq = kmer_properties[link[0]][1]
+                                        if freq==minFreq:
+                                            pairTo = min(pairTo,link[0])
+                                        elif minFreq==0 or freq<minFreq:
+                                            minFreq = freq
+                                            pairTo = link[0]
+                                    if not onlyDirectConnections:
+                                        store_paired(pairFrom,pairTo)
+                                if (len(links1)==1) and (len(links0)>0):
+                                    pairFrom = links1[0][0]
+                                    minFreq = 0
+                                    for link in links0:
+                                        freq = kmer_properties[link[0]][1]
+                                        if freq==minFreq:
+                                            pairTo = min(pairTo,link[0])
+                                        elif minFreq==0 or freq<minFreq:
+                                            minFreq = freq
+                                            pairTo = link[0]
+                                    if not onlyDirectConnections and (len(links0)>1):
+                                        store_paired(pairFrom,pairTo)
                     except Empty:
+                        logger.debug("matches ({}): empty".format(os.getpid()))
+                        time.sleep(5)
                         continue   
                 pytablesStorageWorker.flush()
+                logger.debug("matches ({}): create indices temporary tables".format(os.getpid()))
                 tableDirectOther.cols.fromLink.create_csindex()
                 pytablesStorageWorker.flush()
+                if not onlyDirectConnections:
+                    tablePaired.cols.fromLink.create_csindex()
+                    pytablesStorageWorker.flush()
                 pytablesStorageWorker.create_table(pytablesStorageWorker.root, 
                                               name="direct", obj=connections, expectedrows=numberOfKmers)
-                logger.debug("matches: memory storage saved, other connections indexed")
+                logger.debug("matches ({}): found {} direct, {} cycle and {} reversal in {} matches".format(
+                    os.getpid(), totalDirect,totalCycle,totalReversal,totalChecks))
                 pytablesStorageWorker.flush()
                 
             #now the file can be released for merge
             queue_storage.put(pytablesFileWorker) 
+        except Exception as ex:
+           logger.error("matches ({}): problem with worker: {}".format(os.getpid(), ex))
         finally:
             pass
-        queue_finished.put("matches")
-            
-    """
-    Process indirect connections: filtering and efficient storage
-    """
-    def worker_connections(shutdown_event,queue_connections,queue_storage,queue_finished,
-                       filenameBase,numberOfKmers,arrayNumberConnection,maximumFrequency,shm_name):
-        
-        logger = logging.getLogger(__name__)
-        
-        shm = shared_memory.SharedMemory(shm_name)
-        logger.debug("connections: shared memory of {} MB used".format(round(shm.size/1048576)))
-            
-        try:
-            curr_proc = current_process()
-            pytablesFileWorker = filenameBase+"_tmp_connections_"+str(curr_proc.name)+".process.h5"
-            if os.path.exists(pytablesFileWorker):
-                os.remove(pytablesFileWorker)
-
-            with tables.open_file(pytablesFileWorker, mode="a") as pytablesStorageWorker:
-                
-                logger.debug("connections: store additional connections (dimension: {})".format(arrayNumberConnection))
-
-                #connections - define correct maxValues based on previous results             
-                dtype = [("number", haplotyping.index.Database.getUint(arrayNumberConnection+1)),
-                         ("connections", [("c"+str(i),[
-                                                        ("link",haplotyping.index.Database.getUint(numberOfKmers)),
-                                                        ("length",haplotyping.index.Database.getUint(arrayNumberConnection)),
-                                                        ("direct","uint8"),
-                                                        ("hash","int64"),
-                                                        ("number",haplotyping.index.Database.getUint(maximumFrequency))
-                                                      ]) 
-                                                      for i in range(arrayNumberConnection)])]
-                connections = np.ndarray((numberOfKmers,), dtype=dtype, order="C")
-                connections.fill((0,tuple((0,0,0,0,0,) for i in range(arrayNumberConnection))))
-                
-                #paired entries - define correct maxValues based on previous results   
-                #can't however really estimate the required size because this depends 
-                #on the (unknown) distance between paired reads
-                dtype = [("number", haplotyping.index.Database.getUint(arrayNumberConnection+1)),
-                         ("paired", [("p"+str(i),[("link",haplotyping.index.Database.getUint(numberOfKmers)),
-                                                  ("number",haplotyping.index.Database.getUint(maximumFrequency))]) 
-                                     for i in range(arrayNumberConnection)]),]
-                paired = np.ndarray((numberOfKmers,), dtype=dtype, order="C")
-                paired.fill((0,tuple((0,0,) for i in range(arrayNumberConnection))))
-                
-                logger.debug("created memory storage for additional connections: {} MB".format(
-                    round(connections.nbytes/1048576)))
-                logger.debug("created memory storage for paired entries: {} MB".format(
-                    round(paired.nbytes/1048576)))
-                
-                #define correct maxValues based on previous results
-                tablePairedOther = pytablesStorageWorker.create_table(pytablesStorageWorker.root, 
-                    "pairedOther",{
-                    "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
-                    "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1)
-                }, "Temporary to dump other paired relations", track_times=False)
-                
-                mapSplitDirection = [{b"l":"l", b"r":"r", b"b":"b"},{b"l":"r", b"r":"l", b"b":"b"}]
-                
-                def store_connections(connectionsList,direct,tableConnectionsData,tableConnectionsDataNumber):
-                    #compact pairs with equal dosage
-                    compactedConnectionsList = []
-                    for id, (link,direction) in enumerate(connectionsList):
-                        props = kmer_properties[link] 
-                        newEntry = (link,mapSplitDirection[direction][props[0]],props[1],id,)
-                        #contract pairs with equal dosage (rightsplitter -> leftsplitter)                        
-                        if (newEntry[1]=="l" and (len(compactedConnectionsList)>0) and 
-                            compactedConnectionsList[-1][1]=="r"):
-                            compactedConnectionsList[-1] = (compactedConnectionsList[-1],newEntry,)
-                        else:
-                            compactedConnectionsList.append(newEntry)
-                    #select entries with (potential) minimal dosage
-                    potentialDirection = None
-                    potentialId = None
-                    compactedSelection = [] 
-                    # entry: [ link, splitType, frequency, #id connectionsList]
-                    for id,entry in enumerate(compactedConnectionsList):
-                        newDirection = entry[0][1] if len(entry)==2 else entry[1]
-                        if potentialId==None:
-                            potentialDirection = entry[-1][1] if len(entry)==2 else entry[1]
-                            potentialId = id
-                        else:
-                            if potentialDirection=="l":
-                                if newDirection=="l":
-                                    pass
-                                else:
-                                    compactedSelection.append(potentialId)
-                                    potentialDirection = entry[-1][1] if len(entry)==2 else entry[1]
-                                    potentialId = id
-                            elif potentialDirection=="r":
-                                if newDirection=="l":
-                                    raise Exception("can't happen")
-                                else:
-                                    potentialDirection = entry[-1][1] if len(entry)==2 else entry[1]
-                                    potentialId = id
-                            else:
-                                if newDirection=="l":
-                                    pass
-                                else:
-                                    compactedSelection.append(potentialId)
-                                    potentialDirection = entry[-1][1] if len(entry)==2 else entry[1]
-                                    potentialId = id
-                    if not potentialId==None:
-                        compactedSelection.append(potentialId)
-                    #compute final selection and linking entry
-                    finalSelection = []
-                    linkingId = None
-                    linkingNumber = None
-                    def recompute_linking_entry(linkingId,linkingNumber,newId,newNumber):
-                        if linkingId==None or linkingNumber>newNumber:
-                            linkingId = newId
-                            linkingNumber = newNumber
-                        elif linkingNumber==newNumber:
-                            if connectionsList[linkingId][0]>connectionsList[newId][0]:
-                                linkingId = newId
-                                linkingNumber = newNumber
-                        return (linkingId,linkingNumber,)
-                    
-                    for id in compactedSelection:
-                        if len(compactedConnectionsList[id])==2:
-                            if id==0:
-                                finalSelection.append(compactedConnectionsList[id][1][-1])
-                                (linkingId,linkingNumber) = recompute_linking_entry(linkingId,linkingNumber,
-                                                                compactedConnectionsList[id][1][-1],
-                                                                compactedConnectionsList[id][1][2])
-                            elif id==len(compactedConnectionsList)-1:
-                                finalSelection.append(compactedConnectionsList[id][0][-1])
-                                (linkingId,linkingNumber) = recompute_linking_entry(linkingId,linkingNumber,
-                                                                compactedConnectionsList[id][0][-1],
-                                                                compactedConnectionsList[id][0][2])
-                            else:
-                                if compactedConnectionsList[id][0][2]>compactedConnectionsList[id][1][2]:
-                                    finalSelection.append(compactedConnectionsList[id][0][-1])
-                                    (linkingId,linkingNumber) = recompute_linking_entry(linkingId,linkingNumber,
-                                                                compactedConnectionsList[id][0][-1],
-                                                                compactedConnectionsList[id][0][2])
-                                elif compactedConnectionsList[id][1][2]>compactedConnectionsList[id][0][2]:
-                                    finalSelection.append(compactedConnectionsList[id][1][-1])
-                                    (linkingId,linkingNumber) = recompute_linking_entry(linkingId,linkingNumber,
-                                                                compactedConnectionsList[id][1][-1],
-                                                                compactedConnectionsList[id][1][2])
-                                elif compactedConnectionsList[id][0][0]>compactedConnectionsList[id][1][0]:
-                                    finalSelection.append(compactedConnectionsList[id][0][-1])
-                                    (linkingId,linkingNumber) = recompute_linking_entry(linkingId,linkingNumber,
-                                                                compactedConnectionsList[id][0][-1],
-                                                                compactedConnectionsList[id][0][2])
-                                else:
-                                    finalSelection.append(compactedConnectionsList[id][1][-1])
-                                    (linkingId,linkingNumber) = recompute_linking_entry(linkingId,linkingNumber,
-                                                                compactedConnectionsList[id][1][-1],
-                                                                compactedConnectionsList[id][1][2])
-                        else:
-                            finalSelection.append(compactedConnectionsList[id][-1])
-                            (linkingId,linkingNumber) = recompute_linking_entry(linkingId,linkingNumber,
-                                                                compactedConnectionsList[id][-1],
-                                                                compactedConnectionsList[id][2])
-
-                    linkingConnectedKmer = None
-                    
-                    #single entry not informative
-                    if len(compactedSelection)<=1:
-                        pass
-                    #directly neighhbouring entries not informative
-                    elif len(compactedSelection)==2 and (compactedSelection[1]-compactedSelection[0])==1:
-                        pass
-                    elif len(finalSelection)>0:
-                        #get final list of connected k-mers
-                        connectedKmers = [connectionsList[id][0] for id in finalSelection]
-                        linkingConnectedKmer = connectionsList[linkingId][0]
-                        assert linkingConnectedKmer in connectedKmers
-                        #remove neighbouring duplicates
-                        connectedKmers = sorted(set(connectedKmers), key=connectedKmers.index)
-                        #always sorted in same direction
-                        if connectedKmers[0]>connectedKmers[-1]:
-                            connectedKmers = tuple(connectedKmers[::-1])
-                        else:
-                            connectedKmers = tuple(connectedKmers)
-                        connectionsRow = connections[linkingConnectedKmer]
-                        #don't store if too much k-mers are involved or if non-informative
-                        if connectionsRow[0]>arrayNumberConnection or len(connectedKmers)<=1:
-                            pass
-                        else:
-                            lengthValue = len(connectedKmers)
-                            directValue = 1 if direct else 0
-                            hashValue = hash(connectedKmers)
-                            stored = False
-                            #check hash-based if already stored
-                            for i in range(connectionsRow[0]):
-                                if connectionsRow[1][i][3] == hashValue:                                    
-                                    if connectionsRow[1][i][1] == lengthValue:                                        
-                                        connectionsRow[1][i][2] == max(directValue,connectionsRow[1][i][2])
-                                        connectionsRow[1][i][4] += 1    
-                                        stored = True
-                                    else:
-                                        #conflict
-                                        connectionsRow[0] = arrayNumberConnection+1
-                                        for j in range(connectionsRow[0]):
-                                            connectionsRow[1][j] = (0,0,0,0,0,)
-                                    break
-                            if not stored and connectionsRow[0]<=arrayNumberConnection:
-                                if connectionsRow[0]<arrayNumberConnection:
-                                    linkValue = tableConnectionsDataNumber
-                                    tableConnectionsData.append(connectedKmers)
-                                    tableConnectionsDataNumber+=len(connectedKmers)
-                                    connectionsRow[1][connectionsRow[0]] = (linkValue,lengthValue,
-                                                                            directValue,hashValue,1,)
-                                    connectionsRow[0]+=1
-                                    stored = True
-                                else:
-                                    #no space to store, reset all
-                                    for j in range(connectionsRow[0]):
-                                        connectionsRow[1][j] = (0,0,0,0,0,)
-                                    connectionsRow[0] = arrayNumberConnection+1
-                                    
-                            #store (in memory)
-                            connections[linkingConnectedKmer] = connectionsRow
-                            
-                    return (tableConnectionsDataNumber,linkingConnectedKmer)
-                
-                def store_paired(linkedCkmer0,linkedCkmer1):
-                    #only store if potentially necessary
-                    if linkedCkmer0==linkedCkmer1:
-                        pass
-                    elif connections[linkedCkmer0][0]>arrayNumberConnection:
-                        pass
-                    elif connections[linkedCkmer1][0]>arrayNumberConnection:
-                        pass
-                    else:
-                        pairedRow = paired[linkedCkmer0]
-                        stored = False
-                        for i in range(pairedRow[0]):
-                            if pairedRow[1][i][0] == linkedCkmer1:                                    
-                                pairedRow[1][i][1] += 1    
-                                stored = True                                
-                        if not stored:
-                            if pairedRow[0]<arrayNumberConnection:
-                                pairedRow[1][pairedRow[0]] = (linkedCkmer1,1,)
-                                pairedRow[0]+=1                                
-                            else:
-                                dumpPairedRow = tablePairedOther.row
-                                dumpPairedRow["fromLink"] = linkedCkmer0
-                                dumpPairedRow["toLink"] = linkedCkmer1
-                                dumpPairedRow.append()
-                        #store (in memory)
-                        paired[linkedCkmer0] = pairedRow
-                    
-                #get shared memory
-                shm_kmer_link = np.dtype(haplotyping.index.Database.getUint(numberOfKmers)).type
-                shm_kmer_number = np.dtype(haplotyping.index.Database.getUint(maximumFrequency)).type
-                kmer_properties = np.ndarray((numberOfKmers,), dtype=[("type","S1"),("number",shm_kmer_number),
-                                   ("left",shm_kmer_link),("right",shm_kmer_link)], buffer=shm.buf)
+        queue_finished.put("matches:ended")
             
-                tableConnectionsData = pytablesStorageWorker.create_earray(pytablesStorageWorker.root, "data", 
-                               haplotyping.index.Database.getTablesUintAtom(numberOfKmers), (0,), "Data")
-                tableConnectionsDataNumber = 0
-
-                while not shutdown_event.is_set():
-                    try:
-                        item = queue_connections.get(block=True, timeout=1)
-                        if item==None:
-                            break
-                        elif isinstance(item,tuple):
-                            if len(item)==1:
-                                if len(item[0][0])>2:
-                                    tableConnectionsDataNumber = store_connections(
-                                                      item[0][0],item[0][2],
-                                                      tableConnectionsData,tableConnectionsDataNumber)[0]
-                            elif len(item)==2:
-                                if len(item[0][0])==0:
-                                    if len(item[1][0])>0:
-                                        tableConnectionsDataNumber = store_connections(
-                                                      item[1][0],item[1][2],
-                                                      tableConnectionsData,tableConnectionsDataNumber)[0]
-                                elif len(item[1][0])==0:
-                                    if len(item[0][0])>0:
-                                        tableConnectionsDataNumber = store_connections(
-                                                      item[0][0],item[0][2],
-                                                      tableConnectionsData,tableConnectionsDataNumber)[0]
-                                else:
-                                    (tableConnectionsDataNumber,linkedCkmer0) = store_connections(
-                                                      item[0][0],item[0][2],
-                                                      tableConnectionsData,tableConnectionsDataNumber)
-                                    (tableConnectionsDataNumber,linkedCkmer1) = store_connections(
-                                                      item[1][0],item[1][2],
-                                                      tableConnectionsData,tableConnectionsDataNumber)
-                                    #store paired connections
-                                    if not (linkedCkmer0==None or linkedCkmer1==None):
-                                        store_paired(linkedCkmer0,linkedCkmer1)
-                                        store_paired(linkedCkmer1,linkedCkmer0)
-                    except Empty:
-                        continue   
-                
-                pytablesStorageWorker.flush()                
-                tablePairedOther.cols.fromLink.create_csindex()
-                pytablesStorageWorker.flush()                
-                pytablesStorageWorker.create_table(pytablesStorageWorker.root, 
-                    name="connections", obj=connections, expectedrows=numberOfKmers)
-                logger.debug("matches: memory storage connections saved")
-                pytablesStorageWorker.flush()
-                pytablesStorageWorker.create_table(pytablesStorageWorker.root, 
-                    name="paired", obj=paired, expectedrows=numberOfKmers)
-                logger.debug("matches: memory storage paired saved")
-                pytablesStorageWorker.flush()
-                
-            #now the file can be released for merge
-            queue_storage.put(pytablesFileWorker) 
-        finally:
-            shm.close()
-            logger.debug("index: shared memory released")
-
-        queue_finished.put("connections")
                 
-            
     """
     Merge stored direct and indirect connections
     """                
-    def worker_merges(shutdown_event,queue_ranges,queue_merges,storageDirectFiles,storageConnectionFiles,
-                      filenameBase,numberOfKmers,maximumFrequency,minimumFrequency,maximumConnectionLength,shm_name):
+    def worker_mergeDirect(shutdown_event,queue_ranges,queue_merges,storageDirectFiles,
+                      filenameBase,numberOfKmers,maximumFrequency,minimumFrequency,shm_name):
         
-        logger = logging.getLogger(__name__)
+        logger = logging.getLogger("{}.worker.merges".format(__name__))
 
         def merge_direct_storage(pytablesFileWorker, storageDirectFiles, mergeStart, mergeNumber, 
                                  numberOfKmers, kmer_properties):
 
             with tables.open_file(pytablesFileWorker, mode="a") as pytablesStorageWorker:
                 tableCycle = pytablesStorageWorker.root.cycle
                 tableReversal = pytablesStorageWorker.root.reversal
                 tableDirect = pytablesStorageWorker.root.direct
                 tableDeleteDirect = pytablesStorageWorker.root.deleteDirect                
-
+                tablePaired = pytablesStorageWorker.root.tmpPaired
+                
                 with ExitStack() as stack:
                     #get handlers
                     storageHandlers = [{"handler": stack.enter_context(tables.open_file(fname, mode="r"))} 
                                                for fname in storageDirectFiles]
                     
                     #get and position sorted iterators for other entries
                     for i in range(len(storageHandlers)):
@@ -855,14 +771,27 @@
                             for row in storageHandlers[i]["otherIterator"]:
                                 if row["fromLink"]>=mergeStart:
                                     if row["fromLink"]<=mergeEnd:
                                         storageHandlers[i]["otherRow"] = row
                                     break
                         else:
                             storageHandlers[i]["otherIterator"] = None
+                    #get and position sorted iterators for paired entries
+                    for i in range(len(storageHandlers)):
+                        storageHandlers[i]["pairedRow"] = None
+                        if storageHandlers[i]["handler"].root.tmpPaired.shape[0]>0:
+                            storageHandlers[i]["pairedIterator"] = storageHandlers[i]["handler"].root.tmpPaired.itersorted(
+                                "fromLink",checkCSI=True)
+                            for row in storageHandlers[i]["pairedIterator"]:
+                                if row["fromLink"]>=mergeStart:
+                                    if row["fromLink"]<=mergeEnd:
+                                        storageHandlers[i]["pairedRow"] = row
+                                    break
+                        else:
+                            storageHandlers[i]["pairedIterator"] = None
                     
                     #direct connections
                     def add_directData(directDataEntry,fromDirection,toLink,toDirection,distance,number):
                         if not fromDirection in directDataEntry.keys():
                             directDataEntry[fromDirection] = {}
                         if not distance in directDataEntry[fromDirection].keys():
                             directDataEntry[fromDirection][distance] = {}
@@ -1112,22 +1041,21 @@
                                 raise Exception("this should not happen")
                         else:
                             #not enough relevant connections
                             distanceData = set_problematic(distanceData,1)
                         #return
                         return distanceData
                     
-                    stepSizeStorage = 10000
-                    for i in range(mergeStart,mergeEnd+1,stepSizeStorage):
+                    for i in range(mergeStart,mergeEnd+1,Storage.stepSizeStorage):
                         #initialise
                         cycleEntries = {}
                         reversalEntries = {}
-                        directData = [{} for j in range(min(mergeEnd+1-i,stepSizeStorage,(numberOfKmers-i)))]
+                        directData = [{} for j in range(min(mergeEnd+1-i,Storage.stepSizeStorage,(numberOfKmers-i)))]
                         for storageHandler in storageHandlers:
-                            rowData = storageHandler["handler"].root.direct[i:min(mergeEnd+1,i+stepSizeStorage)]
+                            rowData = storageHandler["handler"].root.direct[i:min(mergeEnd+1,i+Storage.stepSizeStorage)]
                             for index, item in enumerate(rowData):
                                 fromLink = i + index
                                 #get and process regular data
                                 for k in range(len(item[2])):
                                     if item[2][k][0]==0:
                                         break
                                     else:
@@ -1197,365 +1125,581 @@
                         for ce in reversalEntries.keys():
                             tableReversalRow = tableReversal.row
                             tableReversalRow["ckmerLink"] = i+ce
                             tableReversalRow["number"] = min(maximumFrequency,reversalEntries[ce][0])
                             tableReversalRow["minimumLength"] = reversalEntries[ce][1]
                             tableReversalRow.append()
                         
+                        unlinkedEntries = []
                         for j in range(len(directData)):
                             fromLink = i + j
-                            for fromDirection in directData[j].keys():
-                                directData[j][fromDirection]= reduceDistances(fromLink,fromDirection, 
-                                                                              directData[j][fromDirection])
-                                #check for multiple distances (inconsistent)
-                                multipleDistances = 1 if not len(directData[j][fromDirection])==1 else 0
-                                for distance in directData[j][fromDirection].keys():
-                                    dataEntry = directData[j][fromDirection][distance]
-                                    for toLink in dataEntry.keys():
-                                        for toDirection in dataEntry[toLink].keys():
-                                            number = dataEntry[toLink][toDirection]["number"]
-                                            problematic = dataEntry[toLink][toDirection]["problematic"]
-                                            direction = dataEntry[toLink][toDirection]["direction"]
-                                            if direction in ["r","b"]:
-                                                reverseBase = dataEntry[toLink][toDirection]["reverseBase"]
-                                            else:
-                                                reverseBase = 0
-                                            if direction in ["f","b"]:
-                                                forwardBase = dataEntry[toLink][toDirection]["forwardBase"]
+                            if len(directData[j])==0:
+                                unlinkedEntries.append(fromLink)
+                            else:
+                                for fromDirection in directData[j].keys():
+                                    directData[j][fromDirection] = reduceDistances(fromLink,fromDirection, 
+                                                                                  directData[j][fromDirection])
+                                    #check for multiple distances (inconsistent)
+                                    multipleDistances = 1 if not len(directData[j][fromDirection])==1 else 0
+                                    for distance in directData[j][fromDirection].keys():
+                                        dataEntry = directData[j][fromDirection][distance]
+                                        for toLink in dataEntry.keys():
+                                            for toDirection in dataEntry[toLink].keys():
+                                                number = dataEntry[toLink][toDirection]["number"]
+                                                problematic = dataEntry[toLink][toDirection]["problematic"]
+                                                direction = dataEntry[toLink][toDirection]["direction"]
+                                                if direction in ["r","b"]:
+                                                    reverseBase = dataEntry[toLink][toDirection]["reverseBase"]
+                                                else:
+                                                    reverseBase = 0
+                                                if direction in ["f","b"]:
+                                                    forwardBase = dataEntry[toLink][toDirection]["forwardBase"]
+                                                else:
+                                                    forwardBase = 0
+                                                tableDirectRow = tableDirect.row
+                                                tableDirectRow["fromLink"] = fromLink
+                                                tableDirectRow["fromDirection"] = "l" if fromDirection==0 else "r"
+                                                tableDirectRow["toLink"] = toLink
+                                                tableDirectRow["toDirection"] = "l" if toDirection==0 else "r"
+                                                tableDirectRow["number"] = min(maximumFrequency,number)
+                                                tableDirectRow["distance"] = distance
+                                                tableDirectRow["splitDirection"] = direction
+                                                tableDirectRow["reverseBase"] = reverseBase
+                                                tableDirectRow["forwardBase"] = forwardBase
+                                                tableDirectRow["problematic"] = multipleDistances + (problematic<<1)
+                                                tableDirectRow.append()
+
+                        #store paired data for not directly connected entries
+                        if (len(unlinkedEntries)>0):
+                            for storageHandler in storageHandlers:
+                                if not storageHandler["pairedRow"]==None:
+                                    try:
+                                        unlinkedIterator = iter(unlinkedEntries)
+                                        paired = storageHandler["pairedRow"]
+                                        unlinked = next(unlinkedIterator)
+                                        while True:
+                                            if paired[0] > unlinked:
+                                                unlinked = next(unlinkedIterator)
                                             else:
-                                                forwardBase = 0
-                                            tableDirectRow = tableDirect.row
-                                            tableDirectRow["fromLink"] = fromLink
-                                            tableDirectRow["fromDirection"] = "l" if fromDirection==0 else "r"
-                                            tableDirectRow["toLink"] = toLink
-                                            tableDirectRow["toDirection"] = "l" if toDirection==0 else "r"
-                                            tableDirectRow["number"] = min(maximumFrequency,number)
-                                            tableDirectRow["distance"] = distance
-                                            tableDirectRow["splitDirection"] = direction
-                                            tableDirectRow["reverseBase"] = reverseBase
-                                            tableDirectRow["forwardBase"] = forwardBase
-                                            tableDirectRow["problematic"] = multipleDistances + (problematic<<1)
-                                            tableDirectRow.append()
-
-                #finished
-                pytablesStorageWorker.flush()
-                
-        def merge_connection_storage(pytablesFileWorker, storageConnectionFiles, mergeStart, mergeNumber, 
-                                 numberOfKmers, maximumConnectionLength):
+                                                if paired[0] == unlinked:     
+                                                    tablePaired.append([(paired[0],paired[1],)])
+                                                paired = next(storageHandler["pairedIterator"])
+                                    except StopIteration:
+                                        pass                           
 
-            with tables.open_file(pytablesFileWorker, mode="a") as pytablesStorageWorker:
-                tableConnections = pytablesStorageWorker.root.connections
-                tableData = pytablesStorageWorker.root.data
-                tablePaired = pytablesStorageWorker.root.paired
-                tableDeletePaired = pytablesStorageWorker.root.deletePaired
-                tableDataCounter = 0
-                
-                with ExitStack() as stack:
-                    #get handlers
-                    storageHandlers = [{"handler": stack.enter_context(tables.open_file(fname, mode="r"))} 
-                                               for fname in storageConnectionFiles]
-                    
-                    #get and position sorted iterators for other entries
-                    for i in range(len(storageHandlers)):
-                        storageHandlers[i]["otherRow"] = None
-                        if storageHandlers[i]["handler"].root.pairedOther.shape[0]>0:
-                            storageHandlers[i]["otherIterator"] = storageHandlers[i]["handler"].root.pairedOther.itersorted(
-                                "fromLink",checkCSI=True)
-                            for row in storageHandlers[i]["otherIterator"]:
-                                if row["fromLink"]>=mergeStart:
-                                    if row["fromLink"]<=mergeEnd:
-                                        storageHandlers[i]["otherRow"] = row
-                                    break
-                        else:
-                            storageHandlers[i]["otherIterator"] = None
-                    
-                    #add connections
-                    def add_connectionData(connectionDataEntry,length,direct,hashValue,number):
-                        if not hashValue in connectionDataEntry[1].keys():
-                            connectionDataEntry[1][hashValue] = {"status": True, "length": length, 
-                                                                 "direct": direct, "number": number}
-                            connectionDataEntry[0]+=1
-                            storeData = True
-                        elif not connectionDataEntry[1][hashValue]["length"]==length:
-                            connectionDataEntry[1][hashValue]["status"] = False
-                            storeData = False
-                        else:
-                            connectionDataEntry[1][hashValue]["number"] += number  
-                            connectionDataEntry[1][hashValue]["direct"] = max(direct,
-                                                      connectionDataEntry[1][hashValue]["direct"])
-                            storeData = False
-                        return (connectionDataEntry,storeData,)
-                    
-                    stepSizeStorage = 10000
-                    for i in range(mergeStart,mergeEnd+1,stepSizeStorage):
-                        #initialise
-                        connectionData = [[0,{}] for j in range(min(mergeEnd+1-i,stepSizeStorage,(numberOfKmers-i)))]
-                        for storageHandler in storageHandlers:
-                            rowData = storageHandler["handler"].root.connections[i:min(mergeEnd+1,i+stepSizeStorage)]
-                            for index, item in enumerate(rowData):
-                                fromLink = i + index
-                                if item[0]>maximumConnectionLength:
-                                    break
-                                else:
-                                    for k in range(min(item[0],len(item[1]))):
-                                        lengthValue = item[1][k][1]
-                                        directValue = item[1][k][2]
-                                        hashValue = item[1][k][3]
-                                        numberValue = item[1][k][4]
-                                        (connectionData[index],storeData) = add_connectionData(connectionData[index],
-                                                                            lengthValue,directValue,
-                                                                            hashValue,numberValue)
-                                        if storeData:
-                                            linkValue = item[1][k][0]
-                                            linkData = storageHandler["handler"].root.data[linkValue:linkValue+lengthValue]
-                                            connectionData[index][1][hashValue]["data"] = linkData
-                        for j in range(len(connectionData)):
-                            fromLink = i + j
-                            if connectionData[j][0]<=maximumConnectionLength:
-                                for hashValue in connectionData[j][1].keys():
-                                    entry = connectionData[j][1][hashValue]
-                                    if entry["status"]:
-                                        tableConnectionsRow = tableConnections.row
-                                        tableConnectionsRow["ckmerLink"] = fromLink
-                                        tableConnectionsRow["dataLink"] = tableDataCounter
-                                        tableConnectionsRow["length"] = entry["length"]
-                                        tableConnectionsRow["number"] = entry["number"]
-                                        tableConnectionsRow["direct"] = entry["direct"]
-                                        tableConnectionsRow.append()
-                                        tableData.append(entry["data"])
-                                        tableDataCounter+=len(entry["data"])
-                                        
-                        #initialise
-                        pairedData = [{} for j in range(min(mergeEnd+1-i,stepSizeStorage,(numberOfKmers-i)))]
-                        for storageHandler in storageHandlers:
-                            rowData = storageHandler["handler"].root.paired[i:min(mergeEnd+1,i+stepSizeStorage)]
-                            for index, item in enumerate(rowData):
-                                fromLink = i + index
-                                for j in range(item[0]):
-                                    toLink = item[1][j][0]
-                                    number = item[1][j][1]
-                                    pairedData[index][toLink] = pairedData[index].get(toLink,0)+number
-                                    
-                                #now check other data
-                                if storageHandler["otherRow"]:
-                                    if storageHandler["otherRow"]["fromLink"]<fromLink:
-                                        storageHandler["otherRow"] = None
-                                        for row in storageHandler["otherIterator"]:
-                                            if row["fromLink"]>=fromLink:
-                                                if row["fromLink"]<=mergeEnd:
-                                                    storageHandler["otherRow"] = row
-                                                break
-                                    if storageHandler["otherRow"] and storageHandler["otherRow"]["fromLink"]==fromLink:
-                                        toLink = storageHandler["otherRow"]["toLink"]
-                                        pairedData[index][toLink] = pairedData[index].get(toLink,0)+1
-                                        for row in storageHandler["otherIterator"]:
-                                            if row["fromLink"]==fromLink:
-                                                storageHandler["otherRow"] = row
-                                                toLink = storageHandler["otherRow"]["toLink"]
-                                                pairedData[index][toLink] = pairedData[index].get(toLink,0)+1
-                                            elif row["fromLink"]<=mergeEnd:
-                                                storageHandler["otherRow"] = row
-                                                break
-                                            else:
-                                                storageHandler["otherRow"] = None
-                                                break
-                                
-                        for j in range(len(pairedData)):
-                            fromLink = i + j
-                            if len(pairedData[j])>maximumConnectionLength:
-                                for toLink in pairedData[j].keys():
-                                    tableDeletePairedRow = tableDeletePaired.row
-                                    tableDeletePairedRow["fromLink"] = toLink
-                                    tableDeletePairedRow["toLink"] = fromLink
-                                    tableDeletePairedRow.append()
-                            else:
-                                for toLink in pairedData[j].keys():
-                                    number = pairedData[j][toLink]
-                                    tablePairedRow = tablePaired.row
-                                    tablePairedRow["fromLink"] = fromLink
-                                    tablePairedRow["toLink"] = toLink
-                                    tablePairedRow["number"] = number
-                                    tablePairedRow.append()          
-                                    
                 #finished
                 pytablesStorageWorker.flush()
                 
+                        
                 
         shm = shared_memory.SharedMemory(shm_name)
-        logger.debug("merges: shared memory of {} MB used".format(round(shm.size/1048576)))
+        logger.debug("merges ({}): shared memory of {} MB used".format(os.getpid(),math.ceil(shm.size/1048576)))
         try:
             #get shared memory
             shm_kmer_link = np.dtype(haplotyping.index.Database.getUint(numberOfKmers)).type
             shm_kmer_number = np.dtype(haplotyping.index.Database.getUint(maximumFrequency)).type
             kmer_properties = np.ndarray((numberOfKmers,), dtype=[("type","S1"),("number",shm_kmer_number),
                                ("left",shm_kmer_link),("right",shm_kmer_link)], buffer=shm.buf)
+            
+            process = psutil.Process(os.getpid())
+            logger.debug("merges ({}): used memory {} MB".format(
+                os.getpid(),math.ceil(process.memory_info().rss/1048576)))
+            
             #handle queue
             while not shutdown_event.is_set():
                 try:
                     item = queue_ranges.get(block=True, timeout=1)
                     if item==None:
                         break
                     elif isinstance(item,tuple):
                         mergeStart = item[0]
                         mergeNumber = item[1]
                         #create storage
                         numberLength = len(str(numberOfKmers))
                         mergeEnd = min(numberOfKmers,mergeStart+mergeNumber)-1
-                        pytablesFileRange = (filenameBase+"_tmp_connections_merge_"+
+                        pytablesFileRange = (filenameBase+"_tmp_direct_merge_"+
                                              str(mergeStart).zfill(numberLength)+"_"+
                                         str(mergeEnd).zfill(numberLength)+".process.h5")
                         if os.path.exists(pytablesFileRange):
                             os.remove(pytablesFileRange)
                         with tables.open_file(pytablesFileRange, mode="a") as pytablesStorageRange:
-                            Storage.create_merge_storage(pytablesStorageRange, numberOfKmers, 
-                                                         maximumFrequency, maximumConnectionLength)
+                            Storage.create_mergeDirect_storage(pytablesStorageRange, numberOfKmers, 
+                                                         maximumFrequency)
                         #merge
                         merge_direct_storage(pytablesFileRange, storageDirectFiles, mergeStart, 
                                              mergeNumber, numberOfKmers, kmer_properties)
-                        merge_connection_storage(pytablesFileRange, storageConnectionFiles, mergeStart, 
-                                             mergeNumber, numberOfKmers, maximumConnectionLength)
                         #now the file can be released for final merge
                         queue_merges.put(pytablesFileRange) 
                 except Empty:
+                    time.sleep(1)
                     continue
+        except Exception as ex:
+            logger.error("merges ({}): problem with worker: {}".format(os.getpid(),ex))
         finally:
             shm.close()
-        logger.debug("index: shared memory released")
             
+            
+    def worker_processReads(shutdown_event,queue_rawReads,queue_filteredReads,queue_finished,filenameBase,numberOfKmers,
+                     numberOfPartitions,maximumFrequency,maximumReadLength,shm_name):
+
+        logger = logging.getLogger("{}.worker.index".format(__name__))
+        
+        shm = shared_memory.SharedMemory(shm_name)
+        shm_kmer_partition = np.dtype(haplotyping.index.Database.getUint(numberOfPartitions)).type
+        shm_kmer_number = np.dtype(haplotyping.index.Database.getUint(maximumFrequency)).type
+        kmer_properties = np.ndarray((numberOfKmers,), 
+                                     dtype=[("partition",shm_kmer_partition),
+                                            ("number",shm_kmer_number),
+                                            ("disconnected","uint8")], 
+                                     buffer=shm.buf)
+        
+        def getRead(counters, structureIterator, stepData,pytablesStorageWorker):
+            row = next(structureIterator)
+            counters[0]=counters[1]
+            counters[1]+=row[0]
+            rowData = stepData[counters[0]-counters[2]:counters[1]-counters[2]]
+            if counters[1]>counters[3]:
+                counters[2] = counters[3]
+                counters[3] += counters[4]
+                stepData = pytablesStorageWorker.root.readRawData[counters[2]:counters[3]]
+                rowData = np.append(rowData,stepData[0:counters[1]-counters[2]])
+            #assert len(rowData)==row[0]
+            return row, rowData, counters, structureIterator, stepData
+        
+        
+        while not shutdown_event.is_set():
+            try:
+                item = queue_rawReads.get(block=True, timeout=1)
+                if item==None:
+                    logger.debug("reads ({}): none".format(os.getpid()))
+                    break
+                else: 
+                    curr_proc = current_process()
+                    pytablesFileWorker = filenameBase+"_tmp_processed_reads_{}.process.h5".format(curr_proc.name)
+                    if os.path.exists(pytablesFileWorker):
+                        os.remove(pytablesFileWorker)                    
+                    with (tables.open_file(item, mode="r") as pytablesStorageWorkerRaw, 
+                          tables.open_file(pytablesFileWorker, mode="w") as pytablesStorageWorkerFiltered):
+                        #create partition table
+                        Storage.create_filteredReads_storage(pytablesStorageWorkerFiltered,
+                                                  pytablesStorageWorkerRaw.root.readRawInfo.shape[0],
+                                                  pytablesStorageWorkerRaw.root.readRawInfo.shape[0],
+                                                  numberOfKmers, numberOfPartitions, maximumReadLength,
+                                                  pytablesStorageWorkerRaw.root.readRawInfo.shape[0])
+                        readPartitionData = pytablesStorageWorkerFiltered.root.readPartitionData
+                        readPartitionInfo = pytablesStorageWorkerFiltered.root.readPartitionInfo
+                        readPaired = pytablesStorageWorkerFiltered.root.readPaired                        
+
+                        #compute and store read partition
+                        stepSize = 1000000
+                        counters = [0,0,0,stepSize,stepSize] #n0,n1,m0,m1,stepSize
+                        #buffer
+                        computedPartitionData = []
+                        computedPartitionInfo = []
+                        computedPaired = []
+                        #initialize
+                        previousPaired = None
+                        try:
+                            structureIterator = pytablesStorageWorkerRaw.root.readRawInfo.iterrows()
+                            stepData = pytablesStorageWorkerRaw.root.readRawData[counters[2]:counters[3]]
+                            while True:
+                                row, rowData, counters, structureIterator, stepData = getRead(
+                                    counters, structureIterator, stepData, pytablesStorageWorkerRaw)
+                                assert row[0]==len(rowData)
+                                #filter
+                                rowData = [nodeId for nodeId in rowData if kmer_properties[nodeId][2]==0]
+                                #only if filtered set non-empty
+                                if len(rowData)>0:     
+                                    if len(rowData)>2:
+                                        partitions = [kmer_properties[nodeId][0] for nodeId in rowData]
+                                        #store
+                                        computedPartitionData.extend(rowData)
+                                        readPartitions = multimode(partitions)
+                                        if len(readPartitions)==1:
+                                            computedPartitionInfo.append((len(rowData),readPartitions[0],))
+                                        else:
+                                            sizes = [kmer_properties[nodeId][1] for nodeId in rowData
+                                                     if kmer_properties[nodeId][2]==0]
+                                            readPartitionSizes = {}
+                                            for p in readPartitions:
+                                                selection = np.where(partitions==p)[0]
+                                                readPartitionSizes[p] = max(np.array(sizes)[selection])
+                                            computedPartitionInfo.append((
+                                                len(rowData),min(readPartitionSizes, key=readPartitionSizes.get),))
+                                    if row[1]==1:
+                                        previousRead = [(nodeId,kmer_properties[nodeId][1]) for nodeId in rowData]
+                                        if len(previousRead)>0:
+                                            previousPaired = min(previousRead,key=lambda x:x[1])[0]
+                                    elif row[1]==2 and not previousPaired==None:
+                                        currentRead = [(nodeId,kmer_properties[nodeId][1]) for nodeId in reversed(rowData)]
+                                        if len(currentRead)>0:
+                                            currentPaired = min(currentRead,key=lambda x:x[1])[0]
+                                            if not previousPaired==currentPaired:
+                                                computedPaired.append((previousPaired,currentPaired,))
+                                                computedPaired.append((currentPaired,previousPaired,))
+                                    else:
+                                        previousPaired = None
+                                else:
+                                    previousPaired = None
+                                    
+                                if len(computedPartitionData)>1000000:
+                                    readPartitionData.append(tuple(computedPartitionData))
+                                    readPartitionInfo.append(computedPartitionInfo)
+                                    computedPartitionData = []
+                                    computedPartitionInfo = []
+                                    if len(computedPaired)>0:
+                                        computedPaired = sorted(computedPaired,key=lambda x:x[0])
+                                        readPaired.append(computedPaired)
+                                        computedPaired = []
+                        except StopIteration:
+                            pass
+                        finally:
+                            if len(computedPartitionData)>0:
+                                readPartitionData.append(tuple(computedPartitionData))
+                                readPartitionInfo.append(computedPartitionInfo)
+                                computedPartitionData = []
+                                computedPartitionInfo = []
+                                if len(computedPaired)>0:
+                                    computedPaired = sorted(computedPaired,key=lambda x:x[0])
+                                    readPaired.append(computedPaired)
+                                    computedPaired = [] 
+                            #flush and finish        
+                            pytablesStorageWorkerFiltered.flush()
+                            logger.debug("reads ({}): filtered {}/{} reads to {}/{}".format(
+                              os.getpid(),
+                              pytablesStorageWorkerRaw.root.readRawInfo.shape[0],
+                              pytablesStorageWorkerRaw.root.readRawData.shape[0],
+                              pytablesStorageWorkerFiltered.root.readPartitionInfo.shape[0],
+                              pytablesStorageWorkerFiltered.root.readPartitionData.shape[0]))
+                            #store filtered read files
+                            queue_filteredReads.put(pytablesFileWorker)
+            except Empty:
+                logger.debug("reads ({}): empty".format(os.getpid()))
+                time.sleep(5)
+                continue            
+
+    def worker_mergeReads(shutdown_event, queue_ranges, queue_merges, storageReadFiles, 
+                          partitionSizes, filenameBase, numberOfKmers, numberOfPartitions, maximumReadLength):
+
+        logger = logging.getLogger("{}.worker.index".format(__name__))
+        
+        def merge_reads_storage(pytablesFileWorker, storageReadFiles, mergeStart, mergeEnd, partitionPosition):
 
+            #initialise buffers
+            buffer = []
+            for i in range(mergeStart,mergeEnd+1):
+                buffer.append([[],[]])
+                
+            def getRead(counters, infoIterator, stepData, pytablesMergeSource):
+                row = next(infoIterator)
+                counters[0]=counters[1]
+                counters[1]+=row[0]
+                rowData = stepData[counters[0]-counters[2]:counters[1]-counters[2]]
+                while counters[1]>counters[3]:                    
+                    counters[2] = counters[3]
+                    counters[3] += counters[4]
+                    stepData = pytablesMergeSource.root.readPartitionData[counters[2]:counters[3]]
+                    rowData = np.append(rowData,stepData[0:counters[1]-counters[2]])
+                #assert len(rowData)==row[0]
+                return row, rowData, counters, infoIterator, stepData
+            
+            with tables.open_file(pytablesFileWorker, mode="a") as pytablesStorageWorker:
+                assert len(partitionPosition) == 1 + mergeEnd - mergeStart
+                #set partitions
+                for i in range(mergeStart,mergeEnd+1):
+                    values = [i] * partitionPosition[i-mergeStart][1]
+                    startPosition = partitionPosition[i-mergeStart][0]
+                    pytablesStorageWorker.root.readPartitionInfo[startPosition:startPosition+len(values)] = values
+                #set data and length
+                for item in storageReadFiles:
+                    with tables.open_file(item, mode="r") as pytablesMergeSource:
+                        #compute and store read partition
+                        stepSize = 10
+                        counters = [0,0,0,stepSize,stepSize] #n0,n1,m0,m1,stepSize
+                        #loop
+                        try:
+                            infoIterator = pytablesMergeSource.root.readPartitionInfo.iterrows()
+                            stepData = pytablesMergeSource.root.readPartitionData[counters[2]:counters[3]]
+                            while True:
+                                row, rowData, counters, infoIterator, stepData = getRead(
+                                    counters, infoIterator, stepData, pytablesMergeSource)
+                                if row[1]<mergeStart or row[1]>mergeEnd:
+                                    continue
+                                assert row[0]==len(rowData)
+                                partitionId = row[1]-mergeStart
+                                buffer[partitionId][0].append(row[0])
+                                buffer[partitionId][1].extend(rowData)
+                                if len(buffer[partitionId][1])>100000:
+                                    startPositionLength = partitionPosition[partitionId][0]
+                                    startPositionData = partitionPosition[partitionId][2]
+                                    pytablesStorageWorker.root.readPartitionLength[
+                                        startPositionLength:
+                                        startPositionLength+len(buffer[partitionId][0])] = buffer[partitionId][0]
+                                    pytablesStorageWorker.root.readPartitionData[
+                                        startPositionData:
+                                        startPositionData+len(buffer[partitionId][1])] = buffer[partitionId][1]
+                                    partitionPosition[partitionId][0] += len(buffer[partitionId][0])
+                                    partitionPosition[partitionId][2] += len(buffer[partitionId][1])
+                                    buffer[partitionId] = [[],[]]
+                                
+                        except StopIteration:
+                            pass
+                        finally:
+                            for i in range(mergeStart,mergeEnd+1):
+                                partitionId = i-mergeStart
+                                if len(buffer[partitionId][1])>0:
+                                    startPositionLength = partitionPosition[partitionId][0]
+                                    startPositionData = partitionPosition[partitionId][2]
+                                    pytablesStorageWorker.root.readPartitionLength[
+                                        startPositionLength:
+                                        startPositionLength+len(buffer[partitionId][0])] = buffer[partitionId][0]
+                                    pytablesStorageWorker.root.readPartitionData[
+                                        startPositionData:
+                                        startPositionData+len(buffer[partitionId][1])] = buffer[partitionId][1]
+                                    partitionPosition[partitionId][0] += len(buffer[partitionId][0])
+                                    partitionPosition[partitionId][2] += len(buffer[partitionId][1])
+                                    buffer[partitionId] = [[],[]]
+   
+        try:
+            #handle queue
+            while not shutdown_event.is_set():
+                try:
+                    item = queue_ranges.get(block=True, timeout=1)
+                    if item==None:
+                        break
+                    elif isinstance(item,tuple):
+                        mergeStart = item[0]
+                        mergeNumber = item[1]
+                        #create storage
+                        numberLength = len(str(numberOfPartitions))
+                        mergeEnd = min(numberOfPartitions,mergeStart+mergeNumber)-1
+                        pytablesFileRange = (filenameBase+"_tmp_read_merge_"+
+                                             str(mergeStart).zfill(numberLength)+"_"+
+                                        str(mergeEnd).zfill(numberLength)+".process.h5")
+                        if os.path.exists(pytablesFileRange):
+                            os.remove(pytablesFileRange)
+                            
+                        #prepare structure to store sorted data
+                        partitionPosition = []
+                        numberOfReads = 0
+                        numberOfData = 0
+                        for i in range(mergeStart,mergeEnd+1):
+                            partitionPosition.append([numberOfReads,partitionSizes[i][0],numberOfData,partitionSizes[i][1]])
+                            numberOfReads+=partitionSizes[i][0]
+                            numberOfData+=partitionSizes[i][1]
+                        #only merge if reads available
+                        if (numberOfReads>0) and (numberOfData>0):
+                            with tables.open_file(pytablesFileRange, mode="a") as pytablesStorageRange:
+                                Storage.create_mergeReads_storage(pytablesStorageRange,
+                                                      numberOfReads, numberOfData, numberOfKmers, 
+                                                      numberOfPartitions, maximumReadLength)
+                            #merge
+                            merge_reads_storage(pytablesFileRange, storageReadFiles, 
+                                                mergeStart, mergeEnd, partitionPosition)
+                            #now the file can be released for final merge
+                            queue_merges.put(pytablesFileRange) 
+                except Empty:
+                    time.sleep(1)
+                    continue
+#         except Exception as ex:
+#             logger.error("merges ({}): problem with worker: {}".format(os.getpid(),ex))
+        finally:
+            pass
+    
     
     """
     Combine merged files: this should be relatively easy, handled by single process
     """
-    def combine_merges(mergeFiles,pytablesStorage,numberOfKmers,maximumFrequency,maximumConnectionLength):
+    def combine_direct_merges(mergeFiles,pytablesStorage,numberOfKmers,maximumFrequency):
         
         nCycle = 0
         nReversal = 0
         nDirect = 0
-        nConnections = 0
-        nData = 0
         nPaired = 0
-
+        
         #get dimensions
         sortedMergeFiles = [{"filename": mergeFile} for mergeFile in sorted(mergeFiles)]
         for i in range(len(sortedMergeFiles)):
             with tables.open_file(sortedMergeFiles[i]["filename"], mode="r") as pytables_merge:
                 sortedMergeFiles[i]["ncycle"] = pytables_merge.root.cycle.shape[0]
                 sortedMergeFiles[i]["nreversal"] = pytables_merge.root.reversal.shape[0]
                 sortedMergeFiles[i]["ndirect"] = pytables_merge.root.direct.shape[0]
                 sortedMergeFiles[i]["ndeleteDirect"] = pytables_merge.root.deleteDirect.shape[0]
-                sortedMergeFiles[i]["nconnections"] = pytables_merge.root.connections.shape[0]
-                sortedMergeFiles[i]["ndata"] = pytables_merge.root.data.shape[0]
-                sortedMergeFiles[i]["npaired"] = pytables_merge.root.paired.shape[0]
-                sortedMergeFiles[i]["ndeletePaired"] = pytables_merge.root.deletePaired.shape[0]
+                sortedMergeFiles[i]["npaired"] = pytables_merge.root.tmpPaired.shape[0]                
                 nCycle += sortedMergeFiles[i]["ncycle"]
                 nReversal += sortedMergeFiles[i]["nreversal"]
                 nDirect += sortedMergeFiles[i]["ndirect"]
-                nConnections += sortedMergeFiles[i]["nconnections"]
-                nData = max(nData,sortedMergeFiles[i]["ndata"])
-                nPaired  += sortedMergeFiles[i]["npaired"]
-
+                nPaired += sortedMergeFiles[i]["npaired"]
+                                
         #create temporary storage with dimensions
-        Storage.create_merge_storage(pytablesStorage, numberOfKmers, maximumFrequency, maximumConnectionLength, 
-                                     nCycle, nReversal, nDirect, nConnections, nPaired)
+        Storage.create_mergeDirect_storage(pytablesStorage, numberOfKmers, maximumFrequency, 
+                                     nCycle, nReversal, nDirect, nPaired)
         tableCycle = pytablesStorage.root.cycle
         tableReversal = pytablesStorage.root.reversal
         tableDirect = pytablesStorage.root.direct
         tableDeleteDirect = pytablesStorage.root.deleteDirect
-        tableConnections = pytablesStorage.root.connections
-        tableData = pytablesStorage.root.data
-        tablePaired = pytablesStorage.root.paired
-        tableDeletePaired = pytablesStorage.root.deletePaired
+        tablePaired = pytablesStorage.root.tmpPaired
         
-        stepSizeStorage = 100 #FIX THIS BACK TO 100000
         maximumCycleLength = 0
         maximumCycleNumber = 0
         maximumReversalLength = 0
         maximumReversalNumber = 0
         maximumDirectDistance = 0
         maximumDirectNumber = 0
-        maximumConnectionsNumber = 0
-        maximumConnectionsLength = 0
-        maximumPairedNumber = 0
-        
-        connectionsDataCounter = 0
         
         #merge delete entries
         for i in range(len(sortedMergeFiles)):
             with tables.open_file(sortedMergeFiles[i]["filename"], mode="r") as pytables_merge:
                 tableDeleteDirect.append(pytables_merge.root.deleteDirect[:])
-                tableDeletePaired.append(pytables_merge.root.deletePaired[:])
         pytablesStorage.flush()
         tableDeleteDirect.cols.fromLink.create_csindex()
-        tableDeletePaired.cols.fromLink.create_csindex()
         pytablesStorage.flush()
                 
         for i in range(len(sortedMergeFiles)):
             with tables.open_file(sortedMergeFiles[i]["filename"], mode="r") as pytables_merge:
-                for j in range(0,sortedMergeFiles[i]["ncycle"],stepSizeStorage):
-                    reducedCycleDataBlock = pytables_merge.root.cycle[j:j+stepSizeStorage]
+                for j in range(0,sortedMergeFiles[i]["ncycle"],Storage.stepSizeStorage):
+                    reducedCycleDataBlock = pytables_merge.root.cycle[j:j+Storage.stepSizeStorage]
                     maximumCycleNumber = max(maximumCycleNumber,max(reducedCycleDataBlock["number"]))
                     maximumCycleLength = max(maximumCycleLength,max(reducedCycleDataBlock["minimumLength"]))
                     tableCycle.append(reducedCycleDataBlock)
-                for j in range(0,sortedMergeFiles[i]["nreversal"],stepSizeStorage):
-                    reducedReversalDataBlock = pytables_merge.root.reversal[j:j+stepSizeStorage]
+                for j in range(0,sortedMergeFiles[i]["nreversal"],Storage.stepSizeStorage):
+                    reducedReversalDataBlock = pytables_merge.root.reversal[j:j+Storage.stepSizeStorage]
                     maximumReversalNumber = max(maximumReversalNumber,max(reducedReversalDataBlock["number"]))
                     maximumReversalLength = max(maximumReversalLength,max(reducedReversalDataBlock["minimumLength"]))
                     tableReversal.append(reducedReversalDataBlock)
-                for j in range(0,sortedMergeFiles[i]["ndirect"],stepSizeStorage):
-                    directDataBlock = pytables_merge.root.direct[j:j+stepSizeStorage]
+                for j in range(0,sortedMergeFiles[i]["ndirect"],Storage.stepSizeStorage):
+                    directDataBlock = pytables_merge.root.direct[j:j+Storage.stepSizeStorage]
                     deleteDataBlock = tableDeleteDirect.read_where(
                         "(fromLink>={}) & (fromLink<={})".format(
                         directDataBlock[0]["fromLink"],directDataBlock[-1]["fromLink"]))
                     deletableIndices = np.where(
                         np.in1d(directDataBlock[["fromLink","fromDirection","toLink","toDirection"]],
                                 deleteDataBlock[["fromLink","fromDirection","toLink","toDirection"]]))[0]
                     reducedDirectDataBlock = np.delete(directDataBlock,deletableIndices,0)
                     maximumDirectNumber = max(maximumDirectNumber,max(reducedDirectDataBlock["number"]))
                     maximumDirectDistance = max(maximumDirectDistance,max(reducedDirectDataBlock["distance"]))
                     #add reduced direct data
-                    tableDirect.append(reducedDirectDataBlock)
-                for j in range(0,sortedMergeFiles[i]["nconnections"],stepSizeStorage):
-                    reducedConnectionsBlock = pytables_merge.root.connections[j:j+stepSizeStorage]
-                    for k in range(len(reducedConnectionsBlock)):
-                        reducedConnectionsBlock[k][1]+=connectionsDataCounter
-                    maximumConnectionsNumber = max(maximumConnectionsNumber,max(reducedConnectionsBlock["number"]))
-                    maximumConnectionsLength = max(maximumConnectionsLength,max(reducedConnectionsBlock["length"]))
-                    tableConnections.append(reducedConnectionsBlock)
-                for j in range(0,sortedMergeFiles[i]["ndata"],stepSizeStorage):
-                    reducedDataBlock = pytables_merge.root.data[j:j+stepSizeStorage]
-                    tableData.append(reducedDataBlock)
-                    connectionsDataCounter+=len(reducedDataBlock)
-                for j in range(0,sortedMergeFiles[i]["npaired"],stepSizeStorage):
-                    pairedDataBlock = pytables_merge.root.paired[j:j+stepSizeStorage]
-                    deleteDataBlock = tableDeletePaired.read_where(
-                        "(fromLink>={}) & (fromLink<={})".format(
-                        pairedDataBlock[0]["fromLink"],pairedDataBlock[-1]["fromLink"]))
-                    deletableIndices = np.where(
-                        np.in1d(pairedDataBlock[["fromLink","toLink"]],
-                                deleteDataBlock[["fromLink","toLink"]]))[0]
-                    reducedPairedDataBlock = np.delete(pairedDataBlock,deletableIndices,0)
-                    maximumPairedNumber = max(maximumPairedNumber,max(reducedPairedDataBlock["number"]))
-                    #add reduced paired data
+                    tableDirect.append(reducedDirectDataBlock)  
+                for j in range(0,sortedMergeFiles[i]["npaired"],Storage.stepSizeStorage):
+                    reducedPairedDataBlock = pytables_merge.root.tmpPaired[j:j+Storage.stepSizeStorage]
                     tablePaired.append(reducedPairedDataBlock)
 
         tableCycle.attrs["maximumNumber"] = maximumCycleNumber
         tableCycle.attrs["maximumLength"] = maximumCycleLength
         tableReversal.attrs["maximumNumber"] = maximumReversalNumber
         tableReversal.attrs["maximumLength"] = maximumReversalLength
         tableDirect.attrs["maximumDistance"] = maximumDirectDistance
         tableDirect.attrs["maximumNumber"] = maximumDirectNumber
-        tableConnections.attrs["maximumNumber"] = maximumConnectionsNumber
-        tableConnections.attrs["maximumLength"] = maximumConnectionsLength
         pytablesStorage.flush()
-            
+        #sort paired data
+        tablePaired.cols.fromLink.create_csindex()
+        pytablesStorage.flush()
+        
+    def combine_filtered_pairs(mergeFiles,pytablesStorage,numberOfKmers):
+        logger = logging.getLogger(__name__) 
+        #collect, sort and combine data
+        dataList = []
+        for item in mergeFiles:
+            with tables.open_file(item, mode="r") as pytablesSource:
+                size = pytablesSource.root.readPaired.shape[0]
+                itemData = pytablesSource.root.readPaired[0:size]
+                dataList.append(np.unique(itemData))
+                del itemData
+        data = np.unique(np.concatenate(dataList))
+        del dataList
+        #store data
+        numberOfPaired = len(data)
+        logger.info("store "+str(numberOfPaired)+" paired")
+        pairedTable = pytablesStorage.create_table(pytablesStorage.root, 
+            "readPaired",{
+            "fromLink": haplotyping.index.Database.getTablesUint(numberOfKmers,0),
+            "toLink": haplotyping.index.Database.getTablesUint(numberOfKmers,1),
+        }, "Paired reads", expectedrows=numberOfPaired)
+        pairedTable.append(data)
+        pairedTable.flush()
+        
+        
+    def combine_read_merges(mergeFiles,pytablesStorage,numberOfKmers,
+                                  numberOfPartitions,maximumReadLength):
+        numberOfReads = 0
+        numberOfData = 0
+        partitionIndex = [0] * numberOfPartitions
+        for item in mergeFiles:
+            with tables.open_file(item, mode="r") as pytablesSource:
+                numberOfReads+=pytablesSource.root.readPartitionInfo.shape[0]
+                numberOfData+=pytablesSource.root.readPartitionData.shape[0]
+                for i in range(0,numberOfReads,Storage.stepSizeStorage):
+                    stepData = pytablesSource.root.readPartitionInfo[i:i+Storage.stepSizeStorage]
+                    for p in stepData:
+                        partitionIndex[p]+=1
+        if numberOfReads>0:
+            Storage.create_filteredMergedReads_storage(pytablesStorage,numberOfReads,numberOfData,numberOfKmers,
+                                  numberOfPartitions,maximumReadLength)
+            tReads = 0
+            tData = 0
+            readPartition=pytablesStorage.root.readPartition
+            readPartitionInfo=pytablesStorage.root.readPartitionInfo
+            readPartitionData=pytablesStorage.root.readPartitionData
+            partition = 0
+            maximumLength = 0
+            maximumTotalLength = 0
+            maximumNumber = 0
+            maximumTotalNumber = 0
+            for item in mergeFiles:
+                with tables.open_file(item, mode="r") as pytablesSource:
+                    sInfo=pytablesSource.root.readPartitionInfo.shape[0]
+                    sLength=pytablesSource.root.readPartitionLength.shape[0]
+                    sData=pytablesSource.root.readPartitionData.shape[0]
+                    pReads=0
+                    pData=0
+                    while pReads<sInfo:
+                        #collect data
+                        nReads = partitionIndex[partition]
+                        partitionLength = pytablesSource.root.readPartitionLength[pReads:pReads+nReads]
+                        nData = sum(partitionLength)
+                        partitionData = pytablesSource.root.readPartitionData[pData:pData+nData]
+                        #filter
+                        partitionDataIndex = {}
+                        partitionDataInfo = []
+                        fData = 0
+                        for i in range(nReads):
+                            rowData = tuple(partitionData[fData:fData+partitionLength[i]])
+                            rowKey = hash(rowData)
+                            if rowKey in partitionDataIndex:
+                                partitionDataInfo[partitionDataIndex[rowKey]][1]+=1
+                            else:
+                                partitionDataIndex[rowKey] = len(partitionDataInfo)
+                                partitionDataInfo.append([partitionLength[i],1])
+                                readPartitionData.append(rowData)
+                                fData+=partitionLength[i]
+                        if len(partitionDataInfo)>0:
+                            readPartitionInfo.append([tuple(item) for item in partitionDataInfo])
+                            maximumLength = max(maximumLength,max([item[0] for item in partitionDataInfo]))
+                            maximumTotalLength = max(maximumTotalLength,sum([item[0] for item in partitionDataInfo]))
+                            maximumNumber = max(maximumNumber,max([item[1] for item in partitionDataInfo]))
+                            maximumTotalNumber = max(maximumTotalNumber,len(partitionDataInfo))
+                        #store
+                        readPartition.append([(tData,fData,tReads,len(partitionDataInfo))])
+                        pReads+=nReads
+                        pData+=nData
+                        tReads+=len(partitionDataInfo)
+                        tData+=fData
+                        partition+=1
+            while partition<numberOfPartitions:
+                readPartition.append((tData,0,tReads,0))
+                partition+=1
+            readPartitionInfo.attrs["maximumLength"] = maximumLength
+            readPartitionInfo.attrs["maximumTotalLength"] = maximumTotalLength
+            readPartitionInfo.attrs["maximumNumber"] = maximumNumber
+            readPartitionInfo.attrs["maximumTotalNumber"] = maximumTotalNumber
+
     """
-    Store everything in the final database, handled by single process
+    Store direct data in the final database, handled by single process
     """    
-    def store_merged_connections(h5file,pytablesStorage,numberOfKmers,minimumFrequency):
+    def store_merged_direct(h5file,pytablesStorage,numberOfKmers,minimumFrequency):
         logger = logging.getLogger(__name__)     
         frequencyHistogram = {"distance": {}}
         
         def classifyDirectProblematic(dataBlock,directGood,directCoverage,directProblematic):
             dataBlock = np.array(dataBlock, dtype=object)                       
             if max(dataBlock[:,4])==0:
                 directGood+=len(dataBlock)
@@ -1569,64 +1713,65 @@
                 dataBlock[:,4] = 2
                 directProblematic+=len(dataBlock)
             number = sum(dataBlock[:,2])
             distinct = len(dataBlock)
             dataBlock = tuple([tuple(e) for e in dataBlock])
             return (dataBlock,directGood,directCoverage,directProblematic,distinct,number)
         
-        stepSizeStorage = 100000
         dsCkmer = h5file["/split/ckmer"]
         
         #cycles
         numberOfCycles = pytablesStorage.root.cycle.shape[0]
         maximumNumber = pytablesStorage.root.cycle.attrs.maximumNumber
         maximumLength = pytablesStorage.root.cycle.attrs.maximumLength
         dtypeCycleList=[("ckmerLink",haplotyping.index.Database.getUint(numberOfKmers)),
                          ("minimumLength",haplotyping.index.Database.getUint(maximumLength)),
                          ("number",haplotyping.index.Database.getUint(maximumNumber))]
         dtCycle=np.dtype(dtypeCycleList)
         dsCycle=h5file["/relations/"].create_dataset("cycle",(numberOfCycles,), 
-                                                     dtype=dtCycle, chunks=None)
+                                                     dtype=dtCycle, chunks=None, 
+                                                     compression="gzip", compression_opts=9)
         maximumCycleLength = 0
         maximumCycleNumber = 0
-        for i in range(0,numberOfCycles,stepSizeStorage):
-            stepData = pytablesStorage.root.cycle[i:i+stepSizeStorage]                    
-            dsCycle[i:i+stepSizeStorage] = stepData
+        for i in range(0,numberOfCycles,Storage.stepSizeStorage):
+            stepData = pytablesStorage.root.cycle[i:i+Storage.stepSizeStorage]                    
+            dsCycle[i:i+Storage.stepSizeStorage] = stepData
             for row in stepData:
                 ckmerRow = dsCkmer[row[0]]
                 ckmerRow[7] = row[2]
                 maximumCycleLength = max(maximumCycleLength,row[1])
                 maximumCycleNumber = max(maximumCycleNumber,row[2])
                 dsCkmer[row[0]] = ckmerRow    
-        h5file["/config/"].attrs["numberOfCycles"]=numberOfCycles        
+        h5file["/config/"].attrs["numberCycles"]=numberOfCycles        
         h5file["/config/"].attrs["maximumCycleLength"]=maximumCycleLength
         h5file["/config/"].attrs["maximumCycleNumber"]=maximumCycleNumber
         logger.info("store "+str(numberOfCycles)+" cycles")
         #reversals
         numberOfReversals = pytablesStorage.root.reversal.shape[0]
         maximumNumber = pytablesStorage.root.reversal.attrs.maximumNumber
         maximumLength = pytablesStorage.root.reversal.attrs.maximumLength
         dtypeReversalList=[("ckmerLink",haplotyping.index.Database.getUint(numberOfKmers)),
                          ("minimumLength",haplotyping.index.Database.getUint(maximumLength)),
                          ("number",haplotyping.index.Database.getUint(maximumNumber))]
         dtReversal=np.dtype(dtypeReversalList)
         dsReversal=h5file["/relations/"].create_dataset("reversal",(numberOfReversals,), 
-                                                        dtype=dtReversal, chunks=None)
+                                                        dtype=dtReversal, chunks=None, 
+                                                        compression="gzip", compression_opts=9)
         maximumReversalLength = 0
         maximumReversalNumber = 0
-        for i in range(0,numberOfReversals,stepSizeStorage):
-            stepData = pytablesStorage.root.reversal[i:i+stepSizeStorage]
-            dsReversal[i:i+stepSizeStorage] = stepData
+        for i in range(0,numberOfReversals,Storage.stepSizeStorage):
+            stepData = pytablesStorage.root.reversal[i:i+Storage.stepSizeStorage]
+            dsReversal[i:i+Storage.stepSizeStorage] = stepData
             for row in stepData:
                 ckmerRow = dsCkmer[row[0]]
                 ckmerRow[8] = row[2]
                 maximumReversalLength = max(maximumReversalLength,row[1])
                 maximumReversalNumber = max(maximumReversalNumber,row[2])
                 dsCkmer[row[0]] = ckmerRow     
-        h5file["/config/"].attrs["numberOfReversals"]=numberOfReversals
+        h5file["/config/"].attrs["numberReversals"]=numberOfReversals
         h5file["/config/"].attrs["maximumReversalLength"]=maximumReversalLength
         h5file["/config/"].attrs["maximumReversalNumber"]=maximumReversalNumber
         logger.info("store "+str(numberOfReversals)+" reversals")
         #direct relations
         numberOfDirectRelations = pytablesStorage.root.direct.shape[0]
         maximumNumber = pytablesStorage.root.direct.attrs.maximumNumber
         maximumDistance = pytablesStorage.root.direct.attrs.maximumDistance
@@ -1635,51 +1780,28 @@
                          ("to",[("ckmerLink",haplotyping.index.Database.getUint(numberOfKmers)),
                                   ("direction","S1")]),
                          ("number",haplotyping.index.Database.getUint(maximumNumber)),
                          ("distance",haplotyping.index.Database.getUint(maximumDistance)),
                          ("problematic","uint8")]
         dtDirect=np.dtype(dtypeDirectList)
         dsDirect=h5file["/relations/"].create_dataset("direct",(numberOfDirectRelations,), 
-                                                      dtype=dtDirect, chunks=None)
-        #connections
-        numberOfConnections = pytablesStorage.root.connections.shape[0]
-        numberOfData = pytablesStorage.root.data.shape[0]
-        numberOfPaired = pytablesStorage.root.paired.shape[0]
-        maximumNumber = pytablesStorage.root.connections.attrs.maximumNumber
-        maximumLength = pytablesStorage.root.connections.attrs.maximumLength
-        dtypeConnectionsList=[("ckmerLink",haplotyping.index.Database.getUint(numberOfKmers)),
-                              ("dataLink",haplotyping.index.Database.getUint(numberOfData)),
-                              ("length",haplotyping.index.Database.getUint(maximumLength)),
-                              ("direct","uint8"),
-                              ("number",haplotyping.index.Database.getUint(maximumNumber))
-                             ]
-        dtConnections=np.dtype(dtypeConnectionsList)
-        dsConnections=h5file["/connections/"].create_dataset("index",(numberOfConnections,), 
-                                                      dtype=dtConnections, chunks=None)
-        dsData=h5file["/connections/"].create_dataset("data",(numberOfData,), 
-                          dtype=haplotyping.index.Database.getUint(numberOfKmers), chunks=None)
-        dtypePairedList=[("fromLink",haplotyping.index.Database.getUint(numberOfKmers)),
-                         ("toLink",haplotyping.index.Database.getUint(numberOfKmers)),
-                         ("number",haplotyping.index.Database.getUint(maximumNumber))
-                        ]
-        dtPaired=np.dtype(dtypePairedList)
-        dsPaired=h5file["/connections/"].create_dataset("paired",(numberOfPaired,), 
-                                                      dtype=dtPaired, chunks=None)
+                                                      dtype=dtDirect, chunks=None, 
+                                                      compression="gzip", compression_opts=9)
         #process direct relations
         directCounter = 0
         previousStepData = []
         directGood = 0
         directCoverage = 0
         directProblematic = 0
-        for i in range(0,numberOfDirectRelations,stepSizeStorage):
-            stepData = pytablesStorage.root.direct[i:i+stepSizeStorage]
+        for i in range(0,numberOfDirectRelations,Storage.stepSizeStorage):
+            stepData = pytablesStorage.root.direct[i:i+Storage.stepSizeStorage]
             #move a bit to get all fromLinks in the selection
             if len(previousStepData)>0:
                 stepData = np.concatenate((previousStepData, stepData))
-            if (i+stepSizeStorage-1)<numberOfDirectRelations:
+            if (i+Storage.stepSizeStorage-1)<numberOfDirectRelations:
                 lastFromLink = stepData[-1]["fromLink"]
                 previousStepData = np.take(stepData, np.where(stepData["fromLink"] == lastFromLink))[0]
                 stepData = np.delete(stepData, np.where(stepData["fromLink"] == lastFromLink))
             else:
                 previousStepData = [] 
             #get relevant ckmer data
             firstFromLink = stepData[0]["fromLink"]
@@ -1733,72 +1855,219 @@
                 raise Exception("unexpected direction")
             newStepData.extend(newStepDataBlock)
             #store all
             dsDirect[directCounter:directCounter+len(newStepData)] = newStepData
             dsCkmer[firstFromLink:(lastFromLink+1)] = ckmerStepData
             directCounter+=len(newStepData)
 
-        logger.info("store {} direct connections, {} low coverage, {} problematic".format(
-            numberOfDirectRelations,directCoverage,directProblematic))
+        logger.info("store {} direct connections".format(numberOfDirectRelations))
+        logger.info("{} low coverage and {} problematic".format(directCoverage,directProblematic))
 
-        #process connections
-        connectionsCounter = 0
-        dataCounter = 0
-        pairedCounter = 0
-        ckmerConnectionsIndexLink = np.zeros(dsCkmer.len(), dtype=int)
-        ckmerConnectionsIndexCounter = np.zeros(dsCkmer.len(), dtype=int)
-        ckmerConnectionsCounter = np.zeros(dsCkmer.len(), dtype=int)
-        ckmerPairedLink = np.zeros(dsCkmer.len(), dtype=int)
-        ckmerPairedCounter = np.zeros(dsCkmer.len(), dtype=int)
-        for i in range(0,numberOfConnections,stepSizeStorage):
-            stepData = pytablesStorage.root.connections[i:i+stepSizeStorage]  
-            for j in range(i,i+len(stepData)):    
-                if ckmerConnectionsIndexCounter[stepData[j-i][0]]==0:
-                    ckmerConnectionsIndexLink[stepData[j-i][0]] = j
-                    ckmerConnectionsIndexCounter[stepData[j-i][0]] = 1
-                else:
-                    ckmerConnectionsIndexCounter[stepData[j-i][0]]+=1
-            dsConnections[connectionsCounter:connectionsCounter+len(stepData)] = stepData
-            connectionsCounter+=len(stepData)
-        for i in range(0,numberOfData,stepSizeStorage):
-            stepData = pytablesStorage.root.data[i:i+stepSizeStorage]   
-            for row in stepData:
-                ckmerConnectionsCounter[row]+=1
-            dsData[dataCounter:dataCounter+len(stepData)] = stepData
-            dataCounter+=len(stepData)
-        for i in range(0,numberOfPaired,stepSizeStorage):
-            stepData = pytablesStorage.root.paired[i:i+stepSizeStorage]   
-            for j in range(i,i+len(stepData)):
-                if ckmerPairedCounter[stepData[j-i][0]]==0:
-                    ckmerPairedLink[stepData[j-i][0]] = j
-                    ckmerPairedCounter[stepData[j-i][0]] = 1
+        # store histogram direct distances
+        if len(frequencyHistogram["distance"])>0:
+            maximumDistance = max(frequencyHistogram["distance"].keys())
+            maximumNumber = max(frequencyHistogram["distance"].values())
+            dtypeFrequencyHistogramDistanceList=[
+                        ("distance",haplotyping.index.Database.getUint(maximumDistance)),
+                        ("number",haplotyping.index.Database.getUint(maximumNumber)),]
+            dtFrequencyHistogramDistance=np.dtype(dtypeFrequencyHistogramDistanceList)
+            dsFrequencyHistogramDistance=h5file["/histogram/"].create_dataset("distance",
+                  (len(frequencyHistogram["distance"]),), dtype=dtFrequencyHistogramDistance, chunks=None, 
+                  compression="gzip", compression_opts=9)
+            logger.info("store {} entries direct distances histogram".format(
+                len(frequencyHistogram["distance"])))
+            #store histogram
+            dsFrequencyHistogramDistance[0:len(frequencyHistogram["distance"])] = list(
+                sorted(frequencyHistogram["distance"].items()))
+            
+    def store_merged_reads(h5file,pytablesStorage,numberOfKmers,numberOfPartitions):
+        logger = logging.getLogger(__name__)    
+        
+        #paired
+        ckmerIndex = [[0,0] for i in range(numberOfKmers)]
+        numberOfPaired = pytablesStorage.root.readPaired.shape[0]
+        dtypePairedList=[("fromLink",haplotyping.index.Database.getUint(numberOfKmers)),
+                         ("toLink",haplotyping.index.Database.getUint(numberOfKmers))]
+        dtPaired=np.dtype(dtypePairedList)
+        dsPaired=h5file["/relations/"].create_dataset("paired",(numberOfPaired,), 
+                                                      dtype=dtPaired, chunks=None, 
+                                                      compression="gzip", compression_opts=9)
+        for i in range(0,numberOfPaired,Storage.stepSizeStorage):
+            stepData = pytablesStorage.root.readPaired[i:i+Storage.stepSizeStorage]
+            for j in range(len(stepData)):
+                row = stepData[j]
+                if ckmerIndex[row[0]][1]>0:
+                    ckmerIndex[row[0]][1] += 1
                 else:
-                    ckmerPairedCounter[stepData[j-i][0]]+=1
-            dsPaired[pairedCounter:pairedCounter+len(stepData)] = stepData
-            pairedCounter+=len(stepData)
-        for i in range(0,dsCkmer.len(),stepSizeStorage):
-            stepData = dsCkmer[i:i+stepSizeStorage]  
-            for j in range(i,i+len(stepData)):                
-                stepData[j-i][5] = (ckmerConnectionsIndexLink[j],ckmerConnectionsIndexCounter[j],ckmerConnectionsCounter[j],)
-                stepData[j-i][6] = (ckmerPairedLink[j],ckmerPairedCounter[j],)
-            dsCkmer[i:i+len(stepData)] = stepData
+                    ckmerIndex[row[0]] = [i+j,1]
+            dsPaired[i:i+len(stepData)] = stepData
+        logger.info("store {} paired connections".format(numberOfPaired))
+        
+        #update kmer properties
+        dsCkmer = h5file["/split/ckmer"]
+        for i in range(0,numberOfKmers,Storage.stepSizeStorage):
+            stepData = dsCkmer[i:i+Storage.stepSizeStorage]
+            stepData["paired"] = [tuple(item) for item in ckmerIndex[i:i+len(stepData)]]
+            dsCkmer[i:i+Storage.stepSizeStorage] = stepData
+        
+        #reads
+        numberOfReadPartition = pytablesStorage.root.readPartition.shape[0]
+        numberOfReadPartitionData = pytablesStorage.root.readPartitionData.shape[0]
+        numberOfReadPartitionInfo = pytablesStorage.root.readPartitionInfo.shape[0]
+        
+        maxReadLength = pytablesStorage.root.readPartitionInfo.attrs["maximumLength"]
+        maxTotalReadLength = pytablesStorage.root.readPartitionInfo.attrs["maximumTotalLength"]
+        maxReadNumber = pytablesStorage.root.readPartitionInfo.attrs["maximumNumber"]
+        maxTotalReadNumber = pytablesStorage.root.readPartitionInfo.attrs["maximumTotalNumber"]
+        
+        dsReadData=h5file["/relations/"].create_dataset("readData",(numberOfReadPartitionData,), 
+                                                      dtype=haplotyping.index.Database.getUint(numberOfKmers), 
+                                                      chunks=None, compression="gzip", compression_opts=9)
+        for i in range(0,numberOfReadPartitionData,Storage.stepSizeStorage):
+            stepData = pytablesStorage.root.readPartitionData[i:i+Storage.stepSizeStorage]
+            dsReadData[i:i+len(stepData)] = stepData
+        logger.info("store {} read data points".format(numberOfReadPartitionData))
+        dtypeReadInfoList=[("length",haplotyping.index.Database.getUint(maxReadLength)),
+                           ("number",haplotyping.index.Database.getUint(maxReadNumber))]
+        dtReadInfo=np.dtype(dtypeReadInfoList)
+        dsReadInfo=h5file["/relations/"].create_dataset("readInfo",(numberOfReadPartitionInfo,), 
+                                                      dtype=dtReadInfo, chunks=None, 
+                                                      compression="gzip", compression_opts=9)
+        for i in range(0,numberOfReadPartitionInfo,Storage.stepSizeStorage):
+            stepData = pytablesStorage.root.readPartitionInfo[i:i+Storage.stepSizeStorage]
+            dsReadInfo[i:i+len(stepData)] = stepData
+        logger.info("store {} read info".format(numberOfReadPartitionInfo))
+        dtypeReadPartitionList=[("readData",[
+                                    ("link",haplotyping.index.Database.getUint(numberOfReadPartitionData)),
+                                    ("number",haplotyping.index.Database.getUint(maxReadLength))]),
+                                ("readInfo",[
+                                    ("link",haplotyping.index.Database.getUint(numberOfReadPartitionInfo)),
+                                    ("number",haplotyping.index.Database.getUint(maxReadLength))])]
+        dtReadPartition=np.dtype(dtypeReadPartitionList)
+        dsReadPartition=h5file["/relations/"].create_dataset("readPartition",(numberOfReadPartition,), 
+                                                      dtype=dtReadPartition, chunks=None, 
+                                                      compression="gzip", compression_opts=9)
+        for i in range(0,numberOfReadPartition,Storage.stepSizeStorage):
+            stepData = pytablesStorage.root.readPartition[i:i+Storage.stepSizeStorage]
+            dsReadPartition[i:i+len(stepData)] = [((item[0],item[1]),(item[2],item[3])) for item in stepData]
+        logger.info("store {} read partitions".format(numberOfReadPartition))
+        
+        
+        
+    """
+    Partition k-mers
+    """    
+    def partition_kmers(h5file,pytablesStorage,maxNumberOfPartitions):
+        #initialize
+        logger = logging.getLogger(__name__)  
+        edges = []
+        disconnected = []
+        
+        #compute edges for partition graph
+        numberOfKmers = h5file["split"]["ckmer"].shape[0]
+        numberOfBases = h5file["split"]["base"].shape[0]
+        numberOfDirect = h5file["relations"]["direct"].shape[0]
+        previousVertex = 0
+        previousNeighbours = []
+        logger.debug("create graph for partitioning")
+        for i in range(0,numberOfDirect,Storage.stepSizeStorage):
+            block = h5file["relations"]["direct"][i:i+Storage.stepSizeStorage]
+            logger.debug("add edges: {}-{} of {} ({}%)".format(
+                i,i+len(block),numberOfDirect,int(100*(i+len(block))/numberOfDirect)))
+            for j in range(len(block)):
+                while block[j][0][0]>previousVertex:
+                    if len(previousNeighbours)==0:
+                        disconnected.append(previousVertex)
+                    edges.append(tuple(previousNeighbours))
+                    previousVertex+=1
+                    previousNeighbours = []
+                if not block[j][1][0] in previousNeighbours:
+                    previousNeighbours.append(block[j][1][0])
+        while numberOfKmers>previousVertex:
+            if len(previousNeighbours)==0:
+                disconnected.append(previousVertex)
+            edges.append(tuple(previousNeighbours))
+            previousVertex+=1
+            previousNeighbours = []
+            
+        #try to add paired connections for disconnected
+        if pytablesStorage.root.tmpPaired.shape[0]>0:
+            logger.debug("try to connect {} disconnected nodes with {} paired nodes".format(
+                len(disconnected),pytablesStorage.root.tmpPaired.shape[0]))
+            dataIterator = pytablesStorage.root.tmpPaired.itersorted("fromLink",checkCSI=True)
+            disconnectedIterator = iter(disconnected)
+            try:
+                dataRow = next(dataIterator)
+                disconnectedEntry = next(disconnectedIterator)
+                while True:
+                    if dataRow[0]>disconnectedEntry:
+                        disconnectedEntry = next(disconnectedIterator)
+                    else:
+                        if dataRow[0]==disconnectedEntry:
+                            if len(edges[disconnectedEntry])==0:
+                                edges[disconnectedEntry] = tuple([dataRow[1]])
+                                edges[dataRow[1]] = edges[dataRow[1]] + (dataRow[0],)
+                            elif not dataRow[1] in edges[disconnectedEntry]:
+                                edges[disconnectedEntry] = edges[disconnectedEntry] + (dataRow[1],)
+                                edges[dataRow[1]] = edges[dataRow[1]] + (dataRow[0],)
+                        dataRow = next(dataIterator)                                        
+            except StopIteration:
+                pass  
+            
+        #update disconnected
+        disconnected = [i for i in range(len(edges)) if len(edges[i])==0]
+        logger.debug("connect {} disconnected nodes to base connections".format(len(disconnected)))
         
-        logger.info("store {} indirect connections with {} data entries and {} paired".format(
-            numberOfConnections,numberOfData,numberOfPaired))
+        #create memory for links with bases
+        bases = h5file["split/base"]
+        ckmers = h5file["/split/ckmer"]
+        disconnectedRows = ckmers[disconnected]
+        for ckmerId,ckmerRow in zip(disconnected,disconnectedRows):
+            if ckmerRow[1]==b"l":
+                baseIds = [ckmerRow[3][0]]
+            elif ckmerRow[1]==b"r":
+                baseIds = [ckmerRow[3][1]]
+            elif ckmerRow[1]==b"b":
+                baseIds = [ckmerRow[3][0],ckmerRow[3][1]]
+            else:
+                baseIds = []
+            ckmerLinks = set()
+            for baseId in baseIds:
+                ckmerLinks.update([baseEntry[1] for baseEntry in bases[baseId][2] if baseEntry[0]>0])
+                ckmerLinks.remove(ckmerId) 
+                if len(edges[ckmerId])==0:
+                    edges[ckmerId] = tuple(ckmerLinks)
+                    for ckmerLink in ckmerLinks:
+                        edges[ckmerLink] = edges[ckmerLink] + (ckmerId,)
+                        
+        #compute partitions
+        logger.debug("compute metis graph partitioning with at most {} partitions".format(maxNumberOfPartitions))
+        m = metis.adjlist_to_metis(edges)
+        del edges
+        (objval,partitions) = metis.part_graph(m,maxNumberOfPartitions)
+        (values, partitions, counts) = np.unique(partitions, return_inverse=True, return_counts=True) 
+        numberOfPartitions = len(counts)
+        logger.debug("computed {} partitions - {}".format(numberOfPartitions,max(partitions)))
 
-        # store histogram direct distances
-        maximumDistance = max(frequencyHistogram["distance"].keys())
-        maximumNumber = max(frequencyHistogram["distance"].values())
-        dtypeFrequencyHistogramDistanceList=[
-                    ("distance",haplotyping.index.Database.getUint(maximumDistance)),
-                    ("number",haplotyping.index.Database.getUint(maximumNumber)),]
-        dtFrequencyHistogramDistance=np.dtype(dtypeFrequencyHistogramDistanceList)
-        dsFrequencyHistogramDistance=h5file["/histogram/"].create_dataset("distance",
-              (len(frequencyHistogram["distance"]),), dtype=dtFrequencyHistogramDistance, chunks=None)
-        logger.info("store {} entries direct distances histogram".format(
-            len(frequencyHistogram["distance"])))
-        #store histogram
-        dsFrequencyHistogramDistance[0:len(frequencyHistogram["distance"])] = list(
-            sorted(frequencyHistogram["distance"].items()))
+        #store partition in ckmer properties
+        dsCkmer = h5file["/split/ckmer"]
+        assert numberOfKmers==len(partitions)
+        for i in range(0,numberOfKmers,Storage.stepSizeStorage):
+            stepData = dsCkmer[i:i+Storage.stepSizeStorage] 
+            stepData["partition"] = partitions[i:i+Storage.stepSizeStorage] 
+            dsCkmer[i:i+Storage.stepSizeStorage] = stepData
+        
+        #store partition size
+        h5file["/config/"].attrs["numberPartitions"]=numberOfPartitions  
+        dtypePartitionList=[("ckmer",haplotyping.index.Database.getUint(numberOfKmers))]
+        dtPartition=np.dtype(dtypePartitionList)
+        dsPartition=h5file["/histogram/"].create_dataset("partition",(numberOfPartitions,), 
+                                                        dtype=dtPartition, chunks=None, 
+                                                        compression="gzip", compression_opts=9)
+        dsPartition[0:numberOfPartitions] = counts
+        
+        return numberOfPartitions 
+        
+
```

### Comparing `haplotyping-0.0.5/haplotyping/service/api.py` & `haplotyping-0.0.6/haplotyping/service/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os,sys,logging,configparser
 from multiprocessing import Process,get_start_method
 from flask import Flask, Blueprint, Response, render_template, current_app, g, request
 from flask_restx import Api, Resource
 from werkzeug.middleware.proxy_fix import ProxyFix
-import json, sqlite3
+import json, sqlite3, re
 from waitress import serve
 
 import haplotyping
 
 from haplotyping.service.api_tools import namespace as ns_api_tools
 from haplotyping.service.api_country import namespace as ns_api_country
 from haplotyping.service.api_collection import namespace as ns_api_collection
@@ -18,23 +18,23 @@
 from haplotyping.service.api_marker import namespace as ns_api_marker
 
 from haplotyping.service.api_kmer import cache as cache_api_kmer
 from haplotyping.service.api_split import cache as cache_api_split
 
 class API:
     
-    def __init__(self, location):
+    def __init__(self, location, configFile="config.ini"):
                                 
         self.location = str(location)
         
         #set logging
         logger_server = logging.getLogger(__name__+".server")
         
         self.config = configparser.ConfigParser()
-        self.config.read(os.path.join(self.location,"server.ini")) 
+        self.config.read(os.path.join(self.location,configFile)) 
         logger_server.info("read configuration file") 
         if self.config.getboolean("api","debug"):
             logger_server.info("run in debug mode") 
             logger_server.setLevel(logging.DEBUG)
         else:
             logger_server.setLevel(logging.INFO)
         
@@ -48,27 +48,29 @@
                 frame = frame.f_back
                 
         #restart on errors
         while True:
             try:
                 process_api = Process(target=self.process_api_messages, args=[])
                 #start everything
-                logger_server.info("start server on port {:s}".format(self.config["api"].get("port","8080")))
+                logger_server.info("start server on port {:s}".format(
+                    self.config["api"].get("port","8080")))
                 process_api.start()
                 #wait until ends  
                 process_api.join()
             except Exception as e:  
                 logger_server.error("error: "+ str(e))  
         
     def get_db_connection():
         db_connection = getattr(g, "_database", None)
         if db_connection is None:
             config = current_app.config.get("config")
             location = current_app.config.get("location")
-            db_connection = g._database = sqlite3.connect(os.path.join(location,config["settings"]["sqlite_db"]))
+            db_connection = g._database = sqlite3.connect(
+                os.path.join(location,config["settings"]["sqlite_db"]))
         return db_connection
     
     def get_kmc_query_library():
         try:
             config = current_app.config.get("config")
             return config["settings"]["kmc_query_library"]
         except:
@@ -180,33 +182,49 @@
         def before_request_func():
             app.logger.info("Request to "+str(request.endpoint)+" ("+str(request.content_length)+")")
             if self.config.getboolean("api","proxy_prefix"):
                 if api._schema:
                     api._schema["basePath"] = api.base_path
                     api.__schema__["basePath"] = api.base_path
 
-        parser = api.parser()
+        #parser = api.parser()
 
         #--- database ---    
         @app.teardown_appcontext
         def close_connection(exception):
             db = getattr(g, "_database", None)
             if db is not None:
                 logger_api.debug("close database connection")
                 db.close()
 
         #--- site ---
         @app.route("/")
-        def index():
-            return render_template("index.html")
+        @app.route("/<path:path>")
+        def index(path=""):
+            pattern = re.compile(r"[^\/]+\/")
+            rootLocation = "../"*len(re.findall(pattern, path))
+            pathSplits = path.split("/")
+            operation = pathSplits[0]
+            if (len(pathSplits)>1):
+                identifier = pathSplits[1]
+            else:
+                identifier = None
+            variables = {
+                "path": path,
+                "operation": operation,
+                "identifier": identifier,
+                "rootLocation": rootLocation
+            }
+            return render_template("index.html", **variables)
+        
         
         #--- start webserver ---
         #app.run(host=self.config["api"].get("host", "::"), port=self.config["api"].get("port", "8080"), 
         #        debug=self.config.getboolean("api","debug"), 
         #        use_reloader=False)   
         serve(app, 
               host=self.config["api"].get("host", "::"), 
               port=self.config["api"].get("port", "8080"), 
               threads=self.config["api"].get("threads", "10"))                            
         
         
-        
+
```

### Comparing `haplotyping-0.0.5/haplotyping/service/api_country.py` & `haplotyping-0.0.6/haplotyping/service/api_country.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/service/api_dataset.py` & `haplotyping-0.0.6/haplotyping/service/api_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                                        "min": item["variety_year_min"], 
                                        "max": item["variety_year_max"]}
     else:
         item["variety"] = None
     del item["variety_uid"]
     del item["variety_name"]
     del item["variety_origin"]
+    del item["variety_country"]
     del item["variety_year_min"]
     del item["variety_year_max"]
     #collection
     if item["collection_uid"]:
         item["collection"] = {
             "uid": item["collection_uid"], 
             "name": item["collection_name"]
@@ -112,14 +113,16 @@
                             LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` \
                             LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` \
                             WHERE "+condition_sql, tuple(condition_variables))  
             total = cursor.fetchone()[0]
             if start<total:
                 cursor.execute("SELECT `dataset`.`uid`, \
                                 `dataset`.`type`, \
+                                `dataset`.`subtype`, \
+                                `dataset`.`version`, \
                                 `collection`.`uid` AS `collection_uid`, \
                                 `collection`.`name` AS `collection_name`, \
                                 `variety`.`uid` AS `variety_uid`, \
                                 `variety`.`name` AS `variety_name`, \
                                 `variety`.`origin` AS `variety_origin`, \
                                 `country`.`name` AS `variety_country`, \
                                 `variety`.`year_min` AS `variety_year_min`, \
@@ -158,14 +161,16 @@
                                 LEFT JOIN `variety` ON `dataset`.`variety` = `variety`.`uid` \
                                 LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` \
                                 LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` \
                                 WHERE "+condition_sql, tuple(condition_variables))  
                 total = cursor.fetchone()[0]
                 cursor.execute("SELECT `dataset`.`uid`, \
                                 `dataset`.`type`, \
+                                `dataset`.`subtype`, \
+                                `dataset`.`version`, \
                                 `collection`.`uid` AS `collection_uid`, \
                                 `collection`.`name` AS `collection_name`, \
                                 `variety`.`uid` AS `variety_uid`, \
                                 `variety`.`name` AS `variety_name`, \
                                 `variety`.`origin` AS `variety_origin`, \
                                 `country`.`name` AS `variety_country`, \
                                 `variety`.`year_min` AS `variety_year_min`, \
@@ -196,14 +201,16 @@
     def get(self,uid):
         try:
             db_connection = haplotyping.service.API.get_db_connection()
             db_connection.row_factory = sqlite3.Row
             cursor = db_connection.cursor()
             cursor.execute("SELECT `dataset`.`uid`, \
                             `dataset`.`type`, \
+                            `dataset`.`subtype`, \
+                            `dataset`.`version`, \
                             `collection`.`uid` AS `collection_uid`, \
                             `collection`.`name` AS `collection_name`, \
                             `variety`.`uid` AS `variety_uid`, \
                             `variety`.`name` AS `variety_name`, \
                             `variety`.`origin` AS `variety_origin`, \
                             `country`.`name` AS `variety_country`, \
                             `variety`.`year_min` AS `variety_year_min`, \
```

### Comparing `haplotyping-0.0.5/haplotyping/service/api_kmer.py` & `haplotyping-0.0.6/haplotyping/service/api_kmer.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,18 +182,18 @@
         distance = max(1,int(request.args.get("distance",1000)))
         minimumFrequency = max(1,int(request.args.get("minimumFrequency",1)))
         try:
             data = _getDataset(uid)
             if data:
                 if not data["collection_location"]==None:
                     location_kmc = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["collection_location"],data["dataset_location"],"kmer.kmc")
+                                   data["collection_location"],data["dataset_location"],"kmer.kmc")
                 else:
                     location_kmc = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["dataset_location"],"kmer.kmc")
+                                   data["dataset_location"],"kmer.kmc")
                 kmc_query_library = haplotyping.service.API.get_kmc_query_library()
                 kmc_query_binary_location = haplotyping.service.API.get_kmc_query_binary_location()
                 #construct path
                 newKmer = kmer1
                 path = kmer1
                 for i in range(distance):
                     rightNeighbours = set()
@@ -201,17 +201,20 @@
                         rightNeighbours.add(newKmer[1:]+rb)
                     kmerList = list(rightNeighbours)                    
                     if kmc_query_library:
                         data = KmerKMC.kmc_library(kmc_query_library,location_kmc,kmerList,0)
                         if not data:
                             abort(500,"no response using kmc query library for "+str(kmerList))
                     elif kmc_query_binary_location:
-                        kmc_query_binary_location_query = os.path.join(kmc_query_binary_location,"kmc_query")
-                        kmc_query_binary_location_analysis = os.path.join(kmc_query_binary_location,"kmc_analysis")
-                        data = KmerKMC.kmc_binary_frequencies(kmc_query_binary_location_query,location_kmc,kmerList,0)
+                        kmc_query_binary_location_query = os.path.join(
+                            kmc_query_binary_location,"kmc_query")
+                        kmc_query_binary_location_analysis = os.path.join(
+                            kmc_query_binary_location,"kmc_analysis")
+                        data = KmerKMC.kmc_binary_frequencies(
+                            kmc_query_binary_location_query,location_kmc,kmerList,0)
                         if not data:
                             abort(500,"no response using kmc query binary for "+str(kmerList))
                     else:
                         abort(500,"no kmc binary or library configured")
                     #analyse result
                     kmerFound = [k for k in data["kmers"].keys() if data["kmers"][k]>=minimumFrequency]
                     rightSplitters = [k for k in rightNeighbours if k in kmerFound or 
@@ -222,29 +225,31 @@
                     elif kmer2 in rightSplitters:
                         for rightSplitter in rightSplitters:
                             if rightSplitter==kmer2:
                                 path = path + rightSplitter[-1]                                
                     else:
                         return None
                     if kmer2==path[-len(kmer2):]:
-                        return Response(json.dumps(path), mimetype="application/json")                    
+                        return Response(json.dumps(path), mimetype="application/json")
                 else:
                     return None
             else:
                 abort(404, "no dataset with k-mers for uid "+str(uid))
         except Exception as e:
             abort(e.code if hasattr(e,"code") else 500, str(e))
         
             
 @namespace.route("/<uid>")
 class KmerMultiple(Resource):            
                 
     dataset_kmers = namespace.model("k-mer list to get frequencies", {
-        "kmers": fields.List(fields.String, attribute="items", required=True, description="list of k-mers"),
-        "mismatches": fields.Integer(min=0,max=2, required=False, description="maximum number of mismatches")
+        "kmers": fields.List(fields.String, attribute="items", default=[],
+                            required=True, description="list of k-mers"),
+        "mismatches": fields.Integer(min=0,max=2, default=0, 
+                            required=False, description="maximum number of mismatches")
     })
                 
     @namespace.doc(description="Get k-mer frequencies from dataset defined by uid")
     @namespace.expect(dataset_kmers)
     @namespace.doc(params={"uid": "unique identifier dataset"})
     @cache.cached(make_cache_key=_make_cache_key)
     def post(self,uid):
@@ -281,53 +286,74 @@
             abort(e.code if hasattr(e,"code") else 500, str(e))
         
             
 @namespace.route("/<uid>/sequence")
 class KmerSequence(Resource):            
                 
     sequence_data = namespace.model("sequence to get k-mer frequencies", {"sequence": 
-                                            fields.String(required=True, description="sequence"),
-                                    "mismatches": fields.Integer(min=0,max=2, required=False, 
-                                                                 description="maximum number of mismatches")})
+                                            fields.String(required=False, default="", 
+                                            description="sequence"),
+                                    "sequences": fields.List(fields.String, attribute="items", 
+                                            required=False, default=[],
+                                            description="list of sequences"),           
+                                    "mismatches": fields.Integer(min=0, max=2, 
+                                            default=0, required=False, 
+                                            description="maximum number of mismatches")})
     
     @namespace.doc(description="Get k-mer frequencies for a sequence from dataset defined by uid")
     @namespace.doc(params={"uid": "unique identifier dataset"})
     @namespace.expect(sequence_data)
     @cache.cached(make_cache_key=_make_cache_key)
     def post(self,uid):  
         mm = min(2,max(0,namespace.payload.get("mismatches",0)))
         sequence = namespace.payload.get("sequence","")
-        kmers = []
+        sequences = namespace.payload.get("sequences",[])
+        def getKmers(k,sequence,sequences):
+            kmers = []
+            if k>0:
+                for i in range(len(sequence)-(k-1)):
+                    kmer = sequence[i:i+k]
+                    if not kmer in kmers:
+                        kmers.append(kmer)
+                for item in sequences:
+                    for i in range(len(item)-(k-1)):
+                        kmer = item[i:i+k]
+                        if not kmer in kmers:
+                            kmers.append(kmer)
+            return kmers
         try:
             data = _getDataset(uid)
             if data:
                 if not data["collection_location"]==None:
                     location_kmc = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["collection_location"],data["dataset_location"],"kmer.kmc")
+                                     data["collection_location"],data["dataset_location"],"kmer.kmc")
                 else:
                     location_kmc = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["dataset_location"],"kmer.kmc")
+                                     data["dataset_location"],"kmer.kmc")
                 kmc_query_library = haplotyping.service.API.get_kmc_query_library()
                 kmc_query_binary_location = haplotyping.service.API.get_kmc_query_binary_location()
                 if kmc_query_library:
                     response = KmerKMC.kmc_library(kmc_query_library,location_kmc,[],0)
                     if not response:
                         abort(500,"no response using kmc query library")
                     k = response["info"].get("kmer_length",0)
-                    kmers = [sequence[i:i+k] for i in range(len(sequence)-(k-1)) if k>0]
+                    kmers = getKmers(k,sequence,sequences)
                     response = KmerKMC.kmc_library(kmc_query_library,location_kmc,kmers,mm)
                     if not response:
                         abort(500,"no response using kmc query library for "+str(kmers))
                 elif kmc_query_binary_location:
-                    kmc_query_binary_location_query = os.path.join(kmc_query_binary_location,"kmc_query")
-                    kmc_query_binary_location_analysis = os.path.join(kmc_query_binary_location,"kmc_analysis")
+                    kmc_query_binary_location_query = os.path.join(
+                        kmc_query_binary_location,"kmc_query")
+                    kmc_query_binary_location_analysis = os.path.join(
+                        kmc_query_binary_location,"kmc_analysis")
                     info = KmerKMC.kmc_binary_info(kmc_query_binary_location_analysis,location_kmc)
                     k = info.get("kmer_length",0)
-                    kmers = [sequence[i:i+k] for i in range(len(sequence)-(k-1)) if k>0]
-                    response = KmerKMC.kmc_binary_frequencies(kmc_query_binary_location_query,location_kmc,kmers,mm)
+                    kmers = getKmers(k,sequence,sequences)
+                    response = KmerKMC.kmc_binary_frequencies(
+                        kmc_query_binary_location_query,location_kmc,kmers,mm)
                     response["info"] = info;
                     if not response:
                         abort(500,"no response using kmc query binary for "+str(kmers))
                 else:
                     abort(500,"no kmc binary or library configured")
                 return Response(json.dumps(response), mimetype="application/json")                
             else:
```

### Comparing `haplotyping-0.0.5/haplotyping/service/api_marker.py` & `haplotyping-0.0.6/haplotyping/service/api_marker.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 def getDataset(uid):
     db_connection = haplotyping.service.API.get_db_connection()
     db_connection.row_factory = sqlite3.Row
     cursor = db_connection.cursor()
     cursor.execute("SELECT `dataset`.`uid`, \
                     `dataset`.`type`, \
+                    `dataset`.`subtype`, \
+                    `dataset`.`version`, \
                     `dataset`.`internal_id`, \
                     `dataset`.`location` AS `dataset_location`, \
                     `collection`.`location` AS `collection_location` \
                     FROM `dataset` \
                     LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` \
                     WHERE `dataset`.`uid` = ? \
                     AND `dataset`.`type` = 'marker' \
```

### Comparing `haplotyping-0.0.5/haplotyping/service/api_split.py` & `haplotyping-0.0.6/haplotyping/service/api_split.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 def _getDataset(uid):
     db_connection = haplotyping.service.API.get_db_connection()
     db_connection.row_factory = sqlite3.Row
     cursor = db_connection.cursor()
     cursor.execute("SELECT `dataset`.`uid`, \
                     `dataset`.`type`, \
+                    `dataset`.`subtype`, \
+                    `dataset`.`version`, \
                     `dataset`.`location` AS `dataset_location`, \
                     `collection`.`location` AS `collection_location` \
                     FROM `dataset` \
                     LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` \
                     WHERE `dataset`.`uid` = ? \
                     AND (`dataset`.`type` = 'kmer' OR `dataset`.`type` = 'split') \
                     AND NOT `collection`.`location` IS NULL",(str(uid),))  
@@ -156,66 +158,14 @@
                 response = Split.kmer_list_direct(location_split, kmers)
                 return Response(json.dumps(response), mimetype="application/json")                
             else:
                 abort(404, "no dataset with splitting k-mers for uid "+str(uid))
         except Exception as e:
             abort(e.code if hasattr(e,"code") else 500, str(e))  
             
-@namespace.route("/<uid>/kmer/connected/<kmer>")
-class SplitKmerConnectedSingle(Resource):
-    
-    @namespace.doc(description="Get connected splitting k-mers from dataset defined by uid containing specified k-mer")
-    @namespace.doc(params={"uid": "unique identifier dataset","kmer": "splitting k-mer"})
-    @cache.cached(make_cache_key=_make_cache_key)
-    def get(self,uid,kmer):
-        try:
-            data = _getDataset(uid)
-            if data:
-                if not data["collection_location"]==None:
-                    location_split = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["collection_location"],data["dataset_location"],"kmer.data.h5")
-                else:
-                    location_split = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["dataset_location"],"kmer.data.h5")
-                response = Split.kmer_connected(location_split, kmer)
-                return Response(json.dumps(response), mimetype="application/json")                
-            else:
-                abort(404, "no dataset with splitting k-mers for uid "+str(uid))
-        except Exception as e:
-            abort(e.code if hasattr(e,"code") else 500, str(e))      
-            
-@namespace.route("/<uid>/kmer/connected")
-class SplitKmerConnectedMultiple(Resource):
-    
-    dataset_kmers = namespace.model("k-mer list to get connected splitting k-mers", {
-        "kmers": fields.List(fields.String, attribute="items", required=True, description="list of k-mers")
-    })
-    
-    @namespace.doc(description="Get connected splitting k-mers for a list of k-mers from dataset defined by uid")
-    @namespace.doc(params={"uid": "unique identifier dataset"})
-    @namespace.expect(dataset_kmers)
-    @cache.cached(make_cache_key=_make_cache_key)
-    def post(self,uid):
-        kmers = namespace.payload.get("kmers",[])
-        try:
-            data = _getDataset(uid)
-            if data:
-                if not data["collection_location"]==None:
-                    location_split = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["collection_location"],data["dataset_location"],"kmer.data.h5")
-                else:
-                    location_split = os.path.join(haplotyping.service.API.get_data_kmer_location(),
-                                                data["dataset_location"],"kmer.data.h5")
-                response = Split.kmer_list_connected(location_split, kmers)
-                return Response(json.dumps(response), mimetype="application/json")                
-            else:
-                abort(404, "no dataset with splitting k-mers for uid "+str(uid))
-        except Exception as e:
-            abort(e.code if hasattr(e,"code") else 500, str(e))              
-            
 @namespace.route("/<uid>/kmer/sequence")
 class SplitKmerSequence(Resource):
     
     sequence_data = namespace.model("sequence to get splitting k-mer information", {"sequence": 
                                             fields.String(required=True, description="sequence")})
     
     @namespace.doc(description="Get splitting k-mer information for a sequence from dataset defined by uid")
```

### Comparing `haplotyping-0.0.5/haplotyping/service/api_tools.py` & `haplotyping-0.0.6/haplotyping/service/api_tools.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/service/api_variety.py` & `haplotyping-0.0.6/haplotyping/service/api_variety.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 yearRangePattern = re.compile(r"^[\d]{4}\-[\d]{4}$")
 
 def _make_bool(text):
     return str(text).lower() in ("yes", "true", "t", "1")
 
 def get_variety_datasets(uid, collection, dataset, db_connection):
     condition_variables = [uid]
-    condition_sql = "`dataset`.`variety` = ? \
-                        AND (NOT `dataset`.`uid` IS NULL) AND (NOT `dataset`.`type` IS NULL)"
+    condition_sql = """`dataset`.`variety` = ? 
+                        AND (NOT `dataset`.`uid` IS NULL) AND (NOT `dataset`.`type` IS NULL)"""
     if not collection==None:
         collection_list = collection.split(",")
         condition_sql = condition_sql + " AND (`collection`.`uid` IN ("+",".join(["?"]*len(collection_list))+"))"
         condition_variables.extend(collection_list)
     if not dataset==None:
         if dataset=="any":
             condition_sql = condition_sql + " AND NOT (`dataset`.`id` IS NULL)"
@@ -31,23 +31,25 @@
         elif dataset=="split":
             condition_sql = condition_sql + " AND (`dataset`.`type` IS 'split')" 
         elif dataset=="marker":
             condition_sql = condition_sql + " AND (`dataset`.`type` IS 'marker')" 
         else:
             abort(422, "incorrect dataset condition "+str(dataset))
     cursor = db_connection.cursor()
-    cursor.execute("SELECT `dataset`.`uid`, \
-                           `dataset`.`type`, \
-                           `collection`.`uid` AS `collection_uid`, \
-                           `collection`.`name` AS `collection_name`, \
-                           `collection`.`type` AS `collection_type`, \
-                           `collection`.`experiment` AS `collection_experiment` \
-                        FROM `dataset` \
-                        LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` \
-                        WHERE "+condition_sql+" ORDER BY `collection`.`name`, `dataset`.`uid`", 
+    cursor.execute("""SELECT `dataset`.`uid`, 
+                           `dataset`.`type`, 
+                           `dataset`.`subtype`, 
+                           `dataset`.`version`, 
+                           `collection`.`uid` AS `collection_uid`, 
+                           `collection`.`name` AS `collection_name`, 
+                           `collection`.`type` AS `collection_type`, 
+                           `collection`.`experiment` AS `collection_experiment` 
+                        FROM `dataset` 
+                        LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` 
+                        WHERE """+condition_sql+""" ORDER BY `collection`.`name`, `dataset`.`uid`""", 
                    tuple(condition_variables)) 
     return [dict(row) for row in cursor.fetchall()]  
 
 def parents_tree(id,parentData):
     parents = []   
     for item in parentData:
         if item["offspring"]==id:
@@ -72,27 +74,27 @@
             "direct": True if item["offspring"]==None else False
         }
         offspring.append(offspring_item)
     return offspring
         
 def get_variety_parents(uid, db_connection):
     cursor = db_connection.cursor()
-    cursor.execute("SELECT `variety_ancestor`.*, `variety`.`name` FROM `variety_ancestor` \
-                    LEFT JOIN `variety` ON `variety_ancestor`.`ancestor` = `variety`.`uid` \
-                    WHERE `variety_ancestor`.`variety` = ? \
-                    ORDER BY `variety_ancestor`.`type` DESC",(uid,)) 
+    cursor.execute("""SELECT `variety_ancestor`.*, `variety`.`name` FROM `variety_ancestor` 
+                    LEFT JOIN `variety` ON `variety_ancestor`.`ancestor` = `variety`.`uid` 
+                    WHERE `variety_ancestor`.`variety` = ? 
+                    ORDER BY `variety_ancestor`.`type` DESC""",(uid,)) 
     parentData = [dict(row) for row in cursor.fetchall()]
     return parents_tree(None,parentData)
 
 def get_variety_offspring(uid, db_connection):
     cursor = db_connection.cursor()
-    cursor.execute("SELECT `variety_ancestor`.*, `variety`.`name` FROM `variety_ancestor` \
-                    LEFT JOIN `variety` ON `variety_ancestor`.`variety` = `variety`.`uid` \
-                    WHERE `variety_ancestor`.`ancestor` = ? \
-                    ORDER BY `variety`.`name`, `variety`.`uid`",(uid,)) 
+    cursor.execute("""SELECT `variety_ancestor`.*, `variety`.`name` FROM `variety_ancestor` 
+                    LEFT JOIN `variety` ON `variety_ancestor`.`variety` = `variety`.`uid` 
+                    WHERE `variety_ancestor`.`ancestor` = ? 
+                    ORDER BY `variety`.`name`, `variety`.`uid`""",(uid,)) 
     offspringData = [dict(row) for row in cursor.fetchall()]
     return offspring_list(offspringData)
 
 def year_description(year_min,year_max):
     if year_min==None and year_max==None:
         return None
     elif year_min==None:
@@ -148,14 +150,16 @@
     variety_list = parser.copy()
     variety_list.add_argument("start", type=int, required=False, location="args", 
                               help="paging")       
     variety_list.add_argument("number", type=int, required=False, location="args", 
                               help="paging")
     variety_list.add_argument("name", type=str, required=False, location="args", 
                               help="name of variety")
+    variety_list.add_argument("nameContains", type=str, required=False, location="args", 
+                              help="name of variety contains (only if no name condition)")
     variety_list.add_argument("origin", type=str, required=False, location="args", 
                               help="comma separated list of country codes")
     variety_list.add_argument("year", type=str, required=False, location="args", 
                               help="year of variety (e.g. '1995', '<1995', '>1995', '1990-1995')")
     variety_list.add_argument("collection", type=str, required=False, location="args", 
                               help="variety has dataset from comma separated list of collection uids")
     variety_list.add_argument("dataType", type=str, required=False, location="args", 
@@ -171,14 +175,15 @@
     @namespace.doc(description="Get varieties")    
     @namespace.expect(variety_list)
     def get(self):
         try:
             start = int(request.args.get("start",0))
             number = int(request.args.get("number",10))        
             name = request.args.get("name",None)
+            nameContains = request.args.get("nameContains",None)
             origin = request.args.get("origin",None)
             year = request.args.get("year",None)
             collection = request.args.get("collection",None)
             dataType = request.args.get("dataType",None)
             hasParents = request.args.get("hasParents",None)
             hasOffspring = request.args.get("hasOffspring",None)
             condition_sql = "1"
@@ -238,47 +243,47 @@
                 if _make_bool(hasOffspring):
                     condition_sql = condition_sql + " AND NOT (`offspring`.`id` IS NULL)"
                 else:
                     condition_sql = condition_sql + " AND (`offspring`.`id` IS NULL)"     
             db_connection = haplotyping.service.API.get_db_connection()
             db_connection.row_factory = sqlite3.Row
             cursor = db_connection.cursor()
-            cursor.execute("SELECT COUNT(DISTINCT `variety`.`id`) AS `number` \
-                            FROM `variety` \
-                            LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` \
-                            AND NOT `dataset`.`uid` IS NULL AND NOT `dataset`.`type` IS NULL \
-                            LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` \
-                            LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` \
-                            LEFT JOIN `variety_ancestor` AS `ancestor` ON `variety`.`uid` = `ancestor`.`variety` \
-                            LEFT JOIN `variety_ancestor` AS `offspring` ON `variety`.`uid` = `offspring`.`ancestor` \
-                            LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` \
-                            LEFT JOIN `variety_synonym` AS `condition_synonym` ON `variety`.`uid` = \
-                                        `condition_synonym`.`uid` \
-                            WHERE "+condition_sql, tuple(condition_variables))  
+            cursor.execute("""SELECT COUNT(DISTINCT `variety`.`id`) AS `number` 
+                            FROM `variety` 
+                            LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` 
+                            AND NOT `dataset`.`uid` IS NULL AND NOT `dataset`.`type` IS NULL 
+                            LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` 
+                            LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` 
+                            LEFT JOIN `variety_ancestor` AS `ancestor` ON `variety`.`uid` = `ancestor`.`variety` 
+                            LEFT JOIN `variety_ancestor` AS `offspring` ON `variety`.`uid` = `offspring`.`ancestor` 
+                            LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` 
+                            LEFT JOIN `variety_synonym` AS `condition_synonym` ON `variety`.`uid` = 
+                                        `condition_synonym`.`uid` 
+                            WHERE """ + condition_sql, tuple(condition_variables))  
             total = cursor.fetchone()[0]
             if start<total:
-                cursor.execute("SELECT `variety`.`uid`, `variety`.`name`, `variety`.`origin`, \
-                                `country`.`name` AS `country`, \
-                                NULL AS `year`, `variety`.`year_min`, `variety`.`year_max`, \
-                                GROUP_CONCAT(DISTINCT `synonym`.`synonym`) AS `synonyms`, \
-                                COUNT(DISTINCT `dataset`.`id`) as `datasets` \
-                                FROM `variety` \
-                                LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` \
-                                AND NOT `dataset`.`uid` IS NULL AND NOT `dataset`.`type` IS NULL\
-                                LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` \
-                                LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` \
-                                LEFT JOIN `variety_ancestor` AS `ancestor` ON `variety`.`uid` = `ancestor`.`variety` \
-                                LEFT JOIN `variety_ancestor` AS `offspring` ON `variety`.`uid` = `offspring`.`ancestor` \
-                                LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` \
-                                LEFT JOIN `variety_synonym` AS `condition_synonym` ON `variety`.`uid` = \
-                                            `condition_synonym`.`uid` \
-                                WHERE "+condition_sql+" \
-                                GROUP BY `variety`.`id` \
-                                ORDER BY `variety`.`name`, `variety`.`uid` \
-                                LIMIT ?,?",tuple(condition_variables + [start,number]))  
+                cursor.execute("""SELECT `variety`.`uid`, `variety`.`name`, `variety`.`origin`, 
+                                `country`.`name` AS `country`, 
+                                NULL AS `year`, `variety`.`year_min`, `variety`.`year_max`, 
+                                GROUP_CONCAT(DISTINCT `synonym`.`synonym`) AS `synonyms`, 
+                                COUNT(DISTINCT `dataset`.`id`) as `datasets` 
+                                FROM `variety` 
+                                LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` 
+                                AND NOT `dataset`.`uid` IS NULL AND NOT `dataset`.`type` IS NULL
+                                LEFT JOIN `collection` ON `dataset`.`collection_id` = `collection`.`id` 
+                                LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` 
+                                LEFT JOIN `variety_ancestor` AS `ancestor` ON `variety`.`uid` = `ancestor`.`variety` 
+                                LEFT JOIN `variety_ancestor` AS `offspring` ON `variety`.`uid` = `offspring`.`ancestor` 
+                                LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` 
+                                LEFT JOIN `variety_synonym` AS `condition_synonym` ON `variety`.`uid` = 
+                                            `condition_synonym`.`uid` 
+                                WHERE """+condition_sql+""" 
+                                GROUP BY `variety`.`id` 
+                                ORDER BY `variety`.`name`, `variety`.`uid` 
+                                LIMIT ?,?""",tuple(condition_variables + [start,number]))  
                 resultList = [dict(row) for row in cursor.fetchall()]
             else:
                 resultList = []
             for i in range(len(resultList)):
                 resultList[i] = adjust_variety_response(resultList[i], collection, dataType, db_connection)                
             response = {"start": start, "number": number, "total": total, "list": resultList}
             return Response(json.dumps(response), mimetype="application/json") 
@@ -292,35 +297,35 @@
         try:
             if len(uids)>0:
                 condition_sql = "`variety`.`uid` IN ("+(",".join(["?"]*len(uids)))+")"
                 condition_variables = [] + uids;
                 db_connection = haplotyping.service.API.get_db_connection()
                 db_connection.row_factory = sqlite3.Row
                 cursor = db_connection.cursor()
-                cursor.execute("SELECT COUNT(DISTINCT `variety`.`id`) AS `number` \
-                                FROM `variety` \
-                                LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` \
-                                AND NOT (`dataset`.`uid` IS NULL) AND NOT (`dataset`.`type` IS NULL) \
-                                LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` \
-                                LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` \
-                                WHERE "+condition_sql, tuple(condition_variables))  
+                cursor.execute("""SELECT COUNT(DISTINCT `variety`.`id`) AS `number` 
+                                FROM `variety` 
+                                LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` 
+                                AND NOT (`dataset`.`uid` IS NULL) AND NOT (`dataset`.`type` IS NULL) 
+                                LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` 
+                                LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` 
+                                WHERE """+condition_sql, tuple(condition_variables))  
                 total = cursor.fetchone()[0]
-                cursor.execute("SELECT `variety`.`uid`, `variety`.`name`, `variety`.`origin`, \
-                                `country`.`name` AS `country`, \
-                                NULL AS `year`, `variety`.`year_min`, `variety`.`year_max`, \
-                                GROUP_CONCAT(DISTINCT `synonym`.`synonym`) AS `synonyms`, \
-                                COUNT(DISTINCT `dataset`.`id`) as `datasets` \
-                                FROM `variety` \
-                                LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` \
-                                AND NOT (`dataset`.`uid` IS NULL) AND NOT (`dataset`.`type` IS NULL) \
-                                LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` \
-                                LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` \
-                                WHERE "+condition_sql+" \
-                                GROUP BY `variety`.`id` \
-                                ORDER BY `variety`.`name`, `variety`.`uid`",tuple(condition_variables))  
+                cursor.execute("""SELECT `variety`.`uid`, `variety`.`name`, `variety`.`origin`, 
+                                `country`.`name` AS `country`, 
+                                NULL AS `year`, `variety`.`year_min`, `variety`.`year_max`, 
+                                GROUP_CONCAT(DISTINCT `synonym`.`synonym`) AS `synonyms`, 
+                                COUNT(DISTINCT `dataset`.`id`) as `datasets` 
+                                FROM `variety` 
+                                LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` 
+                                AND NOT (`dataset`.`uid` IS NULL) AND NOT (`dataset`.`type` IS NULL) 
+                                LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` 
+                                LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` 
+                                WHERE """+condition_sql+""" 
+                                GROUP BY `variety`.`id` 
+                                ORDER BY `variety`.`name`, `variety`.`uid`""",tuple(condition_variables))  
                 resultList = [dict(row) for row in cursor.fetchall()]
             else:
                 total = 0
                 resultList = []
             for i in range(len(resultList)):
                 resultList[i] = adjust_variety_response(resultList[i], None, None, db_connection)                
             response = {"total": total, "list": resultList}
@@ -334,26 +339,26 @@
     
     @namespace.doc(description="Get variety by uid")
     def get(self,uid):
         try:
             db_connection = haplotyping.service.API.get_db_connection()
             db_connection.row_factory = sqlite3.Row
             cursor = db_connection.cursor()
-            cursor.execute("SELECT `variety`.`uid`, `variety`.`name`, `variety`.`origin`, \
-                            `country`.`name` AS `country`, \
-                            GROUP_CONCAT(DISTINCT `synonym`.`synonym`) AS `synonyms`, \
-                            NULL AS `year`, `variety`.`year_min`, `variety`.`year_max`, \
-                            NULL as `datasets` \
-                            FROM `variety` \
-                            LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` \
-                            AND NOT (`dataset`.`uid` IS NULL) AND NOT (`dataset`.`type` IS NULL) \
-                            LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` \
-                            LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` \
-                            WHERE `variety`.`uid` = ? \
-                            GROUP BY `variety`.`id`",(uid,))  
+            cursor.execute("""SELECT `variety`.`uid`, `variety`.`name`, `variety`.`origin`, 
+                            `country`.`name` AS `country`, 
+                            GROUP_CONCAT(DISTINCT `synonym`.`synonym`) AS `synonyms`, 
+                            NULL AS `year`, `variety`.`year_min`, `variety`.`year_max`, 
+                            NULL as `datasets` 
+                            FROM `variety` 
+                            LEFT JOIN `dataset` ON `variety`.`uid` = `dataset`.`variety` 
+                            AND NOT (`dataset`.`uid` IS NULL) AND NOT (`dataset`.`type` IS NULL) 
+                            LEFT JOIN `country` ON `variety`.`origin` = `country`.`uid` 
+                            LEFT JOIN `variety_synonym` AS `synonym` ON `variety`.`uid` = `synonym`.`uid` 
+                            WHERE `variety`.`uid` = ? 
+                            GROUP BY `variety`.`id`""",(uid,))  
             data = cursor.fetchone()
             if data:
                 response = adjust_variety_response(dict(data), None, None, db_connection)
                 return Response(json.dumps(response), mimetype="application/json")
             else:
                 abort(404, "no variety with uid "+str(uid))
         except Exception as e:
```

### Comparing `haplotyping-0.0.5/haplotyping/service/kmer_kmc.py` & `haplotyping-0.0.6/haplotyping/service/kmer_kmc.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/service/marker.py` & `haplotyping-0.0.6/haplotyping/service/marker.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping/service/split.py` & `haplotyping-0.0.6/haplotyping/service/split.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/haplotyping.egg-info/SOURCES.txt` & `haplotyping-0.0.6/haplotyping.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 haplotyping/graph/__init__.py
 haplotyping/graph/api.py
 haplotyping/graph/baseGraph.py
 haplotyping/graph/sections.py
 haplotyping/graph/sequence.py
 haplotyping/index/__init__.py
 haplotyping/index/database.py
-haplotyping/index/reads.py
+haplotyping/index/direct.py
 haplotyping/index/splits.py
 haplotyping/index/storage.py
 haplotyping/service/__init__.py
 haplotyping/service/api.py
 haplotyping/service/api_collection.py
 haplotyping/service/api_country.py
 haplotyping/service/api_dataset.py
```

### Comparing `haplotyping-0.0.5/setup.py` & `haplotyping-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,18 +24,20 @@
       "tables >= 3.7.0",
       "pyahocorasick >= 1.4.4",
       "flask >= 2.2.2",
       "flask-restx >= 1.0.3",
       "waitress >= 2.1.2",
       "flask-caching >= 2.0.1",
       "openpyxl >= 3.0.10",
-      "frictionless >= 4.40.8"
+      "frictionless == 5.10.5",
+      "psutil >= 5.9.5",
+      "metis >= 0.2a5"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     test_suite="tests",
     include_package_data=True,
     package_data={"": ["data/schema/*.json"]},
 )
```

### Comparing `haplotyping-0.0.5/tests/index/test_database.py` & `haplotyping-0.0.6/tests/index/test_database.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/tests/service/test_api.py` & `haplotyping-0.0.6/tests/service/test_api.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.5/tests/test_general.py` & `haplotyping-0.0.6/tests/test_general.py`

 * *Files identical despite different names*

