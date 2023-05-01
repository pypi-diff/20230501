# Comparing `tmp/gosdk-0.8.18.tar.gz` & `tmp/gosdk-0.9.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gosdk-0.8.18.tar", last modified: Mon Apr  1 15:18:08 2019, max compression
+gzip compressed data, was "gosdk-0.9.23.tar", last modified: Mon May  1 19:53:05 2023, max compression
```

## Comparing `gosdk-0.8.18.tar` & `gosdk-0.9.23.tar`

### file list

```diff
@@ -1,344 +1,398 @@
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/
--rw-r--r--   0 ian        (501) staff       (20)     3815 2019-04-01 15:18:08.000000 gosdk-0.8.18/PKG-INFO
--rw-r--r--   0 ian        (501) staff       (20)       54 2018-11-27 16:45:15.000000 gosdk-0.8.18/MANIFEST.in
--rw-r--r--   0 ian        (501) staff       (20)     1586 2019-04-01 15:04:13.000000 gosdk-0.8.18/setup_gosdk.py
--rw-r--r--   0 ian        (501) staff       (20)       38 2019-04-01 15:18:08.000000 gosdk-0.8.18/setup.cfg
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/
--rw-r--r--   0 ian        (501) staff       (20)      613 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/models.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/contents/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/contents/{uuid}/
--rw-r--r--   0 ian        (501) staff       (20)      236 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/contents/{uuid}/delete.yaml
--rw-r--r--   0 ian        (501) staff       (20)      383 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/contents/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/classifications/
--rw-r--r--   0 ian        (501) staff       (20)      425 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/classifications/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/concepts/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/concepts/alterations/
--rw-r--r--   0 ian        (501) staff       (20)      499 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/concepts/alterations/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)      372 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/curation/concepts/alterations/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/
--rw-r--r--   0 ian        (501) staff       (20)     3209 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/match/
--rw-r--r--   0 ian        (501) staff       (20)     2453 2019-01-28 21:29:34.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/match/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/detail/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/detail/{uuid}/
--rw-r--r--   0 ian        (501) staff       (20)      351 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/detail/{uuid}/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/set/
--rw-r--r--   0 ian        (501) staff       (20)      799 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/set/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/counts/
--rw-r--r--   0 ian        (501) staff       (20)     1686 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/contents/counts/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/prognoses/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/prognoses/matches/
--rw-r--r--   0 ian        (501) staff       (20)     3956 2019-01-28 21:29:34.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/prognoses/matches/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/trials/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/trials/matches/
--rw-r--r--   0 ian        (501) staff       (20)     8211 2019-01-28 21:29:34.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/trials/matches/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/transcripts/
--rw-r--r--   0 ian        (501) staff       (20)      549 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/transcripts/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/prognoses/
--rwxr-xr-x   0 ian        (501) staff       (20)      566 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/trials/
--rwxr-xr-x   0 ian        (501) staff       (20)     1705 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/
--rwxr-xr-x   0 ian        (501) staff       (20)     1528 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/markers/
--rwxr-xr-x   0 ian        (501) staff       (20)     1485 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)      382 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/like-mine/
--rwxr-xr-x   0 ian        (501) staff       (20)     2365 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/
--rwxr-xr-x   0 ian        (501) staff       (20)      780 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/content/
--rwxr-xr-x   0 ian        (501) staff       (20)      789 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/
--rwxr-xr-x   0 ian        (501) staff       (20)     3344 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/therapies/
--rwxr-xr-x   0 ian        (501) staff       (20)     1738 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/annotations/
--rwxr-xr-x   0 ian        (501) staff       (20)     1527 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/classifications/
--rwxr-xr-x   0 ian        (501) staff       (20)     1699 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/
--rwxr-xr-x   0 ian        (501) staff       (20)     3500 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/off-label/
--rwxr-xr-x   0 ian        (501) staff       (20)     1747 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)     2245 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/cases/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_variants/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_variants/{pk}/
--rw-r--r--   0 ian        (501) staff       (20)      385 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_variants/{pk}/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1625 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_variants/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)      437 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_variants/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/info/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/info/annotation_bundle/
--rw-r--r--   0 ian        (501) staff       (20)      279 2019-01-28 21:30:41.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/info/annotation_bundle/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/therapies/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/therapies/matches/
--rw-r--r--   0 ian        (501) staff       (20)     5325 2019-01-28 21:29:34.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/therapies/matches/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/
--rw-r--r--   0 ian        (501) staff       (20)     1017 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/
--rw-r--r--   0 ian        (501) staff       (20)      685 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{pk}/
--rw-r--r--   0 ian        (501) staff       (20)      373 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{pk}/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/
--rw-r--r--   0 ian        (501) staff       (20)      378 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/hgvs/
--rw-r--r--   0 ian        (501) staff       (20)     1034 2019-01-28 21:30:41.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/delete/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/
--rw-r--r--   0 ian        (501) staff       (20)      247 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/delete.yaml
--rw-r--r--   0 ian        (501) staff       (20)     2184 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/refresh/
--rw-r--r--   0 ian        (501) staff       (20)     1105 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/refresh/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{build_id}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/
--rw-r--r--   0 ian        (501) staff       (20)      821 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{identifier}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/
--rw-r--r--   0 ian        (501) staff       (20)     2278 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/load/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/load/{data_set}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/
--rw-r--r--   0 ian        (501) staff       (20)      703 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/
--rw-r--r--   0 ian        (501) staff       (20)      485 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/put.yaml
--rw-r--r--   0 ian        (501) staff       (20)      376 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/delete.yaml
--rw-r--r--   0 ian        (501) staff       (20)      402 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)      487 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/patch.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/batch/
--rw-r--r--   0 ian        (501) staff       (20)      538 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/hgvs_overrides/
--rw-r--r--   0 ian        (501) staff       (20)      558 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/merged/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/merged/{pk}/
--rw-r--r--   0 ian        (501) staff       (20)      389 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/merged/{pk}/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/{pk}/
--rw-r--r--   0 ian        (501) staff       (20)      432 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/{pk}/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)     3000 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/match/
--rw-r--r--   0 ian        (501) staff       (20)     1939 2019-01-28 21:29:34.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/match/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/users/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/users/login/
--rw-r--r--   0 ian        (501) staff       (20)      357 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/users/login/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/genes/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/genes/filter_genes/
--rw-r--r--   0 ian        (501) staff       (20)      587 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/genes/gene_boundaries/
--rw-r--r--   0 ian        (501) staff       (20)      525 2019-01-30 20:00:19.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1817 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/genes/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_features/
--rw-r--r--   0 ian        (501) staff       (20)      437 2018-12-19 15:13:45.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_features/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/alterations/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/alterations/{pk}/
--rw-r--r--   0 ian        (501) staff       (20)      412 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/alterations/{pk}/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1714 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/api/alterations/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/lab-result-attachments/
--rw-r--r--   0 ian        (501) staff       (20)      495 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/lab-result-attachments/post.yaml
--rw-r--r--   0 ian        (501) staff       (20)      677 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/search/
--rw-r--r--   0 ian        (501) staff       (20)      914 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/search/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/quick-add/
--rw-r--r--   0 ian        (501) staff       (20)     1749 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/
--rwxr-xr-x   0 ian        (501) staff       (20)      236 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/delete.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/samples/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/
--rw-r--r--   0 ian        (501) staff       (20)      399 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)      560 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/
--rw-r--r--   0 ian        (501) staff       (20)      476 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/
--rw-r--r--   0 ian        (501) staff       (20)      411 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)      588 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/
--rw-r--r--   0 ian        (501) staff       (20)      422 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/
--rw-r--r--   0 ian        (501) staff       (20)      414 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)      580 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml
--rw-r--r--   0 ian        (501) staff       (20)      354 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/
--rw-r--r--   0 ian        (501) staff       (20)     1122 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/
--rw-r--r--   0 ian        (501) staff       (20)      318 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/
--rw-r--r--   0 ian        (501) staff       (20)      339 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/
--rw-r--r--   0 ian        (501) staff       (20)     1235 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/
--rw-r--r--   0 ian        (501) staff       (20)      443 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/
--rw-r--r--   0 ian        (501) staff       (20)      493 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{uuid}/
--rwxr-xr-x   0 ian        (501) staff       (20)      230 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{uuid}/delete.yaml
--rw-r--r--   0 ian        (501) staff       (20)      338 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/post.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/uploads/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/uploads/{id}/
--rw-r--r--   0 ian        (501) staff       (20)      299 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/uploads/{id}/get.yaml
--rw-r--r--   0 ian        (501) staff       (20)      720 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/paths/consult/uploads/post.yaml
--rw-r--r--   0 ian        (501) staff       (20)      268 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/specd.yaml
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk/specs/definitions/
--rw-r--r--   0 ian        (501) staff       (20)      110 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Settings.yaml
--rw-r--r--   0 ian        (501) staff       (20)      221 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/LogicSet.yaml
--rw-r--r--   0 ian        (501) staff       (20)      115 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/UserCredentials.yaml
--rw-r--r--   0 ian        (501) staff       (20)      211 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Marker.yaml
--rw-r--r--   0 ian        (501) staff       (20)      200 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AlterationList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      203 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugGFIncludeComponent.yaml
--rw-r--r--   0 ian        (501) staff       (20)      165 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugIngredient.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1138 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AlterationsDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      386 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewLabResultDataFile.yaml
--rw-r--r--   0 ian        (501) staff       (20)      120 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewRecommendationsReport.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1930 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/TherapiesDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      535 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugPharmacology.yaml
--rw-r--r--   0 ian        (501) staff       (20)      205 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/QuickAdd.yaml
--rw-r--r--   0 ian        (501) staff       (20)      359 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugTarget.yaml
--rw-r--r--   0 ian        (501) staff       (20)      223 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DetectedAlteration.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1520 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugPolypeptide.yaml
--rw-r--r--   0 ian        (501) staff       (20)      134 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugLiteratureReference.yaml
--rw-r--r--   0 ian        (501) staff       (20)      128 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Facets.yaml
--rw-r--r--   0 ian        (501) staff       (20)      234 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AnnotationList.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)      281 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/PatientMetaData.yaml
--rw-r--r--   0 ian        (501) staff       (20)       98 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Phenotype.yaml
--rw-r--r--   0 ian        (501) staff       (20)      299 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Patient.yaml
--rw-r--r--   0 ian        (501) staff       (20)      218 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewReferenceAttachment.yaml
--rw-r--r--   0 ian        (501) staff       (20)      634 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/WarehouseVariant.yaml
--rw-r--r--   0 ian        (501) staff       (20)      165 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/RefreshCursor.yaml
--rw-r--r--   0 ian        (501) staff       (20)      287 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Content.yaml
--rw-r--r--   0 ian        (501) staff       (20)      191 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/GenesList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      168 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/definitions/GeneBoundaries.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1933 2019-01-28 21:30:41.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Annotation.yaml
--rw-r--r--   0 ian        (501) staff       (20)      469 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Evidence.yaml
--rw-r--r--   0 ian        (501) staff       (20)      105 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugGoClass.yaml
--rw-r--r--   0 ian        (501) staff       (20)      212 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/PrognosesDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      297 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewLabResult.yaml
--rw-r--r--   0 ian        (501) staff       (20)       88 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Error.yaml
--rw-r--r--   0 ian        (501) staff       (20)      216 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AnnotationsDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      145 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugModificationOf.yaml
--rw-r--r--   0 ian        (501) staff       (20)       50 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/TreatmentContexts.yaml
--rw-r--r--   0 ian        (501) staff       (20)      126 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/MatchedDisease.yaml
--rw-r--r--   0 ian        (501) staff       (20)      339 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/TherapiesDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      132 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugGeneticFactors.yaml
--rw-r--r--   0 ian        (501) staff       (20)       67 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Arguments.yaml
--rw-r--r--   0 ian        (501) staff       (20)      737 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Upload.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1578 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/PrognosesDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      377 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugStructuredIndications.yaml
--rw-r--r--   0 ian        (501) staff       (20)      124 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/OutOnlyGenesOffPanel.yaml
--rw-r--r--   0 ian        (501) staff       (20)      837 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/LabResult.yaml
--rw-r--r--   0 ian        (501) staff       (20)      302 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugGFInclude.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)      323 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewLabResultAttachmentFile.yaml
--rw-r--r--   0 ian        (501) staff       (20)      124 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NDGenes.yaml
--rw-r--r--   0 ian        (501) staff       (20)      227 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/PatientList.yaml
--rw-r--r--   0 ian        (501) staff       (20)       50 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewAlteration.yaml
--rw-r--r--   0 ian        (501) staff       (20)     3984 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/TrialsDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      244 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/UserToken.yaml
--rw-r--r--   0 ian        (501) staff       (20)      107 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugIngredientStrength.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1605 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/ClassificationsDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      678 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Gene.yaml
--rw-r--r--   0 ian        (501) staff       (20)      166 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/MarkerList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      230 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Annotations_MergedDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      210 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/ContentsDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      118 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Refs.yaml
--rw-r--r--   0 ian        (501) staff       (20)      224 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/ClassificationsDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      940 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AnnotationsDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      275 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewPatientDiagnosis.yaml
--rw-r--r--   0 ian        (501) staff       (20)      216 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AlterationsDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      318 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Location.yaml
--rw-r--r--   0 ian        (501) staff       (20)      379 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewSample.yaml
--rw-r--r--   0 ian        (501) staff       (20)      206 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/RecommendationList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      169 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AnnotationsDocumentAndNotFoundList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      165 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/LabResultDataFileList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      327 2018-12-06 18:19:43.000000 gosdk-0.8.18/src/gosdk/specs/definitions/TranscriptList.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)     1210 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/MarkersDocument.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)      384 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/LabResultAttachmentFile.yaml
--rw-r--r--   0 ian        (501) staff       (20)      137 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/HgvsGMetadata.yaml
--rw-r--r--   0 ian        (501) staff       (20)       70 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugLabeller.yaml
--rw-r--r--   0 ian        (501) staff       (20)      355 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/EligibilitiesAsCurated.yaml
--rw-r--r--   0 ian        (501) staff       (20)      180 2018-12-19 15:13:45.000000 gosdk-0.8.18/src/gosdk/specs/definitions/WarehouseFeatureList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      495 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Sample.yaml
--rw-r--r--   0 ian        (501) staff       (20)      200 2019-01-30 20:00:19.000000 gosdk-0.8.18/src/gosdk/specs/definitions/GeneBoundariesList.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1244 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/ContentsDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      820 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewClassification.yaml
--rw-r--r--   0 ian        (501) staff       (20)      377 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugClassification.yaml
--rw-r--r--   0 ian        (501) staff       (20)      180 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/WarehouseVariantList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      103 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugSeverity.yaml
--rw-r--r--   0 ian        (501) staff       (20)     2375 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewRecommendation.yaml
--rw-r--r--   0 ian        (501) staff       (20)      110 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Counts.yaml
--rw-r--r--   0 ian        (501) staff       (20)      401 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/LabResultDataFile.yaml
--rw-r--r--   0 ian        (501) staff       (20)      502 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/ReferenceAttachment.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1186 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewCase.yaml
--rw-r--r--   0 ian        (501) staff       (20)      307 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugGeneralReferences.yaml
--rw-r--r--   0 ian        (501) staff       (20)      101 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugSynonym.yaml
--rw-r--r--   0 ian        (501) staff       (20)      412 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Reference.yaml
--rw-r--r--   0 ian        (501) staff       (20)      247 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugBase.yaml
--rw-r--r--   0 ian        (501) staff       (20)      186 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/CaseList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      532 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Alteration.yaml
--rw-r--r--   0 ian        (501) staff       (20)      333 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/TrialsDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      719 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewPatient.yaml
--rw-r--r--   0 ian        (501) staff       (20)      600 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/User.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)      419 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewPatientMetaData.yaml
--rw-r--r--   0 ian        (501) staff       (20)       92 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewSelectedMarker.yaml
--rw-r--r--   0 ian        (501) staff       (20)     2161 2019-01-28 21:30:41.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      198 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/ResponseList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      802 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewContent.yaml
--rw-r--r--   0 ian        (501) staff       (20)      211 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Document.yaml
--rw-r--r--   0 ian        (501) staff       (20)      267 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/WarehouseVariantJoin.yaml
--rw-r--r--   0 ian        (501) staff       (20)      155 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NormalizedHGVSList.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1601 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/CasesDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      227 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugCondition.yaml
--rw-r--r--   0 ian        (501) staff       (20)      146 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/SelectedMarker.yaml
--rw-r--r--   0 ian        (501) staff       (20)       94 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugFdaLabel.yaml
--rw-r--r--   0 ian        (501) staff       (20)      249 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/WarehouseVariantPage.yaml
--rw-r--r--   0 ian        (501) staff       (20)      105 2019-01-28 21:30:41.000000 gosdk-0.8.18/src/gosdk/specs/definitions/AnnotationBundleVersion.yaml
--rw-r--r--   0 ian        (501) staff       (20)       50 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/OutcomeCohorts.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)      208 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/MarkersDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)     1814 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Case.yaml
--rw-r--r--   0 ian        (501) staff       (20)       99 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugExternalLink.yaml
--rwxr-xr-x   0 ian        (501) staff       (20)      204 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/CasesDocumentList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      702 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugProduct.yaml
--rw-r--r--   0 ian        (501) staff       (20)      210 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Recommendation.yaml
--rw-r--r--   0 ian        (501) staff       (20)      352 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewOncologicTreatment.yaml
--rw-r--r--   0 ian        (501) staff       (20)      434 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Eligibility.yaml
--rw-r--r--   0 ian        (501) staff       (20)      815 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewMarker.yaml
--rw-r--r--   0 ian        (501) staff       (20)      887 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugData.yaml
--rw-r--r--   0 ian        (501) staff       (20)       97 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugPfam.yaml
--rw-r--r--   0 ian        (501) staff       (20)      244 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/CountsList.yaml
--rw-r--r--   0 ian        (501) staff       (20)      443 2018-12-19 15:13:45.000000 gosdk-0.8.18/src/gosdk/specs/definitions/WarehouseFeature.yaml
--rw-r--r--   0 ian        (501) staff       (20)       88 2019-04-01 14:50:29.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NormalizedHGVS.yaml
--rw-r--r--   0 ian        (501) staff       (20)      851 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/NewDocument.yaml
--rw-r--r--   0 ian        (501) staff       (20)      335 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Classification.yaml
--rw-r--r--   0 ian        (501) staff       (20)      103 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/DrugWithDrugs.yaml
--rw-r--r--   0 ian        (501) staff       (20)      228 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/OverallContact.yaml
--rw-r--r--   0 ian        (501) staff       (20)      368 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/Pagination.yaml
--rw-r--r--   0 ian        (501) staff       (20)      344 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/specs/definitions/TimeCourse.yaml
--rw-r--r--   0 ian        (501) staff       (20)      447 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/variables.py
--rw-r--r--   0 ian        (501) staff       (20)      490 2019-04-01 15:04:30.000000 gosdk-0.8.18/src/gosdk/__init__.py
--rw-r--r--   0 ian        (501) staff       (20)     1519 2018-11-27 16:45:15.000000 gosdk-0.8.18/src/gosdk/logger.py
--rw-r--r--   0 ian        (501) staff       (20)     4026 2018-12-19 15:13:45.000000 gosdk-0.8.18/src/gosdk/construct.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk.egg-info/
--rw-r--r--   0 ian        (501) staff       (20)     3815 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk.egg-info/PKG-INFO
--rw-r--r--   0 ian        (501) staff       (20)    11904 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk.egg-info/SOURCES.txt
--rw-r--r--   0 ian        (501) staff       (20)       67 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk.egg-info/requires.txt
--rw-r--r--   0 ian        (501) staff       (20)        6 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk.egg-info/top_level.txt
--rw-r--r--   0 ian        (501) staff       (20)        1 2019-04-01 15:18:08.000000 gosdk-0.8.18/src/gosdk.egg-info/dependency_links.txt
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.323009 gosdk-0.9.23/
+-rw-r--r--   0 ian        (501) staff       (20)       54 2022-01-14 17:53:17.000000 gosdk-0.9.23/MANIFEST.in
+-rw-r--r--   0 ian        (501) staff       (20)     3148 2023-05-01 19:53:05.322879 gosdk-0.9.23/PKG-INFO
+-rw-r--r--   0 ian        (501) staff       (20)     5323 2022-01-14 17:53:17.000000 gosdk-0.9.23/README.md
+-rw-r--r--   0 ian        (501) staff       (20)       38 2023-05-01 19:53:05.323053 gosdk-0.9.23/setup.cfg
+-rw-r--r--   0 ian        (501) staff       (20)     2540 2023-04-17 13:52:06.000000 gosdk-0.9.23/setup.py
+-rw-r--r--   0 ian        (501) staff       (20)     1638 2023-05-01 19:52:46.000000 gosdk-0.9.23/setup_gosdk.py
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.223968 gosdk-0.9.23/src/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.253548 gosdk-0.9.23/src/gosdk/
+-rw-r--r--   0 ian        (501) staff       (20)      490 2023-05-01 19:52:46.000000 gosdk-0.9.23/src/gosdk/__init__.py
+-rw-r--r--   0 ian        (501) staff       (20)     4693 2022-05-11 19:59:06.000000 gosdk-0.9.23/src/gosdk/construct.py
+-rw-r--r--   0 ian        (501) staff       (20)     1519 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/logger.py
+-rw-r--r--   0 ian        (501) staff       (20)     4535 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/models.py
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.257146 gosdk-0.9.23/src/gosdk/specs/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.307358 gosdk-0.9.23/src/gosdk/specs/definitions/
+-rw-r--r--   0 ian        (501) staff       (20)      532 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Alteration.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      200 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AlterationList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1138 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AlterationsDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      216 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AlterationsDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1999 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Annotation.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      105 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationBundleVersion.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      234 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      400 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationMatch.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      239 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationMatchList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      940 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationsDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      169 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationsDocumentAndNotFoundList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      216 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationsDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      336 2022-05-11 19:59:06.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationsSVDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      157 2022-05-11 19:59:06.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationsSVDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     2161 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      230 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Annotations_MergedDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       67 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Arguments.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      208 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Assay.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      165 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/AssayList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1814 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Case.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      186 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/CaseList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1675 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/CasesDocument.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      204 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/CasesDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      335 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Classification.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1605 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/ClassificationsDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      224 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/ClassificationsDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      287 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Content.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1244 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/ContentsDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      210 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/ContentsDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      110 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Counts.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      244 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/CountsList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      223 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DetectedAlteration.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      211 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Document.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      247 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugBase.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      377 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugClassification.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      227 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugCondition.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      887 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugData.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       99 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugExternalLink.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       94 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugFdaLabel.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      302 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugGFInclude.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      203 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugGFIncludeComponent.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      307 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugGeneralReferences.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      132 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugGeneticFactors.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      105 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugGoClass.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      165 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugIngredient.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      107 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugIngredientStrength.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       70 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugLabeller.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      134 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugLiteratureReference.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      145 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugModificationOf.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       97 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugPfam.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      535 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugPharmacology.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1520 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugPolypeptide.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      702 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugProduct.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      103 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugSeverity.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      377 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugStructuredIndications.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      101 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugSynonym.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      359 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugTarget.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      103 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/DrugWithDrugs.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      355 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/EligibilitiesAsCurated.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      434 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Eligibility.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       88 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Error.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      469 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Evidence.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      128 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Facets.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      678 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Gene.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      168 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/GeneBoundaries.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      200 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/GeneBoundariesList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      191 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/GenesList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      137 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/HgvsGMetadata.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      837 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/LabResult.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      384 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/LabResultAttachmentFile.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      401 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/LabResultDataFile.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      165 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/LabResultDataFileList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      318 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Location.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      221 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/LogicSet.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      929 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Marker.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      166 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MarkerList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      178 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MarkerMetaData.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)     1210 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MarkersDocument.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      208 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MarkersDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      430 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MatchResult.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      192 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MatchedDisease.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       90 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Meeting.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      192 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MeetingList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      447 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MegaMatchResult.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      988 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MegaMatchSingleTherapyObject.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1312 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MegaMatchTherapyDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      585 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MegaMatchTrialArmObject.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      591 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/MegaMatchTrialDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      124 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NDGenes.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       50 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewAlteration.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      255 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewAssay.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1186 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewCase.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      820 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewClassification.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      802 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewContent.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      851 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      297 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewLabResult.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      323 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewLabResultAttachmentFile.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      386 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewLabResultDataFile.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      874 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewMarker.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      324 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewOncologicTreatment.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      328 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewPanel.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      845 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewPatient.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      313 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewPatientDiagnosis.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      419 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewPatientMetaData.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     2375 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewRecommendation.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      120 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewRecommendationsReport.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      218 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewReferenceAttachment.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      414 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewSample.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       92 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NewSelectedMarker.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       88 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NormalizedHGVS.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      155 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/NormalizedHGVSList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      124 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/OutOnlyGenesOffPanel.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       50 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/OutcomeCohorts.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      228 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/OverallContact.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      368 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Pagination.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      160 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Panel.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      165 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/PanelList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      299 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Patient.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      227 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/PatientList.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      281 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/PatientMetaData.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       98 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Phenotype.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1578 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/PrognosesDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      212 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/PrognosesDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      231 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/ProteinEffect.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      205 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/QuickAdd.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      210 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Recommendation.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      206 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/RecommendationList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      412 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Reference.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      502 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/ReferenceAttachment.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      165 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/RefreshCursor.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      118 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Refs.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      198 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/ResponseList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      495 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Sample.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      146 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/SelectedMarker.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      110 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Settings.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1930 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/TherapiesDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      339 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/TherapiesDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      344 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/TimeCourse.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      327 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/TranscriptList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)       50 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/TreatmentContexts.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     3984 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/TrialsDocument.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      333 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/TrialsDocumentList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      737 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/Upload.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      600 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/User.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      115 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/UserCredentials.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      244 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/UserToken.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      359 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/VariantInterpretation.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      197 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/VariantInterpretationResponse.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      360 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/VariantInterpretationSingleResponse.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      443 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/WarehouseFeature.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      180 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/WarehouseFeatureList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      634 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/WarehouseVariant.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      267 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/WarehouseVariantJoin.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      180 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/WarehouseVariantList.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      249 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/definitions/WarehouseVariantPage.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.250824 gosdk-0.9.23/src/gosdk/specs/paths/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.242568 gosdk-0.9.23/src/gosdk/specs/paths/api/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.307516 gosdk-0.9.23/src/gosdk/specs/paths/api/alterations/
+-rw-r--r--   0 ian        (501) staff       (20)     1714 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/alterations/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.307670 gosdk-0.9.23/src/gosdk/specs/paths/api/alterations/{pk}/
+-rw-r--r--   0 ian        (501) staff       (20)      412 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/alterations/{pk}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.307827 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.225303 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.225403 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.225505 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.225607 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.225709 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.307989 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/
+-rw-r--r--   0 ian        (501) staff       (20)     1017 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.226150 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/delete/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.308149 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/
+-rw-r--r--   0 ian        (501) staff       (20)      247 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/delete.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.308317 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/
+-rw-r--r--   0 ian        (501) staff       (20)      685 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     2184 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.308608 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/hgvs/
+-rw-r--r--   0 ian        (501) staff       (20)     1034 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1047 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/hgvs/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.308755 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/hgvs_overrides/
+-rw-r--r--   0 ian        (501) staff       (20)      558 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.227034 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/load/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.227139 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/load/{data_set}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.308904 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/
+-rw-r--r--   0 ian        (501) staff       (20)      703 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.309053 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/match/
+-rw-r--r--   0 ian        (501) staff       (20)     1059 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/match/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.227902 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/merged/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.309199 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/merged/{pk}/
+-rw-r--r--   0 ian        (501) staff       (20)      389 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/merged/{pk}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.309349 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/refresh/
+-rw-r--r--   0 ian        (501) staff       (20)     1105 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/refresh/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.309490 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/sv_match/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1497 2022-05-11 19:59:06.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/sv_match/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.228875 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{build_id}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.228986 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.229104 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.229422 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.309644 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/
+-rw-r--r--   0 ian        (501) staff       (20)      821 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.230006 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.309793 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/batch/
+-rw-r--r--   0 ian        (501) staff       (20)      538 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.310378 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/
+-rw-r--r--   0 ian        (501) staff       (20)      376 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/delete.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      402 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      487 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/patch.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      485 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/put.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.230378 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{identifier}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.310557 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/
+-rw-r--r--   0 ian        (501) staff       (20)     2278 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.310713 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{pk}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.310887 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/
+-rw-r--r--   0 ian        (501) staff       (20)      378 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      373 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{pk}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.311052 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/
+-rwxr-xr-x   0 ian        (501) staff       (20)     2245 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.311209 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.311373 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/annotations/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1527 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.311547 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1528 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.311714 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/classifications/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1699 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.311885 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/
+-rwxr-xr-x   0 ian        (501) staff       (20)      780 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.312045 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/content/
+-rwxr-xr-x   0 ian        (501) staff       (20)      789 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.312205 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/
+-rwxr-xr-x   0 ian        (501) staff       (20)     3344 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.312354 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/
+-rwxr-xr-x   0 ian        (501) staff       (20)     3500 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      382 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.312515 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/like-mine/
+-rwxr-xr-x   0 ian        (501) staff       (20)     2365 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.312685 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/markers/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1485 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.312847 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/off-label/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1747 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.313002 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/prognoses/
+-rwxr-xr-x   0 ian        (501) staff       (20)      566 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.313167 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/therapies/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1738 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.313327 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/trials/
+-rwxr-xr-x   0 ian        (501) staff       (20)     1705 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.313486 gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/
+-rw-r--r--   0 ian        (501) staff       (20)     3000 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.313628 gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/match/
+-rw-r--r--   0 ian        (501) staff       (20)     1939 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/match/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.313787 gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/{pk}/
+-rw-r--r--   0 ian        (501) staff       (20)      432 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/{pk}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.313934 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.314079 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/counts/
+-rw-r--r--   0 ian        (501) staff       (20)     1686 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/counts/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.239216 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/detail/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.314236 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/detail/{uuid}/
+-rw-r--r--   0 ian        (501) staff       (20)      351 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/detail/{uuid}/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     3209 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.314389 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/match/
+-rw-r--r--   0 ian        (501) staff       (20)     2453 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/match/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.314537 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/set/
+-rw-r--r--   0 ian        (501) staff       (20)      799 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/contents/set/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.314679 gosdk-0.9.23/src/gosdk/specs/paths/api/genes/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.314824 gosdk-0.9.23/src/gosdk/specs/paths/api/genes/filter_genes/
+-rw-r--r--   0 ian        (501) staff       (20)      587 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.314988 gosdk-0.9.23/src/gosdk/specs/paths/api/genes/gene_boundaries/
+-rw-r--r--   0 ian        (501) staff       (20)      525 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)     1817 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/genes/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.240264 gosdk-0.9.23/src/gosdk/specs/paths/api/info/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.315136 gosdk-0.9.23/src/gosdk/specs/paths/api/info/annotation_bundle/
+-rw-r--r--   0 ian        (501) staff       (20)      279 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/info/annotation_bundle/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.240540 gosdk-0.9.23/src/gosdk/specs/paths/api/prognoses/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.315280 gosdk-0.9.23/src/gosdk/specs/paths/api/prognoses/matches/
+-rw-r--r--   0 ian        (501) staff       (20)     3956 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/prognoses/matches/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.315431 gosdk-0.9.23/src/gosdk/specs/paths/api/region_search/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.315587 gosdk-0.9.23/src/gosdk/specs/paths/api/region_search/batch/
+-rw-r--r--   0 ian        (501) staff       (20)      439 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/region_search/batch/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      549 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/region_search/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.241405 gosdk-0.9.23/src/gosdk/specs/paths/api/therapies/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.315733 gosdk-0.9.23/src/gosdk/specs/paths/api/therapies/matches/
+-rw-r--r--   0 ian        (501) staff       (20)     5325 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/therapies/matches/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.315899 gosdk-0.9.23/src/gosdk/specs/paths/api/therapies/therapy_matches/
+-rw-r--r--   0 ian        (501) staff       (20)     4969 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/therapies/therapy_matches/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.241669 gosdk-0.9.23/src/gosdk/specs/paths/api/trials/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.316052 gosdk-0.9.23/src/gosdk/specs/paths/api/trials/matches/
+-rw-r--r--   0 ian        (501) staff       (20)     8211 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/trials/matches/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.241936 gosdk-0.9.23/src/gosdk/specs/paths/api/users/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.316203 gosdk-0.9.23/src/gosdk/specs/paths/api/users/login/
+-rw-r--r--   0 ian        (501) staff       (20)      357 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/users/login/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.242204 gosdk-0.9.23/src/gosdk/specs/paths/api/variant_interpretations/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.316357 gosdk-0.9.23/src/gosdk/specs/paths/api/variant_interpretations/generate/
+-rw-r--r--   0 ian        (501) staff       (20)     1070 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/variant_interpretations/generate/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.316517 gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_features/
+-rw-r--r--   0 ian        (501) staff       (20)      437 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_features/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.316806 gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_variants/
+-rw-r--r--   0 ian        (501) staff       (20)     1625 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_variants/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      437 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_variants/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.316960 gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_variants/{pk}/
+-rw-r--r--   0 ian        (501) staff       (20)      385 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_variants/{pk}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.250466 gosdk-0.9.23/src/gosdk/specs/paths/consult/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.317249 gosdk-0.9.23/src/gosdk/specs/paths/consult/assays/
+-rw-r--r--   0 ian        (501) staff       (20)      210 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/assays/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.317529 gosdk-0.9.23/src/gosdk/specs/paths/consult/assays/panels/
+-rw-r--r--   0 ian        (501) staff       (20)      240 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/assays/panels/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      342 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/assays/panels/post.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      345 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/assays/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.317826 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/
+-rw-r--r--   0 ian        (501) staff       (20)     1122 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      338 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.318114 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.318256 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/added-markers/
+-rw-r--r--   0 ian        (501) staff       (20)      476 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/added-markers/post.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      235 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/delete.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.318401 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/
+-rw-r--r--   0 ian        (501) staff       (20)      318 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.318554 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/
+-rw-r--r--   0 ian        (501) staff       (20)      443 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.318700 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/
+-rw-r--r--   0 ian        (501) staff       (20)      339 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      424 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/put.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.318848 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/
+-rw-r--r--   0 ian        (501) staff       (20)     1235 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.318991 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/
+-rw-r--r--   0 ian        (501) staff       (20)      493 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.246981 gosdk-0.9.23/src/gosdk/specs/paths/consult/markers/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.247157 gosdk-0.9.23/src/gosdk/specs/paths/consult/markers/{uuid}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.319146 gosdk-0.9.23/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/
+-rw-r--r--   0 ian        (501) staff       (20)      517 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.319433 gosdk-0.9.23/src/gosdk/specs/paths/consult/meetings/
+-rw-r--r--   0 ian        (501) staff       (20)      826 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/meetings/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      350 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/meetings/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.319728 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/
+-rw-r--r--   0 ian        (501) staff       (20)      677 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.319880 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/lab-result-attachments/
+-rw-r--r--   0 ian        (501) staff       (20)      495 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/lab-result-attachments/post.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      354 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.320023 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/quick-add/
+-rw-r--r--   0 ian        (501) staff       (20)     1749 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.320193 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/search/
+-rw-r--r--   0 ian        (501) staff       (20)      998 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/search/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.320338 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.320499 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/cases/
+-rw-r--r--   0 ian        (501) staff       (20)      339 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/cases/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.249111 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.249202 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.320804 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/
+-rw-r--r--   0 ian        (501) staff       (20)      411 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      588 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml
+-rwxr-xr-x   0 ian        (501) staff       (20)      236 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/delete.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.320962 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/
+-rw-r--r--   0 ian        (501) staff       (20)      422 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.249781 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.321275 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/
+-rw-r--r--   0 ian        (501) staff       (20)      414 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      580 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.321418 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/
+-rw-r--r--   0 ian        (501) staff       (20)      476 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.321557 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/samples/
+-rw-r--r--   0 ian        (501) staff       (20)      560 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.321695 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/
+-rw-r--r--   0 ian        (501) staff       (20)      399 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.321838 gosdk-0.9.23/src/gosdk/specs/paths/consult/uploads/
+-rw-r--r--   0 ian        (501) staff       (20)      720 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/uploads/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.321985 gosdk-0.9.23/src/gosdk/specs/paths/consult/uploads/{id}/
+-rw-r--r--   0 ian        (501) staff       (20)      299 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/consult/uploads/{id}/get.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.251321 gosdk-0.9.23/src/gosdk/specs/paths/curation/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.322124 gosdk-0.9.23/src/gosdk/specs/paths/curation/classifications/
+-rw-r--r--   0 ian        (501) staff       (20)      425 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/curation/classifications/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.251162 gosdk-0.9.23/src/gosdk/specs/paths/curation/concepts/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.322397 gosdk-0.9.23/src/gosdk/specs/paths/curation/concepts/alterations/
+-rw-r--r--   0 ian        (501) staff       (20)      499 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/curation/concepts/alterations/get.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      372 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/curation/concepts/alterations/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.322538 gosdk-0.9.23/src/gosdk/specs/paths/curation/contents/
+-rw-r--r--   0 ian        (501) staff       (20)      383 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/curation/contents/post.yaml
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.322676 gosdk-0.9.23/src/gosdk/specs/paths/curation/contents/{uuid}/
+-rw-r--r--   0 ian        (501) staff       (20)      236 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/paths/curation/contents/{uuid}/delete.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      268 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/specs/specd.yaml
+-rw-r--r--   0 ian        (501) staff       (20)      447 2022-01-14 17:53:17.000000 gosdk-0.9.23/src/gosdk/variables.py
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2023-05-01 19:53:05.256967 gosdk-0.9.23/src/gosdk.egg-info/
+-rw-r--r--   0 ian        (501) staff       (20)     3148 2023-05-01 19:53:05.000000 gosdk-0.9.23/src/gosdk.egg-info/PKG-INFO
+-rw-r--r--   0 ian        (501) staff       (20)    13996 2023-05-01 19:53:05.000000 gosdk-0.9.23/src/gosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ian        (501) staff       (20)        1 2023-05-01 19:53:05.000000 gosdk-0.9.23/src/gosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ian        (501) staff       (20)       60 2023-05-01 19:53:05.000000 gosdk-0.9.23/src/gosdk.egg-info/requires.txt
+-rw-r--r--   0 ian        (501) staff       (20)        6 2023-05-01 19:53:05.000000 gosdk-0.9.23/src/gosdk.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gosdk-0.8.18/setup_gosdk.py` & `gosdk-0.9.23/setup_gosdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "pytest-asyncio >= 0.8.0",
     "aioconsole >= 0.1.8",
     "addict >= 2.1.3",
 ]
 
 setup(
     name="gosdk",
-    version='0.8.18',
+    version='0.9.23',
     author="Ian Maurer",
     author_email='ian@genomoncology.com',
 
     packages=[
         "gosdk",
     ],
     package_dir={
@@ -40,29 +40,30 @@
     },
 
     include_package_data=True,
 
     tests_require=tests_require,
 
     install_requires=[
-        "specd >= 0.8.1",
-        "backoff >= 1.5.0",
-        "structlog >= 18.1.0",
+        "specd >= 0.8.2",
+        "backoff >= 1.10.0",
+        "structlog >= 20.1.0",
         "flask == 1.0.2",
     ],
 
     setup_requires=[
         'pytest-runner',
     ],
 
     license="Proprietary",
     keywords='Bioinformatics HGVS VCF Clinical Trials Genomics',
 
     description="gosdk",
     long_description="%s\n\n%s" % (readme, history),
+    long_description_content_type='text/markdown',
 
     entry_points={
     },
 
     classifiers=[
         'License :: Other/Proprietary License',
         'Development Status :: 4 - Beta',
```

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/contents/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/contents/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/contents/match/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/contents/match/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/contents/set/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/contents/set/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/contents/counts/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/contents/counts/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/prognoses/matches/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/prognoses/matches/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/trials/matches/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/trials/matches/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/transcripts/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/region_search/get.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-operationId: get_transcripts
+operationId: region_search
 parameters:
 - description: Chromosome number for region search
   in: query
   name: chromosome
   required: true
   type: string
 - description: Start of region search range
@@ -21,8 +21,8 @@
     schema:
       $ref: '#/definitions/TranscriptList'
   default:
     description: Error
     schema:
       $ref: '#/definitions/Error'
 tags:
-- transcripts
+- region_search
```

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/cases/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/cases/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/warehouse_variants/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/warehouse_variants/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/therapies/matches/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/therapies/matches/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/refresh/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/refresh/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/classifications/match/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/classifications/match/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/genes/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/genes/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/api/alterations/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/api/alterations/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/search/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/search/get.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 - description: null
   in: query
   name: patient_mrn
   required: false
   type: string
 - description: null
   in: query
+  name: identifier
+  required: false
+  type: string
+- description: null
+  in: query
   name: race
   required: false
   type: string
 - description: null
   in: query
   name: gender
   required: false
```

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/paths/consult/uploads/post.yaml` & `gosdk-0.9.23/src/gosdk/specs/paths/consult/uploads/post.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/AlterationsDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/AlterationsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/TherapiesDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/TherapiesDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/DrugPharmacology.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/DrugPharmacology.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/DrugPolypeptide.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/DrugPolypeptide.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/WarehouseVariant.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/WarehouseVariant.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/Annotation.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/Annotation.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -112,8 +112,12 @@
     type: array
   uuid:
     type: string
   variant_type:
     type: string
   annotation_bundle_version:
     type: string
+  gene_annotations:
+    items:
+      type: object
+    type: array
 type: object
```

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/Upload.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/Upload.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/PrognosesDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/PrognosesDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/LabResult.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/LabResult.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/TrialsDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/TrialsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/ClassificationsDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/ClassificationsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/Gene.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/Gene.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/AnnotationsDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/AnnotationsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/MarkersDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/MarkersDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/ContentsDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/ContentsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/NewClassification.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/NewClassification.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/NewRecommendation.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/NewRecommendation.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/NewCase.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/NewCase.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/Alteration.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/Alteration.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/NewPatient.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/NewPatient.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -38,8 +38,16 @@
     type: string
   status:
     type: string
   tumor_type:
     type: string
   zipcode:
     type: string
+  identifier:
+    type: string
+  cdw_associated:
+    type: boolean
+  diagnosis:
+    items:
+      type: object
+    type: array
 type: object
```

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/User.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/User.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/NewContent.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/NewContent.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/CasesDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/CasesDocument.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -91,9 +91,13 @@
   tobacco:
     type: string
   updated:
     format: date-time
     type: string
   uuid:
     type: string
+  comments:
+    type: string
+  relevant_new_information:
+    type: string
 title: CasesDocument
 type: object
```

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/Case.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/Case.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/DrugProduct.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/DrugProduct.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/NewMarker.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/NewMarker.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     type: number
   fold_change_std:
     format: float
     type: number
   is_het:
     x-nullable: true
     type: boolean
+  is_negative_alt:
+    type: boolean
   is_phased:
     x-nullable: true
     type: boolean
   is_somatic:
     type: boolean
   lab_uuid:
     type: string
@@ -42,9 +44,10 @@
   vaf:
     format: float
     type: number
   vaf_alt:
     format: float
     type: number
 required:
-- mut_hash_type
+  - mut_hash_type
+  - is_negative_alt
 type: object
```

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/DrugData.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/DrugData.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/specs/definitions/NewDocument.yaml` & `gosdk-0.9.23/src/gosdk/specs/definitions/NewDocument.yaml`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/logger.py` & `gosdk-0.9.23/src/gosdk/logger.py`

 * *Files identical despite different names*

### Comparing `gosdk-0.8.18/src/gosdk/construct.py` & `gosdk-0.9.23/src/gosdk/construct.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 import backoff
 import specd.sdk
 from configparser import ConfigParser
 from bravado.exception import HTTPInternalServerError
 from urllib3.exceptions import TimeoutError
 from aiohttp.client_exceptions import ClientConnectionError
 
@@ -16,14 +17,15 @@
 KMS_SCHEMES = KMS_SCHEMES.split(",") if KMS_SCHEMES else None
 DEFAULT_SPECD_PATH = os.path.join(os.path.dirname(__file__), "./specs/")
 HTTP_EXCEPTIONS = (
     OSError,
     ConnectionError,
     TimeoutError,
     ClientConnectionError,
+    # HTTPGatewayTimeout,
 )
 MAX_TIME = 600
 
 
 # retrieve variables from environment (higher precedence) or .ini (lower)
 
 CONFIG_SECTION = "gocli-options"
@@ -43,18 +45,32 @@
     verify_ssl=False,
     loop=None,
     specd_path=None,
     schemes=None,
     enable_validation=False,
     config=None,
     max_time=MAX_TIME,
+    max_tries=12,
+    timeout=600,
+    custom_header_option=None,
 ):
 
     token = token or KMS_TOKEN
-    headers = dict(Authorization=f"Token {token}") if token else None
+
+    # add custom headers to the current headers var
+    # creates a dict of key:val by iterating through
+    # the tuple of custom_header_option and initializes
+    # the dict by separating each element in the tuple
+    # by ':'. ex. ('key1:val1','key2:val2') will be
+    # {'key1':'val1','key2:'val2'}
+
+    headers = dict(map(lambda x: x.split(":"), custom_header_option or []))
+    if token:
+        headers["Authorization"] = f"Token {token}"
+
     specd_path = specd_path or DEFAULT_SPECD_PATH
 
     config = config or {}
 
     # validating requests/responses causes problems for extra fields
     # when they cannot be supported by additionalProperties
     # (e.g. differing types in the same record: ao__int, sig__string)
@@ -79,19 +95,24 @@
         schemes=schemes or KMS_SCHEMES,
         config=config,
     )
 
     if async_enabled:
 
         @backoff.on_exception(
-            backoff.expo, HTTP_EXCEPTIONS, max_time=max_time, max_tries=5
+            backoff.expo,
+            HTTP_EXCEPTIONS,
+            max_time=max_time,
+            max_tries=max_tries,
         )
         async def _async_with_retry(sdk_func, **kwargs):
             try:
