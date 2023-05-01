# Comparing `tmp/ranx-0.3.7.tar.gz` & `tmp/ranx-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ranx-0.3.7.tar", last modified: Mon Apr 17 09:43:02 2023, max compression
+gzip compressed data, was "ranx-0.3.8.tar", last modified: Mon May  1 17:04:48 2023, max compression
```

## Comparing `ranx-0.3.7.tar` & `ranx-0.3.8.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.709992 ranx-0.3.7/
--rw-r--r--   0 elias      (501) staff       (20)     1070 2022-12-02 22:30:34.000000 ranx-0.3.7/LICENSE
--rw-r--r--   0 elias      (501) staff       (20)    15899 2023-04-17 09:43:02.709367 ranx-0.3.7/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)    15225 2023-02-13 16:41:37.000000 ranx-0.3.7/README.md
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.644794 ranx-0.3.7/ranx/
--rw-r--r--   0 elias      (501) staff       (20)      232 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/__init__.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.653281 ranx-0.3.7/ranx/data_structures/
--rw-r--r--   0 elias      (501) staff       (20)      509 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     3241 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/common.py
--rw-r--r--   0 elias      (501) staff       (20)      524 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/frozenset_dict.py
--rw-r--r--   0 elias      (501) staff       (20)      639 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/generic.py
--rw-r--r--   0 elias      (501) staff       (20)     3312 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/optimization_report.py
--rw-r--r--   0 elias      (501) staff       (20)    11093 2023-01-26 20:56:50.000000 ranx-0.3.7/ranx/data_structures/qrels.py
--rw-r--r--   0 elias      (501) staff       (20)    11274 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/report.py
--rw-r--r--   0 elias      (501) staff       (20)    11288 2023-04-17 09:21:00.000000 ranx-0.3.7/ranx/data_structures/run.py
--rw-r--r--   0 elias      (501) staff       (20)     2056 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/downloader.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.671092 ranx-0.3.7/ranx/fusion/
--rw-r--r--   0 elias      (501) staff       (20)     2821 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     4744 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/bayesfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     3243 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/bordafuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_anz.py
--rw-r--r--   0 elias      (501) staff       (20)     2148 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_gmnz.py
--rw-r--r--   0 elias      (501) staff       (20)     2138 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_max.py
--rw-r--r--   0 elias      (501) staff       (20)     2212 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_med.py
--rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_min.py
--rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_mnz.py
--rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_sum.py
--rw-r--r--   0 elias      (501) staff       (20)     1703 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/common.py
--rw-r--r--   0 elias      (501) staff       (20)     4732 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/condorcet.py
--rw-r--r--   0 elias      (501) staff       (20)     2391 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/isr.py
--rw-r--r--   0 elias      (501) staff       (20)     2691 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/log_isr.py
--rw-r--r--   0 elias      (501) staff       (20)     2949 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/logn_isr.py
--rw-r--r--   0 elias      (501) staff       (20)     3018 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/mapfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2780 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/mixed.py
--rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/posfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     4446 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/probfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2632 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/rbc.py
--rw-r--r--   0 elias      (501) staff       (20)     2073 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/rrf.py
--rw-r--r--   0 elias      (501) staff       (20)     4044 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/segfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     3083 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/slidefuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1912 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/weighted_bordafuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/weighted_condorcet.py
--rw-r--r--   0 elias      (501) staff       (20)     2903 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/wmnz.py
--rw-r--r--   0 elias      (501) staff       (20)     1895 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/wsum.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.683397 ranx-0.3.7/ranx/fusion_optimization/
--rw-r--r--   0 elias      (501) staff       (20)     2568 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)      240 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_bayesfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1183 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_comb_gmnz.py
--rw-r--r--   0 elias      (501) staff       (20)     1179 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_logn_isr.py
--rw-r--r--   0 elias      (501) staff       (20)      233 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_mapfuse.py
--rw-r--r--   0 elias      (501) staff       (20)      623 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_mixed.py
--rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_posfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1137 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_probfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1126 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_rbc.py
--rw-r--r--   0 elias      (501) staff       (20)      961 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_rrf.py
--rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_segfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1062 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_slidefuse.py
--rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_bordafuse.py
--rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_condorcet.py
--rw-r--r--   0 elias      (501) staff       (20)     1408 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_weights.py
--rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_wmnz.py
--rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_wsum.py
--rw-r--r--   0 elias      (501) staff       (20)     1661 2023-02-21 13:26:31.000000 ranx-0.3.7/ranx/io.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.687834 ranx-0.3.7/ranx/meta/
--rw-r--r--   0 elias      (501) staff       (20)      259 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     5017 2023-04-17 09:30:20.000000 ranx-0.3.7/ranx/meta/compare.py
--rw-r--r--   0 elias      (501) staff       (20)     5312 2023-04-17 09:32:51.000000 ranx-0.3.7/ranx/meta/evaluate.py
--rw-r--r--   0 elias      (501) staff       (20)     1134 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/fuse.py
--rw-r--r--   0 elias      (501) staff       (20)      158 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/normalize.py
--rw-r--r--   0 elias      (501) staff       (20)     2469 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/optimize_fusion.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.699972 ranx-0.3.7/ranx/metrics/
--rw-r--r--   0 elias      (501) staff       (20)     1564 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     2917 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/average_precision.py
--rw-r--r--   0 elias      (501) staff       (20)     2403 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/bpref.py
--rw-r--r--   0 elias      (501) staff       (20)      305 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/common.py
--rw-r--r--   0 elias      (501) staff       (20)     2509 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/f1.py
--rw-r--r--   0 elias      (501) staff       (20)     2433 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/get_hit_lists.py
--rw-r--r--   0 elias      (501) staff       (20)     2095 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/get_non_rel_lists.py
--rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/get_unjudged_lists.py
--rw-r--r--   0 elias      (501) staff       (20)     2313 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/hit_rate.py
--rw-r--r--   0 elias      (501) staff       (20)     2188 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/hits.py
--rw-r--r--   0 elias      (501) staff       (20)     6493 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/ndcg.py
--rw-r--r--   0 elias      (501) staff       (20)     2237 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/precision.py
--rw-r--r--   0 elias      (501) staff       (20)     1979 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/r_precision.py
--rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/rank_biased_precision.py
--rw-r--r--   0 elias      (501) staff       (20)     2405 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/recall.py
--rw-r--r--   0 elias      (501) staff       (20)     2225 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/reciprocal_rank.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.705662 ranx-0.3.7/ranx/normalization/
--rw-r--r--   0 elias      (501) staff       (20)      776 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     2057 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/borda_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1076 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/common.py
--rw-r--r--   0 elias      (501) staff       (20)     1426 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/max_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1701 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/min_max_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1322 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/rank_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1547 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/sum_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1511 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/zmuv_norm.py
--rw-r--r--   0 elias      (501) staff       (20)      412 2023-02-21 13:43:14.000000 ranx-0.3.7/ranx/ranxhub.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.708460 ranx-0.3.7/ranx/statistical_tests/
--rw-r--r--   0 elias      (501) staff       (20)     3441 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/statistical_tests/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     1368 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/statistical_tests/fisher_randomization_test.py
--rw-r--r--   0 elias      (501) staff       (20)      550 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/statistical_tests/paired_student_t_test.py
--rw-r--r--   0 elias      (501) staff       (20)      711 2023-02-13 16:35:22.000000 ranx-0.3.7/ranx/statistical_tests/tukey_hsd_test.py
--rw-r--r--   0 elias      (501) staff       (20)     1782 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/utils.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.648401 ranx-0.3.7/ranx.egg-info/
--rw-r--r--   0 elias      (501) staff       (20)    15899 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)     2923 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (501) staff       (20)        1 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (501) staff       (20)       88 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/requires.txt
--rw-r--r--   0 elias      (501) staff       (20)        5 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/top_level.txt
--rw-r--r--   0 elias      (501) staff       (20)       38 2023-04-17 09:43:02.710160 ranx-0.3.7/setup.cfg
--rw-r--r--   0 elias      (501) staff       (20)     1227 2023-04-17 09:42:16.000000 ranx-0.3.7/setup.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.110676 ranx-0.3.8/
+-rw-r--r--   0 elias      (501) staff       (20)     1070 2022-12-02 22:30:34.000000 ranx-0.3.8/LICENSE
+-rw-r--r--   0 elias      (501) staff       (20)    16182 2023-05-01 17:04:48.109811 ranx-0.3.8/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)    15508 2023-05-01 17:04:32.000000 ranx-0.3.8/README.md
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.042954 ranx-0.3.8/ranx/
+-rw-r--r--   0 elias      (501) staff       (20)      250 2023-05-01 16:45:12.000000 ranx-0.3.8/ranx/__init__.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.050582 ranx-0.3.8/ranx/data_structures/
+-rw-r--r--   0 elias      (501) staff       (20)      509 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/data_structures/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     3241 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/data_structures/common.py
+-rw-r--r--   0 elias      (501) staff       (20)      524 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/data_structures/frozenset_dict.py
+-rw-r--r--   0 elias      (501) staff       (20)      639 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/data_structures/generic.py
+-rw-r--r--   0 elias      (501) staff       (20)     3312 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/data_structures/optimization_report.py
+-rw-r--r--   0 elias      (501) staff       (20)    11093 2023-01-26 20:56:50.000000 ranx-0.3.8/ranx/data_structures/qrels.py
+-rw-r--r--   0 elias      (501) staff       (20)    11274 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/data_structures/report.py
+-rw-r--r--   0 elias      (501) staff       (20)    11288 2023-04-17 09:21:00.000000 ranx-0.3.8/ranx/data_structures/run.py
+-rw-r--r--   0 elias      (501) staff       (20)     2056 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/downloader.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.069434 ranx-0.3.8/ranx/fusion/
+-rw-r--r--   0 elias      (501) staff       (20)     2821 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     4744 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/bayesfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     3243 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/bordafuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/comb_anz.py
+-rw-r--r--   0 elias      (501) staff       (20)     2148 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/comb_gmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     2138 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/comb_max.py
+-rw-r--r--   0 elias      (501) staff       (20)     2212 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/comb_med.py
+-rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/comb_min.py
+-rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/comb_mnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/comb_sum.py
+-rw-r--r--   0 elias      (501) staff       (20)     1703 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/common.py
+-rw-r--r--   0 elias      (501) staff       (20)     4732 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/condorcet.py
+-rw-r--r--   0 elias      (501) staff       (20)     2391 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/isr.py
+-rw-r--r--   0 elias      (501) staff       (20)     2691 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/log_isr.py
+-rw-r--r--   0 elias      (501) staff       (20)     2949 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/logn_isr.py
+-rw-r--r--   0 elias      (501) staff       (20)     3018 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/mapfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2780 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/mixed.py
+-rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/posfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     4446 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/probfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2632 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/rbc.py
+-rw-r--r--   0 elias      (501) staff       (20)     2073 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/rrf.py
+-rw-r--r--   0 elias      (501) staff       (20)     4044 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/segfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     3083 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/slidefuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1912 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/weighted_bordafuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/weighted_condorcet.py
+-rw-r--r--   0 elias      (501) staff       (20)     2903 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/wmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     1895 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion/wsum.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.081802 ranx-0.3.8/ranx/fusion_optimization/
+-rw-r--r--   0 elias      (501) staff       (20)     2568 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)      240 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_bayesfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1183 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_comb_gmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     1179 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_logn_isr.py
+-rw-r--r--   0 elias      (501) staff       (20)      233 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_mapfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      623 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_mixed.py
+-rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_posfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1137 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_probfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1126 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_rbc.py
+-rw-r--r--   0 elias      (501) staff       (20)      961 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_rrf.py
+-rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_segfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1062 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_slidefuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_weighted_bordafuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_weighted_condorcet.py
+-rw-r--r--   0 elias      (501) staff       (20)     1408 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_weights.py
+-rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_wmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/fusion_optimization/optimize_wsum.py
+-rw-r--r--   0 elias      (501) staff       (20)     1661 2023-02-21 13:26:31.000000 ranx-0.3.8/ranx/io.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.087031 ranx-0.3.8/ranx/meta/
+-rw-r--r--   0 elias      (501) staff       (20)      294 2023-05-01 16:44:35.000000 ranx-0.3.8/ranx/meta/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     5017 2023-04-17 09:30:20.000000 ranx-0.3.8/ranx/meta/compare.py
+-rw-r--r--   0 elias      (501) staff       (20)     5255 2023-05-01 16:25:01.000000 ranx-0.3.8/ranx/meta/evaluate.py
+-rw-r--r--   0 elias      (501) staff       (20)     1134 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/meta/fuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      158 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/meta/normalize.py
+-rw-r--r--   0 elias      (501) staff       (20)     2469 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/meta/optimize_fusion.py
+-rw-r--r--   0 elias      (501) staff       (20)     1680 2023-05-01 16:51:21.000000 ranx-0.3.8/ranx/meta/plot.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.099824 ranx-0.3.8/ranx/metrics/
+-rw-r--r--   0 elias      (501) staff       (20)     1683 2023-05-01 16:26:21.000000 ranx-0.3.8/ranx/metrics/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     2917 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/average_precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     2403 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/bpref.py
+-rw-r--r--   0 elias      (501) staff       (20)      305 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/common.py
+-rw-r--r--   0 elias      (501) staff       (20)     2509 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/f1.py
+-rw-r--r--   0 elias      (501) staff       (20)     2433 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/get_hit_lists.py
+-rw-r--r--   0 elias      (501) staff       (20)     2095 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/get_non_rel_lists.py
+-rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/get_unjudged_lists.py
+-rw-r--r--   0 elias      (501) staff       (20)     2313 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/hit_rate.py
+-rw-r--r--   0 elias      (501) staff       (20)     2188 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/hits.py
+-rw-r--r--   0 elias      (501) staff       (20)     3444 2023-05-01 16:10:21.000000 ranx-0.3.8/ranx/metrics/interpolated_precision_at_recall.py
+-rw-r--r--   0 elias      (501) staff       (20)     6493 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/ndcg.py
+-rw-r--r--   0 elias      (501) staff       (20)     2237 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     1979 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/r_precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/rank_biased_precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     2405 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/recall.py
+-rw-r--r--   0 elias      (501) staff       (20)     2225 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/metrics/reciprocal_rank.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.106087 ranx-0.3.8/ranx/normalization/
+-rw-r--r--   0 elias      (501) staff       (20)      776 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     2057 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/borda_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1076 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/common.py
+-rw-r--r--   0 elias      (501) staff       (20)     1426 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/max_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1701 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/min_max_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1322 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/rank_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1547 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/sum_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1511 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/normalization/zmuv_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)      412 2023-02-21 13:43:14.000000 ranx-0.3.8/ranx/ranxhub.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.108771 ranx-0.3.8/ranx/statistical_tests/
+-rw-r--r--   0 elias      (501) staff       (20)     3441 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/statistical_tests/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     1368 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/statistical_tests/fisher_randomization_test.py
+-rw-r--r--   0 elias      (501) staff       (20)      550 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/statistical_tests/paired_student_t_test.py
+-rw-r--r--   0 elias      (501) staff       (20)      711 2023-02-13 16:35:22.000000 ranx-0.3.8/ranx/statistical_tests/tukey_hsd_test.py
+-rw-r--r--   0 elias      (501) staff       (20)     1782 2022-12-02 22:30:35.000000 ranx-0.3.8/ranx/utils.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-01 17:04:48.045960 ranx-0.3.8/ranx.egg-info/
+-rw-r--r--   0 elias      (501) staff       (20)    16182 2023-05-01 17:04:47.000000 ranx-0.3.8/ranx.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)     2990 2023-05-01 17:04:47.000000 ranx-0.3.8/ranx.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (501) staff       (20)        1 2023-05-01 17:04:47.000000 ranx-0.3.8/ranx.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (501) staff       (20)       88 2023-05-01 17:04:47.000000 ranx-0.3.8/ranx.egg-info/requires.txt
+-rw-r--r--   0 elias      (501) staff       (20)        5 2023-05-01 17:04:47.000000 ranx-0.3.8/ranx.egg-info/top_level.txt
+-rw-r--r--   0 elias      (501) staff       (20)       38 2023-05-01 17:04:48.110862 ranx-0.3.8/setup.cfg
+-rw-r--r--   0 elias      (501) staff       (20)     1227 2023-05-01 17:00:25.000000 ranx-0.3.8/setup.py
```

### Comparing `ranx-0.3.7/LICENSE` & `ranx-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/PKG-INFO` & `ranx-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranx
-Version: 0.3.7
+Version: 0.3.8
 Summary: ranx: A Blazing-Fast Python Library for Ranking Evaluation, Comparison, and Fusion
 Home-page: https://github.com/AmenRa/ranx
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: trec_eval,information retrieval,recommender systems,evaluation,ranking,fusion,metasearch,numba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,24 +34,21 @@
   <a href="https://lbesson.mit-license.org/"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
   <!-- Google Colab -->
   <a href="https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/1_overview.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/></a>
 </p>
 
 ## 🔥 News
 
