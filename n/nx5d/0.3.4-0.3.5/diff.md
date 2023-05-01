# Comparing `tmp/nx5d-0.3.4.tar.gz` & `tmp/nx5d-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx5d-0.3.4.tar", last modified: Thu Apr 27 15:34:05 2023, max compression
+gzip compressed data, was "nx5d-0.3.5.tar", last modified: Mon May  1 16:09:54 2023, max compression
```

## Comparing `nx5d-0.3.4.tar` & `nx5d-0.3.5.tar`

### file list

```diff
@@ -1,181 +1,182 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.648910 nx5d-0.3.4/
--rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.4/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.4/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.4/.readthedocs.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.4/COPYING.md
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-04-27 15:34:05.648910 nx5d-0.3.4/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.4/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.623910 nx5d-0.3.4/doc/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.625910 nx5d-0.3.4/doc/mkdocs/
--rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.4/doc/mkdocs/about.md
--rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.4/doc/mkdocs/api.md
--rw-r--r--   0 florin    (1000) florin    (1000)    27056 2023-04-25 09:48:18.000000 nx5d-0.3.4/doc/mkdocs/concepts.md
--rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.4/doc/mkdocs/frame.svg
--rw-r--r--   0 florin    (1000) florin    (1000)     2483 2023-04-25 09:48:18.000000 nx5d-0.3.4/doc/mkdocs/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.4/doc/mkdocs/license.md
--rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.4/doc/mkdocs/module-nx.md
--rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.4/doc/mkdocs/scan.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.4/doc/mkdocs/streak1.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.4/doc/mkdocs/streak2.svg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.626910 nx5d-0.3.4/doc/mkdocs/tutorials/
--rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.4/doc/mkdocs/tutorials/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.627910 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/
--rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
--rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
--rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
--rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
--rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
--rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.627910 nx5d-0.3.4/doc/mkdocs/tutorials/scansource-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.4/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.627910 nx5d-0.3.4/doc/mkdocs/user-guide/
--rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.4/doc/mkdocs/user-guide/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.4/doc/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.4/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.4/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.4/scratch.org
--rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-04-27 15:34:05.649910 nx5d-0.3.4/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.621910 nx5d-0.3.4/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.628910 nx5d-0.3.4/src/nx5d/
--rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d/_version.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/edf.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.629910 nx5d-0.3.4/src/nx5d/h5like/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.4/src/nx5d/h5like/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)    11230 2023-04-27 15:18:39.000000 nx5d-0.3.4/src/nx5d/h5like/petra3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.4/src/nx5d/h5like/pypod.py
--rw-r--r--   0 florin    (1000) florin    (1000)    10119 2023-04-27 15:05:03.000000 nx5d-0.3.4/src/nx5d/h5like/spec.py
--rw-r--r--   0 florin    (1000) florin    (1000)    11246 2023-04-18 08:03:50.000000 nx5d-0.3.4/src/nx5d/h5like/tools.py
--rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.4/src/nx5d/h5like/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/nx.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/runlog.py
--rw-r--r--   0 florin    (1000) florin    (1000)    14860 2023-04-27 14:19:57.000000 nx5d-0.3.4/src/nx5d/scan.py
--rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.4/src/nx5d/streaks.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.631910 nx5d-0.3.4/src/nx5d/xrd/
--rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/ColonelSandersFinest.py
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/__init__.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/analysis.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/esrf_id09.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/experiment-xpp.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/experiment.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1939 2023-04-27 14:16:35.000000 nx5d-0.3.4/src/nx5d/xrd/kmc3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/roi.py
--rw-r--r--   0 florin    (1000) florin    (1000)    19453 2023-04-25 09:48:18.000000 nx5d-0.3.4/src/nx5d/xrd/signal.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-25 09:48:18.000000 nx5d-0.3.4/src/nx5d/xrd/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/xraytest.py
--rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.4/src/nx5d/xrd/xrd_helpers.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.629910 nx5d-0.3.4/src/nx5d.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     7794 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-04-27 15:34:05.000000 nx5d-0.3.4/src/nx5d.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.632910 nx5d-0.3.4/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     1167 2023-04-27 15:21:20.000000 nx5d-0.3.4/tests/fio_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-17 15:45:54.000000 nx5d-0.3.4/tests/pabst_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-17 15:45:54.000000 nx5d-0.3.4/tests/pypod_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/runlog_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/spec_test.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.632910 nx5d-0.3.4/tests/test_data/fioh5/
--rw-r--r--   0 florin    (1000) florin    (1000)    13611 2023-04-25 09:48:18.000000 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00342.fio
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.632910 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744/lambda/
--rw-r--r--   0 florin    (1000) florin    (1000)   302228 2023-04-25 10:50:01.000000 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
--rw-r--r--   0 florin    (1000) florin    (1000)    13952 2023-04-25 09:48:18.000000 nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744.fio
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.637910 nx5d-0.3.4/tests/test_data/runfile/
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_brokendata1.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_brokendata2.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_brokenheader.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/run105_simple.log
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0001.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0002.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0003.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0004.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0005.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0006.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0007.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0008.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0009.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0010.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0011.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0012.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0013.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0014.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0015.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0016.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0017.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0018.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0019.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0020.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0021.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0022.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0023.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0024.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0025.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0026.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0027.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0028.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0029.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0030.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0031.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0032.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0033.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0034.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0035.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0036.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/runfile/short_run04_0037.edf
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/spech5/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.637910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/
--rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.622910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.640910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
--rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-27 15:34:05.648910 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
--rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.4/tests/xfel_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.4/tests/xrd_data_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.618691 nx5d-0.3.5/
+-rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-24 10:31:16.000000 nx5d-0.3.5/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-24 10:31:16.000000 nx5d-0.3.5/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-30 12:37:15.000000 nx5d-0.3.5/.readthedocs.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-30 12:37:15.000000 nx5d-0.3.5/COPYING.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-01 16:09:54.619691 nx5d-0.3.5/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-30 12:37:15.000000 nx5d-0.3.5/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.576691 nx5d-0.3.5/doc/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.579691 nx5d-0.3.5/doc/mkdocs/
+-rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/about.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-24 10:31:17.000000 nx5d-0.3.5/doc/mkdocs/api.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    27056 2023-04-25 08:54:47.000000 nx5d-0.3.5/doc/mkdocs/concepts.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/frame.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)     2483 2023-04-25 08:54:47.000000 nx5d-0.3.5/doc/mkdocs/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/license.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/module-nx.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/scan.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/streak1.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/streak2.svg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.579691 nx5d-0.3.5/doc/mkdocs/tutorials/
+-rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.582691 nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/
+-rw-r--r--   0 florin    (1000) florin    (1000)    44315 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    19430 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
+-rw-r--r--   0 florin    (1000) florin    (1000)    25263 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
+-rw-r--r--   0 florin    (1000) florin    (1000)    23184 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
+-rw-r--r--   0 florin    (1000) florin    (1000)    13289 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
+-rw-r--r--   0 florin    (1000) florin    (1000)    16038 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.582691 nx5d-0.3.5/doc/mkdocs/tutorials/scansource-howto/
+-rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.583691 nx5d-0.3.5/doc/mkdocs/user-guide/
+-rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-24 10:31:17.000000 nx5d-0.3.5/doc/mkdocs/user-guide/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-30 12:37:15.000000 nx5d-0.3.5/doc/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-30 12:37:15.000000 nx5d-0.3.5/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-30 12:37:15.000000 nx5d-0.3.5/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)     2974 2023-03-30 12:37:15.000000 nx5d-0.3.5/scratch.org
+-rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-05-01 16:09:54.619691 nx5d-0.3.5/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.573691 nx5d-0.3.5/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.586691 nx5d-0.3.5/src/nx5d/
+-rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-05-01 16:09:54.000000 nx5d-0.3.5/src/nx5d/_version.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/edf.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.589691 nx5d-0.3.5/src/nx5d/h5like/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-24 10:31:17.000000 nx5d-0.3.5/src/nx5d/h5like/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    12534 2023-05-01 15:31:12.000000 nx5d-0.3.5/src/nx5d/h5like/petra3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-24 10:31:17.000000 nx5d-0.3.5/src/nx5d/h5like/pypod.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    10119 2023-05-01 15:16:41.000000 nx5d-0.3.5/src/nx5d/h5like/spec.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11159 2023-05-01 15:49:22.000000 nx5d-0.3.5/src/nx5d/h5like/tools.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-24 10:31:17.000000 nx5d-0.3.5/src/nx5d/h5like/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/nx.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/runlog.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    14860 2023-05-01 15:16:41.000000 nx5d-0.3.5/src/nx5d/scan.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-24 10:31:17.000000 nx5d-0.3.5/src/nx5d/streaks.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.592691 nx5d-0.3.5/src/nx5d/xrd/
+-rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/ColonelSandersFinest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/__init__.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/analysis.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/esrf_id09.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/experiment-xpp.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/experiment.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1939 2023-05-01 15:16:41.000000 nx5d-0.3.5/src/nx5d/xrd/kmc3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      681 2023-05-01 15:51:21.000000 nx5d-0.3.5/src/nx5d/xrd/petra3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/roi.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    19798 2023-05-01 16:02:44.000000 nx5d-0.3.5/src/nx5d/xrd/signal.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-24 10:31:17.000000 nx5d-0.3.5/src/nx5d/xrd/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/xraytest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-30 12:37:15.000000 nx5d-0.3.5/src/nx5d/xrd/xrd_helpers.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.587691 nx5d-0.3.5/src/nx5d.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-01 16:09:54.000000 nx5d-0.3.5/src/nx5d.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     7817 2023-05-01 16:09:54.000000 nx5d-0.3.5/src/nx5d.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-05-01 16:09:54.000000 nx5d-0.3.5/src/nx5d.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-05-01 16:09:54.000000 nx5d-0.3.5/src/nx5d.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-05-01 16:09:54.000000 nx5d-0.3.5/src/nx5d.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.593691 nx5d-0.3.5/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     1167 2023-05-01 15:16:41.000000 nx5d-0.3.5/tests/fio_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-24 10:31:17.000000 nx5d-0.3.5/tests/pabst_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-24 10:31:17.000000 nx5d-0.3.5/tests/pypod_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/runlog_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-05-01 15:16:41.000000 nx5d-0.3.5/tests/spec_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.574691 nx5d-0.3.5/tests/test_data/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.594691 nx5d-0.3.5/tests/test_data/fioh5/
+-rw-r--r--   0 florin    (1000) florin    (1000)    13611 2023-05-01 15:16:41.000000 nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00342.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.573691 nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00744/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.594691 nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00744/lambda/
+-rw-r--r--   0 florin    (1000) florin    (1000)   302228 2023-05-01 15:16:41.000000 nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
+-rw-r--r--   0 florin    (1000) florin    (1000)    13952 2023-05-01 15:16:41.000000 nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00744.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.605691 nx5d-0.3.5/tests/test_data/runfile/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/run105.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/run105_brokendata1.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/run105_brokendata2.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/run105_brokenheader.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/run105_simple.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0001.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0002.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0003.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0004.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0005.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0006.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0007.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0008.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0009.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0010.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0011.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0012.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0013.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0014.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0015.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0016.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0017.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0018.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0019.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0020.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0021.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0022.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0023.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0024.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0025.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0026.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0027.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0028.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0029.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0030.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0031.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0032.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0033.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0034.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0035.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0036.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/runfile/short_run04_0037.edf
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.574691 nx5d-0.3.5/tests/test_data/spech5/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.605691 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.574691 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.606691 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
+-rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:09:54.618691 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-24 10:31:17.000000 nx5d-0.3.5/tests/xfel_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-30 12:37:15.000000 nx5d-0.3.5/tests/xrd_data_test.py
```

### Comparing `nx5d-0.3.4/.gitlab-ci.yml` & `nx5d-0.3.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/COPYING.md` & `nx5d-0.3.5/COPYING.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/PKG-INFO` & `nx5d-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.4
+Version: 0.3.5
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.4/README.md` & `nx5d-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/concepts.md` & `nx5d-0.3.5/doc/mkdocs/concepts.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/frame.svg` & `nx5d-0.3.5/doc/mkdocs/frame.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/index.md` & `nx5d-0.3.5/doc/mkdocs/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/license.md` & `nx5d-0.3.5/doc/mkdocs/license.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/module-nx.md` & `nx5d-0.3.5/doc/mkdocs/module-nx.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/scan.svg` & `nx5d-0.3.5/doc/mkdocs/scan.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/streak1.svg` & `nx5d-0.3.5/doc/mkdocs/streak1.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/streak2.svg` & `nx5d-0.3.5/doc/mkdocs/streak2.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/index.md` & `nx5d-0.3.5/doc/mkdocs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md` & `nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png` & `nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png` & `nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png` & `nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png` & `nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png` & `nx5d-0.3.5/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md` & `nx5d-0.3.5/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/doc/mkdocs.yml` & `nx5d-0.3.5/doc/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/scratch.org` & `nx5d-0.3.5/scratch.org`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/setup.cfg` & `nx5d-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/edf.py` & `nx5d-0.3.5/src/nx5d/edf.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/h5like/petra3.py` & `nx5d-0.3.5/src/nx5d/h5like/petra3.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from os import path, walk
 from glob import glob
 from itertools import chain
 
 import h5py
 import re
 
+import logging
+
 ''' Selected data formats for the PETRA3 synchrotron at DESY.
 '''
 
 def read_fio(f):
     ''' Reads a FIO file and returns an xarray dataset.
 
     Returns:
@@ -29,23 +31,26 @@
 
         parts = data.split('=')
         assert len(parts) == 2
         
         key = parts[-2].strip()
         val = parts[-1].strip()
 
-        if val[0] != '[':
-            return {key: float(val)}
-
-        else:
-            return {
-                key: np.array([
-                    float(i.strip(',')) for i in val.strip('[]').split(' ')
-                ])
-            }
+        try:
+            if val[0] == '[':
+                return {
+                    key: np.array([
+                        float(i.strip(',')) for i in val.strip('[]').split(' ')
+                    ])
+                }
+            else:
+                return {key: float(val)}
+        except Exception as e:
+            logging.error("Don't understand parameter '%s': %s" % (key, str(e)))
+            return {key: val.encode('utf-8')}
 
 
     # Columns data (%d) stuff.
     # Data line is either a "Col ..." line, specifying ("Col", index, name, data_type)
     # or is an acutal space-separated list of items (numbers).
     data_types = { 'DOUBLE': float }   # Data type translators; so far, only DOUBLE
     data_column_types = []             # Here we'll store the types (one for each column)
@@ -53,15 +58,16 @@
     def data_eval(data):
         dl = data.split(' ')
         if dl[0] == "Col":
             data_column_types.append(dl[3])
             data_column_names.append(dl[2])
             return None
         return { data_column_names[i]:\
-                 np.array([data_types[data_column_types[i]](d)]) for i,d in enumerate(dl) }
+                 np.array([data_types[data_column_types[i]](d)]) \
+                 for i,d in enumerate(dl) }
 
     
     # Reading FIO file in several "states" demarked by the '%...' magic.
     # Each "state" has a parsing function associated with it.
     cur_state = None    
     read_states = { '%c': lambda l: None,
                     '%p': param_eval,
@@ -170,15 +176,15 @@
         return self.h5node.visit(*a, **kw)
 
     def visititems(self, *a, **kw):
         return self.h5node.visititems(*a, **kw)
         
             
 class FioH5(ch5.File):
-    ''' Bastard HDF5 API fake for the "FIO" data format, e.g. as used as PETRA3/P08 beamline.
+    ''' Bastard HDF5 API fake for the "FIO" data format, e.g. for PETRA3/P08.
 
     Currently (as of: April 2023) the data format appears to be this:
     
       - A master `.fio` file appearing somewhere on the filesystem, containing
         variables with scalar data, variables with vector data, and some
         "scanning values" a.k.a. positioners. This is an ASCII file with
         a proprietary format, but not terribly complicated to parse.
@@ -224,14 +230,46 @@
     For convenience we're also bein opinionated about the HDF5 layout by default,
     rewarding a `./<basename>/<detector>/<basename><extra>.nxs` layout by
     auto-detecting such files, and automatically integrating them as
     `/<detector><extra>/...` in `FioH5`.
 
     On top of that, extra HDF5 files need to be integrated by manually specifying
     a key-value map of folder name to file path.
+
+    Usage example:
+    
+    ```
+    In [1]: from nx5d.h5like.petra3 import FioH5
+    
+    In [2]: fh = FioH5("m3_2507_00744.fio")
+    
+    In [3]: fh.keys()
+    Out[3]: odict_keys(['fio', 'lambda_00001', 'lambda_00002', 'lambda_00000'])
+    
+    In [4]: fh['fio/data/om'].shape
+    Out[4]: (61,)
+    
+    In [5]: fh['lambda_00000/entry/instrument/detector/data'].shape
+    Out[5]: (61, 516, 1554)
+    ```
+
+    Usage with the nx5d `ScanReader`:
+    
+    ```
+    In [7]: reader = ScanReader(FioH5, ("/var/home/florin/tmp/Downloads/"
+                                        "P08_data/example/raw/m3_2507_00744.fio",))
+
+    In [8]: d1 = reader.read(slice(None), omega="@/fio/data/om",
+                       images="@/lambda_00000/entry/instrument/detector/data")
+    ...
+    ```
+
+    (Note that the example "m3_2507_00744.fio" provided as test data with this package's
+    source code does _not_ have a dataset named `data` -- it's called `"mock_data"`
+    instead, and has a reduced shape of `"(61, 100, 100)"` for size reasons.)
     '''
 
 
     def __init__(self, fio, fiogrp='fio', h5extra=None):
         ''' Loads FIO (text) file, underlining its data with existing HDF5 data.
 
         Normally with every `.fio` file comes a directory of the same name, containing
@@ -269,15 +307,17 @@
                 extra_re.match(path.basename(f)).groups()[0] : f
                 for f in glob(path.join(device, fio_base+"*.nxs"))
             } 
             for device in glob(path.join(fio_datadir, '*'))
         }
 
         # This is a flat {<device><extra>: <file path>, ...} map.
-        flat_devices = { dev+ext:devices[dev][ext] for dev in devices for ext in devices[dev] }
+        flat_devices = { dev+ext:devices[dev][ext] \
+                         for dev in devices \
+                         for ext in devices[dev] }
         
         if h5extra is not None:
             devices.update(h5extra)
 
         self.fioGroup = FioGroup(fio, name=fiogrp or fio_base, parent=self)
         self.add_node(self.fioGroup)
```