-                return handle_errors(await sdk_func(**kwargs).result())
+                return handle_errors(
+                    await sdk_func(**kwargs).result(timeout=timeout)
+                )
 
             except HTTPInternalServerError as error:
                 logger.get_logger().error(
                     "_async_with_retry",
                     sdk_func=sdk_func,
                     kwargs=kwargs,
                     error=error,
@@ -99,19 +120,24 @@
                 raise
 
         sdk.call_with_retry = _async_with_retry
 
     else:
 
         @backoff.on_exception(
-            backoff.expo, HTTP_EXCEPTIONS, max_time=max_time, max_tries=5
+            backoff.expo,
+            HTTP_EXCEPTIONS,
+            max_time=max_time,
+            max_tries=max_tries,
         )
         def _sync_with_retry(sdk_func, **kwargs):
             try:
-                return handle_errors(sdk_func(**kwargs).result())
+                return handle_errors(
+                    sdk_func(**kwargs).result(timeout=timeout)
+                )
 
             except HTTPInternalServerError as error:
                 logger.get_logger().error(
                     "_sync_with_retry",
                     sdk_func=sdk_func,
                     kwargs=kwargs,
                     error=error,
```

### Comparing `gosdk-0.8.18/src/gosdk.egg-info/SOURCES.txt` & `gosdk-0.9.23/src/gosdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 MANIFEST.in
+README.md
+setup.py
 setup_gosdk.py
 src/gosdk/__init__.py
 src/gosdk/construct.py
 src/gosdk/logger.py
 src/gosdk/models.py
 src/gosdk/variables.py
 src/gosdk.egg-info/PKG-INFO
@@ -14,20 +16,26 @@
 src/gosdk/specs/definitions/Alteration.yaml
 src/gosdk/specs/definitions/AlterationList.yaml
 src/gosdk/specs/definitions/AlterationsDocument.yaml
 src/gosdk/specs/definitions/AlterationsDocumentList.yaml
 src/gosdk/specs/definitions/Annotation.yaml
 src/gosdk/specs/definitions/AnnotationBundleVersion.yaml
 src/gosdk/specs/definitions/AnnotationList.yaml
+src/gosdk/specs/definitions/AnnotationMatch.yaml
+src/gosdk/specs/definitions/AnnotationMatchList.yaml
 src/gosdk/specs/definitions/AnnotationsDocument.yaml
 src/gosdk/specs/definitions/AnnotationsDocumentAndNotFoundList.yaml
 src/gosdk/specs/definitions/AnnotationsDocumentList.yaml
+src/gosdk/specs/definitions/AnnotationsSVDocument.yaml
+src/gosdk/specs/definitions/AnnotationsSVDocumentList.yaml
 src/gosdk/specs/definitions/Annotations_MergedDocument.yaml
 src/gosdk/specs/definitions/Annotations_MergedDocumentList.yaml
 src/gosdk/specs/definitions/Arguments.yaml
+src/gosdk/specs/definitions/Assay.yaml
+src/gosdk/specs/definitions/AssayList.yaml
 src/gosdk/specs/definitions/Case.yaml
 src/gosdk/specs/definitions/CaseList.yaml
 src/gosdk/specs/definitions/CasesDocument.yaml
 src/gosdk/specs/definitions/CasesDocumentList.yaml
 src/gosdk/specs/definitions/Classification.yaml
 src/gosdk/specs/definitions/ClassificationsDocument.yaml
 src/gosdk/specs/definitions/ClassificationsDocumentList.yaml
@@ -77,48 +85,62 @@
 src/gosdk/specs/definitions/LabResultAttachmentFile.yaml
 src/gosdk/specs/definitions/LabResultDataFile.yaml
 src/gosdk/specs/definitions/LabResultDataFileList.yaml
 src/gosdk/specs/definitions/Location.yaml
 src/gosdk/specs/definitions/LogicSet.yaml
 src/gosdk/specs/definitions/Marker.yaml
 src/gosdk/specs/definitions/MarkerList.yaml
+src/gosdk/specs/definitions/MarkerMetaData.yaml
 src/gosdk/specs/definitions/MarkersDocument.yaml
 src/gosdk/specs/definitions/MarkersDocumentList.yaml
+src/gosdk/specs/definitions/MatchResult.yaml
 src/gosdk/specs/definitions/MatchedDisease.yaml
+src/gosdk/specs/definitions/Meeting.yaml
+src/gosdk/specs/definitions/MeetingList.yaml
+src/gosdk/specs/definitions/MegaMatchResult.yaml
+src/gosdk/specs/definitions/MegaMatchSingleTherapyObject.yaml
+src/gosdk/specs/definitions/MegaMatchTherapyDocument.yaml
+src/gosdk/specs/definitions/MegaMatchTrialArmObject.yaml
+src/gosdk/specs/definitions/MegaMatchTrialDocument.yaml
 src/gosdk/specs/definitions/NDGenes.yaml
 src/gosdk/specs/definitions/NewAlteration.yaml
+src/gosdk/specs/definitions/NewAssay.yaml
 src/gosdk/specs/definitions/NewCase.yaml
 src/gosdk/specs/definitions/NewClassification.yaml
 src/gosdk/specs/definitions/NewContent.yaml
 src/gosdk/specs/definitions/NewDocument.yaml
 src/gosdk/specs/definitions/NewLabResult.yaml
 src/gosdk/specs/definitions/NewLabResultAttachmentFile.yaml
 src/gosdk/specs/definitions/NewLabResultDataFile.yaml
 src/gosdk/specs/definitions/NewMarker.yaml
 src/gosdk/specs/definitions/NewOncologicTreatment.yaml
+src/gosdk/specs/definitions/NewPanel.yaml
 src/gosdk/specs/definitions/NewPatient.yaml
 src/gosdk/specs/definitions/NewPatientDiagnosis.yaml
 src/gosdk/specs/definitions/NewPatientMetaData.yaml
 src/gosdk/specs/definitions/NewRecommendation.yaml
 src/gosdk/specs/definitions/NewRecommendationsReport.yaml
 src/gosdk/specs/definitions/NewReferenceAttachment.yaml
 src/gosdk/specs/definitions/NewSample.yaml
 src/gosdk/specs/definitions/NewSelectedMarker.yaml
 src/gosdk/specs/definitions/NormalizedHGVS.yaml
 src/gosdk/specs/definitions/NormalizedHGVSList.yaml
 src/gosdk/specs/definitions/OutOnlyGenesOffPanel.yaml
 src/gosdk/specs/definitions/OutcomeCohorts.yaml
 src/gosdk/specs/definitions/OverallContact.yaml
 src/gosdk/specs/definitions/Pagination.yaml
+src/gosdk/specs/definitions/Panel.yaml
+src/gosdk/specs/definitions/PanelList.yaml
 src/gosdk/specs/definitions/Patient.yaml
 src/gosdk/specs/definitions/PatientList.yaml
 src/gosdk/specs/definitions/PatientMetaData.yaml
 src/gosdk/specs/definitions/Phenotype.yaml
 src/gosdk/specs/definitions/PrognosesDocument.yaml
 src/gosdk/specs/definitions/PrognosesDocumentList.yaml
+src/gosdk/specs/definitions/ProteinEffect.yaml
 src/gosdk/specs/definitions/QuickAdd.yaml
 src/gosdk/specs/definitions/Recommendation.yaml
 src/gosdk/specs/definitions/RecommendationList.yaml
 src/gosdk/specs/definitions/Reference.yaml
 src/gosdk/specs/definitions/ReferenceAttachment.yaml
 src/gosdk/specs/definitions/RefreshCursor.yaml
 src/gosdk/specs/definitions/Refs.yaml
@@ -133,31 +155,37 @@
 src/gosdk/specs/definitions/TreatmentContexts.yaml
 src/gosdk/specs/definitions/TrialsDocument.yaml
 src/gosdk/specs/definitions/TrialsDocumentList.yaml
 src/gosdk/specs/definitions/Upload.yaml
 src/gosdk/specs/definitions/User.yaml
 src/gosdk/specs/definitions/UserCredentials.yaml
 src/gosdk/specs/definitions/UserToken.yaml
+src/gosdk/specs/definitions/VariantInterpretation.yaml
+src/gosdk/specs/definitions/VariantInterpretationResponse.yaml
+src/gosdk/specs/definitions/VariantInterpretationSingleResponse.yaml
 src/gosdk/specs/definitions/WarehouseFeature.yaml
 src/gosdk/specs/definitions/WarehouseFeatureList.yaml
 src/gosdk/specs/definitions/WarehouseVariant.yaml
 src/gosdk/specs/definitions/WarehouseVariantJoin.yaml
 src/gosdk/specs/definitions/WarehouseVariantList.yaml
 src/gosdk/specs/definitions/WarehouseVariantPage.yaml
 src/gosdk/specs/paths/api/alterations/get.yaml
 src/gosdk/specs/paths/api/alterations/{pk}/get.yaml
 src/gosdk/specs/paths/api/annotations/get.yaml
 src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
 src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/delete.yaml
 src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml
 src/gosdk/specs/paths/api/annotations/hgvs/get.yaml
+src/gosdk/specs/paths/api/annotations/hgvs/post.yaml
 src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml
 src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml
+src/gosdk/specs/paths/api/annotations/match/post.yaml
 src/gosdk/specs/paths/api/annotations/merged/{pk}/get.yaml
 src/gosdk/specs/paths/api/annotations/refresh/get.yaml
+src/gosdk/specs/paths/api/annotations/sv_match/post.yaml
 src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
 src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml
 src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/delete.yaml
 src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/get.yaml
 src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/patch.yaml
 src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/put.yaml
 src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml
@@ -187,36 +215,49 @@
 src/gosdk/specs/paths/api/contents/match/post.yaml
 src/gosdk/specs/paths/api/contents/set/get.yaml
 src/gosdk/specs/paths/api/genes/get.yaml
 src/gosdk/specs/paths/api/genes/filter_genes/get.yaml
 src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml
 src/gosdk/specs/paths/api/info/annotation_bundle/get.yaml
 src/gosdk/specs/paths/api/prognoses/matches/post.yaml
+src/gosdk/specs/paths/api/region_search/get.yaml
+src/gosdk/specs/paths/api/region_search/batch/get.yaml
 src/gosdk/specs/paths/api/therapies/matches/post.yaml
-src/gosdk/specs/paths/api/transcripts/get.yaml
+src/gosdk/specs/paths/api/therapies/therapy_matches/post.yaml
 src/gosdk/specs/paths/api/trials/matches/post.yaml
 src/gosdk/specs/paths/api/users/login/post.yaml
+src/gosdk/specs/paths/api/variant_interpretations/generate/post.yaml
 src/gosdk/specs/paths/api/warehouse_features/post.yaml
 src/gosdk/specs/paths/api/warehouse_variants/get.yaml
 src/gosdk/specs/paths/api/warehouse_variants/post.yaml
 src/gosdk/specs/paths/api/warehouse_variants/{pk}/get.yaml
+src/gosdk/specs/paths/consult/assays/get.yaml
+src/gosdk/specs/paths/consult/assays/post.yaml
+src/gosdk/specs/paths/consult/assays/panels/get.yaml
+src/gosdk/specs/paths/consult/assays/panels/post.yaml
 src/gosdk/specs/paths/consult/cases/get.yaml
 src/gosdk/specs/paths/consult/cases/post.yaml
+src/gosdk/specs/paths/consult/cases/{case_uuid}/delete.yaml
+src/gosdk/specs/paths/consult/cases/{case_uuid}/put.yaml
+src/gosdk/specs/paths/consult/cases/{case_uuid}/added-markers/post.yaml
 src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/post.yaml
 src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/post.yaml
 src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/get.yaml
 src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml
 src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/post.yaml
-src/gosdk/specs/paths/consult/cases/{uuid}/delete.yaml
+src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/post.yaml
+src/gosdk/specs/paths/consult/meetings/get.yaml
+src/gosdk/specs/paths/consult/meetings/post.yaml
 src/gosdk/specs/paths/consult/patients/get.yaml
 src/gosdk/specs/paths/consult/patients/post.yaml
 src/gosdk/specs/paths/consult/patients/lab-result-attachments/post.yaml
 src/gosdk/specs/paths/consult/patients/quick-add/post.yaml
 src/gosdk/specs/paths/consult/patients/search/get.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/delete.yaml
+src/gosdk/specs/paths/consult/patients/{uuid}/cases/get.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/get.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/post.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/get.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/post.yaml
 src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml
```

