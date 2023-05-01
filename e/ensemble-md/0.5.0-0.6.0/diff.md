# Comparing `tmp/ensemble_md-0.5.0.tar.gz` & `tmp/ensemble_md-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble_md-0.5.0.tar", last modified: Tue Mar 28 17:34:17 2023, max compression
+gzip compressed data, was "ensemble_md-0.6.0.tar", last modified: Mon May  1 20:24:45 2023, max compression
```

## Comparing `ensemble_md-0.5.0.tar` & `ensemble_md-0.6.0.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.768572 ensemble_md-0.5.0/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3557 2022-10-26 04:45:46.000000 ensemble_md-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1069 2022-10-26 04:45:45.000000 ensemble_md-0.5.0/LICENSE
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      145 2022-10-26 04:45:46.000000 ensemble_md-0.5.0/MANIFEST.in
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3040 2023-03-28 17:34:17.768808 ensemble_md-0.5.0/PKG-INFO
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1605 2023-03-28 00:20:22.000000 ensemble_md-0.5.0/README.md
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.770951 ensemble_md-0.5.0/ensemble_md/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    53248 2023-01-19 17:24:20.000000 ensemble_md-0.5.0/ensemble_md/.coverage
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      339 2022-10-26 04:45:50.000000 ensemble_md-0.5.0/ensemble_md/__init__.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      497 2023-03-28 17:34:17.771084 ensemble_md-0.5.0/ensemble_md/_version.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.724973 ensemble_md-0.5.0/ensemble_md/analysis/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    14013 2023-02-17 07:55:13.000000 ensemble_md-0.5.0/ensemble_md/analysis/analyze_free_energy.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     9962 2023-03-14 22:37:17.000000 ensemble_md-0.5.0/ensemble_md/analysis/analyze_matrix.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    19990 2023-03-14 22:56:07.000000 ensemble_md-0.5.0/ensemble_md/analysis/analyze_traj.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5451 2023-02-17 07:55:38.000000 ensemble_md-0.5.0/ensemble_md/analysis/msm_analysis.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.729956 ensemble_md-0.5.0/ensemble_md/cli/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    21265 2023-02-22 20:06:27.000000 ensemble_md-0.5.0/ensemble_md/cli/analyze_EEXE.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5516 2023-03-01 07:43:32.000000 ensemble_md-0.5.0/ensemble_md/cli/explore_EEXE.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    12119 2023-03-06 23:12:30.000000 ensemble_md-0.5.0/ensemble_md/cli/run_EEXE.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.732355 ensemble_md-0.5.0/ensemble_md/data/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1139 2022-10-26 04:45:53.000000 ensemble_md-0.5.0/ensemble_md/data/README.md
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      333 2022-10-26 04:45:52.000000 ensemble_md-0.5.0/ensemble_md/data/look_and_say.dat
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    57170 2023-03-28 07:26:57.000000 ensemble_md-0.5.0/ensemble_md/ensemble_EXE.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.740892 ensemble_md-0.5.0/ensemble_md/tests/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    53248 2023-01-19 17:22:30.000000 ensemble_md-0.5.0/ensemble_md/tests/.coverage
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      113 2022-10-26 04:45:53.000000 ensemble_md-0.5.0/ensemble_md/tests/__init__.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.745578 ensemble_md-0.5.0/ensemble_md/tests/data/
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.750868 ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6769 2022-10-26 04:45:56.000000 ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6739 2022-10-26 04:45:55.000000 ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6731 2022-10-26 04:45:55.000000 ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6749 2022-10-26 04:45:54.000000 ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2200 2023-03-02 09:35:40.000000 ensemble_md-0.5.0/ensemble_md/tests/data/expanded.mdp
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.763810 ensemble_md-0.5.0/ensemble_md/tests/data/log/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    38509 2022-10-26 04:45:58.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32761 2022-10-26 04:45:54.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_0.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2022-10-26 04:45:55.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_1.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32763 2022-10-26 04:45:57.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_2.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2022-10-26 04:45:56.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_3.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7992 2023-03-14 22:24:53.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/HREX.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    71966 2022-10-26 04:45:56.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/case2_1.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    65113 2022-10-26 04:45:55.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/case2_2.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    44910 2022-10-26 04:45:57.000000 ensemble_md-0.5.0/ensemble_md/tests/data/log/case3.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)   113593 2022-10-26 04:45:55.000000 ensemble_md-0.5.0/ensemble_md/tests/data/sys.gro
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2067 2022-10-26 04:45:57.000000 ensemble_md-0.5.0/ensemble_md/tests/data/sys.top
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7307 2023-03-14 22:42:13.000000 ensemble_md-0.5.0/ensemble_md/tests/test_analyze_matrix.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1424 2023-03-26 20:04:55.000000 ensemble_md-0.5.0/ensemble_md/tests/test_analyze_traj.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    33449 2023-03-28 07:27:41.000000 ensemble_md-0.5.0/ensemble_md/tests/test_ensemble_EXE.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3826 2023-03-03 10:18:32.000000 ensemble_md-0.5.0/ensemble_md/tests/test_gmx_parser.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5632 2023-03-03 09:36:17.000000 ensemble_md-0.5.0/ensemble_md/tests/test_utils.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.767620 ensemble_md-0.5.0/ensemble_md/utils/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      858 2022-10-26 04:45:51.000000 ensemble_md-0.5.0/ensemble_md/utils/exceptions.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    14104 2023-03-03 10:00:10.000000 ensemble_md-0.5.0/ensemble_md/utils/gmx_parser.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7715 2023-03-03 08:52:56.000000 ensemble_md-0.5.0/ensemble_md/utils/utils.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-03-28 17:34:17.719690 ensemble_md-0.5.0/ensemble_md.egg-info/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3040 2023-03-28 17:34:17.000000 ensemble_md-0.5.0/ensemble_md.egg-info/PKG-INFO
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1626 2023-03-28 17:34:17.000000 ensemble_md-0.5.0/ensemble_md.egg-info/SOURCES.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)        1 2023-03-28 17:34:17.000000 ensemble_md-0.5.0/ensemble_md.egg-info/dependency_links.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      157 2023-03-28 17:34:17.000000 ensemble_md-0.5.0/ensemble_md.egg-info/entry_points.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      152 2023-03-28 17:34:17.000000 ensemble_md-0.5.0/ensemble_md.egg-info/requires.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)       12 2023-03-28 17:34:17.000000 ensemble_md-0.5.0/ensemble_md.egg-info/top_level.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      360 2023-03-28 17:34:17.770297 ensemble_md-0.5.0/setup.cfg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     4626 2023-03-03 07:19:17.000000 ensemble_md-0.5.0/setup.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    68611 2022-10-26 04:45:45.000000 ensemble_md-0.5.0/versioneer.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.058627 ensemble_md-0.6.0/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3557 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1069 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/LICENSE
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      145 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/MANIFEST.in
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3017 2023-05-01 20:24:45.058929 ensemble_md-0.6.0/PKG-INFO
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1605 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/README.md
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.060784 ensemble_md-0.6.0/ensemble_md/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      339 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/__init__.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      497 2023-05-01 20:24:45.061053 ensemble_md-0.6.0/ensemble_md/_version.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.021900 ensemble_md-0.6.0/ensemble_md/analysis/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    14013 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/analyze_free_energy.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     9937 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/analyze_matrix.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    20028 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/analyze_traj.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5451 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/msm_analysis.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.024212 ensemble_md-0.6.0/ensemble_md/cli/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    21672 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/cli/analyze_EEXE.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5516 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/cli/explore_EEXE.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    13152 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/cli/run_EEXE.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.025432 ensemble_md-0.6.0/ensemble_md/data/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1139 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/data/README.md
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      333 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/data/look_and_say.dat
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    62953 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/ensemble_EXE.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.031463 ensemble_md-0.6.0/ensemble_md/tests/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      113 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/__init__.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.035949 ensemble_md-0.6.0/ensemble_md/tests/data/
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.040769 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6769 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6739 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6731 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6749 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2200 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/expanded.mdp
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.053746 ensemble_md-0.6.0/ensemble_md/tests/data/log/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    38509 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32761 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_0.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_1.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32763 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_2.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_3.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7992 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/HREX.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    71966 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_1.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    65113 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_2.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    44910 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/case3.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)   113593 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/sys.gro
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2067 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/sys.top
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7426 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_analyze_matrix.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1424 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_analyze_traj.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32028 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_ensemble_EXE.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     4495 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_gmx_parser.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3796 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_utils.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.057897 ensemble_md-0.6.0/ensemble_md/utils/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      858 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/utils/exceptions.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    16515 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/utils/gmx_parser.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7954 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/utils/utils.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.019121 ensemble_md-0.6.0/ensemble_md.egg-info/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3017 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/PKG-INFO
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1576 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/SOURCES.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)        1 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/dependency_links.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      157 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/entry_points.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)       94 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/requires.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)       12 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/top_level.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      360 2023-05-01 20:24:45.060192 ensemble_md-0.6.0/setup.cfg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     4646 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/setup.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    68611 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/versioneer.py
```

### Comparing `ensemble_md-0.5.0/CODE_OF_CONDUCT.md` & `ensemble_md-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/LICENSE` & `ensemble_md-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/PKG-INFO` & `ensemble_md-0.6.0/ensemble_md.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ensemble_md
-Version: 0.5.0
+Name: ensemble-md
+Version: 0.6.0
 Summary: A package for setting up, performing, and analyzing molecular dynamics ensembles using GROMACS
 Author: Wei-Tse Hsu
 Author-email: wehs7661@colorado.edu
 License: MIT
 Project-URL: Documentation, https://ensemble-md.readthedocs.io/
 Project-URL: Source Code, https://github.com/wehs7661/ensemble_md
 Keywords: molecular mechanics,free energy calculations,advanced sampling