### Comparing `nx5d-0.3.4/src/nx5d/h5like/pypod.py` & `nx5d-0.3.5/src/nx5d/h5like/pypod.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/h5like/spec.py` & `nx5d-0.3.5/src/nx5d/h5like/spec.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/h5like/tools.py` & `nx5d-0.3.5/src/nx5d/h5like/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,80 +173,81 @@
             else:
                 my_slicer = (slicer, *value[1:])
             value = value[0]
 
 
         if isinstance(value, str):
             # The main feature: loading data from HDF5 if we encounter an "@..." string.
-            # FIXME: need to actually rewrite this and base this on the __call__() feature
-            # (see below). This will simplify many things.
-
             if (len(value) == 0) or (value[0] not in  ['@', '$']):
                 return value
 
             # Only HDF5 addresses prefixed with '@' will be subject to slicing.
             # Prefix '$' will take the data verbatim, no slicing.
             doSlicing = (value[0] == '@')
             
             nodeAddrFmt = value[1:]
             
             try:
                 nodeAddr = nodeAddrFmt.format(**fmtKeys)
 
                 node = h5like[nodeAddr]
 
-                logging.debug("Loading data from %s (only node: %r)" % (nodeAddr, opts.get('nodeOnly', False)))
+                logging.debug("Loading data from %s (only node: %r)" % \
+                              (nodeAddr, opts.get('nodeOnly', False)))
                 
                 if opts.get('nodeOnly', False):
                     return node
                 else:
                     try:
                         if doSlicing:
