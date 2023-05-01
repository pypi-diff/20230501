# Comparing `tmp/sil-thot-3.4.0.tar.gz` & `tmp/sil-thot-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sil-thot-3.4.0.tar", last modified: Fri Jan 27 11:13:59 2023, max compression
+gzip compressed data, was "sil-thot-3.4.1.tar", last modified: Mon May  1 10:47:11 2023, max compression
```

## Comparing `sil-thot-3.4.0.tar` & `sil-thot-3.4.1.tar`

### file list

```diff
@@ -1,431 +1,431 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.940896 sil-thot-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-27 11:13:49.000000 sil-thot-3.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-01-27 11:13:49.000000 sil-thot-3.4.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-01-27 11:13:49.000000 sil-thot-3.4.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-27 11:13:49.000000 sil-thot-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-01-27 11:13:59.940896 sil-thot-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-27 11:13:49.000000 sil-thot-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.884895 sil-thot-3.4.0/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-01-27 11:13:49.000000 sil-thot-3.4.0/cmake/FindGMP.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.880895 sil-thot-3.4.0/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.884895 sil-thot-3.4.0/include/hat_trie/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/array_growth_policy.h
--rw-r--r--   0 runner    (1001) docker     (123)    65286 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/array_hash.h
--rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/array_map.h
--rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/array_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    80533 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/htrie_hash.h
--rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/htrie_map.h
--rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-01-27 11:13:49.000000 sil-thot-3.4.0/include/hat_trie/htrie_set.h
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-27 11:13:49.000000 sil-thot-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 11:13:59.940896 sil-thot-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-01-27 11:13:49.000000 sil-thot-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.884895 sil-thot-3.4.0/sil_thot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-01-27 11:13:59.000000 sil-thot-3.4.0/sil_thot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-01-27 11:13:59.000000 sil-thot-3.4.0/sil_thot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 11:13:59.000000 sil-thot-3.4.0/sil_thot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 11:13:59.000000 sil-thot-3.4.0/sil_thot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-27 11:13:59.000000 sil-thot-3.4.0/sil_thot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-27 11:13:59.000000 sil-thot-3.4.0/sil_thot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.884895 sil-thot-3.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.884895 sil-thot-3.4.0/src/downhill_simplex/
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/downhill_simplex/step_by_step_dhs.c
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/downhill_simplex/step_by_step_dhs.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.892895 sil-thot-3.4.0/src/error_correction/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/BaseEcModelForNbUcat.h
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/BaseEcmForWg.h
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/BaseEditDist.h
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/BaseErrorCorrectionModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/BaseErrorCorrectionModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/BaseWgProcessorForAnlp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/EditDistForStr.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/EditDistForStr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/EditDistForVec.h
--rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/EditDistForVecString.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/EditDistForVecString.h
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/HypStateIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/NbSearchHighLevelHyp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/NbSearchHyp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/NbSearchStack.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/NbSearchStack.h
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/NbestCorrections.h
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/NonPbEcModelForNbUcat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/NonPbEcModelForNbUcat.h
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/PfsmEcm.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/PfsmEcm.h
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/PfsmEcmForWg.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/PfsmEcmForWg.h
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/PfsmEcmForWgEsi.h
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/PrefAlignInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/RejectedWordsSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WgHandler.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WgHandler.h
--rw-r--r--   0 runner    (1001) docker     (123)    55383 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WgProcessorForAnlp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WordAndCharLevelOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    45664 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WordGraph.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WordGraph.h
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WordGraphArc.h
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WordGraphArcId.h
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/WordGraphStateData.h
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/_editDist.h
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/_editDistBasedEcm.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/error_correction/_editDistBasedEcm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.892895 sil-thot-3.4.0/src/incr_models/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/BaseIncrCondProbModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/BaseIncrCondProbTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/BaseIncrEncCondProbModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/BaseIncrEncoder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/BaseWordPenaltyModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/IncrCondProbTable.h
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/IncrEncoder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/IncrJelMerNgramLM.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/IncrJelMerNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/IncrNgramLM.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/IncrNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/WordPenaltyModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/WordPenaltyModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/WordPredictor.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/WordPredictor.h
--rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/_incrEncCondProbModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/_incrJelMerNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (123)    19692 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/_incrNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/im_pair.h
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/lm_ienc.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/lm_ienc.h
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/vecx_x_incr_cptable.h
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/vecx_x_incr_ecpm.h
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/incr_models/vecx_x_incr_enc.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.900895 sil-thot-3.4.0/src/nlp_common/
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/AwkInputStream.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/AwkInputStream.h
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/BaseIncrNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/BaseNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/BidTrie.h
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Bitset.h
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Count.h
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/ErrorDefs.h
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/LM_Defs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/LogCount.h
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/MathDefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/MathFuncs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/MathFuncs.h
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/NbestTableNode.h
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/NbestTransTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/OrderedVector.h
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/PositionIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Prob.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Prob.h
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Score.h
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/SingleWordVocab.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/SingleWordVocab.h
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/SmtDefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/StrProcUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/StrProcUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/TranslationData.h
--rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/Trie.h
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/TrieVecs.h
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/WordAlignmentMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/WordAlignmentMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/WordClasses.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/WordClasses.h
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/WordIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/ctimer.c
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/ctimer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/getdelim.c
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/getdelim.h
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/getline.c
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/getline.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/ins_op_pair.h
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/lt_op_vec.h
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/printAligFuncs.cc
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/printAligFuncs.h
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/uiHashF.h
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/nlp_common/uiPairHashF.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.908896 sil-thot-3.4.0/src/phrase_models/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/AligInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/AlignmentContainer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/AlignmentContainer.h
--rw-r--r--   0 runner    (1001) docker     (123)    16515 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/AlignmentExtractor.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/AlignmentExtractor.h
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BaseCountPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BaseIncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BaseIncrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BasePhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BasePhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BasePhrasePairFilter.h
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BasePhraseTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BpSet.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BpSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/BpSetInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/CategPhrasePairFilter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/CategPhrasePairFilter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/CellAlignment.h
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/CellID.h
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/HatTriePhraseTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/HatTriePhraseTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/IncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/IncrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseDefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseExtractParameters.h
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseExtractUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseExtractUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseExtractionCell.h
--rw-r--r--   0 runner    (1001) docker     (123)    35713 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseExtractionTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseExtractionTable.h
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseId.h
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhrasePair.h
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhrasePairInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseSortCriterion.h
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/PhraseTransTableNodeData.h
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SegLenTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SegLenTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SentSegmentation.h
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrcSegmLenTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrcSegmLenTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrfBisegm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrfNodeInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrfNodeInfoMap.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrfNodeInfoMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrfNodeKey.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/SrfNodeKey.h
--rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/StlPhraseTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/StlPhraseTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/StrictCategPhrasePairFilter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/StrictCategPhrasePairFilter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/TrgCutsTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/TrgCutsTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/TrgSegmLenTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/TrgSegmLenTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/VecUnsignedIntSortCriterion.h
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/WbaIncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/WbaIncrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/_incrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/_incrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/_wbaIncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/phrase_models/_wbaIncrPhraseModel.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.908896 sil-thot-3.4.0/src/python_module/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/python_module/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    44740 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/python_module/module.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.908896 sil-thot-3.4.0/src/shared_library/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/shared_library/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    37169 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/shared_library/thot.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/shared_library/thot.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.924896 sil-thot-3.4.0/src/stack_dec/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseAssistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseHypState.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseHypState.h
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseHypothesis.h
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseHypothesisRec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseLogLinWeightUpdater.h
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseMiraScorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BasePbTransModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BasePbTransModelFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BasePbTransModelStats.h
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BasePhraseHypothesis.h
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BasePhraseHypothesisRec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseScorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseSmtModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseSmtMultiStack.h
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseSmtStack.h
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseStackDecoder.h
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/BaseTranslationMetadata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/DictFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/DictFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/DirectPhraseModelFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/DirectPhraseModelFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/FeaturesInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/HypSortCriterion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/HypStateDict.h
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/HypStateDictData.h
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/InversePhraseModelFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/InversePhraseModelFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/KbMiraLlWu.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/KbMiraLlWu.h
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/LM_State.h
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/LangModelFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/LangModelFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/LangModelInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/LangModelPars.h
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraBleu.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraBleu.h
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraChrF.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraChrF.h
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraGtm.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraGtm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraWer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/MiraWer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/NbestTransCacheData.h
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/OnTheFlyDictFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/OnTheFlyDictFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/OnlineTrainingPars.h
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PbTransModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PbTransModelInputVars.h
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PbTransModelPars.h
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypData.h
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypDataStr.h
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypEqClassF.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypEqClassF.h
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumps01EqClassF.h
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumpsEqClassF.h
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypState.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrHypState.h
--rw-r--r--   0 runner    (1001) docker     (123)    48659 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrLocalSwLiTm.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrLocalSwLiTm.h
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrLocalSwLiTmHypRec.h
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrNbestTransTable.h
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrNbestTransTablePref.h
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrNbestTransTablePrefKey.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrNbestTransTablePrefKey.h
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrNbestTransTableRef.h
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrNbestTransTableRefKey.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrNbestTransTableRefKey.h
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrScoreInfo.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrScoreInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhraseBasedTmHyp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhraseBasedTmHypRec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhraseCacheTable.h
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhraseModelInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhraseModelPars.h
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/PhrasePairCacheTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/ScoreCompDefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SmtModelUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SmtModelUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SmtMultiStackRec.h
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SmtStack.h
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SourceSegmentation.h
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SrcPhraseLenFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SrcPhraseLenFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SrcPosJumpFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SrcPosJumpFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SwModelInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/SwModelPars.h
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/TranslationMetadata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/TrgPhraseLenFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/TrgPhraseLenFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/WeightUpdateUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/WeightUpdateUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/WgUncoupledAssistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/WordPenaltyFeat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/WordPenaltyFeat.h
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_assistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_nbUncoupledAssistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (123)   105202 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_pbTransModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_phrSwTransModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    99378 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_phraseBasedTransModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_phraseHypothesis.h
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_phraseHypothesisRec.h
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_smtModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_smtMultiStack.h
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_smtStack.h
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_stackDecoder.h
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_stackDecoderRec.h
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/_stack_decoder_statistics.h
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/bleu.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/bleu.h
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/chrf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/chrf.h
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/stack_dec/multi_stack_decoder_rec.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.936896 sil-thot-3.4.0/src/sw_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Aligner.h
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/AlignmentInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/AlignmentModelBase.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/AlignmentModelBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/AlignmentTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/AlignmentTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/CachedHmmAligLgProb.cc
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/CachedHmmAligLgProb.h
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/DiagonalAlignment.h
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/DistortionTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/DistortionTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/DoubleMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/DoubleMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    25734 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/FastAlignModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/FastAlignModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/FertilityTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/FertilityTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/HeadDistortionTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/HeadDistortionTable.h
--rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/HmmAlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/HmmAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/HmmAlignmentTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/HmmAlignmentTable.h
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm1AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm1AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm2AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm2AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    35398 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm3AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm3AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm4AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Ibm4AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentTrainer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentTrainer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentTrainer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentTrainer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentTrainer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentTrainer.h
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/LexCounts.h
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/LexTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/LightSentenceHandler.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/LightSentenceHandler.h
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/Md.h
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/MemoryLexTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/MemoryLexTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/NonheadDistortionTable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/NonheadDistortionTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/NormalSentenceLengthModel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/NormalSentenceLengthModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/SentenceHandler.h
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/SentenceLengthModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/SentenceLengthModelBase.cc
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/SentenceLengthModelBase.h
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/StepwiseAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/SwDefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/SymmetrizedAligner.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/SymmetrizedAligner.h
--rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/anjiMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/anjiMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/anjm1ip_anjiMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-01-27 11:13:49.000000 sil-thot-3.4.0/src/sw_models/anjm1ip_anjiMatrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.936896 sil-thot-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.936896 sil-thot-3.4.0/tests/nlp_common/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/nlp_common/WordAlignmentMatrixTest.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.936896 sil-thot-3.4.0/tests/phrase_models/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/phrase_models/HatTriePhraseTableTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/phrase_models/StlPhraseTableTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18181 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/phrase_models/_phraseTableTest.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.936896 sil-thot-3.4.0/tests/stack_dec/
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/stack_dec/KbMiraLlWuTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/stack_dec/MiraChrFTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/stack_dec/PhrLocalSwLiTmTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/stack_dec/TranslationMetadataTest.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.940896 sil-thot-3.4.0/tests/sw_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/sw_models/FastAlignModelTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/sw_models/Ibm4AlignmentModelTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/sw_models/IncrHmmAlignmentModelTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/sw_models/LexTableTest.h
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/sw_models/MemoryLexTableTest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/sw_models/TestUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/sw_models/TestUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-01-27 11:13:49.000000 sil-thot-3.4.0/tests/test_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.940896 sil-thot-3.4.0/thot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.940896 sil-thot-3.4.0/thot/alignment/
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-01-27 11:13:49.000000 sil-thot-3.4.0/thot/alignment/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.940896 sil-thot-3.4.0/thot/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-01-27 11:13:49.000000 sil-thot-3.4.0/thot/common/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:49.000000 sil-thot-3.4.0/thot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 11:13:59.940896 sil-thot-3.4.0/thot/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-01-27 11:13:49.000000 sil-thot-3.4.0/thot/translation/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.502314 sil-thot-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-01 10:47:01.000000 sil-thot-3.4.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-01 10:47:01.000000 sil-thot-3.4.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-01 10:47:01.000000 sil-thot-3.4.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 10:47:01.000000 sil-thot-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-01 10:47:11.502314 sil-thot-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-01 10:47:01.000000 sil-thot-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.454313 sil-thot-3.4.1/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-01 10:47:01.000000 sil-thot-3.4.1/cmake/FindGMP.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.450313 sil-thot-3.4.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.454313 sil-thot-3.4.1/include/hat_trie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/array_growth_policy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65286 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/array_hash.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/array_map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80533 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/htrie_hash.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/htrie_map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-05-01 10:47:01.000000 sil-thot-3.4.1/include/hat_trie/htrie_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-01 10:47:01.000000 sil-thot-3.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:47:11.502314 sil-thot-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-01 10:47:01.000000 sil-thot-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.454313 sil-thot-3.4.1/sil_thot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-01 10:47:11.000000 sil-thot-3.4.1/sil_thot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-05-01 10:47:11.000000 sil-thot-3.4.1/sil_thot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:47:11.000000 sil-thot-3.4.1/sil_thot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:47:11.000000 sil-thot-3.4.1/sil_thot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 10:47:11.000000 sil-thot-3.4.1/sil_thot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 10:47:11.000000 sil-thot-3.4.1/sil_thot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.454313 sil-thot-3.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.454313 sil-thot-3.4.1/src/downhill_simplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/downhill_simplex/step_by_step_dhs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/downhill_simplex/step_by_step_dhs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.458313 sil-thot-3.4.1/src/error_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/BaseEcModelForNbUcat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/BaseEcmForWg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/BaseEditDist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/BaseErrorCorrectionModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/BaseErrorCorrectionModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/BaseWgProcessorForAnlp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/EditDistForStr.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/EditDistForStr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/EditDistForVec.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/EditDistForVecString.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/EditDistForVecString.h
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/HypStateIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/NbSearchHighLevelHyp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/NbSearchHyp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/NbSearchStack.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/NbSearchStack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/NbestCorrections.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/NonPbEcModelForNbUcat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/NonPbEcModelForNbUcat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/PfsmEcm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/PfsmEcm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/PfsmEcmForWg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/PfsmEcmForWg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/PfsmEcmForWgEsi.h
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/PrefAlignInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/RejectedWordsSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WgHandler.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WgHandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55383 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WgProcessorForAnlp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WordAndCharLevelOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45668 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WordGraph.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WordGraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WordGraphArc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WordGraphArcId.h
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/WordGraphStateData.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/_editDist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/_editDistBasedEcm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/error_correction/_editDistBasedEcm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.462313 sil-thot-3.4.1/src/incr_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/BaseIncrCondProbModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/BaseIncrCondProbTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/BaseIncrEncCondProbModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/BaseIncrEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/BaseWordPenaltyModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/IncrCondProbTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/IncrEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/IncrJelMerNgramLM.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/IncrJelMerNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/IncrNgramLM.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/IncrNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/WordPenaltyModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/WordPenaltyModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/WordPredictor.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/WordPredictor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/_incrEncCondProbModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/_incrJelMerNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19692 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/_incrNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/im_pair.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/lm_ienc.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/lm_ienc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/vecx_x_incr_cptable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/vecx_x_incr_ecpm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/incr_models/vecx_x_incr_enc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.470313 sil-thot-3.4.1/src/nlp_common/
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/AwkInputStream.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/AwkInputStream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/BaseIncrNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/BaseNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/BidTrie.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Count.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/ErrorDefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/LM_Defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/LogCount.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/MathDefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/MathFuncs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/MathFuncs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/NbestTableNode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/NbestTransTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/OrderedVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/PositionIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Prob.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Prob.h
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Score.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/SingleWordVocab.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/SingleWordVocab.h
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/SmtDefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/StrProcUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/StrProcUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/TranslationData.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/Trie.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/TrieVecs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/WordAlignmentMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/WordAlignmentMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/WordClasses.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/WordClasses.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/WordIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/ctimer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/ctimer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/getdelim.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/getdelim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/getline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/getline.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/ins_op_pair.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/lt_op_vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/printAligFuncs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/printAligFuncs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/uiHashF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/nlp_common/uiPairHashF.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.478314 sil-thot-3.4.1/src/phrase_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/AligInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/AlignmentContainer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/AlignmentContainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16515 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/AlignmentExtractor.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/AlignmentExtractor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BaseCountPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BaseIncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BaseIncrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BasePhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BasePhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BasePhrasePairFilter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BasePhraseTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BpSet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BpSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/BpSetInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/CategPhrasePairFilter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/CategPhrasePairFilter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/CellAlignment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/CellID.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/HatTriePhraseTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/HatTriePhraseTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/IncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/IncrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseDefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseExtractParameters.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseExtractUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseExtractUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseExtractionCell.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35713 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseExtractionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseExtractionTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseId.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhrasePair.h
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhrasePairInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseSortCriterion.h
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/PhraseTransTableNodeData.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SegLenTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SegLenTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SentSegmentation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrcSegmLenTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrcSegmLenTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrfBisegm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrfNodeInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrfNodeInfoMap.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrfNodeInfoMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrfNodeKey.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/SrfNodeKey.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/StlPhraseTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/StlPhraseTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/StrictCategPhrasePairFilter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/StrictCategPhrasePairFilter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/TrgCutsTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/TrgCutsTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/TrgSegmLenTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/TrgSegmLenTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/VecUnsignedIntSortCriterion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/WbaIncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/WbaIncrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/_incrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/_incrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/_wbaIncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/phrase_models/_wbaIncrPhraseModel.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.478314 sil-thot-3.4.1/src/python_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/python_module/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    44740 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/python_module/module.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.478314 sil-thot-3.4.1/src/shared_library/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/shared_library/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37169 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/shared_library/thot.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/shared_library/thot.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.490314 sil-thot-3.4.1/src/stack_dec/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseAssistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseHypState.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseHypState.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseHypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseHypothesisRec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseLogLinWeightUpdater.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseMiraScorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BasePbTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BasePbTransModelFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BasePbTransModelStats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BasePhraseHypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BasePhraseHypothesisRec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseScorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseSmtModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseSmtMultiStack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseSmtStack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseStackDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/BaseTranslationMetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/DictFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/DictFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/DirectPhraseModelFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/DirectPhraseModelFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/FeaturesInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/HypSortCriterion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/HypStateDict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/HypStateDictData.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/InversePhraseModelFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/InversePhraseModelFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/KbMiraLlWu.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/KbMiraLlWu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/LM_State.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/LangModelFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/LangModelFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/LangModelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/LangModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraBleu.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraBleu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraChrF.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraChrF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraGtm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraGtm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraWer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/MiraWer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/NbestTransCacheData.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/OnTheFlyDictFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/OnTheFlyDictFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/OnlineTrainingPars.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PbTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PbTransModelInputVars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PbTransModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypData.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypDataStr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypEqClassF.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypEqClassF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumps01EqClassF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumpsEqClassF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypState.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrHypState.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48659 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrLocalSwLiTm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrLocalSwLiTm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrLocalSwLiTmHypRec.h
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrNbestTransTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrNbestTransTablePref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrNbestTransTablePrefKey.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrNbestTransTablePrefKey.h
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrNbestTransTableRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrNbestTransTableRefKey.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrNbestTransTableRefKey.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrScoreInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrScoreInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhraseBasedTmHyp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhraseBasedTmHypRec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhraseCacheTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhraseModelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhraseModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/PhrasePairCacheTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/ScoreCompDefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SmtModelUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SmtModelUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SmtMultiStackRec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SmtStack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SourceSegmentation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SrcPhraseLenFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SrcPhraseLenFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SrcPosJumpFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SrcPosJumpFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SwModelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/SwModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/TranslationMetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/TrgPhraseLenFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/TrgPhraseLenFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/WeightUpdateUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/WeightUpdateUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/WgUncoupledAssistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/WordPenaltyFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/WordPenaltyFeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_assistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_nbUncoupledAssistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105202 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_pbTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_phrSwTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    99378 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_phraseBasedTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_phraseHypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_phraseHypothesisRec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_smtModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_smtMultiStack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_smtStack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_stackDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_stackDecoderRec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/_stack_decoder_statistics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/bleu.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/bleu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/chrf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/chrf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/stack_dec/multi_stack_decoder_rec.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/src/sw_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Aligner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/AlignmentInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/AlignmentModelBase.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/AlignmentModelBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/AlignmentTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/AlignmentTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/CachedHmmAligLgProb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/CachedHmmAligLgProb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/DiagonalAlignment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/DistortionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/DistortionTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/DoubleMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/DoubleMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25734 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/FastAlignModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/FastAlignModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/FertilityTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/FertilityTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/HeadDistortionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/HeadDistortionTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/HmmAlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/HmmAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/HmmAlignmentTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/HmmAlignmentTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm1AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm1AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm2AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm2AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35398 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm3AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm3AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm4AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Ibm4AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentTrainer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentTrainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentTrainer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentTrainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentTrainer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentTrainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/LexCounts.h
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/LexTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/LightSentenceHandler.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/LightSentenceHandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/Md.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/MemoryLexTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/MemoryLexTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/NonheadDistortionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/NonheadDistortionTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/NormalSentenceLengthModel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/NormalSentenceLengthModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/SentenceHandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/SentenceLengthModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/SentenceLengthModelBase.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/SentenceLengthModelBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/StepwiseAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/SwDefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/SymmetrizedAligner.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/SymmetrizedAligner.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/anjiMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/anjiMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/anjm1ip_anjiMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-01 10:47:01.000000 sil-thot-3.4.1/src/sw_models/anjm1ip_anjiMatrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/tests/nlp_common/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/nlp_common/WordAlignmentMatrixTest.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/tests/phrase_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/phrase_models/HatTriePhraseTableTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/phrase_models/StlPhraseTableTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18181 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/phrase_models/_phraseTableTest.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/tests/stack_dec/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/stack_dec/KbMiraLlWuTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/stack_dec/MiraChrFTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/stack_dec/PhrLocalSwLiTmTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/stack_dec/TranslationMetadataTest.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/tests/sw_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/sw_models/FastAlignModelTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/sw_models/Ibm4AlignmentModelTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/sw_models/IncrHmmAlignmentModelTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/sw_models/LexTableTest.h
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/sw_models/MemoryLexTableTest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/sw_models/TestUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/sw_models/TestUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-01 10:47:01.000000 sil-thot-3.4.1/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/thot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.498314 sil-thot-3.4.1/thot/alignment/
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-05-01 10:47:01.000000 sil-thot-3.4.1/thot/alignment/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.502314 sil-thot-3.4.1/thot/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-01 10:47:01.000000 sil-thot-3.4.1/thot/common/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:01.000000 sil-thot-3.4.1/thot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:47:11.502314 sil-thot-3.4.1/thot/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-01 10:47:01.000000 sil-thot-3.4.1/thot/translation/__init__.pyi
```

### Comparing `sil-thot-3.4.0/CMakeLists.txt` & `sil-thot-3.4.1/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     cmake_policy(SET CMP0135 OLD)
 endif()
 if(POLICY CMP0127)
     set(CMAKE_POLICY_DEFAULT_CMP0127 OLD)
 endif()
 set(CMAKE_POLICY_DEFAULT_CMP0077 NEW)
 # set(CMAKE_MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")