@@ -26,23 +26,22 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gmxapi
 License-File: LICENSE
 
 Ensemble Molecular Dynamics
 ==============================
 [//]: # (Badges)
 [![wehs7661](https://circleci.com/gh/wehs7661/ensemble_md.svg?style=shield)](https://app.circleci.com/pipelines/github/wehs7661/ensemble_md?branch=master)
 [![codecov](https://codecov.io/gh/wehs7661/ensemble_md/branch/master/graph/badge.svg)](https://app.codecov.io/gh/wehs7661/ensemble_md/tree/master)
-[![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble_md.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble-md.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Actions Lint Status](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml/badge.svg)](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml)
 [![PyPI version](https://badge.fury.io/py/ensemble-md.svg)](https://badge.fury.io/py/ensemble-md)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 **ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble_md.readthedocs.io/).
 
 ### Copyright
```

### Comparing `ensemble_md-0.5.0/README.md` & `ensemble_md-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Ensemble Molecular Dynamics
 ==============================
 [//]: # (Badges)
 [![wehs7661](https://circleci.com/gh/wehs7661/ensemble_md.svg?style=shield)](https://app.circleci.com/pipelines/github/wehs7661/ensemble_md?branch=master)
 [![codecov](https://codecov.io/gh/wehs7661/ensemble_md/branch/master/graph/badge.svg)](https://app.codecov.io/gh/wehs7661/ensemble_md/tree/master)
-[![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble_md.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble-md.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Actions Lint Status](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml/badge.svg)](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml)
 [![PyPI version](https://badge.fury.io/py/ensemble-md.svg)](https://badge.fury.io/py/ensemble-md)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 **ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble_md.readthedocs.io/).
 
 ### Copyright
```

### Comparing `ensemble_md-0.5.0/ensemble_md/analysis/analyze_free_energy.py` & `ensemble_md-0.6.0/ensemble_md/analysis/analyze_free_energy.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/analysis/analyze_matrix.py` & `ensemble_md-0.6.0/ensemble_md/analysis/analyze_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,16 @@
     trans_mtx : numpy.ndarray
         The input state transition matrix
 
     Returns
     -------
     spectral_gap : float
         The spectral gap of the input transition matrix
+    eig_vals : list
+        The list of eigenvalues
     """
     check_row = sum([np.isclose(np.sum(trans_mtx[i]), 1) for i in range(len(trans_mtx))])
     check_col = sum([np.isclose(np.sum(trans_mtx[:, i]), 1) for i in range(len(trans_mtx))])
 
     if check_row == len(trans_mtx):
         eig_vals, eig_vecs = np.linalg.eig(trans_mtx.T)
     elif check_col == len(trans_mtx):
@@ -149,18 +151,17 @@
         print(result_str)
         return None
 
     eig_vals = np.sort(eig_vals)[::-1]  # descending order
     if np.isclose(eig_vals[0], 1, atol=1e-4) is False:
         raise ParameterError(f'The largest eigenvalue of the input transition matrix {eig_vals[0]} is not close to 1.')
 
-    print(f'The two largest eigenvalues are {eig_vals[0]:.5f} and {eig_vals[1]:.5f}.')
     spectral_gap = np.abs(eig_vals[0]) - np.abs(eig_vals[1])
 
-    return spectral_gap
+    return spectral_gap, eig_vals
 
 
 def split_transmtx(trans_mtx, n_sim, n_sub):
     """
     Split the input transition matrix into blocks of smaller matrices corresponding to
     difrerent alchemical ranges of different replicas. Notably, the function assumes
     homogeneous shifts and number of states across replicas. Also, the blocks of the
```

### Comparing `ensemble_md-0.5.0/ensemble_md/analysis/analyze_traj.py` & `ensemble_md-0.6.0/ensemble_md/analysis/analyze_traj.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,7 +489,11 @@
                 plt.legend()
                 if fig_prefix is None:
                     plt.savefig(f'{folder}/hist_{fig_names[t]}', dpi=600)
                 else:
                     plt.savefig(f'{folder}/{fig_prefix}_hist_{fig_names[t]}', dpi=600)
 
     return t_0k_list, t_k0_list, t_roundtrip_list, units
+
+
+def plot_g_vecs(f_g_vecs):
+    pass
```

### Comparing `ensemble_md-0.5.0/ensemble_md/analysis/msm_analysis.py` & `ensemble_md-0.6.0/ensemble_md/analysis/msm_analysis.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/cli/analyze_EEXE.py` & `ensemble_md-0.6.0/ensemble_md/cli/analyze_EEXE.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     print('1-2. Plotting the replica transition matrix (considering all configurations) ...')
     counts = [analyze_traj.traj2transmtx(rep_trajs[i], EEXE.n_sim, normalize=False) for i in range(len(rep_trajs))]
     reps_mtx = np.sum(counts, axis=0)  # First sum up the counts. This should be symmetric if n_ex=1. Otherwise it might not be. # noqa: E501
     reps_mtx /= np.sum(reps_mtx, axis=1)[:, None]   # and then normalize each row
     analyze_matrix.plot_matrix(reps_mtx, f'{args.dir}/rep_transmtx_allconfigs.png')
 
     # 1-3. Calculate the spectral gap for the replica transition amtrix
-    spectral_gap = analyze_matrix.calc_spectral_gap(reps_mtx)
+    spectral_gap, eig_vals = analyze_matrix.calc_spectral_gap(reps_mtx)
     print(f'1-3. The spectral gap of the replica transition matrix: {spectral_gap:.3f}')
 
     # Section 2. Analysis based on transitions between states
     print('\n[ Section 2. Analysis based on transitions between states ]')
     section_idx += 1
 
     # 2-0. Stitch the trajectories for each configuration
@@ -168,18 +168,18 @@
     for i in range(EEXE.n_sim):
         mtx = analyze_traj.traj2transmtx(state_trajs[i], EEXE.n_tot)
         mtx_list.append(mtx)
         analyze_matrix.plot_matrix(mtx, f'{args.dir}/config_{i}_state_transmtx.png')
 
     # 2-4. For each configurration, calculate the spectral gap of the overall transition matrix obtained in step 2-2.
     print('\n2-4. Calculating the spectral gap of the state transition matrices ...')
-    spectral_gaps = [analyze_matrix.calc_spectral_gap(mtx) for mtx in mtx_list]
+    spectral_gaps, eig_vals = [analyze_matrix.calc_spectral_gap(mtx) for mtx in mtx_list]
     if None not in spectral_gaps:
         for i in range(EEXE.n_sim):
-            print(f'   - Configuration {i}: {spectral_gaps[i]:.3f}')
+            print(f'   - Configuration {i}: {spectral_gaps[i]:.3f} (λ_1: {eig_vals[0]:.5f}, λ_2: {eig_vals[1]:.5f})')
         print(f'   - Average of the above: {np.mean(spectral_gaps):.3f} (std: {np.std(spectral_gaps, ddof=1):.3f})')
 
     # 2-5. For each configuration, calculate the stationary distribution from the overall transition matrix obtained in step 2-2.  # noqa: E501
     print('\n2-5. Calculating the stationary distributions ...')
     pi_list = [analyze_matrix.calc_equil_prob(mtx) for mtx in mtx_list]
     if any([x is None for x in pi_list]):
         pass  # None is in the list
@@ -306,15 +306,15 @@
         is_transmtx = [is_transition_matrix(i) for i in mtx_list]
         for i in range(len(is_transmtx)):
             if is_transmtx[i] is False:
                 print(f'     The sums of the rows are not 1 (but {np.sum(mtx_list[i], axis=1)}) for the transition matrix of configuration {i}.')  # noqa: E501
 
         # 3-5. Calculate the spectral gap from the transition matrix of each configuration
         print('\n3-5. Calculating the spectral gap of the state transition matrices obtained from MSMs ...')
-        spectral_gaps = [analyze_matrix.calc_spectral_gap(mtx) for mtx in mtx_list]
+        spectral_gaps, eig_vals = [analyze_matrix.calc_spectral_gap(mtx) for mtx in mtx_list]
         for i in range(EEXE.n_sim):
             print(f'       - Configuration {i}: {spectral_gaps[i]:.3f}')
 
         # 3-6. Calculate the stationary distribution for each configuration
         print('\n3-6. Calculating the stationary distributions from the transition matrices obtained from MSMs ...')
         pi_list = [m.pi for m in models]
         for i in range(EEXE.n_sim):
@@ -375,8 +375,13 @@
         print('Plotting the full-range free energy profile ...')
         analyze_free_energy.plot_free_energy(f, f_err, f'{args.dir}/free_energy_profile.png')
 
         print('The full-range free energy profile averaged over all replicas:')
         print(f"  {', '.join(f'{f[i]: .3f} +/- {f_err[i]: .3f} kT' for i in range(EEXE.n_tot))}")
         print(f'The free energy difference between the coupled and decoupled states: {f[-1]: .3f} +/- {f_err[-1]: .3f} kT')  # noqa: E501
 
+    # Section 4. Calculate the time spent in GROMACS (This could take a while.)
+    t_wall_tot, t_sync = utils.analyze_EEXE_time()
+    print(f'\nTotal wall time GROMACS spent to finish all iterations: {utils.format_time(t_wall_tot)}')
+    print(f'Total time spent in syncrhonizing all replicas: {utils.format_time(t_sync)}')
+
     print(f'\nTime elpased: {utils.format_time(time.time() - t0)}')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ensemble_md-0.5.0/ensemble_md/cli/explore_EEXE.py` & `ensemble_md-0.6.0/ensemble_md/cli/explore_EEXE.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/cli/run_EEXE.py` & `ensemble_md-0.6.0/ensemble_md/cli/run_EEXE.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #                                                                  #
 #    Written by Wei-Tse Hsu <wehs7661@colorado.edu>                #
 #    Copyright (c) 2022 University of Colorado Boulder             #
 #                                                                  #
 ####################################################################
 import os
 import sys
-import glob
 import time
 import copy
 import shutil
 import argparse
 import numpy as np
 from mpi4py import MPI
 from datetime import datetime
@@ -78,75 +77,56 @@
 
     if rank == 0:
         # Print out simulation parameters
         EEXE.print_params()
 
         # Print out warnings and fail if needed
         for i in EEXE.warnings:
-            print()
-            print(f'{i}')
-            print()
+            print(f'\n{i}\n')
 
         if len(EEXE.warnings) > args.maxwarn:
             raise ParameterError(
                 f"The execution failed due to warning(s) about parameter spcificaiton. Check the warnings, or consider setting maxwarn in the input YAML file if you find them harmless.")  # noqa: E501, F541
 
     # Step 2: If there is no checkpoint file found/provided, perform the 1st iteration (index 0)
     if os.path.isfile(args.ckpt) is False:
+        start_idx = 1
+
         # 2-1. Set up input files for all simulations with 1 rank
         if rank == 0:
             for i in range(EEXE.n_sim):
                 os.mkdir(f'sim_{i}')
                 os.mkdir(f'sim_{i}/iteration_0')
                 MDP = EEXE.initialize_MDP(i)
                 MDP.write(f"sim_{i}/iteration_0/{EEXE.mdp.split('/')[-1]}", skipempty=True)
-                shutil.copy(f'{EEXE.gro}', f"sim_{i}/iteration_0/{EEXE.gro.split('/')[-1]}")
-                shutil.copy(f'{EEXE.top}', f"sim_{i}/iteration_0/{EEXE.top.split('/')[-1]}")
 
         # 2-2. Run the first ensemble of simulations
-        md = EEXE.run_EEXE(0)
+        EEXE.run_EEXE(0)
 
-        # 2-3. Restructure the directory (move the files from mdrun_0_i0_* to sim_*/iteration_0)
-        if rank == 0:
-            work_dir = md.output.directory.result()
-            for i in range(EEXE.n_sim):
-                if EEXE.verbose is True:
-                    print(f'  Moving files from {work_dir[i].split("/")[-1]}/ to sim_{i}/iteration_0/ ...')
-                    print(f'  Removing the empty folder {work_dir[i].split("/")[-1]} ...')
-                for f in glob.glob(f'{work_dir[i]}/*'):
-                    shutil.move(f, f'sim_{i}/iteration_0/')
-                os.rmdir(work_dir[i])
-        start_idx = 1
     else:
         if rank == 0:
             # If there is a checkpoint file, we see the execution as an extension of an EEXE simulation
             ckpt_data = np.load(args.ckpt)
-            start_idx = len(ckpt_data[0])
+            start_idx = len(ckpt_data[0])  # The length should be the same for the same axis
             print(f'\nGetting prepared to extend the EEXE simulation from iteration {start_idx} ...')
 
-            print('Deleting corrupted data ...')
-            corrupted = glob.glob('gmxapi.commandline.cli*')  # corrupted iteration
-            corrupted.extend(glob.glob('mdrun*'))
-            for i in corrupted:
-                shutil.rmtree(i)
-            if len(corrupted) == 0:
-                corrupt_bool = False
-
-            for i in range(EEXE.n_sim):
-                n_finished = len(next(os.walk(f'sim_{i}'))[1])  # number of finished iterations (the last might be initialized but corrupted though)  # noqa: E501
-                if n_finished == EEXE.n_iter and corrupt_bool is False:
-                    print('Extension aborted: The expected number of iterations have been completed!')
-                    sys.exit()
-                else:
-                    print('Deleting data generated after the checkpoint ...')
+            if start_idx == EEXE.n_iter:
+                print('Extension aborted: The expected number of iterations have been completed!')
+                sys.exit()
+            else:
+                print('Deleting data generated after the checkpoint ...')
+                for i in range(EEXE.n_sim):
+                    n_finished = len(next(os.walk(f'sim_{i}'))[1])  # number of finished iterations
                     for j in range(start_idx, n_finished):
                         print(f'  Deleting the folder sim_{i}/iteration_{j}')
                         shutil.rmtree(f'sim_{i}/iteration_{j}')
 
             # Read g_vecs.npy and rep_trajs.npy so that new data can be appended, if any.
+            # Note that these two arrays are created in rank 0 and should always be operated in rank 0,
+            # or broadcasting is required.
             EEXE.rep_trajs = [list(i) for i in ckpt_data]
             if os.path.isfile(args.g_vecs) is True:
                 EEXE.g_vecs = [list(i) for i in np.load(args.g_vecs)]
         else:
             start_idx = None
 
         start_idx = comm.bcast(start_idx, root=0)  # so that all the ranks are aware of start_idx
@@ -155,70 +135,97 @@
         if rank == 0:
             # Step 3: Swap the coordinates
             # 3-1. For all the replica simulations,
             #   (1) Find the last sampled state and the corresponding lambda values from the DHDL files.
             #   (2) Find the final Wang-Landau incrementors and weights from the LOG files.
             dhdl_files = [f'sim_{j}/iteration_{i - 1}/dhdl.xvg' for j in range(EEXE.n_sim)]
             log_files = [f'sim_{j}/iteration_{i - 1}/md.log' for j in range(EEXE.n_sim)]
-            states = EEXE.extract_final_dhdl_info(dhdl_files)
-            wl_delta, weights, counts = EEXE.extract_final_log_info(log_files)
+            states_ = EEXE.extract_final_dhdl_info(dhdl_files)
+            wl_delta, weights_, counts = EEXE.extract_final_log_info(log_files)
             print()
 
             # 3-2. Identify swappable pairs, propose swap(s), calculate P_acc, and accept/reject swap(s)
-            # Note after `get_swapping_pattern`, `states` won't be necessarily since it is updated by
-            # `get_swapping_pattern`. (Even if the function does not explicitly returns `states`, `states`
-            # can still be different after the use of the function.) Therefore, here we create copy of states
-            # before the use of `get_swapping_pattern`, so we can use the copy in `update_MDP`.
-            states_copy = copy.deepcopy(states)
-            swap_pattern = EEXE.get_swapping_pattern(dhdl_files, states, weights)
-
-            # 3-3. Perform histogram correction for the weights as needed
-            weights = EEXE.histogram_correction(weights, counts)
-
-            # 3-4. Combine the weights. Note that this is just for initializing the next iteration and is indepdent of swapping itself.  # noqa: E501
-            weights, g_vec = EEXE.combine_weights(weights, method=EEXE.w_scheme)
-            EEXE.g_vecs.append(g_vec)
+            # Note after `get_swapping_pattern`, `states_` and `weights_` won't be necessarily
+            # since they are updated by `get_swapping_pattern`. (Even if the function does not explicitly
+            # returns `states_` and `weights_`, `states_` and `weights_` can still be different after
+            # the use of the function.) Therefore, here we create copyes for `states_` and `weights_`
+            # before the use of `get_swapping_pattern`, so we can use them in `histogram_correction`,
+            # `combine_weights` and `update_MDP`.
+            states = copy.deepcopy(states_)
+            weights = copy.deepcopy(weights_)
+            swap_pattern = EEXE.get_swapping_pattern(dhdl_files, states_, weights_)
+
+            # 3-3. Calculate the weights averaged since the last update of the Wang-Landau incrementor.
+            # Note that the averaged weights are used for histogram correction/weight combination.
+            # For the calculation of the acceptance ratio (inside get_swapping_pattern), final weights should be used.
+            if EEXE.N_cutoff != -1 or EEXE.w_combine is True:
+                # Only when histogram correction/weight combination is needed.
+                weights_avg, weights_err = EEXE.get_averaged_weights(log_files)
+
+            # 3-4. Perform histogram correction/weight combination
+            # Note that we never use final weights but averaged weights here.
+            # The product of this step should always be named as "weights" to be used in update_MDP
+            if wl_delta != [None for i in range(EEXE.n_sim)]:  # weight-updating
+                print(f'\nCurrent Wang-Landau incrementors: {wl_delta}')
+            if EEXE.N_cutoff != -1 and EEXE.w_combine is True:
+                # perform both
+                weights_avg = EEXE.histogram_correction(weights_avg, counts)
+                weights, g_vec = EEXE.combine_weights(weights_avg)
+                EEXE.g_vecs.append(g_vec)
+            elif EEXE.N_cutoff == -1 and EEXE.w_combine is True:
+                # only perform weight combination
+                print('\nNote: No histogram correction will be performed.')
+                weights, g_vec = EEXE.combine_weights(weights_avg)
+                EEXE.g_vecs.append(g_vec)
+            elif EEXE.N_cutoff != -1 and EEXE.w_combine is False:
+                # only perform histogram correction
+                print('\nNote: No weight combination will be performed.')
+                weights = EEXE.histogram_correction(weights_avg, counts)
+            else:
+                print('\nNote: No histogram correction will be performed.')
+                print('Note: No weight combination will be performed.')
 
             # 3-5. Modify the MDP files and swap out the GRO files (if needed)
             # Here we keep the lambda range set in mdp the same across different iterations in the same folder but swap out the gro file  # noqa: E501
-            # Note we use states_copy instead of states in update_MDP.
+            # Note we use states (copy of states_) instead of states_ in update_MDP.
             for j in list(range(EEXE.n_sim)):
                 os.mkdir(f'sim_{j}/iteration_{i}')
-                MDP = EEXE.update_MDP(f"sim_{j}/iteration_{i - 1}/{EEXE.mdp.split('/')[-1]}", j, i, states_copy, wl_delta, weights)   # modify with a new template  # noqa: E501
+                MDP = EEXE.update_MDP(f"sim_{j}/iteration_{i - 1}/{EEXE.mdp.split('/')[-1]}", j, i, states, wl_delta, weights, counts)   # modify with a new template  # noqa: E501
                 MDP.write(f"sim_{j}/iteration_{i}/{EEXE.mdp.split('/')[-1]}", skipempty=True)
-                shutil.copy(f'{EEXE.top}', f"sim_{j}/iteration_{i}/{EEXE.top.split('/')[-1]}")
+                # In run_EEXE(i, swap_pattern), where the tpr files will be generated, we use the top file at the
+                # level of the simulation (the file that will be shared by all simulations). For the gro file, we pass
+                # swap_pattern to the function to figure it out internally.
+        else:
+            swap_pattern = None
 
-                # Now we swap out the GRO files as needed
-                shutil.copy(f'sim_{swap_pattern[j]}/iteration_{i-1}/confout.gro', f"sim_{j}/iteration_{i}/{EEXE.gro.split('/')[-1]}")  # noqa: E501
+        if -1 not in EEXE.equil and 0 not in EEXE.equil:
+            # This is the case where the weights are equilibrated in a weight-updating simulation.
+            # As a remidner, EEXE.equil should be a list of 0 after extract_final_log_info in a
+            # fixed-weight simulation, and a list of -1 for a weight-updating simulation with unequilibrated weights.
+            print('\nSimulation terminated: The weights have been equilibrated for all replicas.')
+            break
 
         # Step 4: Perform another iteration
         # 4-1. Run another ensemble of simulations
-        md = EEXE.run_EEXE(i)
+        swap_pattern = comm.bcast(swap_pattern, root=0)
+        EEXE.run_EEXE(i, swap_pattern)
 
         if rank == 0:
-            # 4-2. Restructure the directory (move the files from mdrun_{i}_i0_* to sim_*/iteration_{i})
-            work_dir = md.output.directory.result()
-            for j in range(EEXE.n_sim):
-                if EEXE.verbose is True:
-                    print(f'  Moving files from {work_dir[j].split("/")[-1]}/ to sim_{j}/iteration_{i}/ ...')
-                    print(f'  Removing the empty folder {work_dir[j].split("/")[-1]} ...')
-                for f in glob.glob(f'{work_dir[j]}/*'):
-                    shutil.move(f, f'sim_{j}/iteration_{i}/')
-                os.rmdir(work_dir[j])
-
-            # 4-3. Checkpoint as needed
+            # 4-2. Save data
             if (i + 1) % EEXE.n_ckpt == 0:
-                print('\n----- Saving .npy files to checkpoint the simulation ---')
-                if EEXE.g_vecs[0] is not None:
+                if len(EEXE.g_vecs) != 0:
+                    # Save g_vec as a function of time if weight combination was used.
                     np.save('g_vecs.npy', EEXE.g_vecs)
+
+                print('\n----- Saving .npy files to checkpoint the simulation ---')
                 np.save('rep_trajs.npy', EEXE.rep_trajs)
 
     # Save the npy files at the end of the simulation anyway.
     if rank == 0:
-        if EEXE.g_vecs[0] is not None:
+        if len(EEXE.g_vecs) != 0:  # The length will be 0 only if there is no weight combination.
             np.save('g_vecs.npy', EEXE.g_vecs)
         np.save('rep_trajs.npy', EEXE.rep_trajs)
 
     # Step 5: Write a summary for the simulation ensemble
     if rank == 0:
         print('\nSummary of the simulation ensemble')
         print('==================================')
@@ -231,12 +238,15 @@
             else:
                 idx = int(np.floor(EEXE.equil[i] / (EEXE.dt * EEXE.nst_sim)))
                 if EEXE.equil[i] > 1000:
                     units = 'ns'
                     EEXE.equil[i] /= 1000
                 else:
                     units = 'ps'
-                print(f'  - Rep {i}: The weights have been equilibrated at {EEXE.equil[i]} {units} (iteration {idx}).')
+                print(f'  - Rep {i}: The weights have been equilibrated at {EEXE.equil[i]:.2f} {units} (iteration {idx}).')  # noqa: E501
 
-        print(f'\n{EEXE.n_rejected} out of {EEXE.n_swap_attempts}, or {EEXE.n_rejected / EEXE.n_swap_attempts * 100:.1f}% of attempted exchanges were rejected.')  # noqa: E501
+        print(f'\n{EEXE.n_empty_swappable} out of {EEXE.n_iter}, or {EEXE.n_empty_swappable / EEXE.n_iter * 100:.1f}% iterations had an empty list of swappable pairs.')  # noqa: E501
+        print(f'{EEXE.n_rejected} out of {EEXE.n_swap_attempts}, or {EEXE.n_rejected / EEXE.n_swap_attempts * 100:.1f}% of attempted exchanges were rejected.')  # noqa: E501
 
         print(f'\nTime elapsed: {utils.format_time(time.time() - t1)}')
+
+    sys.exit()
```

### Comparing `ensemble_md-0.5.0/ensemble_md/data/README.md` & `ensemble_md-0.6.0/ensemble_md/data/README.md`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/ensemble_EXE.py` & `ensemble_md-0.6.0/ensemble_md/ensemble_EXE.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,29 @@
 """
 import os
 import sys
 import copy
 import yaml
 import shutil
 import random
+import subprocess
 import numpy as np
 from mpi4py import MPI
 from itertools import combinations
 from collections import OrderedDict
 from alchemlyb.parsing.gmx import extract_dHdl
 from alchemlyb.parsing.gmx import _get_headers as get_headers
 from alchemlyb.parsing.gmx import _extract_dataframe as extract_dataframe
 
-import gmxapi as gmx
 import ensemble_md
-from ensemble_md.utils import utils
 from ensemble_md.utils import gmx_parser
 from ensemble_md.utils.exceptions import ParameterError
 
-
-rank = MPI.COMM_WORLD.Get_rank()  # Note that this is a GLOBAL variable
+comm = MPI.COMM_WORLD
+rank = comm.Get_rank()  # Note that this is a GLOBAL variable
 
 
 class EnsembleEXE:
     """
     This class provides a variety of functions useful for setting up and running
     an ensemble of expanded ensemble. Upon instantiation, all parameters in the YAML
     file will be assigned to an attribute in the class. In addition to these variables,
@@ -47,27 +46,38 @@
     :ivar reformatted_mdp: Whether the templated MDP file has been reformatted by replacing hyphens
         with underscores or not.
     :ivar template: The instance of the :obj:`MDP` class based on the template MDP file.
     :ivar nsteps: The number of steps per iteration.
     :ivar dt: The simulation timestep in ps.
     :ivar temp: The simulation temperature in Kelvin.
     :ivar fixed_weights: Whether the weights will be fixed during the simulation (according to the template MDP file).
+    :ivar updating_weights: The list of weights as a function of time (since the last update of the Wang-Landau
+        incrementor) for different replicas. The length is equal to the number of replicas. This is only relevant for
+        weight-updating simulations.
+    :ivar equilibrated_weights: The equilibrated weights of different replicas. For weight-equilibrating simulations,
+        this list is initialized as a list of empty lists. Otherwise (weight-fixed), it is initialized as a list of
+        :code:`None`.
+    :ivar current_wl_delta: The current value of the Wang-Landau incrementor. This is only relevent for weight-updating
+        simulations.
     :ivar kT: 1 kT in kJ/mol at the simulation temperature.
     :ivar lambda_types: The types of lambda variables involved in expanded ensemble simulations, e.g.
         :code:`fep_lambdas`, :code:`mass_lambdas`, :code:`coul_lambdas`, etc.
     :ivar n_tot: The total number of states for all replicas.
     :ivar n_sub: The numbmer of states for each replica. The current implementation assumes homogenous replicas.
     :ivar state_ranges: A list of list of state indices for each replica.
-    :ivar equil: A list of times it took to equilibrated the weights for different replicas.
+    :ivar equil: A list of times it took to equilibrated the weights for different replicas. This
+        list is initialized with a list of -1, where -1 means that the weights haven't been equilibrated. Also,
+        a value of 0 means that the simulation is a fixed-weight simulation.
     :ivar lambda_dict: A dictionary with keys being the tuples of coupling parameters used in each replicas and
         values being the corresponding global index (starting from 0). Assigned by :obj:`map_lambda2state`.
     :ivar lambda_ranges: A list of lambda vectors of state range of each replica. Assigned by :obj:`map_lambda2state`.
     :ivar n_rejected: The number of proposed exchanges that have been rejected. Updated by :obj:`accept_or_reject`.
     :ivar n_swap_attempts: The number of swaps attempted so far. This does not include the cases
         where there is no swappable pair. Updated by :obj:`get_swapping_pattern`.
+    :ivar n_emtpy_swappable: The number of times when there was no swappable pair.
     :ivar rep_trajs: The replica-space trajectories of all replicas.
     :ivar configs: A list that thows the current configuration index that each replica is sampling.
     :ivar g_vecs: The time series of the (processed) whole-range alchemical weights. If no weight combination is
         applied, this list will just be a list of :code:`None`'s.
     :ivar get_u_nk: Whether to get the :math:`u_{nk}` dataset from the DHDL files. Only meaningful during
         data analysis and if :code:`df_method` is specified.
     :ivar get_dHdl: Whether to get the :math:`dH/dλ` dataset from the DHDL files. Only meaningful
@@ -120,39 +130,44 @@
         # Step 1: Read in parameters from the YAML file.
         with open(self.yaml) as f:
             params = yaml.load(f, Loader=yaml.FullLoader)
 
         for attr in params:
             setattr(self, attr, params[attr])
 
-        # Step 2: Handle the YAML parameters
+        # Step 2: Handle the compulsory YAML parameters
         required_args = [
+            "gmx_executable",
             "gro",
             "top",
             "mdp",
-            "parallel",
             "n_sim",
             "n_iter",
             "s",
         ]
         for i in required_args:
             if hasattr(self, i) is False or getattr(self, i) is None:
                 raise ParameterError(
                     f"Required parameter '{i}' not specified in {self.yaml}."
                 )  # noqa: F405
 
+        # Check the GROMACS executable
+        self.check_gmx_executable()
+
+        # Step 3: Handle the optional YAML parameters
         # Key: Optional argument; Value: Default value
         optional_args = {
             "nst_sim": None,
             "proposal": 'exhaustive',
             "acceptance": "metropolis",
-            "w_scheme": None,
+            "w_combine": False,
             "N_cutoff": 1000,
             "n_ex": 'N^3',   # only active for multiple swaps.
             "verbose": True,
+            "grompp_args": None,
             "runtime_args": None,
             "n_ckpt": 100,
             "msm": False,
             "free_energy": False,
             "df_spacing": 1,
             "df_method": "MBAR",
             "err_method": "propagate",
@@ -165,24 +180,21 @@
 
         # all_args: Arguments that can be specified in the YAML file.
         all_args = required_args + list(optional_args.keys())
         for i in params:
             if i not in all_args:
                 self.warnings.append(f'Warning: Parameter "{i}" specified in the input YAML file is not recognizable.')
 
-        # Step 3: Check if the parameters in the YAML file are well-defined
+        # Step 4: Check if the parameters in the YAML file are well-defined
         if self.proposal not in [None, 'single', 'neighboring', 'exhaustive', 'multiple']:
             raise ParameterError("The specified proposal scheme is not available. Available options include 'single', 'neighboring', 'exhaustive', and 'multiple'.")  # noqa: E501
 
         if self.acceptance not in [None, 'same-state', 'same_state', 'metropolis', 'metropolis-eq', 'metropolis_eq']:
             raise ParameterError("The specified acceptance scheme is not available. Available options include 'same-state', 'metropolis', and 'metropolis-eq'.")  # noqa: E501
 
-        if self.w_scheme not in [None, 'mean', 'geo-mean', 'g-diff']:
-            raise ParameterError("The specified weight combining scheme is not available. Available options include None, 'mean', 'geo-mean'/'geo_mean' and 'g-diff/g_diff'.")  # noqa: E501
-
         if self.df_method not in [None, 'TI', 'BAR', 'MBAR']:
             raise ParameterError("The specified free energy estimator is not available. Available options include 'TI', 'BAR', and 'MBAR'.")  # noqa: E501
 
         if self.err_method not in [None, 'propagate', 'bootstrap']:
             raise ParameterError("The specified method for error estimation is not available. Available options include 'propagate', and 'bootstrap'.")  # noqa: E501
 
         params_int = ['n_sim', 'n_iter', 's', 'N_cutoff', 'df_spacing', 'n_ckpt', 'n_bootstrap']  # integer parameters  # noqa: E501
@@ -210,139 +222,171 @@
             raise ParameterError("The parameter 'N_cutoff' should be non-negative unless no histogram correction is needed, i.e. N_cutoff = -1.")  # noqa: E501
 
         params_str = ['gro', 'top', 'mdp']
         for i in params_str:
             if type(getattr(self, i)) != str:
                 raise ParameterError(f"The parameter '{i}' should be a string.")
 
-        params_bool = ['parallel', 'verbose', 'msm']
+        params_bool = ['verbose', 'msm']
         for i in params_bool:
             if type(getattr(self, i)) != bool:
                 raise ParameterError(f"The parameter '{i}' should be a boolean variable.")
 
-        # Step 4: Reformat the input MDP file to replace all hypens with underscores.
+        # Step 5: Reformat the input MDP file to replace all hypens with underscores.
         self.reformat_MDP()
 
-        # Step 5: Read in parameters from the MDP template
+        # Step 6: Read in parameters from the MDP template
         self.template = gmx_parser.MDP(self.mdp)
         self.nsteps = self.template["nsteps"]  # will be overwritten by self.nst_sim if nst_sim is specified.
         self.dt = self.template["dt"]  # ps
         self.temp = self.template["ref_t"]
 
         if self.nst_sim is None:
             self.nst_sim = self.nsteps
 
         if 'wl_scale' in self.template.keys():
             if isinstance(self.template['wl_scale'], np.ndarray):
                 # If wl_scale in the MDP file is a blank (i.e. fixed weights), mdp['wl_scale'] will be an empty array.
                 # This is the only case where mdp['wl_scale'] is a numpy array.
                 self.fixed_weights = True
+                self.equilibrated_weights = [None for i in range(self.n_sim)]
             else:
                 self.fixed_weights = False
+                self.equilibrated_weights = [[] for i in range(self.n_sim)]
+                self.updating_weights = [[] for i in range(self.n_sim)]
+                self.current_wl_delta = [0 for i in range(self.n_sim)]
         else:
             self.fixed_weights = True
+            self.equilibrated_weights = [None for i in range(self.n_sim)]
+
+        if self.fixed_weights is True:
+            if self.N_cutoff != -1 or self.w_combine is not False:
+                self.warnings.append('Warning: The histogram correction/weight combination method is specified but will not be used since the weights are fixed.')  # noqa: E501
+                # In the case that the warning is ignored, enforce the defaults.
+                self.N_cutoff = -1
+                self.w_combine = False
 
         if 'lmc_seed' in self.template and self.template['lmc_seed'] != -1:
             self.warnings.append('Warning: We recommend setting lmc_seed as -1 so the random seed is different for each iteration.')  # noqa: E501
 
         if 'gen_seed' in self.template and self.template['gen_seed'] != -1:
             self.warnings.append('Warning: We recommend setting gen_seed as -1 so the random seed is different for each iteration.')  # noqa: E501
 
         if 'symmetrized_transition_matrix' in self.template and self.template['symmetrized_transition_matrix'] == 'yes':  # noqa: E501
             self.warnings.append('Warning: We recommend setting symmetrized-transition-matrix to no instead of yes.')
 
         if self.template['nstlog'] > self.nst_sim:
             raise ParameterError(
                 'The parameter "nstlog" should be equal to or smaller than "nst_sim" specified in the YAML file so that the sampling information can be parsed.')  # noqa: E501
 
-        # Step 6: Set up derived parameters
-        # 6-1. kT in kJ/mol
+        # Step 7: Set up derived parameters
+        # 7-1. kT in kJ/mol
         self.kT = k * NA * self.temp / 1000  # 1 kT in kJ/mol
 
-        # 6-2. Figure out what types of lambda variables are involved
+        # 7-2. Figure out what types of lambda variables are involved
         # Here is we possible lambda types in the order read by GROMACS, which is likely also the order when being printed to the log file.  # noqa: E501
         # See https://gitlab.com/gromacs/gromacs/-/blob/main/src/gromacs/gmxpreprocess/readir.cpp#L2543
         lambdas_types_all = ['fep_lambdas', 'mass_lambdas', 'coul_lambdas', 'vdw_lambdas', 'bonded_lambdas', 'restraint_lambdas', 'temperature_lambdas']  # noqa: E501
         self.lambda_types = []  # lambdas specified in the MDP file
         for i in lambdas_types_all:
             if i in self.template.keys():  # there shouldn't be parameters like "fep-lambdas" after reformatting the MDP file  # noqa: E501
                 self.lambda_types.append(i)
 
-        # 6-3. Total # of states: n_tot = n_sub * n_sim - (n_overlap) * (n_sim - 1), where n_overlap = n_sub - s
+        # 7-3. Total # of states: n_tot = n_sub * n_sim - (n_overlap) * (n_sim - 1), where n_overlap = n_sub - s
         self.n_tot = len(self.template[self.lambda_types[0]])
 
-        # 6-4. Number of states of each replica (assuming the same for all rep)
+        # 7-4. Number of states of each replica (assuming the same for all rep)
         self.n_sub = self.n_tot - self.s * (self.n_sim - 1)
         if self.n_sub < 1:
             raise ParameterError(
                 f"There must be at least two states for each replica (current value: {self.n_sub}). The current specified configuration (n_tot={self.n_tot}, n_sim={self.n_sim}, s={self.s}) does not work for EEXE.")  # noqa: E501
 
-        # 6-5. A list of sets of state indices
+        # 7-5. A list of sets of state indices
         start_idx = [i * self.s for i in range(self.n_sim)]
         self.state_ranges = [list(np.arange(i, i + self.n_sub)) for i in start_idx]
 
-        # 6-6. A list of time it took to get the weights equilibrated
+        # 7-6. A list of time it took to get the weights equilibrated
         self.equil = [-1 for i in range(self.n_sim)]   # -1 means unequilibrated
 
-        # 6-7. Map the lamda vectors to state indices
+        # 7-7. Map the lamda vectors to state indices
         self.map_lambda2state()
 
-        # 6-8. For counting the number swap attempts and the rejected ones
+        # 7-8. Some variables for counting
         self.n_rejected = 0
         self.n_swap_attempts = 0
+        self.n_empty_swappable = 0
 
-        # 6-9. Replica space trajectories. For example, rep_trajs[0] = [0, 2, 3, 0, 1, ...] means
+        # 7-9. Replica space trajectories. For example, rep_trajs[0] = [0, 2, 3, 0, 1, ...] means
         # that configuration 0 transitioned to replica 2, then 3, 0, 1, in iterations 1, 2, 3, 4, ...,
         # respectively. The first element of rep_traj[i] should always be i.
         self.rep_trajs = [[i] for i in range(self.n_sim)]
 
-        # 6-10. configs shows the current configuration that each replica is sampling.
+        # 7-10. configs shows the current configuration that each replica is sampling.
         # For example, self.configs = [0, 2, 1, 3] means that configurations 0, 2, 1, and 3 are
         # in replicas, 0, 1, 2, 3, respectively. This list will be constantly updated during the simulation.
         self.configs = list(range(self.n_sim))
 
-        # 6-11. The time series of the (processed) whole-range alchemical weights
+        # 7-11. The time series of the (processed) whole-range alchemical weights
         # If no weight combination is applied, self.g_vecs will just be a list of None's.
         self.g_vecs = []
 
-        # 6-12. Data analysis
+        # 7-12. Data analysis
         if self.df_method == 'MBAR':
             self.get_u_nk = True
             self.get_dHdl = False
         else:
             self.get_u_nk = False
             self.get_dHdl = True
 
+    def check_gmx_executable(self):
+        """
+        Checks if the GROMACS executable can be used and  gets its absolute path and version.
+        """
+        try:
+            result = subprocess.run(['which', self.gmx_executable], capture_output=True, text=True, check=True)
+            self.gmx_path = result.stdout.strip()  # this can be exactly the same as self.gmx_executable
+
+            version_output = subprocess.run([self.gmx_path, "-version"], capture_output=True, text=True, check=True)
+            for line in version_output.stdout.splitlines():
+                if "GROMACS version" in line:
+                    self.gmx_version = line.split()[-1]
+                    break
+        except subprocess.CalledProcessError:
+            print(f"{self.gmx_executable} is not available on this system.")
+        except Exception as e:
+            print(f"An error occurred:\n{e}")
+
     def print_params(self, params_analysis=False):
         """
         Prints important parameters related to the EXEE simulation.
 
         Parameters
         ----------
         params_analysis : bool, optional
             If True, additional parameters related to data analysis will be printed. Default is False.
         """
         print("Important parameters of EXEE")
         print("============================")
         print(f"Python version: {sys.version}")
-        print(f"gmxapi version: {gmx.__version__}")
+        print(f"GROMACS executable: {self.gmx_path}")  # we print the full path here
+        print(f"GROMACS version: {self.gmx_version}")
         print(f"ensemble_md version: {ensemble_md.__version__}")
         print(f'Simulation inputs: {self.gro}, {self.top}, {self.mdp}')
         print(f"Verbose log file: {self.verbose}")
-        print(f"Whether the replicas run in parallel: {self.parallel}")
         print(f"Proposal scheme: {self.proposal}")
         print(f"Acceptance scheme for swapping simulations: {self.acceptance}")
-        print(f"Scheme for combining weights: {self.w_scheme}")
+        print(f"Whether to perform weight combination: {self.w_combine}")
         print(f"Histogram cutoff: {self.N_cutoff}")
         print(f"Number of replicas: {self.n_sim}")
         print(f"Number of iterations: {self.n_iter}")
         print(f"Number of attempted swaps in one exchange interval: {self.n_ex}")
         print(f"Length of each replica: {self.dt * self.nst_sim} ps")
         print(f"Frequency for checkpointing: {self.n_ckpt} iterations")
         print(f"Total number of states: {self.n_tot}")
+        print(f"Additional grompp arguments: {self.grompp_args}")
         print(f"Additional runtime arguments: {self.runtime_args}")
         print("Alchemical ranges of each replica in EEXE:")
         for i in range(self.n_sim):
             print(f"  - Replica {i}: States {self.state_ranges[i]}")
 
         if params_analysis is True:
             print()
@@ -422,15 +466,15 @@
             MDP[i] = self.template[i][start_idx:start_idx + self.n_sub]
 
         if "init_lambda_weights" in self.template:
             MDP["init_lambda_weights"] = self.template["init_lambda_weights"][start_idx:start_idx + self.n_sub]
 
         return MDP
 
-    def update_MDP(self, new_template, sim_idx, iter_idx, states, wl_delta, weights):
+    def update_MDP(self, new_template, sim_idx, iter_idx, states, wl_delta, weights, counts=None):
         """
         Updates the MDP file for a new iteration based on the new MDP template coming from the previous iteration.
         Note that if the weights got equilibrated in the previous iteration, then the weights will be fixed
         at these equilibrated values for all the following iterations.
 
         Parameters
         ----------
@@ -442,27 +486,35 @@
             The index of the iteration to be performed later.
         states : list
             A list of last sampled states of all simulaitons in the previous iteration.
         wl_delta : list
             A list of final Wang-Landau incrementors of all simulations.
         weights : list
             A list of lists final weights of all simulations.
+        counts : list
+            A list of lists final counts of all simulations. If the value is :code:`None`,
+            then the MDP parameter :code:`init-histogram-counts` won't be specified in the next iteration.
+            Note that not all the GROMACS versions have the MDP parameter :code:`init-histogram-counts` available,
+            in which case one should always pass :code:`None`, or set :code:`-maxwarn` in :code:`grompp_args`
+            in the input YAML file.
 
         Return
         ------
         MDP : :obj:`.gmx_parser.MDP` obj
             An updated object of :obj:`.gmx_parser.MDP` that can be used to write MDP files.
         """
         new_template = gmx_parser.MDP(new_template)  # turn into a gmx_parser.MDP object
         MDP = copy.deepcopy(new_template)
         MDP["tinit"] = self.nst_sim * self.dt * iter_idx
         MDP["nsteps"] = self.nst_sim
         MDP["init_lambda_state"] = (states[sim_idx] - sim_idx * self.s)  # 2nd term is for shifting from the global to local index.  # noqa: E501
-        MDP["init_lambda_weights"] = weights[sim_idx]
         MDP["init_wl_delta"] = wl_delta[sim_idx]
+        MDP["init_lambda_weights"] = weights[sim_idx]
+        if counts is not None:
+            MDP["init_histogram_counts"] = counts[sim_idx]
 
         if self.equil[sim_idx] == -1:   # the weights haven't been equilibrated
             MDP["init_wl_delta"] = wl_delta[sim_idx]
         else:
             MDP["lmc_stats"] = "no"
             MDP["wl_scale"] = ""
             MDP["wl_ratio"] = ""
@@ -476,30 +528,30 @@
         """
         For all the replica simulations, finds the last sampled state
         and the corresponding lambda values from a dhdl file.
 
         Parameters
         ----------
         dhdl_files : list
-            A list of GROMACS DHDL file names.
+            A list of file paths to GROMACS DHDL files of different replicas.
 
         Returns
         -------
         states : list
             A list of the global indices of the last sampled states of all simulaitons.
         """
         states, lambda_vecs = [], []
         print("\nBelow are the final states being visited:")
-        for j in range(self.n_sim):
-            dhdl = extract_dHdl(dhdl_files[j], T=self.temp)
+        for i in range(self.n_sim):
+            dhdl = extract_dHdl(dhdl_files[i], T=self.temp)
             lambda_vecs.append(dhdl.index[-1][1:])
             states.append(self.lambda_dict[lambda_vecs[-1]])  # absolute order
             print(
-                f"  Simulation {j}: Global state {states[j]}, (coul, vdw) = \
-                {list(self.lambda_dict.keys())[list(self.lambda_dict.values()).index(states[j])]}"
+                f"  Simulation {i}: Global state {states[i]}, (coul, vdw) = \
+                {list(self.lambda_dict.keys())[list(self.lambda_dict.values()).index(states[i])]}"
             )
         print('\n', end='')
 
         return states
 
     def extract_final_log_info(self, log_files):
         """
@@ -509,49 +561,88 @@
           - The final lists of weights.
           - The final lists of counts.
           - Whether the weights were equilibrated in the simulations.
 
         Parameters
         ----------
         log_files : list
-            A list of file paths to GROMACS LOG files.
+            A list of file paths to GROMACS LOG files of different replicas.
 
         Returns
         -------
         wl_delta : list
             A list of final Wang-Landau incrementors of all simulations.
         weights : list
             A list of lists of final weights of all simulations.
         counts : list
             A list of lists of final counts of all simulations.
         """
         wl_delta, weights, counts = [], [], []
 
-        # 2. Find the final Wang-Landau incrementors and weights
-        for j in range(self.n_sim):
+        # Find the final Wang-Landau incrementors and weights
+        for i in range(self.n_sim):
             if self.verbose:
-                print(f'Parsing {log_files[j]} ...')
-            result = gmx_parser.parse_log(log_files[j])
-            wl_delta.append(result[0])
-            weights.append(result[1])
-            counts.append(result[2])
+                print(f'Parsing {log_files[i]} ...')
+            result = gmx_parser.parse_log(log_files[i])  # weights, counts, wl_delta, equil_time
+            weights.append(result[0][-1])
+            counts.append(result[1])
+            wl_delta.append(result[2])
 
             # In Case 3 described in the docstring of parse_log (fixed-weights),
-            # result[3] will be 0 but it will never be passed to self.equil[j]
-            # because once self.equil[j] is not -1, we stop updating. This way, we can keep
+            # result[3] will be 0 but it will never be passed to self.equil[i]
+            # because once self.equil[i] is not -1, we stop updating. This way, we can keep
             # the time when the weights get equilibrated all the way.
-            if self.equil[j] == -1:
+            if self.equil[i] == -1:
                 # At this point self.equil is the equilibration status BEFORE the last iteration
                 # while result[3] is the equilibration status AFTER finishing the last iteraiton.
                 # For any replicas where weights are still equilibrating (i.e. self.equil[j] == -1)
                 # we update its equilibration status.
-                self.equil[j] = result[3]
+                self.equil[i] = result[3]
+
+            if self.equilibrated_weights[i] == []:
+                if self.equil[i] != -1 and self.equil[i] != 0:
+                    # self.equil[i] != -1: uneqilibrated
+                    # self.equil[i] != 0: fixed-weight simulation
+                    self.equilibrated_weights[i] = result[0][-1]
 
         return wl_delta, weights, counts
 
+    def get_averaged_weights(self, log_files):
+        """
+        For each replica, calculate the averaged weights (and the associated error) from the time series
+        of the weights since the previous update of the Wang-Landau incrementor.
+
+        Parameters
+        ----------
+        log_files : list
+            A list of file paths to GROMACS LOG files of different replicas.
+
+        Returned
+        --------
+        weights_avg : list
+            A list of lists of weights averaged since the last update of the Wang-Landau
+            incrementor. The length of the list should be the number of replicas.
+        weights_err : list
+            A list of lists of errors corresponding to the values in :code:`weights_avg`.
+        """
+        for i in range(self.n_sim):
+            weights, _, wl_delta, _ = gmx_parser.parse_log(log_files[i])
+            if self.current_wl_delta[i] == wl_delta:
+                self.updating_weights[i] += weights  # expand the list
+            else:
+                self.current_wl_delta[i] = wl_delta
+                self.updating_weights[i] = weights
+
+        # shape of self.updating_weights is (n_sim, n_points, n_states), but n_points can be different
+        # for different replicas, which will error out np.mean(self.updating_weights, axis=1)
+        weight_avg = [np.mean(self.updating_weights[i], axis=0).tolist() for i in range(self.n_sim)]
+        weight_err = [np.std(self.updating_weights[i], axis=0, ddof=1).tolist() for i in range(self.n_sim)]
+
+        return weight_avg, weight_err
+
     def identify_swappable_pairs(self, states, state_ranges):
         """
         Identify swappable pairs. By definition, a pair of simulation is considered swappable only if
         their last sampled states are in the alchemical ranges of both simulations. This is required
         to ensure that the values of involved ΔH and Δg can always be looked up from the DHDL and LOG files.
         This also automatically guarantee that the simulations to be swapped have overlapping alchemical ranges.
 
@@ -678,16 +769,15 @@
                 swappables = [i for i in swappables if set(i).intersection(set(swap)) == set()]  # noqa: F821
                 print(f'\nRemaining swappable pairs: {swappables}')
 
             if len(swappables) == 0 and self.proposal == 'exhaustive':
                 # This should only happen when the method of exhaustive swaps is used.
                 print(f'{n_ex_exhaustive} swap(s) have been attempted to exhaustively explore all possible swaps.')
                 if i == 0:
-                    self.n_swap_attempts += 1
-                    self.n_rejected += 1
+                    self.n_empty_swappable += 1
                 break
             else:
                 self.n_swap_attempts += 1
                 if self.proposal == 'exhaustive':
                     n_ex_exhaustive += 1
 
                 swap = self.propose_swap(swappables)
@@ -890,248 +980,270 @@
             A list of lists of counts (of ALL simulations).
 
         Return
         ------
         weights : list
             An updated list of lists of corected weights.
         """
-        if self.N_cutoff == -1:
-            print('\nNote: No histogram correction will be performed.')
+        if self.verbose is True:
+            print("\nPerforming histogram correction for the lambda weights ...")
         else:
-            if self.verbose is True:
-                print("\nPerforming histogram correction for the lambda weights ...")
-            else:
-                print("\nPerforming histogram correction for the lambda weights ...", end="")
+            print("\nPerforming histogram correction for the lambda weights ...", end="")
 
-            for i in range(len(weights)):  # loop over the replicas
-                if self.verbose is True:
-                    print(f"  Counts of rep {i}:\t\t{counts[i]}")
-                    print(f'  Original weights of rep {i}:\t{[float(f"{k:.3f}") for k in weights[i]]}')
+        for i in range(len(weights)):  # loop over the replicas
+            if self.verbose is True:
+                print(f"  Counts of rep {i}:\t\t{counts[i]}")
+                print(f'  Original weights of rep {i}:\t{[float(f"{k:.3f}") for k in weights[i]]}')
 
-                for j in range(1, len(weights[i])):  # loop over the alchemical states
-                    if counts[i][j - 1] != 0 and counts[i][j - 1] != 0:
-                        if np.min([counts[i][j - 1], counts[i][j]]) > self.N_cutoff:
-                            weights[i][j] += np.log(counts[i][j - 1] / counts[i][j])
+            for j in range(1, len(weights[i])):  # loop over the alchemical states
+                if counts[i][j - 1] != 0 and counts[i][j - 1] != 0:
+                    if np.min([counts[i][j - 1], counts[i][j]]) > self.N_cutoff:
+                        weights[i][j] += np.log(counts[i][j - 1] / counts[i][j])
 
-                if self.verbose is True:
-                    print(f'  Corrected weights of rep {i}:\t{[float(f"{k:.3f}") for k in weights[i]]}\n')
+            if self.verbose is True:
+                print(f'  Corrected weights of rep {i}:\t{[float(f"{k:.3f}") for k in weights[i]]}\n')
 
-            if self.verbose is False:
-                print(' Done')
+        if self.verbose is False:
+            print(' Done')
 
         return weights
 
-    def combine_weights(self, weights, method):
+    def combine_weights(self, weights):
         """
-        Combine alchemical weights across multiple replicas using probability ratios
-        or weight differences. (See :ref:`doc_w_schemes` for mor details.)
+        Combine alchemical weights across multiple replicas. (See :ref:`doc_w_schemes` for mor details.)
 
         Parameters
         ----------
         weights : list
             A list of Wang-Landau weights of ALL simulations
-        method : str
-            Method for combining weights. Must be one of the following:
-
-              * :code:`None`: No weight combination is performed, and the original weights are returned.
-              * :code:`mean`: The arithmetic mean of the probability ratios is used to scale the weights.
-              * :code:`geo-mean` or :code:`geo_mean`: The geometric mean of the probability ratios is
-                used to scale the weights.
-              * :code:`g-diff` or :code:`g_diff`: The difference between neighboring weights is used
-                to determine the alchemical weights.
 
         Returns
         -------
         weights : list
-            A list of original (if method is :code:`None`) or modified Wang-Landau weights of ALL simulations.
+            A list of modified Wang-Landau weights of ALL simulations.
         g_vec : np.array
             An array of alchemical weights of the whole range of states.
         """
-        if method is None:
-            print('Note: No weight combination will be performed.')
-            g_vec = None
-            return weights, g_vec
+        if self.verbose is True:
+            print('Performing weight combination ...')
         else:
-            if self.verbose is True:
-                print(f'Performing weight combination with the {method} method ...')
-            else:
-                print(f'Performing weight combination with the {method} method ...', end='')
+            print('Performing weight combination ...', end='')
 
-            if self.verbose is True:
-                w = np.round(weights, decimals=3).tolist()  # just for printing
-                print('  Original weights:')
-                for i in range(len(w)):
-                    print(f'    Rep {i}: {w[i]}')
-
-            if method == 'g-diff' or method == 'g_diff':
-                # Method based on weight differences
-                dg_vec = []
-                dg_adjacent = [list(np.diff(weights[i])) for i in range(len(weights))]
-                for i in range(self.n_tot - 1):
-                    dg_list = []
-                    for j in range(len(self.state_ranges)):
-                        if i in self.state_ranges[j] and i + 1 in self.state_ranges[j]:
-                            idx = self.state_ranges[j].index(i)
-                            dg_list.append(dg_adjacent[j][idx])
-                    dg_vec.append(np.mean(dg_list))
-                dg_vec.insert(0, 0)
-                g_vec = np.array([sum(dg_vec[:(i + 1)]) for i in range(len(dg_vec))])
-            else:
-                # Method based on probability ratios
-                # Step 1: Convert the weights into probabilities
-                weights = np.array(weights)
-                prob = np.array([[np.exp(-i)/np.sum(np.exp(-weights[j])) for i in weights[j]] for j in range(len(weights))])  # noqa: E501
-
-                # Step 2: Caclulate the probability ratios (after figuring out overlapped states between adjacent replicas)  # noqa: E501
-                overlapped = [set(self.state_ranges[i]).intersection(set(self.state_ranges[i + 1])) for i in range(len(self.state_ranges) - 1)]  # noqa: E501
-                prob_ratio = [prob[i + 1][: len(overlapped[i])] / prob[i][-len(overlapped[i]):] for i in range(len(overlapped))]  # noqa: E501
-
-                # Step 3: Average the probability ratios
-                avg_ratio = [1]   # This allows easier scaling since the first prob vector stays the same.
-                if method == 'mean':
-                    avg_ratio.extend([np.mean(prob_ratio[i]) for i in range(len(prob_ratio))])
-                elif method == 'geo-mean':
-                    avg_ratio.extend([np.prod(prob_ratio[i])**(1/len(prob_ratio[i])) for i in range(len(prob_ratio))])
-
-                # Step 4: Scale the probabilities for each replica
-                scaled_prob = np.array([prob[i] / np.prod(avg_ratio[: i + 1]) for i in range(len(prob))])
-
-                # Step 5: Average and convert the probabilities
-                p_vec = []
-                for i in range(self.n_tot):   # global state index
-                    p = []   # a list of probabilities to be averaged for each state
-                    for j in range(len(self.state_ranges)):   # j can be regared as the replica index
-                        if i in self.state_ranges[j]:
-                            local_idx = i - j * self.s
-                            p.append(scaled_prob[j][local_idx])
-                    if method == 'mean':
-                        p_vec.append(np.mean(p))
-                    elif method == 'geo-mean' or method == 'geo_mean':
-                        p_vec.append(np.prod(p) ** (1 / len(p)))
-
-                g_vec = -np.log(p_vec)
-                g_vec -= g_vec[0]
-
-            # Determine the vector of alchemical weights for each replica
-            weights = [list(g_vec[i: i + self.n_sub] - g_vec[i: i + self.n_sub][0]) for i in range(self.n_sim)]
-            weights = np.round(weights, decimals=5).tolist()
+        if self.verbose is True:
+            w = np.round(weights, decimals=3).tolist()  # just for printing
+            print('  Original weights:')
+            for i in range(len(w)):
+                print(f'    Rep {i}: {w[i]}')
+
+        # Method based on weight differences (the original g-diff)
+        dg_vec = []
+        dg_adjacent = [list(np.diff(weights[i])) for i in range(len(weights))]
+        for i in range(self.n_tot - 1):
+            dg_list = []
+            for j in range(len(self.state_ranges)):
+                if i in self.state_ranges[j] and i + 1 in self.state_ranges[j]:
+                    idx = self.state_ranges[j].index(i)
+                    dg_list.append(dg_adjacent[j][idx])
+            dg_vec.append(np.mean(dg_list))
+        dg_vec.insert(0, 0)
+        g_vec = np.array([sum(dg_vec[:(i + 1)]) for i in range(len(dg_vec))])
+
+        """  Deprecated methods: mean and geo-mean
+        # Method based on probability ratios
+        # Step 1: Convert the weights into probabilities
+        weights = np.array(weights)
+        prob = np.array([[np.exp(-i)/np.sum(np.exp(-weights[j])) for i in weights[j]] for j in range(len(weights))])  # noqa: E501
+
+        # Step 2: Caclulate the probability ratios (after figuring out overlapped states between adjacent replicas)  # noqa: E501
+        overlapped = [set(self.state_ranges[i]).intersection(set(self.state_ranges[i + 1])) for i in range(len(self.state_ranges) - 1)]  # noqa: E501
+        prob_ratio = [prob[i + 1][: len(overlapped[i])] / prob[i][-len(overlapped[i]):] for i in range(len(overlapped))]  # noqa: E501
+
+        # Step 3: Average the probability ratios
+        avg_ratio = [1]   # This allows easier scaling since the first prob vector stays the same.
+        if self.w_scheme == 'mean':
+            avg_ratio.extend([np.mean(prob_ratio[i]) for i in range(len(prob_ratio))])
+        elif self.w_scheme == 'geo-mean':
+            avg_ratio.extend([np.prod(prob_ratio[i])**(1/len(prob_ratio[i])) for i in range(len(prob_ratio))])
+
+        # Step 4: Scale the probabilities for each replica
+        scaled_prob = np.array([prob[i] / np.prod(avg_ratio[: i + 1]) for i in range(len(prob))])
+
+        # Step 5: Average and convert the probabilities
+        p_vec = []
+        for i in range(self.n_tot):   # global state index
+            p = []   # a list of probabilities to be averaged for each state
+            for j in range(len(self.state_ranges)):   # j can be regared as the replica index
+                if i in self.state_ranges[j]:
+                    local_idx = i - j * self.s
+                    p.append(scaled_prob[j][local_idx])
+            if self.w_scheme == 'mean':
+                p_vec.append(np.mean(p))
+            elif self.w_scheme == 'geo-mean' or self.w_scheme == 'geo_mean':
+                p_vec.append(np.prod(p) ** (1 / len(p)))
 
-            if self.verbose is True:
-                w = np.round(weights, decimals=3).tolist()  # just for printing
-                print('\n  Modified weights:')
-                for i in range(len(w)):
-                    print(f'    Rep {i}: {w[i]}')
-
-            if self.verbose is False:
-                print(' DONE')
-                print(f'The alchemical weights of all states: \n  {list(np.round(g_vec, decimals=3))}')
+        g_vec = -np.log(p_vec)
+        g_vec -= g_vec[0]
+        """
+
+        # Determine the vector of alchemical weights for each replica
+        for i in range(self.n_sim):
+            if self.equil[i] == -1:  # unequilibrated
+                weights[i] = list(g_vec[i: i + self.n_sub] - g_vec[i: i + self.n_sub][0])
             else:
-                print(f'\n  The alchemical weights of all states: \n  {list(np.round(g_vec, decimals=3))}')
+                weights[i] = self.equilibrated_weights[i]
+        weights = np.round(weights, decimals=5).tolist()
+
+        if self.verbose is True:
+            w = np.round(weights, decimals=3).tolist()  # just for printing
+            print('\n  Modified weights:')
+            for i in range(len(w)):
+                print(f'    Rep {i}: {w[i]}')
 
-            return weights, g_vec
+        if self.verbose is False:
+            print(' DONE')
+            print(f'The alchemical weights of all states: \n  {list(np.round(g_vec, decimals=3))}')
+        else:
+            print(f'\n  The alchemical weights of all states: \n  {list(np.round(g_vec, decimals=3))}')
+
+        return weights, g_vec
 
-    def run_EEXE(self, n):
+    def run_gmx_cmd(self, arguments):
         """
-        Makes TPR files and runs an ensemble of expanded ensemble simulations
-        using GROMACS.
+        Run a GROMACS command as a subprocess
 
         Parameters
         ----------
-        n : int
-            The iteration index (starting from 0).
+        arguments : list
+            A list of arguments that compose of the GROMACS command to run, e.g.
+            :code:`['gmx', 'mdrun', '-deffnm', 'sys']`.
 
         Returns
         -------
-        md : :code:`gmxapi.commandline.CommandlineOperation` obj
-            The :code:`gmxapi.commandline.CommandlineOperation` object returned by :code:`gmxapi.mdrun`
-            which contains STDOUT and STDERR of the simulation.
-
-        Notes
-        -----
-        This function performs the following steps:
-
-          1. Prepares TPR files for the simulation ensemble using :code:`grompp`.
-          2. Runs all the simulations simultaneously using :code:`mdrun`.
-          3. Removes any empty directories created by the function.
+        return_code : int
+            The exit code of the GROMACS command. Any number other than 0 indicates an error.
+        stdout : str or None
+            The STDOUT of the process.
+        stderr: str or None
+            The STDERR or the process.
 
-        The function assumes that the GROMACS executable is available.
         """
-        if rank == 0:
-            iter_str = f'\nIteration {n}: {self.dt * self.nst_sim * n: .1f} - {self.dt * self.nst_sim * (n + 1): .1f} ps'  # noqa: E501
-            print(iter_str + '\n' + '=' * (len(iter_str) - 1))
+        try:
+            result = subprocess.run(arguments, capture_output=True, text=True, check=True)
+            return_code, stdout, stderr = result.returncode, result.stdout, None
+        except subprocess.CalledProcessError as e:
+            return_code, stdout, stderr = e.returncode, None, e.stderr
 
-        if rank == 0:
-            dir_before = [
-                i for i in os.listdir(".") if os.path.isdir(os.path.join(".", i))]
-            print("Preparing the tpr files for the simulation ensemble ...", end="")
-
-        grompp = gmx.commandline_operation(
-            "gmx",
-            arguments=["grompp"],  # noqa: E127
-            input_files=[  # noqa: E127
-                {
-                    "-f": f"../sim_{i}/iteration_{n}/{self.mdp.split('/')[-1]}",
-                    "-c": f"../sim_{i}/iteration_{n}/{self.gro.split('/')[-1]}",
-                    "-p": f"../sim_{i}/iteration_{n}/{self.top.split('/')[-1]}",
-                }
-                for i in range(self.n_sim)
-            ],
-            output_files=[  # noqa: E127
-                {  # noqa: E127
-                    "-o": f"../sim_{i}/iteration_{n}/sys_EE.tpr",
-                    "-po": f"../sim_{i}/iteration_{n}/mdout.mdp",
-                }
-                for i in range(self.n_sim)
-            ],
-        )
-        grompp.run()
-        if rank == 0:  # just print the messages once
-            utils.gmx_output(grompp)
+        return return_code, stdout, stderr
 
-        # Run all the simulations simultaneously using gmxapi
-        if rank == 0:
-            print("Running an ensemble of simulations ...", end="")
+    def run_grompp(self, n, swap_pattern):
+        """
+        Prepares TPR files for the simulation ensemble using the GROMACS :code:`grompp` command.
 
-        if self.parallel is True:
-            tpr = [f'{grompp.output.file["-o"].result()[i]}' for i in range(self.n_sim)]
-            inputs = gmx.read_tpr(tpr)
-            md = gmx.mdrun(inputs, runtime_args=self.runtime_args)
-            md.run()
-        else:
-            # Note that we could use output_files argument to customize the output file
-            # names but here we'll just use the defaults.
+        Parameters
+        ----------
+        n : int
+            The iteration index (starting from 0).
+        swap_pattern : list
+            A list generated by :code:`get_swapping_pattern`. It represents how the replicas should be swapped.
+        """
+        args_list = []
+        for i in range(self.n_sim):
+            # mpirun -np 1 does not seem needed here.
+            # Actually, it made stderr and stdout both empty even if the return code is 1 ...
+            arguments = [self.gmx_executable, 'grompp']
+
+            # Input files
+            mdp = f"sim_{i}/iteration_{n}/{self.mdp.split('/')[-1]}"
+            if n == 0:
+                gro = f"{self.gro}"
+            else:
+                gro = f"sim_{swap_pattern[i]}/iteration_{n-1}/confout.gro"  # This effectively swap out GRO files
+            top = f"{self.top}"
 
-            arguments = ['mdrun']  # arguments for gmx.commandline_operation
+            # Add input file arguments
+            arguments.extend(["-f", mdp, "-c", gro, "-p", top])
 
-            if self.runtime_args is not None:
+            # Add output file arguments
+            arguments.extend([
+                "-o", f"sim_{i}/iteration_{n}/sys_EE.tpr",
+                "-po", f"sim_{i}/iteration_{n}/mdout.mdp"
+            ])
+
+            # Add additional arguments if any
+            if self.grompp_args is not None:
                 # Turn the dictionary into a list with the keys alternating with values
-                args_keys = list(self.runtime_args.keys())
-                args_vals = list(self.runtime_args.values())
+                add_args = [elem for pair in self.grompp_args.items() for elem in pair]
+                arguments.extend(add_args)
 
-                add_args = []
-                for i in range(len(args_keys)):
-                    add_args.append(args_keys[i])
-                    add_args.append(args_vals[i])
+            args_list.append(arguments)
 
-                arguments.extend(add_args)
+        # Run the GROMACS grompp commands in parallel
+        if rank < self.n_sim:
+            print(f'Generating a TPR file on rank {rank} ...')
+            returncode, stdout, stderr = self.run_gmx_cmd(args_list[rank])
+            if returncode != 0:
+                print(f'Error on rank {rank}:\n{stderr}')
 
-            md = gmx.commandline_operation(
-                "gmx",
-                arguments=arguments,
-                input_files=[  # noqa: E128
-                    {
-                        "-s": grompp.output.file["-o"].result()[i],
-                    }
-                    for i in range(self.n_sim)
-                ],
-            )
-            md.run()
-            if rank == 0:  # just print the messages once
-                utils.gmx_output(md)
+    def run_mdrun(self, n):
+        """
+        Executes GROMACS mdrun commands in parallel.
+
+        Parameters
+        ----------
+        n : int
+            The iteration index (starting from 0).
+        """
+        # We will change the working directory so the mdrun command should be the same for all replicas.
+        arguments = [self.gmx_executable, 'mdrun']
 
+        # Add input file arguments
+        arguments.extend(['-s', 'sys_EE.tpr'])
+
+        if self.runtime_args is not None:
+            # Turn the dictionary into a list with the keys alternating with values
+            add_args = [elem for pair in self.runtime_args.items() for elem in pair]
+            arguments.extend(add_args)
+
+        # Run the GROMACS mdrun commands in parallel
+        if rank < self.n_sim:
+            print(f'Running an EXE simulation on rank {rank} ...')
+            os.chdir(f'sim_{rank}/iteration_{n}')
+            returncode, stdout, stderr = self.run_gmx_cmd(arguments)
+            if returncode != 0:
+                print(f'Error on rank {rank}:\n{stderr}')
+                sys.exit(returncode)
+            os.chdir('../../')
+
+    def run_EEXE(self, n, swap_pattern=None):
+        """
+        Perform one iteration in the EEXE simulation, which includes generating the
+        TPR files using the GROMACS grompp :code:`command` and running the expanded ensemble simulations
+        in parallel using GROMACS :code:`mdrun` command. The GROMACS commands are launched by as subprocesses.
+        The function assumes that the GROMACS executable is available.
+
+        Parameters
+        ----------
+        n : int
+            The iteration index (starting from 0).
+        swap_pattern : list
+            A list generated by :code:`get_swapping_pattern`. It represents how the replicas should be swapped.
+            This parameter is not needed only if :code:`n` is 0.
+        """
         if rank == 0:
-            dir_after = [
-                i for i in os.listdir(".") if os.path.isdir(os.path.join(".", i))
-            ]
-            utils.clean_up(dir_before, dir_after, self.verbose)
+            iter_str = f'\nIteration {n}: {self.dt * self.nst_sim * n: .1f} - {self.dt * self.nst_sim * (n + 1): .1f} ps'  # noqa: E501
+            print(iter_str + '\n' + '=' * (len(iter_str) - 1))
 
-        return md
+        # 1st synchronizing point for all MPI processes: To make sure ranks other than 0 will not start executing
+        # run_grompp earlier and mess up the order of printing.
+        comm.barrier()
+
+        # Generating all required TPR files simultaneously, then run all simulations simultaneously.
+        # No synchronizing point is needed between run_grompp and run_mdrun, since once rank i finishes run_grompp,
+        # it should run run_mdrun in the same working directory, so there won't be any I/O error.
+        self.run_grompp(n, swap_pattern)
+        self.run_mdrun(n)
+
+        # 2nd synchronizaing point for all MPI processes: To make sure no rank will start getting to the next
+        # iteration earlier than the others. For example, if rank 0 finishes the mdrun command earlier, we don't
+        # want it to start parsing the dhdl file (in the if condition of if rank == 0) of simulation 3 being run by
+        # rank 3 that has not been generated, which will lead to an I/O error.
+        comm.barrier()
```

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg` & `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg` & `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg` & `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg` & `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/expanded.mdp` & `ensemble_md-0.6.0/ensemble_md/tests/data/expanded.mdp`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_0.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_0.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_1.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_1.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_2.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_2.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/EXE_3.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_3.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/HREX.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/HREX.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/case2_1.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_1.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/case2_2.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_2.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/log/case3.log` & `ensemble_md-0.6.0/ensemble_md/tests/data/log/case3.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/sys.gro` & `ensemble_md-0.6.0/ensemble_md/tests/data/sys.gro`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/data/sys.top` & `ensemble_md-0.6.0/ensemble_md/tests/data/sys.top`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/test_analyze_matrix.py` & `ensemble_md-0.6.0/ensemble_md/tests/test_analyze_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,29 +86,32 @@
     assert prob is None
     assert 'The input transition matrix is neither right nor left stochastic' in out
 
 
 def test_calc_spectral_gap(capfd):
     # Case 1 (sanity check): doublly stochastic
     mtx = np.array([[0.5, 0.5], [0.5, 0.5]])
-    s = analyze_matrix.calc_spectral_gap(mtx)
+    s, vals = analyze_matrix.calc_spectral_gap(mtx)
+    assert vals[0] == 1
     assert np.isclose(s, 1)
 
     # Case 2: Right stochastic
     mtx = np.array([[0.8, 0.2], [0.3, 0.7]])
-    s = analyze_matrix.calc_spectral_gap(mtx)
+    s, vals = analyze_matrix.calc_spectral_gap(mtx)
+    assert vals[0] == 1
     assert s == 0.5
 
     # Case 3: Left stochastic
-    s = analyze_matrix.calc_spectral_gap(mtx.T)
+    s, vals = analyze_matrix.calc_spectral_gap(mtx.T)
+    assert vals[0] == 1
     assert s == 0.5
 
     # Case 4: Neither left or right stochastic
     mtx = np.random.rand(3, 3)
-    s = analyze_matrix.calc_spectral_gap(mtx)
+    s = analyze_matrix.calc_spectral_gap(mtx)  # the output should be None
     out, err = capfd.readouterr()
     assert s is None
     assert 'The input transition matrix is neither right nor left stochastic' in out
 
 
 def test_split_transmtx():
     mtx = np.array([[0.6, 0.3, 0.1], [0.1, 0.7, 0.2], [0.2, 0.1, 0.7]])
```

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/test_analyze_traj.py` & `ensemble_md-0.6.0/ensemble_md/tests/test_analyze_traj.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/test_ensemble_EXE.py` & `ensemble_md-0.6.0/ensemble_md/tests/test_ensemble_EXE.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,35 +11,32 @@
 Unit tests for the module ensemble_EXE.py.
 """
 import os
 import sys
 import yaml
 import copy
 import random
-import shutil
 import pytest
 import numpy as np
 import ensemble_md
-import gmxapi as gmx
-from mpi4py import MPI
 from ensemble_md.utils import gmx_parser
 from ensemble_md.ensemble_EXE import EnsembleEXE
 from ensemble_md.utils.exceptions import ParameterError
 
 current_path = os.path.dirname(os.path.abspath(__file__))
 input_path = os.path.join(current_path, "data")
 
 
 @pytest.fixture
 def params_dict():
     """
     Generates a dictionary containing the required EEXE parameters.
     """
     EEXE_dict = {
-        'parallel': False,
+        'gmx_executable': 'gmx',
         'gro': 'ensemble_md/tests/data/sys.gro',
         'top': 'ensemble_md/tests/data/sys.top',
         'mdp': 'ensemble_md/tests/data/expanded.mdp',
         'n_sim': 4,
         'n_iter': 10,
         's': 1,
     }
@@ -75,23 +72,22 @@
 class Test_EnsembleEXE:
     def test_init(self, params_dict):
         EEXE = get_EEXE_instance(params_dict)
         assert EEXE.yaml == 'params.yaml'
 
     def test_set_params_error(self, params_dict):
         # 1. Required parameters
-        del params_dict['parallel']
-        with pytest.raises(ParameterError, match="Required parameter 'parallel' not specified in params.yaml."):
+        del params_dict['n_sim']
+        with pytest.raises(ParameterError, match="Required parameter 'n_sim' not specified in params.yaml."):
             get_EEXE_instance(params_dict)
-        params_dict['parallel'] = False  # so params_dict can be read without failing in the assertions below
+        params_dict['n_sim'] = 4  # so params_dict can be read without failing in the assertions below
 
         # 2. Available options
         check_param_error(params_dict, 'proposal', "The specified proposal scheme is not available. Available options include 'single', 'neighboring', 'exhaustive', and 'multiple'.", 'cool', 'multiple')  # set as multiple for later tests for n_ex # noqa: E501
         check_param_error(params_dict, 'acceptance', "The specified acceptance scheme is not available. Available options include 'same-state', 'metropolis', and 'metropolis-eq'.")  # noqa: E501
-        check_param_error(params_dict, 'w_scheme', "The specified weight combining scheme is not available. Available options include None, 'mean', 'geo-mean'/'geo_mean' and 'g-diff/g_diff'.")  # noqa: E501
         check_param_error(params_dict, 'df_method', "The specified free energy estimator is not available. Available options include 'TI', 'BAR', and 'MBAR'.")  # noqa: E501
         check_param_error(params_dict, 'err_method', "The specified method for error estimation is not available. Available options include 'propagate', and 'bootstrap'.")  # noqa: E501
 
         # 3. Integer parameters
         check_param_error(params_dict, 'nst_sim', "The parameter 'nst_sim' should be an integer.")
         check_param_error(params_dict, 'n_ex', "The parameter 'n_ex' should be an integer.")
         check_param_error(params_dict, 'seed', "The parameter 'seed' should be an integer.")
@@ -105,15 +101,15 @@
         check_param_error(params_dict, 'n_ex', "The parameter 'n_ex' should be non-negative.", -1)
         check_param_error(params_dict, 'N_cutoff', "The parameter 'N_cutoff' should be non-negative unless no histogram correction is needed, i.e. N_cutoff = -1.", -5)  # noqa: E501
 
         # 6. String parameters
         check_param_error(params_dict, 'mdp', "The parameter 'mdp' should be a string.", 3, 'ensemble_md/tests/data/expanded.mdp')  # noqa: E501
 
         # 7. Boolean parameters
-        check_param_error(params_dict, 'parallel', "The parameter 'parallel' should be a boolean variable.", 3, False)
+        check_param_error(params_dict, 'msm', "The parameter 'msm' should be a boolean variable.", 3, False)
 
         # 8. nstlog > nst_sim
         mdp = gmx_parser.MDP(os.path.join(input_path, "expanded.mdp"))  # A perfect mdp file
         mdp['nstlog'] = 200
         mdp.write(os.path.join(input_path, "expanded_test.mdp"))
         params_dict['mdp'] = 'ensemble_md/tests/data/expanded_test.mdp'
         params_dict['nst_sim'] = 100
@@ -138,43 +134,49 @@
         assert warning in EEXE.warnings
 
         # 2. Warnings related to the mdp file
         mdp = gmx_parser.MDP(os.path.join(input_path, "expanded.mdp"))  # A perfect mdp file
         mdp['lmc_seed'] = 1000
         mdp['gen_seed'] = 1000
         mdp['symmetrized_transition_matrix'] = 'yes'
+        mdp['wl_scale'] = ''
         mdp.write(os.path.join(input_path, "expanded_test.mdp"))
+
         params_dict['mdp'] = 'ensemble_md/tests/data/expanded_test.mdp'
+        params_dict['N_cutoff'] = 1000
         EEXE = get_EEXE_instance(params_dict)
-        warning_1 = 'Warning: We recommend setting lmc_seed as -1 so the random seed is different for each iteration.'
-        warning_2 = 'Warning: We recommend setting gen_seed as -1 so the random seed is different for each iteration.'
-        warning_3 = 'Warning: We recommend setting symmetrized-transition-matrix to no instead of yes.'
+
+        warning_1 = 'Warning: The histogram correction/weight combination method is specified but will not be used since the weights are fixed.'  # noqa: E501
+        warning_2 = 'Warning: We recommend setting lmc_seed as -1 so the random seed is different for each iteration.'
+        warning_3 = 'Warning: We recommend setting gen_seed as -1 so the random seed is different for each iteration.'
+        warning_4 = 'Warning: We recommend setting symmetrized-transition-matrix to no instead of yes.'
         assert warning_1 in EEXE.warnings
         assert warning_2 in EEXE.warnings
         assert warning_3 in EEXE.warnings
+        assert warning_4 in EEXE.warnings
 
         os.remove(os.path.join(input_path, "expanded_test.mdp"))
 
     def test_set_params(self, params_dict):
         # 0. Get an EEXE instance to test
         EEXE = get_EEXE_instance(params_dict)
 
         # 1. Check the required EEXE parameters
+        assert EEXE.gmx_executable == 'gmx'
         assert EEXE.gro == "ensemble_md/tests/data/sys.gro"
         assert EEXE.top == "ensemble_md/tests/data/sys.top"
         assert EEXE.mdp == "ensemble_md/tests/data/expanded.mdp"
-        assert EEXE.parallel is False
         assert EEXE.n_sim == 4
         assert EEXE.n_iter == 10
         assert EEXE.s == 1
 
         # 2. Check the default values of the parameters not specified in params.yaml
         assert EEXE.proposal == "exhaustive"
         assert EEXE.acceptance == "metropolis"
-        assert EEXE.w_scheme is None
+        assert EEXE.w_combine is False
         assert EEXE.N_cutoff == 1000
         assert EEXE.n_ex == 'N^3'
         assert EEXE.verbose is True
         assert EEXE.runtime_args is None
         assert EEXE.n_ckpt == 100
         assert EEXE.msm is False
         assert EEXE.free_energy is False
@@ -203,29 +205,32 @@
             [0, 1, 2, 3, 4, 5],
             [1, 2, 3, 4, 5, 6],
             [2, 3, 4, 5, 6, 7],
             [3, 4, 5, 6, 7, 8], ]
         assert EEXE.equil == [-1, -1, -1, -1]  # will be zeros right after the first iteration if the weights are fixed
         assert EEXE.n_rejected == 0
         assert EEXE.n_swap_attempts == 0
+        assert EEXE.n_empty_swappable == 0
         assert EEXE.rep_trajs == [[0], [1], [2], [3]]
 
         params_dict['df_method'] = 'MBAR'
         EEXE = get_EEXE_instance(params_dict)
         assert EEXE.get_u_nk is True
         assert EEXE.get_dHdl is False
 
         params_dict['df_method'] = 'BAR'
         EEXE = get_EEXE_instance(params_dict)
         assert EEXE.get_u_nk is False
         assert EEXE.get_dHdl is True
 
-        params_dict['runtime_args'] = {'-nt': 16, 'ntomp': 8}
+        params_dict['grompp_args'] = {'-maxwarn': 1}
+        params_dict['runtime_args'] = {'-nt': 16, '-ntomp': 8}
         EEXE = get_EEXE_instance(params_dict)
-        assert EEXE.runtime_args == {'-nt': 16, 'ntomp': 8}
+        assert EEXE.runtime_args == {'-nt': 16, '-ntomp': 8}
+        assert EEXE.grompp_args == {'-maxwarn': 1}
 
         assert EEXE.reformatted_mdp is False
 
     def test_set_params_edge_cases(self, params_dict):
         # In the previous unit tests, we have tested the case where fixed_weights is False. Here we test the others.
         mdp = gmx_parser.MDP(os.path.join(input_path, "expanded.mdp"))
 
@@ -315,23 +320,28 @@
     def test_print_params(self, capfd, params_dict):
         # capfd is a fixture in pytest for testing STDOUT
         EEXE = get_EEXE_instance(params_dict)
         EEXE.print_params()
         out_1, err = capfd.readouterr()
         L = ""
         L += "Important parameters of EXEE\n============================\n"
-        L += f"Python version: {sys.version}\ngmxapi version: {gmx.__version__}\nensemble_md version: {ensemble_md.__version__}\n"  # noqa: E501
+        L += f"Python version: {sys.version}\n"
+        L += f"GROMACS executable: {EEXE.gmx_path}\n"  # Easier to pass CI. This is easy to catch anyway
+        L += f"GROMACS version: {EEXE.gmx_version}\n"  # Easier to pass CI. This is easy to catch anyway
+        L += f"ensemble_md version: {ensemble_md.__version__}\n"
         L += "Simulation inputs: ensemble_md/tests/data/sys.gro, ensemble_md/tests/data/sys.top, ensemble_md/tests/data/expanded.mdp\n"  # noqa: E501
-        L += "Verbose log file: True\nWhether the replicas run in parallel: False\n"
+        L += "Verbose log file: True\n"
         L += "Proposal scheme: exhaustive\n"
-        L += "Acceptance scheme for swapping simulations: metropolis\nScheme for combining weights: None\n"
+        L += "Acceptance scheme for swapping simulations: metropolis\n"
+        L += "Whether to perform weight combination: False\n"
         L += "Histogram cutoff: 1000\nNumber of replicas: 4\nNumber of iterations: 10\n"
         L += "Number of attempted swaps in one exchange interval: N^3\n"
         L += "Length of each replica: 1.0 ps\nFrequency for checkpointing: 100 iterations\n"
         L += "Total number of states: 9\n"
+        L += "Additional grompp arguments: None\n"
         L += "Additional runtime arguments: None\n"
         L += "Alchemical ranges of each replica in EEXE:\n  - Replica 0: States [0, 1, 2, 3, 4, 5]\n"
         L += "  - Replica 1: States [1, 2, 3, 4, 5, 6]\n  - Replica 2: States [2, 3, 4, 5, 6, 7]\n"
         L += "  - Replica 3: States [3, 4, 5, 6, 7, 8]\n"
         assert out_1 == L
 
         EEXE.reformatted_mdp = True  # Just to test the case where EEXE.reformatted_mdp is True
@@ -420,30 +430,37 @@
         ]
         states = EEXE.extract_final_dhdl_info(dhdl_files)
         assert states == [5, 2, 2, 8]
 
     def test_extract_final_log_info(self, params_dict):
         EEXE = get_EEXE_instance(params_dict)
         log_files = [
-            os.path.join(input_path, f"log/EXE_{i}.log") for i in range(EEXE.n_sim)
-        ]
+            os.path.join(input_path, f"log/EXE_{i}.log") for i in range(EEXE.n_sim)]
         wl_delta, weights, counts = EEXE.extract_final_log_info(log_files)
         assert wl_delta == [0.4, 0.5, 0.5, 0.5]
         assert np.allclose(weights, [
             [0, 1.03101, 2.55736, 3.63808, 4.47220, 6.13408],
             [0, 1.22635, 2.30707, 2.44120, 4.10308, 6.03106],
             [0, 0.66431, 1.25475, 0.24443, 0.59472, 0.70726],
             [0, 0.09620, 1.59937, -4.31679, -22.89436, -28.08701], ])
         assert counts == [
             [4, 11, 9, 9, 11, 6],
             [9, 8, 8, 11, 7, 7],
             [3, 1, 1, 9, 15, 21],
             [0, 0, 0, 1, 18, 31], ]
         assert EEXE.equil == [-1, -1, -1, -1]
 
+    def test_get_averaged_weights(self, params_dict):
+        EEXE = get_EEXE_instance(params_dict)
+        log_files = [
+            os.path.join(input_path, f"log/EXE_{i}.log") for i in range(EEXE.n_sim)]
+        avg, err = EEXE.get_averaged_weights(log_files)
+        assert np.allclose(avg[0],  [0, 2.55101, 3.35736, 4.83808, 4.8722, 5.89408])
+        assert np.allclose(err[0], [0, 1.14542569, 1.0198039, 0.8, 0.69282032, 0.35777088])
+
     def test_identify_swappable_pairs(self, params_dict):
         EEXE = get_EEXE_instance(params_dict)
         EEXE.state_ranges = [list(range(i, i + 5)) for i in range(EEXE.n_sim)]  # 5 states per replica
         states = [4, 2, 2, 7]   # This would lead to the swappables: [(0, 1), (0, 2), (1, 2)] in the standard case
 
         # Case 1: Any case that is not neighboring swap has the same definition for the swappable pairs
         swappables_1 = EEXE.identify_swappable_pairs(states, EEXE.state_ranges)
@@ -474,16 +491,17 @@
 
         # Case 1: Empty swap list
         EEXE = get_EEXE_instance(params_dict)
         EEXE.verbose = False
         states = [0, 6, 7, 8]  # No swappable pairs
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
         pattern_1 = EEXE.get_swapping_pattern(f, states, w)
-        assert EEXE.n_swap_attempts == 1
-        assert EEXE.n_rejected == 1
+        assert EEXE.n_empty_swappable == 1
+        assert EEXE.n_swap_attempts == 0
+        assert EEXE.n_rejected == 0
         assert pattern_1 == [0, 1, 2, 3]
 
         # Case 2: Single swap (proposal = 'single')
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         EEXE.verbose = True
         EEXE.proposal = 'single'  # n_ex will be set to 1 automatically.
@@ -613,35 +631,31 @@
         assert EEXE.n_rejected == 2
         assert swap_bool_1 is False
         assert swap_bool_2 is False
         assert swap_bool_3 is True
 
     def test_historgam_correction(self, params_dict):
         EEXE = get_EEXE_instance(params_dict)
-        # Case 1: No histogram correction
-        EEXE.N_cutoff = -1
-        weights_1 = [[0, 10.304, 20.073, 29.364]]
-        counts_1 = [[31415, 45701, 55457, 59557]]
-        weights_1 = EEXE.histogram_correction(weights_1, counts_1)
-        assert weights_1 == [[0, 10.304, 20.073, 29.364]]
 
-        # Case 2: Perform histogram correction (N_cutoff reached)
+        # Case 1: Perform histogram correction (N_cutoff reached)
         EEXE.N_cutoff = 5000
         EEXE.verbose = False  # just to increase code coverage
+        weights_1 = [[0, 10.304, 20.073, 29.364]]
+        counts_1 = [[31415, 45701, 55457, 59557]]
         weights_1 = EEXE.histogram_correction(weights_1, counts_1)
         assert np.allclose(weights_1, [
             [
                 0,
                 10.304 + np.log(31415 / 45701),
                 20.073 + np.log(45701 / 55457),
                 29.364 + np.log(55457 / 59557),
             ]
         ])  # noqa: E501
 
-        # Case 3: Perform histogram correction (N_cutoff not reached by both N_k and N_{k-1})
+        # Case 2: Perform histogram correction (N_cutoff not reached by both N_k and N_{k-1})
         EEXE.verbose = True
         weights_2 = [[0, 10.304, 20.073, 29.364]]
         counts_2 = [[3141, 4570, 5545, 5955]]
         weights_2 = EEXE.histogram_correction(weights_2, counts_2)
         assert np.allclose(weights_2, [[0, 10.304, 20.073, 29.364 + np.log(5545 / 5955)]])
 
     def test_combine_weights(self, params_dict):
@@ -649,58 +663,14 @@
         EEXE.n_tot = 6
         EEXE.n_sub = 4
         EEXE.s = 1
         EEXE.n_sim = 3
         EEXE.state_ranges = [[0, 1, 2, 3], [1, 2, 3, 4], [2, 3, 4, 5]]
         weights = [[0, 2.1, 4.0, 3.7], [0, 1.7, 1.2, 2.6], [0, -0.4, 0.9, 1.9]]
 
-        # Method: None
-        w1, g_vec_1 = EEXE.combine_weights(weights, method=None)
-        assert np.allclose(w1, weights)
-        assert g_vec_1 is None
-
-        # Method: mean
-        EEXE.verbose = False  # just to increase code coverage
-        w2, g_vec_2 = EEXE.combine_weights(weights, method='mean')
-        assert np.allclose(w2, [
-            [0.0, 2.20097, 3.99803, 3.59516],
-            [0.0, 1.79706, 1.39419, 2.69607],
-            [0.0, -0.40286, 0.89901, 1.88303]])
-        assert np.allclose(list(g_vec_2), [0.0, 2.200968785917372, 3.9980269151210854, 3.5951633659351256, 4.897041830662871, 5.881054277773005])  # noqa: E501
-
-        # Method: geo-mean
-        EEXE.verbose = True
-        w3, g_vec_3 = EEXE.combine_weights(weights, method='geo-mean')
-        assert np.allclose(w3, [
-            [0.0, 2.2, 3.98889, 3.58889],
-            [0.0, 1.78889, 1.38889, 2.68333],
-            [0.0, -0.4, 0.89444, 1.87778]])
-        assert np.allclose(list(g_vec_3), [0.0, 2.1999999999999997, 3.9888888888888885, 3.5888888888888886, 4.883333333333334, 5.866666666666667])  # noqa: E501
-
-        # Method: g-diff
-        w4, g_vec_4 = EEXE.combine_weights(weights, method='g-diff')
-        assert np.allclose(w4, [
+        EEXE.w_combine = True
+        w, g_vec = EEXE.combine_weights(weights)
+        assert np.allclose(w, [
             [0, 2.1, 3.9, 3.5],
             [0, 1.8, 1.4, 2.75],
             [0, -0.4, 0.95, 1.95]])
-        assert np.allclose(list(g_vec_4), [0, 2.1, 3.9, 3.5, 4.85, 5.85])
-
-    def test_run_EEXE(self, params_dict):
-        # We probably can only test serial EEXE
-        rank = MPI.COMM_WORLD.Get_rank()
-        params_dict['runtime_args'] = {'-nt': 1}
-        EEXE = get_EEXE_instance(params_dict)
-        if rank == 0:
-            for i in range(EEXE.n_sim):
-                os.mkdir(f'sim_{i}')
-                os.mkdir(f'sim_{i}/iteration_0')
-                MDP = EEXE.initialize_MDP(i)
-                MDP.write(f'sim_{i}/iteration_0/expanded.mdp', skipempty=True)
-                shutil.copy('ensemble_md/tests/data/sys.gro', f'sim_{i}/iteration_0/sys.gro')
-                shutil.copy('ensemble_md/tests/data/sys.top', f'sim_{i}/iteration_0/sys.top')
-
-        md = EEXE.run_EEXE(0)   # just test the first iteration is fine
-        assert md.output.returncode.result() == [0, 0, 0, 0]
-
-        if rank == 0:
-            os.system('rm -r sim_*')
-            os.system('rm -r gmxapi.commandline.cli*_i0*')
+        assert np.allclose(list(g_vec), [0, 2.1, 3.9, 3.5, 4.85, 5.85])
```

### Comparing `ensemble_md-0.5.0/ensemble_md/tests/test_gmx_parser.py` & `ensemble_md-0.6.0/ensemble_md/tests/test_gmx_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,43 +20,55 @@
 
 current_path = os.path.dirname(os.path.abspath(__file__))
 input_path = os.path.join(current_path, "data")
 
 
 def test_parse_log():
     """
-    Case 1 has been indirectly tesed in the test for extract_final_log_info.
-    So we only need to test the following two cases.
+      - Case 1: The weights have never been equilibrated.
       - Case 2: The weights were equilibrated during the simulation.
       - Case 3: The weights were fixed in the simulation.
     """
-    # Now let's test Case 2
+    # Case 1: weight-updating simulation
+    weights_0, counts_0, wl_delta_0, equil_time_0 = gmx_parser.parse_log(os.path.join(input_path, 'log/EXE_0.log'))
+    assert len(weights_0) == 5
+    assert weights_0[0] == [0.0, 3.83101, 4.95736, 5.63808, 6.0722, 6.13408]
+    assert weights_0[-1] == [0.00000, 1.03101, 2.55736, 3.63808, 4.47220, 6.13408]
+    assert counts_0 == [4, 11, 9, 9, 11, 6]
+    assert wl_delta_0 == 0.4
+    assert np.isclose(equil_time_0, -1)
+
     # Case 2-1: equil_time < 1000 ps
     # As a note, here we used a very lenient weight-equil-wl-delta as 0.3, with nst_sim = 2000.
     # The log file was from sim_0/iteration_1.
-    wl_delta_1, weights_1, counts_1, equil_time_1 = gmx_parser.parse_log(os.path.join(input_path, 'log/case2_1.log'))
-    assert wl_delta_1 == 0.32
-    assert weights_1 == [0.00000, 1.40453, 2.85258, 2.72480, 3.46220, 5.88607]
+    weights_1, counts_1, wl_delta_1, equil_time_1 = gmx_parser.parse_log(os.path.join(input_path, 'log/case2_1.log'))
+    assert len(weights_1) == 6
+    assert weights_1[0] == [0.0, 2.68453, 4.13258, 4.3248, 4.4222, 6.52607]
+    assert weights_1[-1] == [0.00000, 1.40453, 2.85258, 2.72480, 3.46220, 5.88607]
     assert counts_1 == [11, 13, 15, 4, 4, 50]
+    assert wl_delta_1 is None
     assert np.isclose(equil_time_1, 6.06)
 
-    # Case 2-2: equil_time > 1000 ps
+    # Case 2-2: equil_time > 1000 ps (just another case, nothing special here ...)
     # As a note, here we used weight-equil-wl-delta as 0.3, with nst_sim = 2000,  n_iterations = 1000, n_sim = 2,
     # s = 4, wl-scale = 0.9, and wl-ratio = 0.9. The log file was from sim_0/iteration_475 (t=1.9 ns).
-    wl_delta_2, weights_2, counts_2, equil_time_2 = gmx_parser.parse_log(os.path.join(input_path, 'log/case2_2.log'))
-    assert wl_delta_2 == 0.00099828
-    assert weights_2 == [0.00000, 1.60419, 2.47705, 3.14963, 3.47840]
+    weights_2, counts_2, wl_delta_2, equil_time_2 = gmx_parser.parse_log(os.path.join(input_path, 'log/case2_2.log'))
+    assert len(weights_2) == 19
+    assert weights_2[0] == [0.00000, 1.60863, 2.47927, 3.15184, 3.47507]
+    assert weights_2[-1] == [0.00000, 1.60419, 2.47705, 3.14963, 3.47840]
     assert counts_2 == [2, 3, 1, 2, 1]
+    assert wl_delta_2 is None
     assert equil_time_2 == 1903.82
 
-    # Here we test Case 3
-    wl_delta_3, weights_3, counts_3, equil_time_3 = gmx_parser.parse_log(os.path.join(input_path, 'log/case3.log'))
-    assert wl_delta_3 is None
-    assert weights_3 == [0.00000, 1.55165, 2.55043, 3.15034, 3.26889, 4.37831, 5.28574, 3.29638, 2.22527]
+    # Case 3: fixed-weight simulation
+    weights_3, counts_3, wl_delta_3, equil_time_3 = gmx_parser.parse_log(os.path.join(input_path, 'log/case3.log'))
+    assert len(weights_3) == 1
+    assert weights_3[-1] == [0.00000, 1.55165, 2.55043, 3.15034, 3.26889, 4.37831, 5.28574, 3.29638, 2.22527]
     assert counts_3 == [12, 9, 10, 9, 4, 5, 1, 0, 0]
+    assert wl_delta_3 is None
     assert equil_time_3 == 0
 
 
 def test_filename():
     MDP = gmx_parser.MDP()
     with pytest.raises(ValueError, match="A file name is required because no default file name was defined."):
         MDP.filename()
```

### Comparing `ensemble_md-0.5.0/ensemble_md/utils/exceptions.py` & `ensemble_md-0.6.0/ensemble_md/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.5.0/ensemble_md/utils/gmx_parser.py` & `ensemble_md-0.6.0/ensemble_md/utils/gmx_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,123 +20,154 @@
 from ensemble_md.utils import utils
 from ensemble_md.utils.exceptions import ParseError
 
 
 def parse_log(log_file):
     """
     This function parses a log file generated by expanded ensemble and provides
-    important information especially for running new iterations in EEXE.
+    important information, especially for running new iterations in EEXE.
     Typically, there are three types of log files from an expanded ensemble simulation:
 
-    - Case 1: The weights are equilibrating in the simulation and the equilibration was not done.
-      - :code:`equil_time` should always be -1.
-    - Case 2: The weights were equilibrated during the simulation.
-      - :code:`equil_time` should be the time (ps) that the weights get equilibrated.
-      - The final weights will just be the equilibrated weights.
-    - Case 3: The weights were fixed in the simulation.
-      - :code:`equil_time` should always be 0.
-      - We can still find the final weights (not changed though) and the final counts.
+    - **Case 1**: The weights are still updating in the simulation and have never been equilibrated.
+
+        - The output :code:`equil_time` should always be -1.
+
+    - **Case 2**: The weights were equilibrated during the simulation.
+
+        - The output :code:`equil_time` should be the time (in ps) it took to get the weights equilibrated.
+        - The final weights (:code:`weights`) will just be the equilibrated weights.
+
+    - **Case 3**: The weights were fixed in the simulation.
+
+        - The output :code:`equil_time` should always be 0.
+        - The final weights (which never change during the simulation) and the final counts will
+          still be returned.
 
     Parameters
     ----------
     log_file : str
         The log file to be parsed.
 
     Returns
     -------
-    wl_delta : float
-        The final Wang-Landau incementor
     weights : list
-        The final list of lambda weights.
+        In all cases, :code:`weights` should be a list of lists (of weights).
+
+        - In Case 1, a list of list of weights as a function of time since the last update of the Wang-Landau
+          incrementor will be returned.
+        - In Case 2, a list of list of weights as a function of time since the last update of the Wang-Landau
+          incrementor up to equilibration will be returned.
+        - In Case 3, the returned list will only have one list inside, which is the list of the final weights.
+
+        That is, for all cases, :code:`weights[-1]` will be the final weights, which are useful in EEXE.
     counts : list
         The final histogram counts.
+    wl_delta : float
+        The final Wang-Landau incementor. In Cases 2 and 3, :code:`None` will be returned.
     equil_time : int or float
-        The time in ps that the weights get equilibrated.
-        -1 means that the weights have not been equilibrated (Case 1).
-        0 means that the weights were fixed during the simulation (Case 3).
+        - In Case 1, -1 will be returned, which means that the weights have not been equilibrated.
+        - In Case 2, the time in ps that it took to equilibrate the weights will be returned.
+        - In Case 3, 0 will be returned, which means that the weights were fixed during the simulation.
     """
     f = open(log_file, "r")
     lines = f.readlines()
     f.close()
 
-    wl_delta_found, weights_found = False, False
-    weights, counts = [], []
-    case_1_3, equil_time_found = False, False
+    case = None  # itialized as None and should end up as 1 or 2 or 3.
 
+    # First parse the MD parameters to tell the type of the simulation.
     for l in lines:  # noqa: E741
         if "n-lambdas" in l:
             N_states = int(l.split("=")[1])
         if "tinit" in l:
             tinit = float(l.split("=")[1])
+        if "weight-equil-wl-delta" in l:
+            # For Case 1 and Case 2
+            cutoff = float(l.split("=")[1])
         if "lmc-stats" in l:
-            if l.split("=")[1].split()[0] in ["no", "No"]:
-                # Case 3: The weights are fixed. -> Typically weights have been equilibrated in the previous iteration.
-                fixed_bool = True
+            if l.split("=")[1].split()[0] in ["no", "No"]:  # Case 3
+                case = '3'
                 equil_time = 0
                 wl_delta = None
-                wl_delta_found = True
-                case_1_3 = True
             else:
-                # Either Case 1 or Case 2
-                fixed_bool = False
-                equil_time = -1
+                pass  # Either Case 1 or Case 2
         if "dt  " in l:
             dt = float(l.split("=")[1])
 
-    lines.reverse()  # We find the information from the end
-    n = -1
-    for l in lines:  # noqa: E741
-        n += 1
-        if wl_delta_found is False:  # Case 1 or Case 2
-            if "Wang-Landau incrementor is" in l:
-                wl_delta_found = True
-                wl_delta = float(l.split(":")[1])
-
-        if weights_found is False:
+    # For all cases, we need to find weights and counts
+    weights = []
+    if case == '3':  # could be either '3' or None
+        # We only need the info at the end of the simulation, so it's faster to search from the bottom of the file.
+        lines.reverse()
+        n = -1
+        counts = []
+        for l in lines:  # noqa: E741
+            n += 1
             if "Count   G(in kT)" in l:
-                weights_found = True  # The first occurrence would be the final weights. (We've reversed the lines!)
+                w = []  # the list of weights at this time frame
+                # The first occurrence would be the final weights. (We've reversed the lines!)
                 for i in range(1, N_states + 1):
                     if "<<" in lines[n - i]:
-                        weights.append(float(lines[n - i].split()[-3]))
+                        w.append(float(lines[n - i].split()[-3]))
                         counts.append(int(lines[n - i].split()[-4]))
                     else:
-                        weights.append(float(lines[n - i].split()[-2]))
+                        w.append(float(lines[n - i].split()[-2]))
                         counts.append(int(lines[n - i].split()[-3]))
-                if "Wang-Landau incrementor is" in lines[n + 1]:  # Caes 1
+                weights.append(w)
+                break
+    else:  # Case 1 and Case 2
+        # Here we search from the top, since we need weights as a function of time anyway.
+        n = -1
+        find_equil, append_equil = False, False
+        wl_delta_list = [None]  # We use None so that the change in wl-delta will always get deteced at the beginning
+        for l in lines:  # noqa: E741
+            n += 1
+            if "Count   G(in kT)" in l:  # this line is lines[n]
+                # We should first check if wl_delta is changed, set weights=[] if needed before we append new weights
+                if "Wang-Landau incrementor is" in lines[n - 1]:  # Case 1 so far: wl_delta is still updating
+                    case = '1'
                     equil_time = -1
-                    wl_delta_found = True
-                    wl_delta = float(lines[n + 1].split(":")[1])
-                    case_1_3 = True
-                else:
-                    # This would include Case 2 and 3
-                    if fixed_bool is True:
-                        case_1_3 = True
+                    current_wl_delta = float(lines[n - 1].split(":")[1])
+                    if wl_delta_list[-1] != current_wl_delta and current_wl_delta > cutoff:  # when wl-delta changes
+                        # Note that if the time step the equilibration is reached happens to be a multiple of nstlog,
+                        # a wl-delta right below the cutoff will be printed. In that case, we don't want to reset
+                        # `weights` so we get the time series since the last time when we still have wl_delta > cutoff
+                        weights = []  # we want only time series since the latest update of wl_delta
+                    wl_delta_list.append(float(lines[n - 1].split(":")[1]))
+
+                w, counts = [], []  # the list of weights at this time frame
+                for i in range(1, N_states + 1):
+                    # counts will be constantly updated by new values
+                    if "<<" in lines[n + i]:
+                        w.append(float(lines[n + i].split()[-3]))
+                        counts.append(int(lines[n + i].split()[-4]))
                     else:
-                        case_1_3 = False
+                        w.append(float(lines[n + i].split()[-2]))
+                        counts.append(int(lines[n + i].split()[-3]))
+
+                if find_equil is False or append_equil is False:
+                    weights.append(w)
+                    if find_equil is True:
+                        append_equil = True
 
-        if case_1_3 is False:  # for finding when the weights were equilibrated in Case 2
             if "Weights have equilibrated" in l:
-                equil_time_found = True
+                case = '2'  # we don't break the loop even if equil_time is found, as we need the final counts.
+                find_equil = True  # After this, we will append weights one last time, which are equilibrated weights.
                 equil_step = int(l.split(":")[0].split("Step")[1])
                 equil_time = equil_step * dt + tinit  # ps
+                if wl_delta < cutoff:
+                    # Should only happen when equil_time % nstlog == 0, where the weights should have been appended
+                    append_equil = True
+
+            wl_delta = wl_delta_list[-1]
 
-        # For Case 1 and Case 3 (case_1_3 = True), we can break the loop after getting weights, counts, and wl_delta.
-        if case_1_3 is True and weights_found is True and wl_delta_found is True:
-            break
-
-        # For Case 2, we can break the loop only if equil_time is found as well.
-        if (
-            case_1_3 is False
-            and weights_found is True
-            and wl_delta_found is True
-            and equil_time_found is True
-        ):
-            break
+        if case == '2':
+            wl_delta = None
 
-    return wl_delta, weights, counts, equil_time
+    return weights, counts, wl_delta, equil_time
 
 
 class FileUtils(object):
     """Mixin class to provide additional file-related capabilities.
     Modified from `utilities.py in GromacsWrapper <https://github.com/Becksteinlab/GromacsWrapper>`_.
     Copyright (c) 2009 Oliver Beckstein <orbeckst@gmail.com>
     """
```

### Comparing `ensemble_md-0.5.0/ensemble_md/utils/utils.py` & `ensemble_md-0.6.0/ensemble_md/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 #    Written by Wei-Tse Hsu <wehs7661@colorado.edu>                #
 #    Copyright (c) 2022 University of Colorado Boulder             #
 #                                                                  #
 ####################################################################
 """
 The :obj:`.utils` module provides useful utility functions.
 """
-import os
 import sys
+import glob
 import natsort
 import datetime
+import collections
 import numpy as np
 
 
 class Logger:
     """
     Redirects the STDOUT and STDERR to a specified output file while preserving them on screen.
 
@@ -63,68 +64,14 @@
         This method is needed for Python 3 compatibility. This handles the flush command by doing nothing.
         You might want to specify some extra behavior here.
         """
         # self.terminal.log()
         pass
 
 
-def gmx_output(gmx_obj):
-    """
-    Tells if a command launched by ``gmxapi.commandline_operation`` failed or not.
-    If the command failed, the function will print out STDOUT and STDERR of the process.
-
-    Parameters
-    ----------
-    gmx_obj : obj
-        An object generated by gmx.commandline_operation.
-    """
-    try:
-        rtn_code = gmx_obj.output.returncode.result()
-        if type(rtn_code) == list:  # simulation ensemble
-            if sum(rtn_code) == 0:
-                print(" DONE")
-            else:
-                print(f" Return codes: {rtn_code}")
-                for i in range(len(rtn_code)):
-                    if rtn_code[i] != 0:
-                        print(f"\nSTDERR of the process:\n\n {gmx_obj.output.stderr.result()[i]}\n")
-        else:  # single simulation
-            if rtn_code == 0:
-                print(" DONE")
-            else:
-                print(f"\nSTDERR of the process:\n\n {gmx_obj.output.stderr.result()}\n")
-    except AttributeError:
-        raise RuntimeError("The input object is not an object generated by commandline_operation.")
-
-
-def clean_up(dir_before, dir_after, verbose=False):
-    """
-    Removes newly generated folders that are empty after a command launched by gmxapi.
-
-    Parameters
-    ----------
-    dir_before : list
-        The list of directories existed before the command was executed.
-    dir_after : list
-        The list of directories existed after the command was executed. This helps
-        figure out which directories are newly generated by command.
-    verbose : bool
-        If details should be printed.
-    """
-    new_dirs = natsort.natsorted([i for i in dir_after if i not in dir_before])
-    if len(new_dirs) != 0:
-        if verbose is True:
-            print("\nCleaning up/restructuring the directories ...")
-    for i in new_dirs:
-        if len(os.listdir(i)) == 0:
-            if verbose is True:
-                print(f"  Removing the empty folder {i} ...")
-            os.rmdir(i)
-
-
 def format_time(t):
     """
     Converts time in seconds to the "most readable" format.
 
     Parameters
     ----------
     t : float
@@ -183,15 +130,19 @@
         return s
     for converter in int, float, str:  # try them in increasing order of lenience
         try:
             s = [converter(i) for i in s.split()]
             if len(s) == 1:
                 return s[0]
             else:
-                return np.array(s)
+                if len(s) != 0 and type(s[0]) == str:
+                    # For the case like pull_coord1_dim = Y Y Y, we don't want to us np.array
+                    return s
+                else:
+                    return np.array(s)
         except (ValueError, AttributeError):
             pass
     raise ValueError("Failed to autoconvert {0!r}".format(s))
 
 
 def get_subplot_dimension(n_panels):
     """
@@ -237,7 +188,68 @@
     """
     w = [1 / (i ** 2) for i in errs]
     wx = [w[i] * vals[i] for i in range(len(vals))]
     mean = np.sum(wx) / np.sum(w)
     err = np.sqrt(1 / np.sum(w))
 
     return mean, err
+
+
+def get_time_metrics(log):
+    """
+    Gets the time-based metrics from a log file, including the core time (s),
+    wall time, and performance (ns/day).
+
+    Parameters
+    ----------
+    log : str
+        The input log file.
+
+    Returns
+    -------
+    t_metrics : dict
+        A dictionary having following keys: :code:`t_core`, :code:`t_wall`, :code:`performance`.
+    """
+    t_metrics = {}
+    with open(log, 'r') as f:
+        # Using deque is much faster than using readlines and reversing it since we only need the last few lines.
+        lines = collections.deque(f, 20)  # get the last 20 lines should be enough
+
+    for l in lines:  # noqa: E741
+        if 'Performance: ' in l:
+            t_metrics['performance'] = float(l.split()[1])  # ns/day
+        if 'Time: ' in l:
+            t_metrics['t_core'] = float(l.split()[1])  # s
+            t_metrics['t_wall'] = float(l.split()[2])  # s
+            break
+
+    return t_metrics
+
+
+def analyze_EEXE_time(log_files=None):
+    """
+    Perform simple data analysis on the wall times and performances of all iterations of an EEXE simulation.
+
+    Parameters
+    ----------
+    log_files : None or list
+        A list of sorted file names of all log files.
+
+    Returns
+    -------
+    t_wall_tot : float
+        The total wall time GROMACS spent to finish all iterations for the EEXE simulation.
+    t_sync : float
+        The total time spent in synchronizing all replicas, which is the sum of the differences
+        between the longest and the shortest time elapsed to finish a iteration.
+    """
+    n_iter = len(glob.glob('sim_0/iteration_*'))
+    if log_files is None:
+        log_files = [natsort.natsorted(glob.glob(f'sim_*/iteration_{i}/*log')) for i in range(n_iter)]
+
+    t_wall_tot, t_sync = 0, 0
+    for i in range(n_iter):
+        t_wall = [get_time_metrics(log_files[i][j])['t_wall'] for j in range(len(log_files[i]))]
+        t_wall_tot += max(t_wall)
+        t_sync += (max(t_wall) - min(t_wall))
+
+    return t_wall_tot, t_sync
```

### Comparing `ensemble_md-0.5.0/ensemble_md.egg-info/PKG-INFO` & `ensemble_md-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ensemble-md
-Version: 0.5.0
+Name: ensemble_md
+Version: 0.6.0
 Summary: A package for setting up, performing, and analyzing molecular dynamics ensembles using GROMACS
 Author: Wei-Tse Hsu
 Author-email: wehs7661@colorado.edu
 License: MIT
 Project-URL: Documentation, https://ensemble-md.readthedocs.io/
 Project-URL: Source Code, https://github.com/wehs7661/ensemble_md
 Keywords: molecular mechanics,free energy calculations,advanced sampling
@@ -26,23 +26,22 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gmxapi
 License-File: LICENSE
 
 Ensemble Molecular Dynamics
 ==============================
 [//]: # (Badges)
 [![wehs7661](https://circleci.com/gh/wehs7661/ensemble_md.svg?style=shield)](https://app.circleci.com/pipelines/github/wehs7661/ensemble_md?branch=master)
 [![codecov](https://codecov.io/gh/wehs7661/ensemble_md/branch/master/graph/badge.svg)](https://app.codecov.io/gh/wehs7661/ensemble_md/tree/master)
-[![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble_md.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble-md.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Actions Lint Status](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml/badge.svg)](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml)
 [![PyPI version](https://badge.fury.io/py/ensemble-md.svg)](https://badge.fury.io/py/ensemble-md)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 **ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble_md.readthedocs.io/).
 
 ### Copyright
```

### Comparing `ensemble_md-0.5.0/ensemble_md.egg-info/SOURCES.txt` & `ensemble_md-0.6.0/ensemble_md.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
-ensemble_md/.coverage
 ensemble_md/__init__.py
 ensemble_md/_version.py
 ensemble_md/ensemble_EXE.py
 ensemble_md.egg-info/PKG-INFO
 ensemble_md.egg-info/SOURCES.txt
 ensemble_md.egg-info/dependency_links.txt
 ensemble_md.egg-info/entry_points.txt
@@ -20,15 +19,14 @@
 ensemble_md/analysis/analyze_traj.py
 ensemble_md/analysis/msm_analysis.py
 ensemble_md/cli/analyze_EEXE.py
 ensemble_md/cli/explore_EEXE.py
 ensemble_md/cli/run_EEXE.py
 ensemble_md/data/README.md
 ensemble_md/data/look_and_say.dat
-ensemble_md/tests/.coverage
 ensemble_md/tests/__init__.py
 ensemble_md/tests/test_analyze_matrix.py
 ensemble_md/tests/test_analyze_traj.py
 ensemble_md/tests/test_ensemble_EXE.py
 ensemble_md/tests/test_gmx_parser.py
 ensemble_md/tests/test_utils.py
 ensemble_md/tests/data/expanded.mdp
```

### Comparing `ensemble_md-0.5.0/setup.py` & `ensemble_md-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,29 +89,30 @@
         'argparse',
         'pymbar>=4.0.1',
         'alchemlyb>=2.0.0',
         'pyyaml',
         'seaborn',
         'matplotlib',
         'pyemma',
+        'mpi4py'
     ],
 
-    # The following extra_require directive provides optional dependencies by, in our case, pip install ensemble[gmxapi].
+    # (OBSOLETE) The following extra_require directive provides optional dependencies by, in our case, pip install ensemble[gmxapi].
     # ensemble_md requires GROMACS and gmxapi to be installed before use. 
     # If a working version of GROMACS is available, the user can choose to install ensemble_md along with gmxapi 
     # using the following command: `pip install ensemble_md[gmxapi]`. Otherwise, follow installation 
     # instructions of GROMACS and gmxapi to install each package separately. 
-    extras_require={
-        'gmxapi': [
-            'pybind11>=2.6',
-            'setuptools>=42.0',
-            'mpi4py',
-            'gmxapi>=0.4.0rc2'
-        ],
-    },
+    
+    # extras_require={
+    #    'gmxapi': [
+    #        'pybind11>=2.6',
+    #        'setuptools>=42.0',
+    #        'gmxapi>=0.4.0rc2'
+    #    ],
+    # },
 
     platforms=['Linux',
                'Mac OS-X',
                'Unix',
                'Windows'],            # Valid platforms your code works on, adjust to your flavor
     
     python_requires=">=3.8",          # Python version restrictions
```

### Comparing `ensemble_md-0.5.0/versioneer.py` & `ensemble_md-0.6.0/versioneer.py`

 * *Files identical despite different names*