-                            s = tuple(my_slicer[:len(node.shape)]) if isinstance(my_slicer, tuple) else my_slicer
+                            s = tuple(my_slicer[:len(node.shape)]) \
+                                if isinstance(my_slicer, tuple) else my_slicer
                             data = node[s]
                             #print("Slicing %s: %r" % (value, data))
                         else:
                             data = node[()]
                             #print("Not slicing %s: %r" % (value, data))
 
                         if data.shape[0] == 0 and not opts.get('allowEmpty', False):
                             raise DatasetEmpty
                         return data
                     #except TypeError:  # ...not sure when this happens (?)
                     #    return node
-                    except ValueError: # This happens when value is a scalar and needs to be sliced by ()
+                    except ValueError: # This happens when value is a scalar \
+                           # and needs to be sliced by ()
                         return node[()]
                         
 
             except KeyError as e:
-                logging.error("Path substitition error in '%s' for '%s': %s" % (nodeAddrFmt, value, str(e)))
+                logging.error("Path substitition error in '%s' for '%s': %s" \
+                              % (nodeAddrFmt, value, str(e)))
                 raise
 
             except DatasetEmpty:
                 raise
                     
             except Exception as e:
                 logging.error("%s: error reading node (%r)" % (nodeAddr, str(e)))
                 raise