-project(Thot VERSION 3.4.0 LANGUAGES CXX C)
+project(Thot VERSION 3.4.1 LANGUAGES CXX C)
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
 
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
```

### Comparing `sil-thot-3.4.0/COPYING.LESSER` & `sil-thot-3.4.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/PKG-INFO` & `sil-thot-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sil-thot
-Version: 3.4.0
+Version: 3.4.1
 Summary: A toolkit for statistical word alignment and machine translation
 Home-page: https://github.com/sillsdev/thot
 Author: SIL International
 Maintainer: Damien Daspit
 Maintainer-email: damien_daspit@sil.org
 License: LGPL-3.0
 Project-URL: Repository, https://github.com/sillsdev/thot
```

### Comparing `sil-thot-3.4.0/cmake/FindGMP.cmake` & `sil-thot-3.4.1/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/LICENSE` & `sil-thot-3.4.1/include/hat_trie/LICENSE`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/array_growth_policy.h` & `sil-thot-3.4.1/include/hat_trie/array_growth_policy.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/array_hash.h` & `sil-thot-3.4.1/include/hat_trie/array_hash.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/array_map.h` & `sil-thot-3.4.1/include/hat_trie/array_map.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/array_set.h` & `sil-thot-3.4.1/include/hat_trie/array_set.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/htrie_hash.h` & `sil-thot-3.4.1/include/hat_trie/htrie_hash.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/htrie_map.h` & `sil-thot-3.4.1/include/hat_trie/htrie_map.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/include/hat_trie/htrie_set.h` & `sil-thot-3.4.1/include/hat_trie/htrie_set.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/setup.py` & `sil-thot-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="sil-thot",
-    version="3.4.0",
+    version="3.4.1",
     author="SIL International",
     maintainer="Damien Daspit",
     maintainer_email="damien_daspit@sil.org",
     description="A toolkit for statistical word alignment and machine translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="LGPL-3.0",
```