-- 📌 [October 10, 2022] I released a new sharing platform for pre-computed runs called [ranxhub](https://amenra.github.io/ranxhub), click [here](https://amenra.github.io/ranxhub) to learn more!
+- 📌 [April 4, 2023] [ranxhub](https://amenra.github.io/ranxhub), the [ranx](https://github.com/AmenRa/ranx)'s companion repository, will be featured in [SIGIR 2023](https://sigir.org/sigir2023)!  
+On [ranxhub](https://amenra.github.io/ranxhub), you can download and share pre-computed runs for Information Retrieval datasets, such as [MSMARCO Passage Ranking](https://arxiv.org/abs/1611.09268).
 
-- [November 2, 2022] `ranx` `0.3.3` is out!  
-This release adds support for changing Qrels relevance level, i.e, the minimum relevance judgement score to consider a document to be relevant.  
-You can now define metric-wise relevance levels by appending `-l<num>` to metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`.
-
-- [October 10, 2022] `ranx` `0.3` is out!  
-This release adds integration with [ranxhub](https://amenra.github.io/ranxhub), a new sharing platform for pre-computed runs.  
-Click [here](#off-the-shelf-runs) for a quick example.  
-Click [here](https://amenra.github.io/ranxhub) to learn how to share your own runs with the community and lead by example!
+- [May 1 2023] `ranx` `0.3.8` is out!  
+This release adds early support for results plotting. Specifically, it is now possible to plot Interpolated Precision-Recall Curve. Click [here]() for further details.
+<!-- This release adds support for changing Qrels relevance level, i.e, the minimum relevance judgement score to consider a document to be relevant.   -->
+<!-- You can now define metric-wise relevance levels by appending `-l<num>` to metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`. -->
 
 ## ⚡️ Introduction
 
 [ranx](https://github.com/AmenRa/ranx) ([raŋks]) is a library of fast ranking evaluation metrics implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)), leveraging [Numba](https://github.com/numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization](https://en.wikipedia.org/wiki/Automatic_parallelization).
 It offers a user-friendly interface to evaluate and compare [Information Retrieval](https://en.wikipedia.org/wiki/Information_retrieval) and [Recommender Systems](https://en.wikipedia.org/wiki/Recommender_system).
 [ranx](https://github.com/AmenRa/ranx) allows you to perform statistical tests and export [LaTeX](https://en.wikipedia.org/wiki/LaTeX) tables for your scientific publications.
 Moreover, [ranx](https://github.com/AmenRa/ranx) provides several [fusion algorithms](https://amenra.github.io/ranx/fusion) and [normalization strategies](https://amenra.github.io/ranx/normalization), and an automatic [fusion optimization](https://amenra.github.io/ranx/fusion/#optimize-fusion) functionality.
@@ -221,14 +218,15 @@
 | Name                                                             | Link                                                                                                                                                                                   |
 | ---------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Overview                                                         | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/1_overview.ipynb)              |
 | Qrels and Run                                                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/2_qrels_and_run.ipynb)         |
 | Evaluation                                                       | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/3_evaluation.ipynb)            |
 | Comparison and Report                                            | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/4_comparison_and_report.ipynb) |
 | Fusion                                                           | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/5_fusion.ipynb)                |
+| Plot                                                             | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/7_plot.ipynb)                  |
 | Share your runs with [ranxhub](https://amenra.github.io/ranxhub) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/6_ranxhub.ipynb)               |
 
 
 ## 📚 Documentation
 Browse the [documentation](https://amenra.github.io/ranx) for more details and examples.
```

#### html2text {}

```diff
@@ -1,47 +1,43 @@
-Metadata-Version: 2.1 Name: ranx Version: 0.3.7 Summary: ranx: A Blazing-Fast
+Metadata-Version: 2.1 Name: ranx Version: 0.3.8 Summary: ranx: A Blazing-Fast
 Python Library for Ranking Evaluation, Comparison, and Fusion Home-page: https:
 //github.com/AmenRa/ranx Author: Elias Bassani Author-email:
 elias.bssn@gmail.com Keywords: trec_eval,information retrieval,recommender
 systems,evaluation,ranking,fusion,metasearch,numba Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing :: General Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [https://repository-images.githubusercontent.com/268892956/750228ec-f3f2-465d-
                               9c17-420c688ba2bc]
      [https://badges.aleen42.com/src/python.svg]  [PyPI_version]  [Download
  counter]  [Documentation_Status]  [https://img.shields.io/badge/code%20style-
               black-000000.svg]  [License:_MIT]  [Open_in_Colab]
-## ð¥ News - ð [October 10, 2022] I released a new sharing platform for
-pre-computed runs called [ranxhub](https://amenra.github.io/ranxhub), click
-[here](https://amenra.github.io/ranxhub) to learn more! - [November 2, 2022]
-`ranx` `0.3.3` is out! This release adds support for changing Qrels relevance
-level, i.e, the minimum relevance judgement score to consider a document to be
-relevant. You can now define metric-wise relevance levels by appending `-l` to
-metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or
-setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`.
-- [October 10, 2022] `ranx` `0.3` is out! This release adds integration with
-[ranxhub](https://amenra.github.io/ranxhub), a new sharing platform for pre-
-computed runs. Click [here](#off-the-shelf-runs) for a quick example. Click
-[here](https://amenra.github.io/ranxhub) to learn how to share your own runs
-with the community and lead by example! ## â¡ï¸ Introduction [ranx](https://
-github.com/AmenRa/ranx) ([raÅks]) is a library of fast ranking evaluation
-metrics implemented in [Python](https://en.wikipedia.org/wiki/Python_
-(programming_language)), leveraging [Numba](https://github.com/numba/numba) for
-high-speed [vector operations](https://en.wikipedia.org/wiki/
-Automatic_vectorization) and [automatic parallelization](https://
-en.wikipedia.org/wiki/Automatic_parallelization). It offers a user-friendly
-interface to evaluate and compare [Information Retrieval](https://
-en.wikipedia.org/wiki/Information_retrieval) and [Recommender Systems](https://
-en.wikipedia.org/wiki/Recommender_system). [ranx](https://github.com/AmenRa/
-ranx) allows you to perform statistical tests and export [LaTeX](https://
-en.wikipedia.org/wiki/LaTeX) tables for your scientific publications. Moreover,
-[ranx](https://github.com/AmenRa/ranx) provides several [fusion algorithms]
-(https://amenra.github.io/ranx/fusion) and [normalization strategies](https://
+## ð¥ News - ð [April 4, 2023] [ranxhub](https://amenra.github.io/
+ranxhub), the [ranx](https://github.com/AmenRa/ranx)'s companion repository,
+will be featured in [SIGIR 2023](https://sigir.org/sigir2023)! On [ranxhub]
+(https://amenra.github.io/ranxhub), you can download and share pre-computed
+runs for Information Retrieval datasets, such as [MSMARCO Passage Ranking]
+(https://arxiv.org/abs/1611.09268). - [May 1 2023] `ranx` `0.3.8` is out! This
+release adds early support for results plotting. Specifically, it is now
+possible to plot Interpolated Precision-Recall Curve. Click [here]() for
+further details.   ## â¡ï¸ Introduction [ranx](https://github.com/AmenRa/
+ranx) ([raÅks]) is a library of fast ranking evaluation metrics implemented in
+[Python](https://en.wikipedia.org/wiki/Python_(programming_language)),
+leveraging [Numba](https://github.com/numba/numba) for high-speed [vector
+operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and
+[automatic parallelization](https://en.wikipedia.org/wiki/
+Automatic_parallelization). It offers a user-friendly interface to evaluate and
+compare [Information Retrieval](https://en.wikipedia.org/wiki/
+Information_retrieval) and [Recommender Systems](https://en.wikipedia.org/wiki/
+Recommender_system). [ranx](https://github.com/AmenRa/ranx) allows you to
+perform statistical tests and export [LaTeX](https://en.wikipedia.org/wiki/
+LaTeX) tables for your scientific publications. Moreover, [ranx](https://
+github.com/AmenRa/ranx) provides several [fusion algorithms](https://
+amenra.github.io/ranx/fusion) and [normalization strategies](https://
 amenra.github.io/ranx/normalization), and an automatic [fusion optimization]
 (https://amenra.github.io/ranx/fusion/#optimize-fusion) functionality. [ranx]
 (https://github.com/AmenRa/ranx) was featured in [ECIR 2022](https://
 ecir2022.org) and [CIKM 2022](https://www.cikm2022.org). If you use [ranx]
 (https://github.com/AmenRa/ranx) to evaluate results or conducting experiments
 involving fusion for your scientific publication, please consider citing it:
 [evaluation bibtex](https://dblp.org/rec/conf/ecir/Bassani22.html?view=bibtex),
@@ -149,20 +145,23 @@
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
 3_evaluation.ipynb) | | Comparison and Report | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
 4_comparison_and_report.ipynb) | | Fusion | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
-5_fusion.ipynb) | | Share your runs with [ranxhub](https://amenra.github.io/
-ranxhub) | [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/
-notebooks/6_ranxhub.ipynb) | ## ð Documentation Browse the [documentation]
-(https://amenra.github.io/ranx) for more details and examples. ## ð Citation
-If you use [ranx](https://github.com/AmenRa/ranx) to evaluate results for your
+5_fusion.ipynb) | | Plot | [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/
+blob/master/notebooks/7_plot.ipynb) | | Share your runs with [ranxhub](https://
+amenra.github.io/ranxhub) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
+6_ranxhub.ipynb) | ## ð Documentation Browse the [documentation](https://
+amenra.github.io/ranx) for more details and examples. ## ð Citation If you
+use [ranx](https://github.com/AmenRa/ranx) to evaluate results for your
 scientific publication, please consider citing our [ECIR 2022](https://
 ecir2022.org) paper:  BibTeX ```bibtex @inproceedings{DBLP:conf/ecir/Bassani22,
 author = {Elias Bassani}, title = {ranx: {A} Blazing-Fast Python Library for
 Ranking Evaluation and Comparison}, booktitle = {{ECIR} {(2)}}, series =
 {Lecture Notes in Computer Science}, volume = {13186}, pages = {259--264},
 publisher = {Springer}, year = {2022} } ```  If you use the fusion
 functionalities provided by [ranx](https://github.com/AmenRa/ranx) for
```

### Comparing `ranx-0.3.7/README.md` & `ranx-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,21 @@
   <a href="https://lbesson.mit-license.org/"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
   <!-- Google Colab -->
   <a href="https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/1_overview.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/></a>
 </p>
 
 ## 🔥 News
 
-- 📌 [October 10, 2022] I released a new sharing platform for pre-computed runs called [ranxhub](https://amenra.github.io/ranxhub), click [here](https://amenra.github.io/ranxhub) to learn more!
+- 📌 [April 4, 2023] [ranxhub](https://amenra.github.io/ranxhub), the [ranx](https://github.com/AmenRa/ranx)'s companion repository, will be featured in [SIGIR 2023](https://sigir.org/sigir2023)!  
+On [ranxhub](https://amenra.github.io/ranxhub), you can download and share pre-computed runs for Information Retrieval datasets, such as [MSMARCO Passage Ranking](https://arxiv.org/abs/1611.09268).
 
-- [November 2, 2022] `ranx` `0.3.3` is out!  
-This release adds support for changing Qrels relevance level, i.e, the minimum relevance judgement score to consider a document to be relevant.  
-You can now define metric-wise relevance levels by appending `-l<num>` to metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`.
-
-- [October 10, 2022] `ranx` `0.3` is out!  
-This release adds integration with [ranxhub](https://amenra.github.io/ranxhub), a new sharing platform for pre-computed runs.  
-Click [here](#off-the-shelf-runs) for a quick example.  
-Click [here](https://amenra.github.io/ranxhub) to learn how to share your own runs with the community and lead by example!
+- [May 1 2023] `ranx` `0.3.8` is out!  
+This release adds early support for results plotting. Specifically, it is now possible to plot Interpolated Precision-Recall Curve. Click [here]() for further details.
+<!-- This release adds support for changing Qrels relevance level, i.e, the minimum relevance judgement score to consider a document to be relevant.   -->
+<!-- You can now define metric-wise relevance levels by appending `-l<num>` to metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`. -->
 
 ## ⚡️ Introduction
 
 [ranx](https://github.com/AmenRa/ranx) ([raŋks]) is a library of fast ranking evaluation metrics implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)), leveraging [Numba](https://github.com/numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization](https://en.wikipedia.org/wiki/Automatic_parallelization).
 It offers a user-friendly interface to evaluate and compare [Information Retrieval](https://en.wikipedia.org/wiki/Information_retrieval) and [Recommender Systems](https://en.wikipedia.org/wiki/Recommender_system).
 [ranx](https://github.com/AmenRa/ranx) allows you to perform statistical tests and export [LaTeX](https://en.wikipedia.org/wiki/LaTeX) tables for your scientific publications.
 Moreover, [ranx](https://github.com/AmenRa/ranx) provides several [fusion algorithms](https://amenra.github.io/ranx/fusion) and [normalization strategies](https://amenra.github.io/ranx/normalization), and an automatic [fusion optimization](https://amenra.github.io/ranx/fusion/#optimize-fusion) functionality.
@@ -204,14 +201,15 @@
 | Name                                                             | Link                                                                                                                                                                                   |
 | ---------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Overview                                                         | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/1_overview.ipynb)              |
 | Qrels and Run                                                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/2_qrels_and_run.ipynb)         |
 | Evaluation                                                       | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/3_evaluation.ipynb)            |
 | Comparison and Report                                            | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/4_comparison_and_report.ipynb) |
 | Fusion                                                           | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/5_fusion.ipynb)                |
+| Plot                                                             | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/7_plot.ipynb)                  |
 | Share your runs with [ranxhub](https://amenra.github.io/ranxhub) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/6_ranxhub.ipynb)               |
 
 
 ## 📚 Documentation
 Browse the [documentation](https://amenra.github.io/ranx) for more details and examples.
```

#### html2text {}

```diff
@@ -1,38 +1,34 @@
 [https://repository-images.githubusercontent.com/268892956/750228ec-f3f2-465d-
                               9c17-420c688ba2bc]
      [https://badges.aleen42.com/src/python.svg]  [PyPI_version]  [Download
  counter]  [Documentation_Status]  [https://img.shields.io/badge/code%20style-
               black-000000.svg]  [License:_MIT]  [Open_in_Colab]
-## ð¥ News - ð [October 10, 2022] I released a new sharing platform for
-pre-computed runs called [ranxhub](https://amenra.github.io/ranxhub), click
-[here](https://amenra.github.io/ranxhub) to learn more! - [November 2, 2022]
-`ranx` `0.3.3` is out! This release adds support for changing Qrels relevance
-level, i.e, the minimum relevance judgement score to consider a document to be
-relevant. You can now define metric-wise relevance levels by appending `-l` to
-metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or
-setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`.
-- [October 10, 2022] `ranx` `0.3` is out! This release adds integration with
-[ranxhub](https://amenra.github.io/ranxhub), a new sharing platform for pre-
-computed runs. Click [here](#off-the-shelf-runs) for a quick example. Click
-[here](https://amenra.github.io/ranxhub) to learn how to share your own runs
-with the community and lead by example! ## â¡ï¸ Introduction [ranx](https://
-github.com/AmenRa/ranx) ([raÅks]) is a library of fast ranking evaluation
-metrics implemented in [Python](https://en.wikipedia.org/wiki/Python_
-(programming_language)), leveraging [Numba](https://github.com/numba/numba) for
-high-speed [vector operations](https://en.wikipedia.org/wiki/
-Automatic_vectorization) and [automatic parallelization](https://
-en.wikipedia.org/wiki/Automatic_parallelization). It offers a user-friendly
-interface to evaluate and compare [Information Retrieval](https://
-en.wikipedia.org/wiki/Information_retrieval) and [Recommender Systems](https://
-en.wikipedia.org/wiki/Recommender_system). [ranx](https://github.com/AmenRa/
-ranx) allows you to perform statistical tests and export [LaTeX](https://
-en.wikipedia.org/wiki/LaTeX) tables for your scientific publications. Moreover,
-[ranx](https://github.com/AmenRa/ranx) provides several [fusion algorithms]
-(https://amenra.github.io/ranx/fusion) and [normalization strategies](https://
+## ð¥ News - ð [April 4, 2023] [ranxhub](https://amenra.github.io/
+ranxhub), the [ranx](https://github.com/AmenRa/ranx)'s companion repository,
+will be featured in [SIGIR 2023](https://sigir.org/sigir2023)! On [ranxhub]
+(https://amenra.github.io/ranxhub), you can download and share pre-computed
+runs for Information Retrieval datasets, such as [MSMARCO Passage Ranking]
+(https://arxiv.org/abs/1611.09268). - [May 1 2023] `ranx` `0.3.8` is out! This
+release adds early support for results plotting. Specifically, it is now
+possible to plot Interpolated Precision-Recall Curve. Click [here]() for
+further details.   ## â¡ï¸ Introduction [ranx](https://github.com/AmenRa/
+ranx) ([raÅks]) is a library of fast ranking evaluation metrics implemented in
+[Python](https://en.wikipedia.org/wiki/Python_(programming_language)),
+leveraging [Numba](https://github.com/numba/numba) for high-speed [vector
+operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and
+[automatic parallelization](https://en.wikipedia.org/wiki/
+Automatic_parallelization). It offers a user-friendly interface to evaluate and
+compare [Information Retrieval](https://en.wikipedia.org/wiki/
+Information_retrieval) and [Recommender Systems](https://en.wikipedia.org/wiki/
+Recommender_system). [ranx](https://github.com/AmenRa/ranx) allows you to
+perform statistical tests and export [LaTeX](https://en.wikipedia.org/wiki/
+LaTeX) tables for your scientific publications. Moreover, [ranx](https://
+github.com/AmenRa/ranx) provides several [fusion algorithms](https://
+amenra.github.io/ranx/fusion) and [normalization strategies](https://
 amenra.github.io/ranx/normalization), and an automatic [fusion optimization]
 (https://amenra.github.io/ranx/fusion/#optimize-fusion) functionality. [ranx]
 (https://github.com/AmenRa/ranx) was featured in [ECIR 2022](https://
 ecir2022.org) and [CIKM 2022](https://www.cikm2022.org). If you use [ranx]
 (https://github.com/AmenRa/ranx) to evaluate results or conducting experiments
 involving fusion for your scientific publication, please consider citing it:
 [evaluation bibtex](https://dblp.org/rec/conf/ecir/Bassani22.html?view=bibtex),
@@ -140,20 +136,23 @@
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
 3_evaluation.ipynb) | | Comparison and Report | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
 4_comparison_and_report.ipynb) | | Fusion | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
-5_fusion.ipynb) | | Share your runs with [ranxhub](https://amenra.github.io/
-ranxhub) | [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/
-notebooks/6_ranxhub.ipynb) | ## ð Documentation Browse the [documentation]
-(https://amenra.github.io/ranx) for more details and examples. ## ð Citation
-If you use [ranx](https://github.com/AmenRa/ranx) to evaluate results for your
+5_fusion.ipynb) | | Plot | [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/
+blob/master/notebooks/7_plot.ipynb) | | Share your runs with [ranxhub](https://
+amenra.github.io/ranxhub) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
+6_ranxhub.ipynb) | ## ð Documentation Browse the [documentation](https://
+amenra.github.io/ranx) for more details and examples. ## ð Citation If you
+use [ranx](https://github.com/AmenRa/ranx) to evaluate results for your
 scientific publication, please consider citing our [ECIR 2022](https://
 ecir2022.org) paper:  BibTeX ```bibtex @inproceedings{DBLP:conf/ecir/Bassani22,
 author = {Elias Bassani}, title = {ranx: {A} Blazing-Fast Python Library for
 Ranking Evaluation and Comparison}, booktitle = {{ECIR} {(2)}}, series =
 {Lecture Notes in Computer Science}, volume = {13186}, pages = {259--264},
 publisher = {Springer}, year = {2022} } ```  If you use the fusion
 functionalities provided by [ranx](https://github.com/AmenRa/ranx) for
```

### Comparing `ranx-0.3.7/ranx/data_structures/common.py` & `ranx-0.3.8/ranx/data_structures/common.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/data_structures/frozenset_dict.py` & `ranx-0.3.8/ranx/data_structures/frozenset_dict.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/data_structures/generic.py` & `ranx-0.3.8/ranx/data_structures/generic.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/data_structures/optimization_report.py` & `ranx-0.3.8/ranx/data_structures/optimization_report.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/data_structures/qrels.py` & `ranx-0.3.8/ranx/data_structures/qrels.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/data_structures/report.py` & `ranx-0.3.8/ranx/data_structures/report.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/data_structures/run.py` & `ranx-0.3.8/ranx/data_structures/run.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/downloader.py` & `ranx-0.3.8/ranx/downloader.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/__init__.py` & `ranx-0.3.8/ranx/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/bayesfuse.py` & `ranx-0.3.8/ranx/fusion/bayesfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/bordafuse.py` & `ranx-0.3.8/ranx/fusion/bordafuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/comb_anz.py` & `ranx-0.3.8/ranx/fusion/comb_anz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/comb_gmnz.py` & `ranx-0.3.8/ranx/fusion/comb_gmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/comb_max.py` & `ranx-0.3.8/ranx/fusion/comb_max.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/comb_med.py` & `ranx-0.3.8/ranx/fusion/comb_med.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/comb_min.py` & `ranx-0.3.8/ranx/fusion/comb_min.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/comb_mnz.py` & `ranx-0.3.8/ranx/fusion/comb_mnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/comb_sum.py` & `ranx-0.3.8/ranx/fusion/comb_sum.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/common.py` & `ranx-0.3.8/ranx/fusion/common.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/condorcet.py` & `ranx-0.3.8/ranx/fusion/condorcet.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/isr.py` & `ranx-0.3.8/ranx/fusion/isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/log_isr.py` & `ranx-0.3.8/ranx/fusion/log_isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/logn_isr.py` & `ranx-0.3.8/ranx/fusion/logn_isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/mapfuse.py` & `ranx-0.3.8/ranx/fusion/mapfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/mixed.py` & `ranx-0.3.8/ranx/fusion/mixed.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/posfuse.py` & `ranx-0.3.8/ranx/fusion/posfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/probfuse.py` & `ranx-0.3.8/ranx/fusion/probfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/rbc.py` & `ranx-0.3.8/ranx/fusion/rbc.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/rrf.py` & `ranx-0.3.8/ranx/fusion/rrf.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/segfuse.py` & `ranx-0.3.8/ranx/fusion/segfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/slidefuse.py` & `ranx-0.3.8/ranx/fusion/slidefuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/weighted_bordafuse.py` & `ranx-0.3.8/ranx/fusion/weighted_bordafuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/weighted_condorcet.py` & `ranx-0.3.8/ranx/fusion/weighted_condorcet.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/wmnz.py` & `ranx-0.3.8/ranx/fusion/wmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion/wsum.py` & `ranx-0.3.8/ranx/fusion/wsum.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/__init__.py` & `ranx-0.3.8/ranx/fusion_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_comb_gmnz.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_comb_gmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_logn_isr.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_logn_isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_mixed.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_mixed.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_probfuse.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_probfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_rbc.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_rbc.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_rrf.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_rrf.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_slidefuse.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_slidefuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_bordafuse.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_weighted_bordafuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_condorcet.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_weighted_condorcet.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_weights.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_weights.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_wmnz.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_wmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/fusion_optimization/optimize_wsum.py` & `ranx-0.3.8/ranx/fusion_optimization/optimize_wsum.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/io.py` & `ranx-0.3.8/ranx/io.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/meta/compare.py` & `ranx-0.3.8/ranx/meta/compare.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/meta/evaluate.py` & `ranx-0.3.8/ranx/meta/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Dict, List, Union
 
 import numba as nb
 import numpy as np
 from numba import set_num_threads
 
 from ..data_structures import Qrels, Run
-from ..data_structures.common import set_relevance_level
 from ..metrics import metric_switch
 from ..utils import python_dict_to_typed_list
 
 
 def format_metrics(metrics: Union[List[str], str]) -> List[str]:
     if type(metrics) == str:
         metrics = [metrics]
```

### Comparing `ranx-0.3.7/ranx/meta/fuse.py` & `ranx-0.3.8/ranx/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/meta/optimize_fusion.py` & `ranx-0.3.8/ranx/meta/optimize_fusion.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/__init__.py` & `ranx-0.3.8/ranx/metrics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,24 @@
     "ndcg_burges",
     "ndcg",
     "precision",
     "r_precision",
     "rank_biased_precision",
     "recall",
     "reciprocal_rank",
+    "interpolated_precision_at_recall",
 ]
 
 from .average_precision import average_precision
 from .bpref import bpref
 from .f1 import f1
 from .get_hit_lists import get_hit_lists
 from .hit_rate import hit_rate
 from .hits import hits
+from .interpolated_precision_at_recall import interpolated_precision_at_recall
 from .ndcg import ndcg, ndcg_burges
 from .precision import precision
 from .r_precision import r_precision
 from .rank_biased_precision import rank_biased_precision
 from .recall import recall
 from .reciprocal_rank import reciprocal_rank
```

### Comparing `ranx-0.3.7/ranx/metrics/average_precision.py` & `ranx-0.3.8/ranx/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/bpref.py` & `ranx-0.3.8/ranx/metrics/bpref.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/f1.py` & `ranx-0.3.8/ranx/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/get_hit_lists.py` & `ranx-0.3.8/ranx/metrics/get_hit_lists.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/get_non_rel_lists.py` & `ranx-0.3.8/ranx/metrics/get_non_rel_lists.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/get_unjudged_lists.py` & `ranx-0.3.8/ranx/metrics/get_unjudged_lists.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/hit_rate.py` & `ranx-0.3.8/ranx/metrics/hit_rate.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/hits.py` & `ranx-0.3.8/ranx/metrics/hits.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/ndcg.py` & `ranx-0.3.8/ranx/metrics/ndcg.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/precision.py` & `ranx-0.3.8/ranx/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/r_precision.py` & `ranx-0.3.8/ranx/metrics/r_precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/rank_biased_precision.py` & `ranx-0.3.8/ranx/metrics/rank_biased_precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/recall.py` & `ranx-0.3.8/ranx/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/metrics/reciprocal_rank.py` & `ranx-0.3.8/ranx/metrics/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/__init__.py` & `ranx-0.3.8/ranx/normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/borda_norm.py` & `ranx-0.3.8/ranx/normalization/borda_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/common.py` & `ranx-0.3.8/ranx/normalization/common.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/max_norm.py` & `ranx-0.3.8/ranx/normalization/max_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/min_max_norm.py` & `ranx-0.3.8/ranx/normalization/min_max_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/rank_norm.py` & `ranx-0.3.8/ranx/normalization/rank_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/sum_norm.py` & `ranx-0.3.8/ranx/normalization/sum_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/normalization/zmuv_norm.py` & `ranx-0.3.8/ranx/normalization/zmuv_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/statistical_tests/__init__.py` & `ranx-0.3.8/ranx/statistical_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/statistical_tests/fisher_randomization_test.py` & `ranx-0.3.8/ranx/statistical_tests/fisher_randomization_test.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/statistical_tests/paired_student_t_test.py` & `ranx-0.3.8/ranx/statistical_tests/paired_student_t_test.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/statistical_tests/tukey_hsd_test.py` & `ranx-0.3.8/ranx/statistical_tests/tukey_hsd_test.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx/utils.py` & `ranx-0.3.8/ranx/utils.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.7/ranx.egg-info/PKG-INFO` & `ranx-0.3.8/ranx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranx
-Version: 0.3.7
+Version: 0.3.8
 Summary: ranx: A Blazing-Fast Python Library for Ranking Evaluation, Comparison, and Fusion
 Home-page: https://github.com/AmenRa/ranx
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: trec_eval,information retrieval,recommender systems,evaluation,ranking,fusion,metasearch,numba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,24 +34,21 @@
   <a href="https://lbesson.mit-license.org/"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
   <!-- Google Colab -->
   <a href="https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/1_overview.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/></a>
 </p>
 
 ## 🔥 News
 
-- 📌 [October 10, 2022] I released a new sharing platform for pre-computed runs called [ranxhub](https://amenra.github.io/ranxhub), click [here](https://amenra.github.io/ranxhub) to learn more!
+- 📌 [April 4, 2023] [ranxhub](https://amenra.github.io/ranxhub), the [ranx](https://github.com/AmenRa/ranx)'s companion repository, will be featured in [SIGIR 2023](https://sigir.org/sigir2023)!  
+On [ranxhub](https://amenra.github.io/ranxhub), you can download and share pre-computed runs for Information Retrieval datasets, such as [MSMARCO Passage Ranking](https://arxiv.org/abs/1611.09268).
 
-- [November 2, 2022] `ranx` `0.3.3` is out!  
-This release adds support for changing Qrels relevance level, i.e, the minimum relevance judgement score to consider a document to be relevant.  
-You can now define metric-wise relevance levels by appending `-l<num>` to metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`.
-
-- [October 10, 2022] `ranx` `0.3` is out!  
-This release adds integration with [ranxhub](https://amenra.github.io/ranxhub), a new sharing platform for pre-computed runs.  
-Click [here](#off-the-shelf-runs) for a quick example.  
-Click [here](https://amenra.github.io/ranxhub) to learn how to share your own runs with the community and lead by example!
+- [May 1 2023] `ranx` `0.3.8` is out!  
+This release adds early support for results plotting. Specifically, it is now possible to plot Interpolated Precision-Recall Curve. Click [here]() for further details.
+<!-- This release adds support for changing Qrels relevance level, i.e, the minimum relevance judgement score to consider a document to be relevant.   -->
+<!-- You can now define metric-wise relevance levels by appending `-l<num>` to metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`. -->
 
 ## ⚡️ Introduction
 
 [ranx](https://github.com/AmenRa/ranx) ([raŋks]) is a library of fast ranking evaluation metrics implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)), leveraging [Numba](https://github.com/numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization](https://en.wikipedia.org/wiki/Automatic_parallelization).
 It offers a user-friendly interface to evaluate and compare [Information Retrieval](https://en.wikipedia.org/wiki/Information_retrieval) and [Recommender Systems](https://en.wikipedia.org/wiki/Recommender_system).
 [ranx](https://github.com/AmenRa/ranx) allows you to perform statistical tests and export [LaTeX](https://en.wikipedia.org/wiki/LaTeX) tables for your scientific publications.
 Moreover, [ranx](https://github.com/AmenRa/ranx) provides several [fusion algorithms](https://amenra.github.io/ranx/fusion) and [normalization strategies](https://amenra.github.io/ranx/normalization), and an automatic [fusion optimization](https://amenra.github.io/ranx/fusion/#optimize-fusion) functionality.
@@ -221,14 +218,15 @@
 | Name                                                             | Link                                                                                                                                                                                   |
 | ---------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Overview                                                         | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/1_overview.ipynb)              |
 | Qrels and Run                                                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/2_qrels_and_run.ipynb)         |
 | Evaluation                                                       | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/3_evaluation.ipynb)            |
 | Comparison and Report                                            | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/4_comparison_and_report.ipynb) |
 | Fusion                                                           | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/5_fusion.ipynb)                |
+| Plot                                                             | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/7_plot.ipynb)                  |
 | Share your runs with [ranxhub](https://amenra.github.io/ranxhub) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/6_ranxhub.ipynb)               |
 
 
 ## 📚 Documentation
 Browse the [documentation](https://amenra.github.io/ranx) for more details and examples.
```

#### html2text {}

```diff
@@ -1,47 +1,43 @@
-Metadata-Version: 2.1 Name: ranx Version: 0.3.7 Summary: ranx: A Blazing-Fast
+Metadata-Version: 2.1 Name: ranx Version: 0.3.8 Summary: ranx: A Blazing-Fast
 Python Library for Ranking Evaluation, Comparison, and Fusion Home-page: https:
 //github.com/AmenRa/ranx Author: Elias Bassani Author-email:
 elias.bssn@gmail.com Keywords: trec_eval,information retrieval,recommender
 systems,evaluation,ranking,fusion,metasearch,numba Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing :: General Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [https://repository-images.githubusercontent.com/268892956/750228ec-f3f2-465d-
                               9c17-420c688ba2bc]
      [https://badges.aleen42.com/src/python.svg]  [PyPI_version]  [Download
  counter]  [Documentation_Status]  [https://img.shields.io/badge/code%20style-
               black-000000.svg]  [License:_MIT]  [Open_in_Colab]
-## ð¥ News - ð [October 10, 2022] I released a new sharing platform for
-pre-computed runs called [ranxhub](https://amenra.github.io/ranxhub), click
-[here](https://amenra.github.io/ranxhub) to learn more! - [November 2, 2022]
-`ranx` `0.3.3` is out! This release adds support for changing Qrels relevance
-level, i.e, the minimum relevance judgement score to consider a document to be
-relevant. You can now define metric-wise relevance levels by appending `-l` to
-metric names (e.g., `evaluate(qrels, run, ["map@100-l2", "ndcg-l3])`), or
-setting the Qrels relevance level qrels-wise as `qrels.set_relevance_level(2)`.
-- [October 10, 2022] `ranx` `0.3` is out! This release adds integration with
-[ranxhub](https://amenra.github.io/ranxhub), a new sharing platform for pre-
-computed runs. Click [here](#off-the-shelf-runs) for a quick example. Click
-[here](https://amenra.github.io/ranxhub) to learn how to share your own runs
-with the community and lead by example! ## â¡ï¸ Introduction [ranx](https://
-github.com/AmenRa/ranx) ([raÅks]) is a library of fast ranking evaluation
-metrics implemented in [Python](https://en.wikipedia.org/wiki/Python_
-(programming_language)), leveraging [Numba](https://github.com/numba/numba) for
-high-speed [vector operations](https://en.wikipedia.org/wiki/
-Automatic_vectorization) and [automatic parallelization](https://
-en.wikipedia.org/wiki/Automatic_parallelization). It offers a user-friendly
-interface to evaluate and compare [Information Retrieval](https://
-en.wikipedia.org/wiki/Information_retrieval) and [Recommender Systems](https://
-en.wikipedia.org/wiki/Recommender_system). [ranx](https://github.com/AmenRa/
-ranx) allows you to perform statistical tests and export [LaTeX](https://
-en.wikipedia.org/wiki/LaTeX) tables for your scientific publications. Moreover,
-[ranx](https://github.com/AmenRa/ranx) provides several [fusion algorithms]
-(https://amenra.github.io/ranx/fusion) and [normalization strategies](https://
+## ð¥ News - ð [April 4, 2023] [ranxhub](https://amenra.github.io/
+ranxhub), the [ranx](https://github.com/AmenRa/ranx)'s companion repository,
+will be featured in [SIGIR 2023](https://sigir.org/sigir2023)! On [ranxhub]
+(https://amenra.github.io/ranxhub), you can download and share pre-computed
+runs for Information Retrieval datasets, such as [MSMARCO Passage Ranking]
+(https://arxiv.org/abs/1611.09268). - [May 1 2023] `ranx` `0.3.8` is out! This
+release adds early support for results plotting. Specifically, it is now
+possible to plot Interpolated Precision-Recall Curve. Click [here]() for
+further details.   ## â¡ï¸ Introduction [ranx](https://github.com/AmenRa/
+ranx) ([raÅks]) is a library of fast ranking evaluation metrics implemented in
+[Python](https://en.wikipedia.org/wiki/Python_(programming_language)),
+leveraging [Numba](https://github.com/numba/numba) for high-speed [vector
+operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and
+[automatic parallelization](https://en.wikipedia.org/wiki/
+Automatic_parallelization). It offers a user-friendly interface to evaluate and
+compare [Information Retrieval](https://en.wikipedia.org/wiki/
+Information_retrieval) and [Recommender Systems](https://en.wikipedia.org/wiki/
+Recommender_system). [ranx](https://github.com/AmenRa/ranx) allows you to
+perform statistical tests and export [LaTeX](https://en.wikipedia.org/wiki/
+LaTeX) tables for your scientific publications. Moreover, [ranx](https://
+github.com/AmenRa/ranx) provides several [fusion algorithms](https://
+amenra.github.io/ranx/fusion) and [normalization strategies](https://
 amenra.github.io/ranx/normalization), and an automatic [fusion optimization]
 (https://amenra.github.io/ranx/fusion/#optimize-fusion) functionality. [ranx]
 (https://github.com/AmenRa/ranx) was featured in [ECIR 2022](https://
 ecir2022.org) and [CIKM 2022](https://www.cikm2022.org). If you use [ranx]
 (https://github.com/AmenRa/ranx) to evaluate results or conducting experiments
 involving fusion for your scientific publication, please consider citing it:
 [evaluation bibtex](https://dblp.org/rec/conf/ecir/Bassani22.html?view=bibtex),
@@ -149,20 +145,23 @@
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
 3_evaluation.ipynb) | | Comparison and Report | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
 4_comparison_and_report.ipynb) | | Fusion | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
-5_fusion.ipynb) | | Share your runs with [ranxhub](https://amenra.github.io/
-ranxhub) | [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/blob/master/
-notebooks/6_ranxhub.ipynb) | ## ð Documentation Browse the [documentation]
-(https://amenra.github.io/ranx) for more details and examples. ## ð Citation
-If you use [ranx](https://github.com/AmenRa/ranx) to evaluate results for your
+5_fusion.ipynb) | | Plot | [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/github/AmenRa/ranx/
+blob/master/notebooks/7_plot.ipynb) | | Share your runs with [ranxhub](https://
+amenra.github.io/ranxhub) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/AmenRa/ranx/blob/master/notebooks/
+6_ranxhub.ipynb) | ## ð Documentation Browse the [documentation](https://
+amenra.github.io/ranx) for more details and examples. ## ð Citation If you
+use [ranx](https://github.com/AmenRa/ranx) to evaluate results for your
 scientific publication, please consider citing our [ECIR 2022](https://
 ecir2022.org) paper:  BibTeX ```bibtex @inproceedings{DBLP:conf/ecir/Bassani22,
 author = {Elias Bassani}, title = {ranx: {A} Blazing-Fast Python Library for
 Ranking Evaluation and Comparison}, booktitle = {{ECIR} {(2)}}, series =
 {Lecture Notes in Computer Science}, volume = {13186}, pages = {259--264},
 publisher = {Springer}, year = {2022} } ```  If you use the fusion
 functionalities provided by [ranx](https://github.com/AmenRa/ranx) for
```

### Comparing `ranx-0.3.7/ranx.egg-info/SOURCES.txt` & `ranx-0.3.8/ranx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -65,24 +65,26 @@
 ranx/fusion_optimization/optimize_wsum.py
 ranx/meta/__init__.py
 ranx/meta/compare.py
 ranx/meta/evaluate.py
 ranx/meta/fuse.py
 ranx/meta/normalize.py
 ranx/meta/optimize_fusion.py
+ranx/meta/plot.py
 ranx/metrics/__init__.py
 ranx/metrics/average_precision.py
 ranx/metrics/bpref.py
 ranx/metrics/common.py
 ranx/metrics/f1.py
 ranx/metrics/get_hit_lists.py
 ranx/metrics/get_non_rel_lists.py
 ranx/metrics/get_unjudged_lists.py
 ranx/metrics/hit_rate.py
 ranx/metrics/hits.py
+ranx/metrics/interpolated_precision_at_recall.py
 ranx/metrics/ndcg.py
 ranx/metrics/precision.py
 ranx/metrics/r_precision.py
 ranx/metrics/rank_biased_precision.py
 ranx/metrics/recall.py
 ranx/metrics/reciprocal_rank.py
 ranx/normalization/__init__.py
```

### Comparing `ranx-0.3.7/setup.py` & `ranx-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ranx",
-    version="0.3.7",
+    version="0.3.8",
     author="Elias Bassani",
     author_email="elias.bssn@gmail.com",
     description="ranx: A Blazing-Fast Python Library for Ranking Evaluation, Comparison, and Fusion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AmenRa/ranx",
     packages=setuptools.find_packages(),
```