-                
+
+
+        # Descending into each of the elements if we encounter python basic
+        # data types dict, list, tuple. For everything else, return verbatim.
+            
         elif isinstance(value, dict):
-            # Descending into each of the elements
-            return dict({k:self.__value(h5like, v, fmtKeys, slicer, **opts) for k,v in value.items()})
+            return dict({k:self.__value(h5like, v, fmtKeys, slicer, **opts) \
+                         for k,v in value.items()})
         
-        elif hasattr(value, "__len__"):
-            # It's not a string and it's not a dict, but is iterable?
-            # descend and find out.
-            return tuple([self.__value(h5like, v, fmtKeys, slicer, **opts) for v in value])
-
-        # DEPRECATED!
-        elif hasattr(value, "__call__"):
-            # This allows us to create custom objects that retrieve
-            # data from unconventional sources.
-            return value(h5like, opts.get('nodeOnly', False), slicer)
+        elif isinstance(value, tuple):
+            return tuple([self.__value(h5like, v, fmtKeys, slicer, **opts) \
+                          for v in value])
 
+        elif isinstance(value, list):
+            return [self.__value(h5like, v, fmtKeys, slicer, **opts) for v in value]
+            
         else:
             return value
 
         
     def __call__(self, h5like=None, paths=None, slicer=slice(None), **opts):
         '''
         Uses the stored template to generate meaningful content based on the
```

### Comparing `nx5d-0.3.4/src/nx5d/h5like/xfel.py` & `nx5d-0.3.5/src/nx5d/h5like/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/nx.py` & `nx5d-0.3.5/src/nx5d/nx.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/runlog.py` & `nx5d-0.3.5/src/nx5d/runlog.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/scan.py` & `nx5d-0.3.5/src/nx5d/scan.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/streaks.py` & `nx5d-0.3.5/src/nx5d/streaks.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/ColonelSandersFinest.py` & `nx5d-0.3.5/src/nx5d/xrd/ColonelSandersFinest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/analysis.py` & `nx5d-0.3.5/src/nx5d/xrd/analysis.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/esrf_id09.py` & `nx5d-0.3.5/src/nx5d/xrd/esrf_id09.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/experiment-xpp.yml` & `nx5d-0.3.5/src/nx5d/xrd/experiment-xpp.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/experiment.py` & `nx5d-0.3.5/src/nx5d/xrd/experiment.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/kmc3.py` & `nx5d-0.3.5/src/nx5d/xrd/kmc3.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/roi.py` & `nx5d-0.3.5/src/nx5d/xrd/roi.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/signal.py` & `nx5d-0.3.5/src/nx5d/xrd/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,16 +278,17 @@
         This is introduced as the first dimension in the `xarray` dataset,
         with the name "__index__".
         '''
         
         tmp = next(iter(dsets.items()))
         xdata = Dataset({'index': np.array(range(tmp[1].shape[0]))})
         for k,p in dsets.items():