### Comparing `sil-thot-3.4.0/sil_thot.egg-info/PKG-INFO` & `sil-thot-3.4.1/sil_thot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sil-thot
-Version: 3.4.0
+Version: 3.4.1
 Summary: A toolkit for statistical word alignment and machine translation
 Home-page: https://github.com/sillsdev/thot
 Author: SIL International
 Maintainer: Damien Daspit
 Maintainer-email: damien_daspit@sil.org
 License: LGPL-3.0
 Project-URL: Repository, https://github.com/sillsdev/thot
```

### Comparing `sil-thot-3.4.0/sil_thot.egg-info/SOURCES.txt` & `sil-thot-3.4.1/sil_thot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/CMakeLists.txt` & `sil-thot-3.4.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/downhill_simplex/step_by_step_dhs.c` & `sil-thot-3.4.1/src/downhill_simplex/step_by_step_dhs.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/downhill_simplex/step_by_step_dhs.h` & `sil-thot-3.4.1/src/downhill_simplex/step_by_step_dhs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/BaseEcModelForNbUcat.h` & `sil-thot-3.4.1/src/error_correction/BaseEcModelForNbUcat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/BaseEcmForWg.h` & `sil-thot-3.4.1/src/error_correction/BaseEcmForWg.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/BaseEditDist.h` & `sil-thot-3.4.1/src/error_correction/BaseEditDist.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/BaseErrorCorrectionModel.cc` & `sil-thot-3.4.1/src/error_correction/BaseErrorCorrectionModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/BaseErrorCorrectionModel.h` & `sil-thot-3.4.1/src/error_correction/BaseErrorCorrectionModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/BaseWgProcessorForAnlp.h` & `sil-thot-3.4.1/src/error_correction/BaseWgProcessorForAnlp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/EditDistForStr.cc` & `sil-thot-3.4.1/src/error_correction/EditDistForStr.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/EditDistForStr.h` & `sil-thot-3.4.1/src/error_correction/EditDistForStr.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/EditDistForVec.h` & `sil-thot-3.4.1/src/error_correction/EditDistForVec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/EditDistForVecString.cc` & `sil-thot-3.4.1/src/error_correction/EditDistForVecString.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/EditDistForVecString.h` & `sil-thot-3.4.1/src/error_correction/EditDistForVecString.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/HypStateIndex.h` & `sil-thot-3.4.1/src/error_correction/HypStateIndex.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/NbSearchHighLevelHyp.h` & `sil-thot-3.4.1/src/error_correction/NbSearchHighLevelHyp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/NbSearchHyp.h` & `sil-thot-3.4.1/src/error_correction/NbSearchHyp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/NbSearchStack.cc` & `sil-thot-3.4.1/src/error_correction/NbSearchStack.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/NbSearchStack.h` & `sil-thot-3.4.1/src/error_correction/NbSearchStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/NbestCorrections.h` & `sil-thot-3.4.1/src/error_correction/NbestCorrections.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/NonPbEcModelForNbUcat.cc` & `sil-thot-3.4.1/src/error_correction/NonPbEcModelForNbUcat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/NonPbEcModelForNbUcat.h` & `sil-thot-3.4.1/src/error_correction/NonPbEcModelForNbUcat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/PfsmEcm.cc` & `sil-thot-3.4.1/src/error_correction/PfsmEcm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/PfsmEcm.h` & `sil-thot-3.4.1/src/error_correction/PfsmEcm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/PfsmEcmForWg.cc` & `sil-thot-3.4.1/src/error_correction/PfsmEcmForWg.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/PfsmEcmForWg.h` & `sil-thot-3.4.1/src/error_correction/PfsmEcmForWg.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/PfsmEcmForWgEsi.h` & `sil-thot-3.4.1/src/error_correction/PfsmEcmForWgEsi.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/PrefAlignInfo.h` & `sil-thot-3.4.1/src/error_correction/PrefAlignInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/RejectedWordsSet.h` & `sil-thot-3.4.1/src/error_correction/RejectedWordsSet.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WgHandler.cc` & `sil-thot-3.4.1/src/error_correction/WgHandler.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WgHandler.h` & `sil-thot-3.4.1/src/error_correction/WgHandler.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WgProcessorForAnlp.h` & `sil-thot-3.4.1/src/error_correction/WgProcessorForAnlp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WordAndCharLevelOps.h` & `sil-thot-3.4.1/src/error_correction/WordAndCharLevelOps.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WordGraph.cc` & `sil-thot-3.4.1/src/error_correction/WordGraph.cc`

 * *Files 1% similar despite different names*

```diff
@@ -647,15 +647,15 @@
     WordGraphArcId wgArcId = nbSearchHyp[i];
     WordGraphArc wgArc = wordGraphArcId2WordGraphArc(wgArcId);
 
     for (unsigned int k = 0; k < wgArc.words.size(); ++k)
     {
       data.target.push_back(wgArc.words[k]);
       if (wgArc.unknown)
-        data.targetUnknownWords.insert(data.target.size());
+        data.targetUnknownWords.insert(data.target.size() - 1);
     }
 
     data.sourceSegmentation.push_back(std::make_pair(wgArc.srcStartIndex, wgArc.srcEndIndex));
     data.targetSegmentCuts.push_back(data.target.size());
 
     // Sum score components
     if (wgArcId < scrCompsVec.size())