-            dims = ["index"] + ["%s_%d" % (k,i) for i in range(1,len(p.shape))]
-            xdata[k] = (dims, p)
+            data = self.__arrayify(p)
+            dims = ["index"] + ["%s_%d" % (k,i) for i in range(1,len(data.shape))]
+            xdata[k] = (dims, data)
 
         return xdata
 
 
 
     def __2tuple(self, data, name=""):
         ''' Returns a 2-tuple (X, Y) from a variety of data sets:
@@ -305,15 +306,19 @@
                 return ([data[0], data[1]])
 
         if len(data) > 2:
             return data[0]
 
         raise RuntimeError("Oops: don't know how to handle %s: %r" % (name, data))
 
-        
+
+    def __arrayify(self, val):
+        return val \
+            if hasattr(val, "__len__") \
+            else np.array([a]*len(img))
 
 
     def __init_experiment(self, setup):
         '''
         Initializes the Experiment part (i.e. xrayutilities HXRD object etc)
         with specified device and sample geometry. The optional parameter `roi`
         restricts angle-to-Q conversion to solely this region, if it is
@@ -346,46 +351,53 @@
 
         imageCenter = self.__2tuple(setup['imageCenter'], 'imageCenter')
         imageSize = self.__2tuple(setup['imageSize'], 'imageSize')
         imageDistance = setup['imageDistance'][0] \
             if hasattr(setup['imageDistance'], "__len__") \
                else setup['imageDistance']
 
-        logging.debug("image distance %r, size %r, center at %r" % (imageDistance, imageSize, imageCenter))
+        logging.debug("image distance %r, size %r, center at %r" % \
+                      (imageDistance, imageSize, imageCenter))
         
         if imageCenter[0] <= 1 and imageCenter[1] <= 1:
             # It's a floaring-point number, relative to the detector size
 
             # similar considerations for imageSize as for imageCenter: expected to be
-            # a 1D array with length 2, but will also accept a 2D array with shape (N, 2).
+            # a 1D array with length 2, but will also accept a 2D array
+            # with shape (N, 2).
+            
             # FIXME: really, REALLY need to fix this. This is really ugly.
             imgs = imageSize
             assert imgs is not None
             assert imgs[0] is not None
             assert imgs[1] is not None            
             imageCenter = tuple([c*s for c,s in zip(setup['imageCenter'], imgs)])
 
         chSizeParm = {}
         if ('imageChannelSpan' in setup) and (setup['imageChannelSpan'] is not None):
-            # channelSpan is degrees/channel, but we need to pass channels/degree to Ang2Q
-            imageChannelSize = self.__2tuple(setup['imageChannelSpan'], 'imageChannelSpan')
+            # channelSpan is degrees/channel, but need to pass channels/degree to Ang2Q
+            imageChannelSize = self.__2tuple(setup['imageChannelSpan'],
+                                             'imageChannelSpan')
             chSizeParm = {'chpdeg1': 1.0/imageChannelSpan[0],
                           'chpdeg1': 1.0/imageChannelSpan[1] }
 
         elif ('imageChannelSize' in setup) and (setup['imageChannelSize'] is not None):