```

### Comparing `sil-thot-3.4.0/src/error_correction/WordGraph.h` & `sil-thot-3.4.1/src/error_correction/WordGraph.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WordGraphArc.h` & `sil-thot-3.4.1/src/error_correction/WordGraphArc.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WordGraphArcId.h` & `sil-thot-3.4.1/src/error_correction/WordGraphArcId.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/WordGraphStateData.h` & `sil-thot-3.4.1/src/error_correction/WordGraphStateData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/_editDist.h` & `sil-thot-3.4.1/src/error_correction/_editDist.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/_editDistBasedEcm.cc` & `sil-thot-3.4.1/src/error_correction/_editDistBasedEcm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/error_correction/_editDistBasedEcm.h` & `sil-thot-3.4.1/src/error_correction/_editDistBasedEcm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/BaseIncrCondProbModel.h` & `sil-thot-3.4.1/src/incr_models/BaseIncrCondProbModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/BaseIncrCondProbTable.h` & `sil-thot-3.4.1/src/incr_models/BaseIncrCondProbTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/BaseIncrEncCondProbModel.h` & `sil-thot-3.4.1/src/incr_models/BaseIncrEncCondProbModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/BaseIncrEncoder.h` & `sil-thot-3.4.1/src/incr_models/BaseIncrEncoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/BaseWordPenaltyModel.h` & `sil-thot-3.4.1/src/incr_models/BaseWordPenaltyModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/IncrCondProbTable.h` & `sil-thot-3.4.1/src/incr_models/IncrCondProbTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/IncrEncoder.h` & `sil-thot-3.4.1/src/incr_models/IncrEncoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/IncrJelMerNgramLM.cc` & `sil-thot-3.4.1/src/incr_models/IncrJelMerNgramLM.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/IncrJelMerNgramLM.h` & `sil-thot-3.4.1/src/incr_models/IncrJelMerNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/IncrNgramLM.cc` & `sil-thot-3.4.1/src/incr_models/IncrNgramLM.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/IncrNgramLM.h` & `sil-thot-3.4.1/src/incr_models/IncrNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/WordPenaltyModel.cc` & `sil-thot-3.4.1/src/incr_models/WordPenaltyModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/WordPenaltyModel.h` & `sil-thot-3.4.1/src/incr_models/WordPenaltyModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/WordPredictor.cc` & `sil-thot-3.4.1/src/incr_models/WordPredictor.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/WordPredictor.h` & `sil-thot-3.4.1/src/incr_models/WordPredictor.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/_incrEncCondProbModel.h` & `sil-thot-3.4.1/src/incr_models/_incrEncCondProbModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/_incrJelMerNgramLM.h` & `sil-thot-3.4.1/src/incr_models/_incrJelMerNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/_incrNgramLM.h` & `sil-thot-3.4.1/src/incr_models/_incrNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/im_pair.h` & `sil-thot-3.4.1/src/incr_models/im_pair.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/lm_ienc.cc` & `sil-thot-3.4.1/src/incr_models/lm_ienc.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/lm_ienc.h` & `sil-thot-3.4.1/src/incr_models/lm_ienc.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/vecx_x_incr_cptable.h` & `sil-thot-3.4.1/src/incr_models/vecx_x_incr_cptable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/vecx_x_incr_ecpm.h` & `sil-thot-3.4.1/src/incr_models/vecx_x_incr_ecpm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/incr_models/vecx_x_incr_enc.h` & `sil-thot-3.4.1/src/incr_models/vecx_x_incr_enc.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/AwkInputStream.cc` & `sil-thot-3.4.1/src/nlp_common/AwkInputStream.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/AwkInputStream.h` & `sil-thot-3.4.1/src/nlp_common/AwkInputStream.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/BaseIncrNgramLM.h` & `sil-thot-3.4.1/src/nlp_common/BaseIncrNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/BaseNgramLM.h` & `sil-thot-3.4.1/src/nlp_common/BaseNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/BidTrie.h` & `sil-thot-3.4.1/src/nlp_common/BidTrie.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/Bitset.h` & `sil-thot-3.4.1/src/nlp_common/Bitset.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/Count.h` & `sil-thot-3.4.1/src/nlp_common/Count.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/ErrorDefs.h` & `sil-thot-3.4.1/src/nlp_common/ErrorDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/LM_Defs.h` & `sil-thot-3.4.1/src/nlp_common/LM_Defs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/LogCount.h` & `sil-thot-3.4.1/src/nlp_common/LogCount.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/MathDefs.h` & `sil-thot-3.4.1/src/nlp_common/MathDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/MathFuncs.cc` & `sil-thot-3.4.1/src/nlp_common/MathFuncs.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/MathFuncs.h` & `sil-thot-3.4.1/src/nlp_common/MathFuncs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/Matrix.h` & `sil-thot-3.4.1/src/nlp_common/Matrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/NbestTableNode.h` & `sil-thot-3.4.1/src/nlp_common/NbestTableNode.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/NbestTransTable.h` & `sil-thot-3.4.1/src/nlp_common/NbestTransTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/OrderedVector.h` & `sil-thot-3.4.1/src/nlp_common/OrderedVector.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/PositionIndex.h` & `sil-thot-3.4.1/src/nlp_common/PositionIndex.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/Prob.cc` & `sil-thot-3.4.1/src/nlp_common/Prob.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/Prob.h` & `sil-thot-3.4.1/src/nlp_common/Prob.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/Score.h` & `sil-thot-3.4.1/src/nlp_common/Score.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/SingleWordVocab.cc` & `sil-thot-3.4.1/src/nlp_common/SingleWordVocab.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/SingleWordVocab.h` & `sil-thot-3.4.1/src/nlp_common/SingleWordVocab.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/SmtDefs.h` & `sil-thot-3.4.1/src/nlp_common/SmtDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/StrProcUtils.cc` & `sil-thot-3.4.1/src/nlp_common/StrProcUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/StrProcUtils.h` & `sil-thot-3.4.1/src/nlp_common/StrProcUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/TranslationData.h` & `sil-thot-3.4.1/src/nlp_common/TranslationData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/Trie.h` & `sil-thot-3.4.1/src/nlp_common/Trie.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/TrieVecs.h` & `sil-thot-3.4.1/src/nlp_common/TrieVecs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/WordAlignmentMatrix.cc` & `sil-thot-3.4.1/src/nlp_common/WordAlignmentMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/WordAlignmentMatrix.h` & `sil-thot-3.4.1/src/nlp_common/WordAlignmentMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/WordClasses.cc` & `sil-thot-3.4.1/src/nlp_common/WordClasses.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/WordClasses.h` & `sil-thot-3.4.1/src/nlp_common/WordClasses.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/WordIndex.h` & `sil-thot-3.4.1/src/nlp_common/WordIndex.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/ctimer.c` & `sil-thot-3.4.1/src/nlp_common/ctimer.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/ctimer.h` & `sil-thot-3.4.1/src/nlp_common/ctimer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/getdelim.c` & `sil-thot-3.4.1/src/nlp_common/getdelim.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/getdelim.h` & `sil-thot-3.4.1/src/nlp_common/getdelim.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/getline.c` & `sil-thot-3.4.1/src/nlp_common/getline.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/getline.h` & `sil-thot-3.4.1/src/nlp_common/getline.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/ins_op_pair.h` & `sil-thot-3.4.1/src/nlp_common/ins_op_pair.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/lt_op_vec.h` & `sil-thot-3.4.1/src/nlp_common/lt_op_vec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/printAligFuncs.cc` & `sil-thot-3.4.1/src/nlp_common/printAligFuncs.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/printAligFuncs.h` & `sil-thot-3.4.1/src/nlp_common/printAligFuncs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/uiHashF.h` & `sil-thot-3.4.1/src/nlp_common/uiHashF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/nlp_common/uiPairHashF.h` & `sil-thot-3.4.1/src/nlp_common/uiPairHashF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/AlignmentContainer.cc` & `sil-thot-3.4.1/src/phrase_models/AlignmentContainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/AlignmentContainer.h` & `sil-thot-3.4.1/src/phrase_models/AlignmentContainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/AlignmentExtractor.cc` & `sil-thot-3.4.1/src/phrase_models/AlignmentExtractor.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/AlignmentExtractor.h` & `sil-thot-3.4.1/src/phrase_models/AlignmentExtractor.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BaseCountPhraseModel.h` & `sil-thot-3.4.1/src/phrase_models/BaseCountPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BaseIncrPhraseModel.cc` & `sil-thot-3.4.1/src/phrase_models/BaseIncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BaseIncrPhraseModel.h` & `sil-thot-3.4.1/src/phrase_models/BaseIncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BasePhraseModel.cc` & `sil-thot-3.4.1/src/phrase_models/BasePhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BasePhraseModel.h` & `sil-thot-3.4.1/src/phrase_models/BasePhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BasePhrasePairFilter.h` & `sil-thot-3.4.1/src/phrase_models/BasePhrasePairFilter.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BasePhraseTable.h` & `sil-thot-3.4.1/src/phrase_models/BasePhraseTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BpSet.cc` & `sil-thot-3.4.1/src/phrase_models/BpSet.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BpSet.h` & `sil-thot-3.4.1/src/phrase_models/BpSet.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/BpSetInfo.h` & `sil-thot-3.4.1/src/phrase_models/BpSetInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/CategPhrasePairFilter.cc` & `sil-thot-3.4.1/src/phrase_models/CategPhrasePairFilter.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/CategPhrasePairFilter.h` & `sil-thot-3.4.1/src/phrase_models/CategPhrasePairFilter.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/CellAlignment.h` & `sil-thot-3.4.1/src/phrase_models/CellAlignment.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/CellID.h` & `sil-thot-3.4.1/src/phrase_models/CellID.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/HatTriePhraseTable.cc` & `sil-thot-3.4.1/src/phrase_models/HatTriePhraseTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/HatTriePhraseTable.h` & `sil-thot-3.4.1/src/phrase_models/HatTriePhraseTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/IncrPhraseModel.cc` & `sil-thot-3.4.1/src/phrase_models/IncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/IncrPhraseModel.h` & `sil-thot-3.4.1/src/phrase_models/IncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseDefs.h` & `sil-thot-3.4.1/src/phrase_models/PhraseDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseExtractParameters.h` & `sil-thot-3.4.1/src/phrase_models/PhraseExtractParameters.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseExtractUtils.cc` & `sil-thot-3.4.1/src/phrase_models/PhraseExtractUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseExtractUtils.h` & `sil-thot-3.4.1/src/phrase_models/PhraseExtractUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseExtractionCell.h` & `sil-thot-3.4.1/src/phrase_models/PhraseExtractionCell.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseExtractionTable.cc` & `sil-thot-3.4.1/src/phrase_models/PhraseExtractionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseExtractionTable.h` & `sil-thot-3.4.1/src/phrase_models/PhraseExtractionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseId.h` & `sil-thot-3.4.1/src/phrase_models/PhraseId.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhrasePair.h` & `sil-thot-3.4.1/src/phrase_models/PhrasePair.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhrasePairInfo.h` & `sil-thot-3.4.1/src/phrase_models/PhrasePairInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseSortCriterion.h` & `sil-thot-3.4.1/src/phrase_models/PhraseSortCriterion.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/PhraseTransTableNodeData.h` & `sil-thot-3.4.1/src/phrase_models/PhraseTransTableNodeData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SegLenTable.cc` & `sil-thot-3.4.1/src/phrase_models/SegLenTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SegLenTable.h` & `sil-thot-3.4.1/src/phrase_models/SegLenTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SentSegmentation.h` & `sil-thot-3.4.1/src/phrase_models/SentSegmentation.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrcSegmLenTable.cc` & `sil-thot-3.4.1/src/phrase_models/SrcSegmLenTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrcSegmLenTable.h` & `sil-thot-3.4.1/src/phrase_models/SrcSegmLenTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrfBisegm.h` & `sil-thot-3.4.1/src/phrase_models/SrfBisegm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrfNodeInfo.h` & `sil-thot-3.4.1/src/phrase_models/SrfNodeInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrfNodeInfoMap.cc` & `sil-thot-3.4.1/src/phrase_models/SrfNodeInfoMap.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrfNodeInfoMap.h` & `sil-thot-3.4.1/src/phrase_models/SrfNodeInfoMap.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrfNodeKey.cc` & `sil-thot-3.4.1/src/phrase_models/SrfNodeKey.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/SrfNodeKey.h` & `sil-thot-3.4.1/src/phrase_models/SrfNodeKey.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/StlPhraseTable.cc` & `sil-thot-3.4.1/src/phrase_models/StlPhraseTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/StlPhraseTable.h` & `sil-thot-3.4.1/src/phrase_models/StlPhraseTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/StrictCategPhrasePairFilter.cc` & `sil-thot-3.4.1/src/phrase_models/StrictCategPhrasePairFilter.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/StrictCategPhrasePairFilter.h` & `sil-thot-3.4.1/src/phrase_models/StrictCategPhrasePairFilter.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/TrgCutsTable.cc` & `sil-thot-3.4.1/src/phrase_models/TrgCutsTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/TrgCutsTable.h` & `sil-thot-3.4.1/src/phrase_models/TrgCutsTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/TrgSegmLenTable.cc` & `sil-thot-3.4.1/src/phrase_models/TrgSegmLenTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/TrgSegmLenTable.h` & `sil-thot-3.4.1/src/phrase_models/TrgSegmLenTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/VecUnsignedIntSortCriterion.h` & `sil-thot-3.4.1/src/phrase_models/VecUnsignedIntSortCriterion.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/WbaIncrPhraseModel.cc` & `sil-thot-3.4.1/src/phrase_models/WbaIncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/WbaIncrPhraseModel.h` & `sil-thot-3.4.1/src/phrase_models/WbaIncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/_incrPhraseModel.cc` & `sil-thot-3.4.1/src/phrase_models/_incrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/_incrPhraseModel.h` & `sil-thot-3.4.1/src/phrase_models/_incrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/_wbaIncrPhraseModel.cc` & `sil-thot-3.4.1/src/phrase_models/_wbaIncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/phrase_models/_wbaIncrPhraseModel.h` & `sil-thot-3.4.1/src/phrase_models/_wbaIncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/python_module/CMakeLists.txt` & `sil-thot-3.4.1/src/python_module/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/python_module/module.cc` & `sil-thot-3.4.1/src/python_module/module.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/shared_library/thot.cc` & `sil-thot-3.4.1/src/shared_library/thot.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/shared_library/thot.h` & `sil-thot-3.4.1/src/shared_library/thot.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseAssistedTrans.h` & `sil-thot-3.4.1/src/stack_dec/BaseAssistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseHypState.cc` & `sil-thot-3.4.1/src/stack_dec/BaseHypState.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseHypState.h` & `sil-thot-3.4.1/src/stack_dec/BaseHypState.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseHypothesis.h` & `sil-thot-3.4.1/src/stack_dec/BaseHypothesis.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseHypothesisRec.h` & `sil-thot-3.4.1/src/stack_dec/BaseHypothesisRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseLogLinWeightUpdater.h` & `sil-thot-3.4.1/src/stack_dec/BaseLogLinWeightUpdater.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseMiraScorer.h` & `sil-thot-3.4.1/src/stack_dec/BaseMiraScorer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BasePbTransModel.h` & `sil-thot-3.4.1/src/stack_dec/BasePbTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BasePbTransModelFeature.h` & `sil-thot-3.4.1/src/stack_dec/BasePbTransModelFeature.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BasePbTransModelStats.h` & `sil-thot-3.4.1/src/stack_dec/BasePbTransModelStats.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BasePhraseHypothesis.h` & `sil-thot-3.4.1/src/stack_dec/BasePhraseHypothesis.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BasePhraseHypothesisRec.h` & `sil-thot-3.4.1/src/stack_dec/BasePhraseHypothesisRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseScorer.h` & `sil-thot-3.4.1/src/stack_dec/BaseScorer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseSmtModel.h` & `sil-thot-3.4.1/src/stack_dec/BaseSmtModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseSmtMultiStack.h` & `sil-thot-3.4.1/src/stack_dec/BaseSmtMultiStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseSmtStack.h` & `sil-thot-3.4.1/src/stack_dec/BaseSmtStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseStackDecoder.h` & `sil-thot-3.4.1/src/stack_dec/BaseStackDecoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/BaseTranslationMetadata.h` & `sil-thot-3.4.1/src/stack_dec/BaseTranslationMetadata.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/DictFeat.cc` & `sil-thot-3.4.1/src/stack_dec/DictFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/DictFeat.h` & `sil-thot-3.4.1/src/stack_dec/DictFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/DirectPhraseModelFeat.cc` & `sil-thot-3.4.1/src/stack_dec/DirectPhraseModelFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/DirectPhraseModelFeat.h` & `sil-thot-3.4.1/src/stack_dec/DirectPhraseModelFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/FeaturesInfo.h` & `sil-thot-3.4.1/src/stack_dec/FeaturesInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/HypSortCriterion.h` & `sil-thot-3.4.1/src/stack_dec/HypSortCriterion.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/HypStateDict.h` & `sil-thot-3.4.1/src/stack_dec/HypStateDict.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/HypStateDictData.h` & `sil-thot-3.4.1/src/stack_dec/HypStateDictData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/InversePhraseModelFeat.cc` & `sil-thot-3.4.1/src/stack_dec/InversePhraseModelFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/InversePhraseModelFeat.h` & `sil-thot-3.4.1/src/stack_dec/InversePhraseModelFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/KbMiraLlWu.cc` & `sil-thot-3.4.1/src/stack_dec/KbMiraLlWu.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/KbMiraLlWu.h` & `sil-thot-3.4.1/src/stack_dec/KbMiraLlWu.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/LM_State.h` & `sil-thot-3.4.1/src/stack_dec/LM_State.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/LangModelFeat.cc` & `sil-thot-3.4.1/src/stack_dec/LangModelFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/LangModelFeat.h` & `sil-thot-3.4.1/src/stack_dec/LangModelFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/LangModelInfo.h` & `sil-thot-3.4.1/src/stack_dec/LangModelInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/LangModelPars.h` & `sil-thot-3.4.1/src/stack_dec/LangModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraBleu.cc` & `sil-thot-3.4.1/src/stack_dec/MiraBleu.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraBleu.h` & `sil-thot-3.4.1/src/stack_dec/MiraBleu.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraChrF.cc` & `sil-thot-3.4.1/src/stack_dec/MiraChrF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraChrF.h` & `sil-thot-3.4.1/src/stack_dec/MiraChrF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraGtm.cc` & `sil-thot-3.4.1/src/stack_dec/MiraGtm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraGtm.h` & `sil-thot-3.4.1/src/stack_dec/MiraGtm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraWer.cc` & `sil-thot-3.4.1/src/stack_dec/MiraWer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/MiraWer.h` & `sil-thot-3.4.1/src/stack_dec/MiraWer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/NbestTransCacheData.h` & `sil-thot-3.4.1/src/stack_dec/NbestTransCacheData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/OnTheFlyDictFeat.cc` & `sil-thot-3.4.1/src/stack_dec/OnTheFlyDictFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/OnTheFlyDictFeat.h` & `sil-thot-3.4.1/src/stack_dec/OnTheFlyDictFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/OnlineTrainingPars.h` & `sil-thot-3.4.1/src/stack_dec/OnlineTrainingPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PbTransModel.h` & `sil-thot-3.4.1/src/stack_dec/PbTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PbTransModelInputVars.h` & `sil-thot-3.4.1/src/stack_dec/PbTransModelInputVars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PbTransModelPars.h` & `sil-thot-3.4.1/src/stack_dec/PbTransModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypData.h` & `sil-thot-3.4.1/src/stack_dec/PhrHypData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypDataStr.h` & `sil-thot-3.4.1/src/stack_dec/PhrHypDataStr.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypEqClassF.cc` & `sil-thot-3.4.1/src/stack_dec/PhrHypEqClassF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypEqClassF.h` & `sil-thot-3.4.1/src/stack_dec/PhrHypEqClassF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc` & `sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumps01EqClassF.h` & `sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumps01EqClassF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc` & `sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypNumcovJumpsEqClassF.h` & `sil-thot-3.4.1/src/stack_dec/PhrHypNumcovJumpsEqClassF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypState.cc` & `sil-thot-3.4.1/src/stack_dec/PhrHypState.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrHypState.h` & `sil-thot-3.4.1/src/stack_dec/PhrHypState.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrLocalSwLiTm.cc` & `sil-thot-3.4.1/src/stack_dec/PhrLocalSwLiTm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrLocalSwLiTm.h` & `sil-thot-3.4.1/src/stack_dec/PhrLocalSwLiTm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrLocalSwLiTmHypRec.h` & `sil-thot-3.4.1/src/stack_dec/PhrLocalSwLiTmHypRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrNbestTransTable.h` & `sil-thot-3.4.1/src/stack_dec/PhrNbestTransTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrNbestTransTablePref.h` & `sil-thot-3.4.1/src/stack_dec/PhrNbestTransTablePref.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrNbestTransTablePrefKey.cc` & `sil-thot-3.4.1/src/stack_dec/PhrNbestTransTablePrefKey.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrNbestTransTablePrefKey.h` & `sil-thot-3.4.1/src/stack_dec/PhrNbestTransTablePrefKey.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrNbestTransTableRef.h` & `sil-thot-3.4.1/src/stack_dec/PhrNbestTransTableRef.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrNbestTransTableRefKey.cc` & `sil-thot-3.4.1/src/stack_dec/PhrNbestTransTableRefKey.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrNbestTransTableRefKey.h` & `sil-thot-3.4.1/src/stack_dec/PhrNbestTransTableRefKey.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrScoreInfo.cc` & `sil-thot-3.4.1/src/stack_dec/PhrScoreInfo.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrScoreInfo.h` & `sil-thot-3.4.1/src/stack_dec/PhrScoreInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhraseBasedTmHyp.h` & `sil-thot-3.4.1/src/stack_dec/PhraseBasedTmHyp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhraseBasedTmHypRec.h` & `sil-thot-3.4.1/src/stack_dec/PhraseBasedTmHypRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhraseCacheTable.h` & `sil-thot-3.4.1/src/stack_dec/PhraseCacheTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhraseModelInfo.h` & `sil-thot-3.4.1/src/stack_dec/PhraseModelInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhraseModelPars.h` & `sil-thot-3.4.1/src/stack_dec/PhraseModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/PhrasePairCacheTable.h` & `sil-thot-3.4.1/src/stack_dec/PhrasePairCacheTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/ScoreCompDefs.h` & `sil-thot-3.4.1/src/stack_dec/ScoreCompDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SmtModelUtils.cc` & `sil-thot-3.4.1/src/stack_dec/SmtModelUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SmtModelUtils.h` & `sil-thot-3.4.1/src/stack_dec/SmtModelUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SmtMultiStackRec.h` & `sil-thot-3.4.1/src/stack_dec/SmtMultiStackRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SmtStack.h` & `sil-thot-3.4.1/src/stack_dec/SmtStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SourceSegmentation.h` & `sil-thot-3.4.1/src/stack_dec/SourceSegmentation.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SrcPhraseLenFeat.cc` & `sil-thot-3.4.1/src/stack_dec/SrcPhraseLenFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SrcPhraseLenFeat.h` & `sil-thot-3.4.1/src/stack_dec/SrcPhraseLenFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SrcPosJumpFeat.cc` & `sil-thot-3.4.1/src/stack_dec/SrcPosJumpFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SrcPosJumpFeat.h` & `sil-thot-3.4.1/src/stack_dec/SrcPosJumpFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SwModelInfo.h` & `sil-thot-3.4.1/src/stack_dec/SwModelInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/SwModelPars.h` & `sil-thot-3.4.1/src/stack_dec/SwModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/TranslationMetadata.h` & `sil-thot-3.4.1/src/stack_dec/TranslationMetadata.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/TrgPhraseLenFeat.cc` & `sil-thot-3.4.1/src/stack_dec/TrgPhraseLenFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/TrgPhraseLenFeat.h` & `sil-thot-3.4.1/src/stack_dec/TrgPhraseLenFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/WeightUpdateUtils.cc` & `sil-thot-3.4.1/src/stack_dec/WeightUpdateUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/WeightUpdateUtils.h` & `sil-thot-3.4.1/src/stack_dec/WeightUpdateUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/WgUncoupledAssistedTrans.h` & `sil-thot-3.4.1/src/stack_dec/WgUncoupledAssistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/WordPenaltyFeat.cc` & `sil-thot-3.4.1/src/stack_dec/WordPenaltyFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/WordPenaltyFeat.h` & `sil-thot-3.4.1/src/stack_dec/WordPenaltyFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_assistedTrans.h` & `sil-thot-3.4.1/src/stack_dec/_assistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_nbUncoupledAssistedTrans.h` & `sil-thot-3.4.1/src/stack_dec/_nbUncoupledAssistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_pbTransModel.h` & `sil-thot-3.4.1/src/stack_dec/_pbTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_phrSwTransModel.h` & `sil-thot-3.4.1/src/stack_dec/_phrSwTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_phraseBasedTransModel.h` & `sil-thot-3.4.1/src/stack_dec/_phraseBasedTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_phraseHypothesis.h` & `sil-thot-3.4.1/src/stack_dec/_phraseHypothesis.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_phraseHypothesisRec.h` & `sil-thot-3.4.1/src/stack_dec/_phraseHypothesisRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_smtModel.h` & `sil-thot-3.4.1/src/stack_dec/_smtModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_smtMultiStack.h` & `sil-thot-3.4.1/src/stack_dec/_smtMultiStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_smtStack.h` & `sil-thot-3.4.1/src/stack_dec/_smtStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_stackDecoder.h` & `sil-thot-3.4.1/src/stack_dec/_stackDecoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_stackDecoderRec.h` & `sil-thot-3.4.1/src/stack_dec/_stackDecoderRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/_stack_decoder_statistics.h` & `sil-thot-3.4.1/src/stack_dec/_stack_decoder_statistics.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/bleu.cc` & `sil-thot-3.4.1/src/stack_dec/bleu.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/bleu.h` & `sil-thot-3.4.1/src/stack_dec/bleu.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/chrf.cc` & `sil-thot-3.4.1/src/stack_dec/chrf.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/chrf.h` & `sil-thot-3.4.1/src/stack_dec/chrf.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/stack_dec/multi_stack_decoder_rec.h` & `sil-thot-3.4.1/src/stack_dec/multi_stack_decoder_rec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Aligner.h` & `sil-thot-3.4.1/src/sw_models/Aligner.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/AlignmentInfo.h` & `sil-thot-3.4.1/src/sw_models/AlignmentInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/AlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/AlignmentModelBase.cc` & `sil-thot-3.4.1/src/sw_models/AlignmentModelBase.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/AlignmentModelBase.h` & `sil-thot-3.4.1/src/sw_models/AlignmentModelBase.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/AlignmentTable.cc` & `sil-thot-3.4.1/src/sw_models/AlignmentTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/AlignmentTable.h` & `sil-thot-3.4.1/src/sw_models/AlignmentTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/CachedHmmAligLgProb.cc` & `sil-thot-3.4.1/src/sw_models/CachedHmmAligLgProb.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/CachedHmmAligLgProb.h` & `sil-thot-3.4.1/src/sw_models/CachedHmmAligLgProb.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/DiagonalAlignment.h` & `sil-thot-3.4.1/src/sw_models/DiagonalAlignment.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/DistortionTable.cc` & `sil-thot-3.4.1/src/sw_models/DistortionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/DistortionTable.h` & `sil-thot-3.4.1/src/sw_models/DistortionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/DoubleMatrix.cc` & `sil-thot-3.4.1/src/sw_models/DoubleMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/DoubleMatrix.h` & `sil-thot-3.4.1/src/sw_models/DoubleMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/FastAlignModel.cc` & `sil-thot-3.4.1/src/sw_models/FastAlignModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/FastAlignModel.h` & `sil-thot-3.4.1/src/sw_models/FastAlignModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/FertilityTable.cc` & `sil-thot-3.4.1/src/sw_models/FertilityTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/FertilityTable.h` & `sil-thot-3.4.1/src/sw_models/FertilityTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/HeadDistortionTable.cc` & `sil-thot-3.4.1/src/sw_models/HeadDistortionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/HeadDistortionTable.h` & `sil-thot-3.4.1/src/sw_models/HeadDistortionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/HmmAlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/HmmAlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/HmmAlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/HmmAlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/HmmAlignmentTable.cc` & `sil-thot-3.4.1/src/sw_models/HmmAlignmentTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/HmmAlignmentTable.h` & `sil-thot-3.4.1/src/sw_models/HmmAlignmentTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm1AlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/Ibm1AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm1AlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/Ibm1AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm2AlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/Ibm2AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm2AlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/Ibm2AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm3AlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/Ibm3AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm3AlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/Ibm3AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm4AlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/Ibm4AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Ibm4AlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/Ibm4AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrAlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/IncrAlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentTrainer.cc` & `sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentTrainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrHmmAlignmentTrainer.h` & `sil-thot-3.4.1/src/sw_models/IncrHmmAlignmentTrainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentTrainer.cc` & `sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentTrainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm1AlignmentTrainer.h` & `sil-thot-3.4.1/src/sw_models/IncrIbm1AlignmentTrainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentModel.cc` & `sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentModel.h` & `sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentTrainer.cc` & `sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentTrainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/IncrIbm2AlignmentTrainer.h` & `sil-thot-3.4.1/src/sw_models/IncrIbm2AlignmentTrainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/LexCounts.h` & `sil-thot-3.4.1/src/sw_models/LexCounts.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/LexTable.h` & `sil-thot-3.4.1/src/sw_models/LexTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/LightSentenceHandler.cc` & `sil-thot-3.4.1/src/sw_models/LightSentenceHandler.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/LightSentenceHandler.h` & `sil-thot-3.4.1/src/sw_models/LightSentenceHandler.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/Md.h` & `sil-thot-3.4.1/src/sw_models/Md.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/MemoryLexTable.cc` & `sil-thot-3.4.1/src/sw_models/MemoryLexTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/MemoryLexTable.h` & `sil-thot-3.4.1/src/sw_models/MemoryLexTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/NonheadDistortionTable.cc` & `sil-thot-3.4.1/src/sw_models/NonheadDistortionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/NonheadDistortionTable.h` & `sil-thot-3.4.1/src/sw_models/NonheadDistortionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/NormalSentenceLengthModel.cc` & `sil-thot-3.4.1/src/sw_models/NormalSentenceLengthModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/NormalSentenceLengthModel.h` & `sil-thot-3.4.1/src/sw_models/NormalSentenceLengthModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/SentenceHandler.h` & `sil-thot-3.4.1/src/sw_models/SentenceHandler.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/SentenceLengthModel.h` & `sil-thot-3.4.1/src/sw_models/SentenceLengthModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/SentenceLengthModelBase.cc` & `sil-thot-3.4.1/src/sw_models/SentenceLengthModelBase.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/SentenceLengthModelBase.h` & `sil-thot-3.4.1/src/sw_models/SentenceLengthModelBase.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/SymmetrizedAligner.cc` & `sil-thot-3.4.1/src/sw_models/SymmetrizedAligner.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/SymmetrizedAligner.h` & `sil-thot-3.4.1/src/sw_models/SymmetrizedAligner.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/anjiMatrix.cc` & `sil-thot-3.4.1/src/sw_models/anjiMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/anjiMatrix.h` & `sil-thot-3.4.1/src/sw_models/anjiMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/anjm1ip_anjiMatrix.cc` & `sil-thot-3.4.1/src/sw_models/anjm1ip_anjiMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/src/sw_models/anjm1ip_anjiMatrix.h` & `sil-thot-3.4.1/src/sw_models/anjm1ip_anjiMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/CMakeLists.txt` & `sil-thot-3.4.1/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/nlp_common/WordAlignmentMatrixTest.cc` & `sil-thot-3.4.1/tests/nlp_common/WordAlignmentMatrixTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/phrase_models/HatTriePhraseTableTest.cc` & `sil-thot-3.4.1/tests/phrase_models/HatTriePhraseTableTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/phrase_models/StlPhraseTableTest.cc` & `sil-thot-3.4.1/tests/phrase_models/StlPhraseTableTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/phrase_models/_phraseTableTest.h` & `sil-thot-3.4.1/tests/phrase_models/_phraseTableTest.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/stack_dec/KbMiraLlWuTest.cc` & `sil-thot-3.4.1/tests/stack_dec/KbMiraLlWuTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/stack_dec/MiraChrFTest.cc` & `sil-thot-3.4.1/tests/stack_dec/MiraChrFTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/stack_dec/PhrLocalSwLiTmTest.cc` & `sil-thot-3.4.1/tests/stack_dec/PhrLocalSwLiTmTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/stack_dec/TranslationMetadataTest.cc` & `sil-thot-3.4.1/tests/stack_dec/TranslationMetadataTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/sw_models/FastAlignModelTest.cc` & `sil-thot-3.4.1/tests/sw_models/FastAlignModelTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/sw_models/Ibm4AlignmentModelTest.cc` & `sil-thot-3.4.1/tests/sw_models/Ibm4AlignmentModelTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/sw_models/IncrHmmAlignmentModelTest.cc` & `sil-thot-3.4.1/tests/sw_models/IncrHmmAlignmentModelTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/sw_models/LexTableTest.h` & `sil-thot-3.4.1/tests/sw_models/LexTableTest.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/sw_models/TestUtils.cc` & `sil-thot-3.4.1/tests/sw_models/TestUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/sw_models/TestUtils.h` & `sil-thot-3.4.1/tests/sw_models/TestUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/tests/test_module.py` & `sil-thot-3.4.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/thot/alignment/__init__.pyi` & `sil-thot-3.4.1/thot/alignment/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/thot/common/__init__.pyi` & `sil-thot-3.4.1/thot/common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.0/thot/translation/__init__.pyi` & `sil-thot-3.4.1/thot/translation/__init__.pyi`

 * *Files identical despite different names*