-            # Ang2Q takes one explicit distance parameter, but we're assuming that channelSize
-            # is relative to the distance itself (putting the distance always at 1.0 units)
-            imageChannelSize = self.__2tuple(setup['imageChannelSize'], 'imageChannelSize')
+            # Ang2Q takes one explicit distance parameter, but we're assuming that
+            # channelSize is relative to the distance itself (putting the distance
+            # always at 1.0 units)
+            imageChannelSize = self.__2tuple(setup['imageChannelSize'],
+                                             'imageChannelSize')
             logging.debug("pixel size: %r" % (imageChannelSize,))
             chSizeParm = { 'pwidth1':  imageChannelSize[0],
                            'pwidth2':  imageChannelSize[1],
                            'distance': imageDistance }
 
         else:
-            raise RuntimeError("Experiment setup needs either the channel span or channel size")
+            raise RuntimeError("Experiment setup needs either the "
+                               "channel span or channel size")
 
         tarAngles = setup.get('detectorTARAngles', [0, 0, 0])
 
         roi = setup.get('roi', (0, imageSize[0], 0, imageSize[1]))
 
         hxrd.Ang2Q.init_area(detectorDir1=setup['imageAxes'][0],
                              detectorDir2=setup['imageAxes'][1],
@@ -442,20 +454,21 @@
         if isinstance(dims, str):
             dims = (dims,)
 
         if len(dims) < 1 or len(dims) > 3:
             raise RuntimeError("Bad Q-axis specification: %r" % dims)
         
         if len(img.shape) != 3:
-            raise RuntimeError("Don't know how to transform objects of shape %r" % (img.shape,))
+            raise RuntimeError("Don't know how to transform objects of shape %r" \
+                               % (img.shape,))
 
 
-        # Make sure all angles are arrays (even those that might have been passed as floats)
-        ang = [self.xdata[a].values if hasattr(a, "__len__") else np.array([a]*len(img)) \
-               for a in self._angle_keys]
+        # Make sure all angles are arrays (even those that might have been
+        # passed as floats)
+        ang = [self.__arrayify(self.xdata[a].values) for a in self._angle_keys]
             
         self.q = self.Ang2Q.area(*ang, **(kwargs.get('_ang2qDict', {})))
 
         # For transforming strings to dimension indices
         qspec = { 'x': 0, 'qx': 0,
                   'y': 1, 'qy': 1,
                   'z': 2, 'qz': 2 }
```

### Comparing `nx5d-0.3.4/src/nx5d/xrd/xfel.py` & `nx5d-0.3.5/src/nx5d/xrd/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/xraytest.py` & `nx5d-0.3.5/src/nx5d/xrd/xraytest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d/xrd/xrd_helpers.py` & `nx5d-0.3.5/src/nx5d/xrd/xrd_helpers.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/src/nx5d.egg-info/PKG-INFO` & `nx5d-0.3.5/src/nx5d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.4
+Version: 0.3.5
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.4/src/nx5d.egg-info/SOURCES.txt` & `nx5d-0.3.5/src/nx5d.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 src/nx5d/xrd/ColonelSandersFinest.py
 src/nx5d/xrd/__init__.py
 src/nx5d/xrd/analysis.py
 src/nx5d/xrd/esrf_id09.py
 src/nx5d/xrd/experiment-xpp.yml
 src/nx5d/xrd/experiment.py
 src/nx5d/xrd/kmc3.py
+src/nx5d/xrd/petra3.py
 src/nx5d/xrd/roi.py
 src/nx5d/xrd/signal.py
 src/nx5d/xrd/xfel.py
 src/nx5d/xrd/xraytest.py
 src/nx5d/xrd/xrd_helpers.py
 tests/.gitignore
 tests/fio_test.py
```

### Comparing `nx5d-0.3.4/tests/fio_test.py` & `nx5d-0.3.5/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/pabst_test.py` & `nx5d-0.3.5/tests/pabst_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/pypod_test.py` & `nx5d-0.3.5/tests/pypod_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/runlog_test.py` & `nx5d-0.3.5/tests/runlog_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/spec_test.py` & `nx5d-0.3.5/tests/spec_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00342.fio` & `nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00342.fio`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs` & `nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/fioh5/m3_2507_00744.fio` & `nx5d-0.3.5/tests/test_data/fioh5/m3_2507_00744.fio`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/run04.log` & `nx5d-0.3.5/tests/test_data/runfile/run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/run105.log` & `nx5d-0.3.5/tests/test_data/runfile/run105.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/run105_brokendata1.log` & `nx5d-0.3.5/tests/test_data/runfile/run105_brokendata1.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/run105_brokendata2.log` & `nx5d-0.3.5/tests/test_data/runfile/run105_brokendata2.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/run105_brokenheader.log` & `nx5d-0.3.5/tests/test_data/runfile/run105_brokenheader.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/run105_simple.log` & `nx5d-0.3.5/tests/test_data/runfile/run105_simple.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04.log` & `nx5d-0.3.5/tests/test_data/runfile/short_run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0001.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0001.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0002.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0002.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0003.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0003.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0004.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0004.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0005.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0005.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0006.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0006.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0007.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0007.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0008.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0008.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0009.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0009.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0010.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0010.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0011.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0011.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0012.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0012.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0013.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0013.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0014.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0014.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0015.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0015.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0016.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0016.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0017.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0017.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0018.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0018.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0019.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0019.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0020.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0020.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0021.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0021.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0022.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0022.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0023.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0023.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0024.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0024.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0025.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0025.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0026.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0026.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0027.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0027.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0028.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0028.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0029.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0029.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0030.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0030.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0031.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0031.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0032.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0032.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0033.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0033.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0034.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0034.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0035.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0035.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0036.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0036.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/runfile/short_run04_0037.edf` & `nx5d-0.3.5/tests/test_data/runfile/short_run04_0037.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif` & `nx5d-0.3.5/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/xfel_test.py` & `nx5d-0.3.5/tests/xfel_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.4/tests/xrd_data_test.py` & `nx5d-0.3.5/tests/xrd_data_test.py`

 * *Files identical despite different names*

