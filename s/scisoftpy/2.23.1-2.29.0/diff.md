# Comparing `tmp/scisoftpy-2.23.1.tar.gz` & `tmp/scisoftpy-2.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/scratch/work/tp-update/dawn2/workspace_git/scisoft-core.git/uk.ac.diamond.scisoft.python/src/dist/tmpvzy9c59h/scisoftpy-2.23.1", last modified: Thu Aug 19 17:11:14 2021, max compression
+gzip compressed data, was "scisoftpy-2.29.0.tar", last modified: Mon May  1 11:02:09 2023, max compression
```

## Comparing `scisoftpy-2.23.1.tar` & `scisoftpy-2.29.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      678 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/PKG-INFO
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5803 2021-08-19 16:45:43.000000 scisoftpy-2.23.1/scisoftpy/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      727 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/crystallography.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      988 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/data.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    15992 2020-07-14 12:55:33.000000 scisoftpy-2.23.1/scisoftpy/dictutils.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      719 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/diffraction.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    20936 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/external.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      756 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/fft.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy/fit/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      788 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/fit/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1074 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/flatten.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      718 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/image.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    11164 2021-07-05 13:37:50.000000 scisoftpy-2.23.1/scisoftpy/io.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy/jython/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    19637 2020-07-14 12:55:33.000000 scisoftpy-2.23.1/scisoftpy/jython/fitcore.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4653 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/function.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2107 2020-07-14 12:55:33.000000 scisoftpy-2.23.1/scisoftpy/jython/jybeans.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4137 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jycomparisons.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    61437 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jycore.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1849 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jycrystallography.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      516 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jydata.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2815 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jydiffraction.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2294 2020-07-14 12:55:33.000000 scisoftpy-2.23.1/scisoftpy/jython/jyfft.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      905 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyflatten.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7262 2021-08-19 16:36:51.000000 scisoftpy-2.23.1/scisoftpy/jython/jyhdf5io.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4287 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyimage.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    13632 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4636 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jylinalg.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    18721 2021-08-19 16:45:43.000000 scisoftpy-2.23.1/scisoftpy/jython/jymaths.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1639 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jynxio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     6057 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyplot.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1427 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyplottingsystem.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2898 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyrandom.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     8280 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyroi.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4739 2021-01-05 14:54:20.000000 scisoftpy-2.23.1/scisoftpy/jython/jyrpc.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3691 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jyscisoft.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2166 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/jython/jysignal.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      993 2021-01-05 14:54:20.000000 scisoftpy-2.23.1/scisoftpy/jython/jywrapper.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/linalg.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy/nexus/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      770 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/nexus/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5720 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/nexus/hdf5.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    16967 2020-11-20 10:31:20.000000 scisoftpy-2.23.1/scisoftpy/nexus/nxclasses.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2128 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/nexus/utils.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    32790 2021-07-05 13:37:50.000000 scisoftpy-2.23.1/scisoftpy/plot.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy/python/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7931 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pybeans.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1127 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pycomparisons.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    10742 2020-07-14 12:55:33.000000 scisoftpy-2.23.1/scisoftpy/python/pycore.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      309 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pydata.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    23572 2020-12-04 15:35:37.000000 scisoftpy-2.23.1/scisoftpy/python/pyflatten.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     8424 2021-08-19 16:36:51.000000 scisoftpy-2.23.1/scisoftpy/python/pyh5py.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      790 2021-08-19 16:36:51.000000 scisoftpy-2.23.1/scisoftpy/python/pyhdf5io.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    21099 2021-07-05 13:37:50.000000 scisoftpy-2.23.1/scisoftpy/python/pyio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3666 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pymaths.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      912 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pynxio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5296 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pyplot.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      836 2021-07-05 13:37:50.000000 scisoftpy-2.23.1/scisoftpy/python/pyplottingsystem.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     9226 2021-07-05 13:37:50.000000 scisoftpy-2.23.1/scisoftpy/python/pyroi.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7597 2020-11-25 23:19:00.000000 scisoftpy-2.23.1/scisoftpy/python/pyrpc.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4449 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pyscisoft.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1112 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pysignal.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2500 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/python/pywrapper.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/random.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1951 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/roi.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2346 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/rpc.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      780 2020-07-14 12:55:34.000000 scisoftpy-2.23.1/scisoftpy/signal.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy.egg-info/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      678 2021-08-19 17:11:13.000000 scisoftpy-2.23.1/scisoftpy.egg-info/PKG-INFO
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1912 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy.egg-info/SOURCES.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy.egg-info/dependency_links.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)       22 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy.egg-info/requires.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)       10 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/scisoftpy.egg-info/top_level.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2021-07-28 10:25:05.000000 scisoftpy-2.23.1/scisoftpy.egg-info/zip-safe
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      469 2021-08-19 17:11:14.000000 scisoftpy-2.23.1/setup.cfg
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1179 2021-08-19 16:45:43.000000 scisoftpy-2.23.1/setup.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.471651 scisoftpy-2.29.0/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      692 2023-05-01 11:02:09.472651 scisoftpy-2.29.0/PKG-INFO
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      101 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/pyproject.toml
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.467651 scisoftpy-2.29.0/scisoftpy/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5809 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      727 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/crystallography.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      988 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/data.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    15992 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/dictutils.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      719 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/diffraction.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    21434 2023-05-01 11:00:38.000000 scisoftpy-2.29.0/scisoftpy/external.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      756 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/fft.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.467651 scisoftpy-2.29.0/scisoftpy/fit/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      788 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/fit/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1074 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/flatten.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      718 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/image.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    11231 2023-03-09 14:46:32.000000 scisoftpy-2.29.0/scisoftpy/io.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.470651 scisoftpy-2.29.0/scisoftpy/jython/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    20722 2023-03-09 14:46:32.000000 scisoftpy-2.29.0/scisoftpy/jython/fitcore.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4653 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/function.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2107 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jybeans.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4137 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jycomparisons.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    60797 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/jython/jycore.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1849 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jycrystallography.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      516 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jydata.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2815 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jydiffraction.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2294 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyfft.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      905 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyflatten.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7320 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/jython/jyhdf5io.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4287 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jyimage.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    13632 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4636 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jylinalg.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    19173 2022-11-29 10:59:56.000000 scisoftpy-2.29.0/scisoftpy/jython/jymaths.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1672 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/jython/jynxio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     6095 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/jython/jyplot.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1427 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyplottingsystem.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2898 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jyrandom.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     8515 2023-03-16 13:37:01.000000 scisoftpy-2.29.0/scisoftpy/jython/jyroi.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4739 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jyrpc.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3196 2022-11-29 10:59:56.000000 scisoftpy-2.29.0/scisoftpy/jython/jyscisoft.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2166 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jysignal.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      993 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jywrapper.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/linalg.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.470651 scisoftpy-2.29.0/scisoftpy/nexus/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      770 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/nexus/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5809 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/nexus/hdf5.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    17001 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/nexus/nxclasses.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2128 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/nexus/utils.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    33907 2023-03-16 13:37:01.000000 scisoftpy-2.29.0/scisoftpy/plot.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.471651 scisoftpy-2.29.0/scisoftpy/python/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7924 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/python/pybeans.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1127 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pycomparisons.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    10966 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/python/pycore.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      309 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pydata.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    23547 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/python/pyflatten.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     8720 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/python/pyh5py.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      790 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pyhdf5io.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    22658 2023-03-09 14:46:32.000000 scisoftpy-2.29.0/scisoftpy/python/pyio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3733 2022-11-29 10:59:56.000000 scisoftpy-2.29.0/scisoftpy/python/pymaths.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      912 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/python/pynxio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5296 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pyplot.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      836 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/python/pyplottingsystem.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     9310 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/python/pyroi.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7597 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pyrpc.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3600 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/python/pyscisoft.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1112 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pysignal.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2500 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pywrapper.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/random.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1927 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/roi.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2346 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/rpc.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      780 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/signal.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.467651 scisoftpy-2.29.0/scisoftpy.egg-info/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      692 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/PKG-INFO
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1927 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)       77 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/requires.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)       10 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/top_level.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2022-09-07 15:14:39.000000 scisoftpy-2.29.0/scisoftpy.egg-info/zip-safe
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      469 2023-05-01 11:02:09.472651 scisoftpy-2.29.0/setup.cfg
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1095 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scisoftpy-2.23.1/PKG-INFO` & `scisoftpy-2.29.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: scisoftpy
-Version: 2.23.1
+Version: 2.29.0
 Summary: DAWN Python Extensions
 Home-page: https://gerrit.diamond.ac.uk/plugins/gitiles/scisoft/scisoft-core
 Author: Peter Chang
-Author-email: scientificsoftware@diamond.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: dataanalysis@diamond.ac.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-
-UNKNOWN
-
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `scisoftpy-2.23.1/scisoftpy/__init__.py` & `scisoftpy-2.29.0/scisoftpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ###
 
 '''
 scisoftpy is a NumPy-like wrapper around the Diamond Scisoft Analysis plugin
 ----------------------------------------------------------------------------
 
 Check the documentation at
-  http://www.opengda.org/documentation/manuals/Diamond_SciSoft_Python_Guide/trunk/contents.html
+  https://alfred.diamond.ac.uk/documentation/manuals/Diamond_SciSoft_Python_Guide/trunk/contents.html
 
 Classes available:
     ndarray - dataset
     ndarrayRGB - colour RGB dataset
 
 dtypes available:
     bool
@@ -126,15 +126,15 @@
     from .jython.jyscisoft import *
 else:
     from .python.pycore import *
     from .python.pymaths import *
     from .python.pycomparisons import *
     from .python.pyscisoft import *
 
-__version__ = "2.23.1"
+__version__ = "2.29.0"
 
 '''
 Imports should work with python+numpy only agreed with MB 11 Nov 2011
 '''
 try:
     from . import nexus
 except Exception as e:
```

### Comparing `scisoftpy-2.23.1/scisoftpy/crystallography.py` & `scisoftpy-2.29.0/scisoftpy/crystallography.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/data.py` & `scisoftpy-2.29.0/scisoftpy/data.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/dictutils.py` & `scisoftpy-2.29.0/scisoftpy/dictutils.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/diffraction.py` & `scisoftpy-2.29.0/scisoftpy/diffraction.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/external.py` & `scisoftpy-2.29.0/scisoftpy/external.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 # limitations under the License.
 ###
 
 '''External python caller
 '''
 
 from __future__ import print_function
+import inspect
 import os
+import traceback
+
+
 if os.name == 'java':
     _isjava = True
     from .jython.jycore import ndarray, ndgeneric, scalarToPython #@UnusedImport
 else:
     _isjava = False
     from .python.pycore import ndarray, ndgeneric, scalarToPython #@Reimport
 
@@ -126,15 +130,14 @@
         fn = _path.join(d, fa)
         if fn.endswith('.pkl'):
             try:
                 f = open(fn, 'rb')
                 fdict[fa] = _pload(f)
             except:
                 sys.stderr.write('Could not load %s\n' % fa)
-                import traceback
                 traceback.print_exc()
             finally:
                 f.close()
         else:
             from scisoftpy.io import load as _aload
             nd = _aload(fn)
             fdict[fa] = nd if isinstance(nd, ndarray) else nd[0]
@@ -163,17 +166,16 @@
 def wrapper(func):
     '''Decorator to run a function
     '''
     def run_func(*args, **kwargs):
         try:
             ret = func(*args, **kwargs)
         except Exception:
-            import traceback
             ex_type, ex_value, tb = sys.exc_info()
-            error = ex_type, ex_value, traceback.extract_tb(tb)[1:]
+            error = ex_type, ex_value, traceback.format_list(traceback.extract_tb(tb)[1:])
             ret = None
         else:
             error = None
         
         return (ret, error)
 
     return run_func
@@ -184,15 +186,20 @@
     path -- list of paths
     ldpath -- list of dynamic library paths
     return tuple containing python executable string, python path as list 
     '''
 
 #    print 'ScisoftPy package is in', pkg
     if _isjava:
-        pyexe, pypath, pyldpath = _cached_pyenv
+        if _cached_pyenv is None:
+            if exe is None:
+                raise ValueError('Python executable must be specified when no python environment cached')
+            pypath = pyldpath = None
+        else:
+            pyexe, pypath, pyldpath = _cached_pyenv
 
         if exe:
             pyexe = exe
     
         if path is not None:
 #            pypath = [ p for p in sys.path if not p.endswith('jar') ]
             pypath = list(path)
@@ -235,15 +242,15 @@
     return pyexe, pypath, pyldpath
 
 
 _dls_modules = dict() # cache for modules
 
 _PYTHONPATH = 'PYTHONPATH'
 
-def get_dls_module(module='python/2.7', module_init='/etc/profile.d/modules.sh'):
+def get_dls_module(module='python/3.7', module_init='/etc/profile.d/modules.sh'):
     if module in _dls_modules:
         return _dls_modules[module]
 
     if sys.platform == 'win32':
         raise ValueError('Cannot use dls_module argument on Windows')
     elif sys.platform == 'darwin':
         raise ValueError('Cannot use dls_module argument on Mac OS X')
@@ -263,15 +270,15 @@
     p.stdin.close()
     exe, path, ldpath = parse_for_env(p.stdout)
     if exe is None:
         raise RuntimeError('Problem with running external process: ' + p.stderr.read())
     _dls_modules[module] = exe, path, ldpath
     return exe, path, ldpath
 
-def get_python(py3=False):
+def get_python(py3=True):
     env = dict(_env)
     env.pop(_PYTHONPATH, None)
     pyexe = 'python2' if not py3 else 'python3'
     p = sub.Popen(pyexe, env=env, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
     p.stdin.write('import sys\n')
     p.stdin.write('print("EXEC|" + sys.executable)\n')
     p.stdin.write('print("PATH|" + "|".join(sys.path))\n')
@@ -307,15 +314,26 @@
                 path = [a for a in r[1:] if a]
             elif r[0] == 'LDPATH':
                 ldpath = [a for a in r[1:] if a]
 
     return exe, path, ldpath
 
 if _isjava:
-    _cached_pyenv = get_python()
+    try:
+        _cached_pyenv = get_python()
+    except:
+        print('Problem caching python3 environment')
+        ex_type, ex_value, tb = sys.exc_info()
+        try:
+            _cached_pyenv = get_python(False)
+        except:
+            traceback.print_exception(ex_type, ex_value, tb)
+            print('Problem caching python2 environment: ')
+            traceback.print_exc()
+            _cached_pyenv = None
 
 #PYDEV_SRC='/scratch/eclipse441_64/plugins/org.python.pydev_3.9.2.201502050007/pysrc'
 
 def find_module_path(path, module):
     modulefile = module + '.py'
     for p in path:
         p = _path.abspath(p)
@@ -396,15 +414,15 @@
 
     class PythonSubProcess(object):
         READY = 'READY\n'
         TIMEOUT = 0.005
         def __init__(self, exe='python', env=None):
             if env is None:
                 env = dict(os.environ)
-                env.pop(_PYTHONPATH)
+                env.pop(_PYTHONPATH, None)
 #             print('PyExe: %s' % exe, file=sys.stderr)
 #             if _PYTHONPATH in env:
 #                 print('PyEnv: %s' % env[_PYTHONPATH], file=sys.stderr)
             self.proc = sub.Popen([exe, '-c', cmds], bufsize=1, env=env, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
 #             self.out = StreamHandler(self.proc.stdout, 'out')
 #             self.err = StreamHandler(self.proc.stderr, 'err')
             self.out = StreamHandler(self.proc.stdout)
@@ -524,16 +542,15 @@
                     if l.startswith('FWOUT'):
                         r = l.split('|')
                         if len(r) > 1:
                             d = r[1]
                             try:
                                 ret, err = load_args(d)
                                 if err:
-                                    import traceback
-                                    sys.stderr.write('\n'.join(traceback.format_list(err[2])) + '\n')
+                                    sys.stderr.writelines(err[2])
                                     raise err[1]
                                 return ret
                             finally:
                                 shutil.rmtree(d)
                     else:
                         print(l)
             if err:
@@ -581,15 +598,14 @@
             p_parts = _path.split(p)
             for m in reversed(module_parts):
                 if m == p_parts[1]:
                     p = p_parts[0]
                     p_parts = _path.split(p)
     else: # use caller's directory
         p = None
-        import inspect
         stack = inspect.stack()
         if len(stack) > 1:
             f = stack[1][1] # see if module is in directory of previous frame's file
             if _path.exists(f):
                 p = find_module_path([_path.dirname(f)], module)
 
     ldpath = None
```

### Comparing `scisoftpy-2.23.1/scisoftpy/fft.py` & `scisoftpy-2.29.0/scisoftpy/fft.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/fit/__init__.py` & `scisoftpy-2.29.0/scisoftpy/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/flatten.py` & `scisoftpy-2.29.0/scisoftpy/flatten.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/image.py` & `scisoftpy-2.29.0/scisoftpy/image.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/io.py` & `scisoftpy-2.29.0/scisoftpy/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 def setloadwarning(warn):
     '''Assign a default for whether warnings should be shown when loading
     Initially, this is set to True
     '''
     global _LDRWARN
     _LDRWARN = warn
 
-def load(name, format=None, formats=None, withmetadata=True, ascolour=False, warn=None, **kwarg):  # @ReservedAssignment
+def load(name, format=None, formats=None, withmetadata=True, ascolour=False, warn=None, **kwargs):  # @ReservedAssignment
     '''Load a file and return a list of datasets (or a dictionary of datasets) and
     optionally a dictionary of metadata items
 
     format (or formats) -- list of formats to try. Supported input formats:
         png, gif, jpeg, tiff
         adsc, crysalis, mar, pilatus, ocs -> image detectors
         cbf
@@ -82,14 +82,15 @@
         npy (NumPy)
         pgm
         hdf5 -> returns a HDF5 tree
         nx   -> returns a NeXus tree
     withmetadata -- if True, load metadata as well
     ascolour -- if True, attempt load as colour dataset
     warn -- if False, suppress warning
+    **kwargs -- other loader specific keyword arguments
     '''
     if warn is None:
         warn = _LDRWARN
     try:
         f = open(name)
         f.close()
     except:
@@ -140,15 +141,15 @@
 
             try:
                 if l in _colourclasses:
                     ldr = l(name, not ascolour)
                 else:
                     ldr = l(name)
                 ldr.setloadmetadata(withmetadata)
-                lfh = ldr.load(warn=warn)
+                lfh = ldr.load(warn=warn, **kwargs)
                 break
             except _ioexception as e:
                 if warn:
                     errors.append("Could not load using " + l.__name__)
                     errors.extend(str(e).splitlines())
             except:
                 if warn:
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/fitcore.py` & `scisoftpy-2.29.0/scisoftpy/jython/fitcore.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,22 +77,26 @@
         This constructor consumes creates a fit function from given jython function and parameter list
 
         Arguments:
         fn     -- function
         name   -- function name
         plist  -- list of Parameter objects
         '''
+        self.n_params = len(plist)
         _absfn.__init__(self, plist) #@UndefinedVariable
         self.func = fn
         self.args = args
         self.name = name
 
     def setNames(self):
         pass
 
+    def getNoOfParameters(self):
+        return self.n_params
+
     @_wrap
     def val(self, coords):
         '''Evaluate function at single set of coordinates
         '''
         try:
             l = [p for p in self.parameterValues]
             l.append([_dnp.array(c) for c in _toList(coords)])
@@ -114,32 +118,32 @@
             l.append(self.args)
             d = self.func(*l)
             d.name = self.name
             return d
         except ValueError:
             raise ValueError("Problem with function '" + self.name + "' with params  " + self.parameterValues)
 
-    def residual(self, allvalues, data, weights, *coords):
+    def residual(self, allvalues, data, weight, *coords):
         '''Find residual as sum of squared differences of function and data
         
         Arguments:
         allvalues -- boolean, currently ignored
         data      -- used to subtract from evaluated function
-        weights   -- weighting for each squared difference, can be None
+        weight    -- weighting for each squared difference, can be None
         coords    -- coordinates over which the function is evaluated
         '''
         if len(coords) == 0: # workaround deprecated method
-            coords = (weights,)
-            weights = None
+            coords = (weight,)
+            weight = None
         try:
             l = [p for p in self.parameterValues]
             l.append([_sciwrap(c) for c in coords])
             l.append(self.args)
             d = self.func(*l)
-            return _dnp.residual(d, data, weights)
+            return _dnp.residual(d, data, weight)
         except ValueError:
             raise ValueError("Problem with function '" + self.name + "' with params  " + self.parameterValues)
 
 class cfitfunc(_compfn):
     '''Composite function for situation where there's a mixture of jython and Java fitting functions
     '''
     def __init__(self):
@@ -165,41 +169,43 @@
             v = _sciwrap(self.getFunction(n).calculateValues(*coords))
             if vt is None:
                 vt = v
             else:
                 vt += v
         return vt
 
-    def residual(self, allvalues, data, weights, coords):
+    def residual(self, allvalues, data, weight, coords):
         '''Find residual as sum of squared differences of function and data
         
         Arguments:
         allvalues -- boolean, currently ignored 
         data      -- used to subtract from evaluated function
-        weights   -- weighting for each squared difference, can be None
+        weight    -- weighting for each squared difference, can be None
         coords    -- coordinates over which the function is evaluated
         '''
         if len(coords) == 0: # workaround deprecated method
-            coords = (weights,)
-            weights = None
-        return _dnp.residual(self.calculateValues(coords), data, weights)
+            coords = (weight,)
+            weight = None
+        return _dnp.residual(self.calculateValues(coords), data, weight)
 
 
 class fitresult(object):
     '''This is used to contain results from a fit
     '''
-    def __init__(self, func, coords, data):
+    def __init__(self, func, coords, data, weight=None):
         '''Arguments:
-        func   -- function after fitting as occurred
-        coords -- coordinate(s)
-        data   -- scalar dataset that was fitted to
+        func    -- function after fitting as occurred
+        coords  -- coordinate(s)
+        data    -- scalar data that was fitted to
+        weight -- array used to weight residuals (it multiplies the squared differences between function and data)
         '''
         self.func = func
         self.coords = coords
         self.data = data
+        self.weight = weight
 
     def _calcdelta(self, coords):
         delta = 1.
         r = coords[0].ndim
         if r > 1:
             for n in range(len(coords)):
                 x = coords[n]
@@ -223,34 +229,34 @@
             raise IndexError
 
     def __len__(self):
         '''Number of parameters
         '''
         return self.func.getNoOfParameters()
 
-    def makeplotdata(self, all=True):
+    def makeplotdata(self, all=True, log10=False):
         '''Make a list of datasets to plot
-        all   -- if True, then make datasets for all functions
+        all   -- if True, then make datasets for all constituent functions and difference
         '''
-        pdata = self.makefuncdata(all=all)
-        pdata.insert(0, self.data)
+        odata = self.makefuncdata(all=all)
+        odata.insert(0, self.data)
+        
+        pdata = [ _dnp.log10(_dnp.abs(p)) for p in odata ] if log10 else odata
+        if log10:
+            lomin = pdata[0].min() # crop to log10(data)
+            pdata = [ _dnp.maximum(p, lomin) for p in pdata ]
+
         if all:
-            offset = self.data.min() - ((self.data.max() - self.data.min()) / 5.0)
-            edata = self.data - pdata[1] + offset
-            edata.name = "Error value"
-            odata = _dnp.zeros_like(edata)
-            odata.fill(offset)
-            odata.name = "Error offset"
-            pdata.insert(2, odata)
-            pdata.insert(2, edata)
+            edata = self.data - odata[1]
+            pdata.append(edata)
         return pdata
 
     def makefuncdata(self, all=True):
         '''Make a list of datasets for composite fitting function and its components
-        all   -- if True, then make datasets for all contributing functions
+        all   -- if True, then make datasets for all constituent functions and difference
         '''
         nf = self.func.noOfFunctions
         coords = _jinput(self.coords)
         if nf >= 1:
             fdata = [_sciwrap(self.func.calculateValues(coords))]
             if all:
                 if nf > 1:
@@ -258,21 +264,27 @@
                 for n in range(nf):
                     fdata.append(_sciwrap(self.func.getFunction(n).calculateValues(*coords)))
         else:
             fdata = []
 
         return fdata
 
-    def plot(self, title=None, name=None, all=False):
+    def plot(self, title=None, name=None, all=False, log10=False):
         '''Plot fit as 1D
         title -- title of plot
         name  -- name of plot view to use (if None, use default name)
-        all   -- if True, then plot all
+        all   -- if True, then plot all constituent functions and difference
+        log10 -- if True, then take log10 of data and function (
         '''
-        _dnp.plot.line(self.coords[0], self.makeplotdata(all=all), title, name)
+        pd = self.makeplotdata(all=all, log10=log10)
+        if all:
+            ed = pd.pop()
+        _dnp.plot.line(self.coords[0], pd, title, name)
+        if all:
+            _dnp.plot.addline(self.coords[0], {('', 'right'):(ed, 'error')}, name)
 
     def _parameters(self):
         '''Array of all parameter values
         '''
         return _asDS([p for p in self.func.getParameterValues()])
     parameters = property(_parameters)
 
@@ -305,34 +317,37 @@
                 np = len(p)
                 out += "    function '%s' (%d) has %d parameters = %s\n" % (f.name, n, np, p)
         else:
             f = self.func.getFunction(n)
             p = [q for q in f.getParameterValues()]
             np = len(p)
             out += "    function '%s' has %d parameters = %s\n" % (f.name, np, p)
-            
+        out += "Residual: %g\n" % self.residual
         return out
 
 import inspect as _inspect
 
-def fit(func, coords, data, p0, bounds=[], args=None, ptol=1e-4, seed=None, optimizer="apache_nm"):
+ALL_OPTIMIZERS = ('simplex','genetic', 'gradient','apache_nm','apache_md','apache_cg')
+
+def fit(func, coords, data, p0, bounds=[], args=None, weight=None, ptol=1e-4, seed=None, optimizer="apache_nm"):
     '''
     Arguments:
     func      -- function (or list of functions)
     coords    -- coordinate dataset(s)
     data      -- data to fit
     p0        -- list of initial parameters
     bounds    -- list of parameter bounds, bounds are tuples of lower and upper values (any can be None)
-    args      -- extra arguments
+    args      -- extra arguments (for functions)
+    weight    -- dataset used to weight residuals (it multiplies the squared differences between function and data)
     ptol      -- parameter fit tolerance
     seed      -- seed value for genetic algorithm-based optimiser
     optimizer -- description of the optimizer to use, e.g. ['local','global','simplex','genetic',
-                 'gradient','apache_nm','apache_md','apache_cg']
+                 'gradient','apache_nm','apache_md','apache_cg','apache_lm']
                  local and global are general settings, which point the one of the specific methods
-                 If any global methods are picked, the bounds argument must also be filled in.
+                 (Nelder Mead, Genetic). If any global methods are picked, the bounds argument must also be filled in.
     Returns:
     fitresult object
     '''
     fnlist = []
     func = _toList(func)
     p0 = _toList(p0)
     if not isinstance(bounds, list):
@@ -379,38 +394,41 @@
             coords[i] = c[ns]
 
     if seed:
         _fitter.seed = int(seed)
 
     jcoords = [ __cvt_jobj(c, copy=False, force=True) for c in coords ]
     jdata = data._jdataset()
+    jweight = None if weight is None else weight._jdataset()
 
     # use the appropriate fitter for the task
     if optimizer == 'local':
-        _fitter.ApacheNelderMeadFit(jcoords, jdata, cfunc)
+        _fitter.ApacheNelderMeadFit(jcoords, jdata, jweight, cfunc)
     elif optimizer == 'global':
         if n_bounds == 0:
             print("Using a global optimizer with no bounds is unlikely to work, please use the bounds argument to narrow the search space")
-        _fitter.geneticFit(ptol, jcoords, jdata, cfunc)
+        _fitter.geneticFit(ptol, jcoords, jdata, jweight, cfunc)
     elif optimizer == 'simplex':
-        _fitter.simplexFit(ptol, jcoords, jdata, cfunc)
+        _fitter.simplexFit(ptol, jcoords, jdata, jweight, cfunc)
     elif optimizer == 'gradient':
-        _fitter.GDFit(ptol, jcoords, jdata, cfunc)
+        _fitter.GDFit(ptol, jcoords, jdata, jweight, cfunc)
     elif optimizer == 'apache_nm':
-        _fitter.ApacheNelderMeadFit(jcoords, jdata, cfunc)
+        _fitter.ApacheNelderMeadFit(jcoords, jdata, jweight, cfunc)
     elif optimizer == 'apache_md':
-        _fitter.ApacheMultiDirectionFit(jcoords, jdata, cfunc)
+        _fitter.ApacheMultiDirectionFit(jcoords, jdata, jweight, cfunc)
     elif optimizer == 'apache_cg':
-        _fitter.ApacheConjugateGradientFit(jcoords, jdata, cfunc)
+        _fitter.ApacheConjugateGradientFit(jcoords, jdata, jweight, cfunc)
+    elif optimizer == 'apache_lm':
+        _fitter.ApacheLevenbergMarquardtFit(jcoords, jdata, jweight, cfunc)
     elif optimizer == 'genetic':
         if n_bounds == 0:
             print("Using a global optimizer with no bounds is unlikely to work, please use the bounds argument to narrow the search space")
-        _fitter.geneticFit(ptol, jcoords, jdata, cfunc)
+        _fitter.geneticFit(ptol, jcoords, jdata, jweight, cfunc)
 
-    return fitresult(cfunc, coords, data)
+    return fitresult(cfunc, coords, data, weight)
 
 # genfit = _genfit
 
 def _polycoeff(roots):
     '''Calculate polynomial coefficients from roots'''
     nr = len(roots)
     oc = [1.0]
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/function.py` & `scisoftpy-2.29.0/scisoftpy/jython/function.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jybeans.py` & `scisoftpy-2.29.0/scisoftpy/jython/jybeans.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jycomparisons.py` & `scisoftpy-2.29.0/scisoftpy/jython/jycomparisons.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jycore.py` & `scisoftpy-2.29.0/scisoftpy/jython/jycore.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,44 +28,51 @@
 import org.eclipse.january.dataset.ShortDataset as _shortds
 import org.eclipse.january.dataset.IntegerDataset as _integerds
 import org.eclipse.january.dataset.LongDataset as _longds
 import org.eclipse.january.dataset.CompoundByteDataset as _cpdbyteds
 import org.eclipse.january.dataset.CompoundShortDataset as _cpdshortds
 import org.eclipse.january.dataset.CompoundIntegerDataset as _cpdintegerds
 import org.eclipse.january.dataset.CompoundLongDataset as _cpdlongds
-import org.eclipse.january.dataset.RGBDataset as _rgbds
+import org.eclipse.january.dataset.RGBByteDataset as _rgbds
 import org.eclipse.january.dataset.FloatDataset as _floatds
 import org.eclipse.january.dataset.DoubleDataset as _doubleds
 import org.eclipse.january.dataset.ComplexFloatDataset as _cpxfloatds
 import org.eclipse.january.dataset.ComplexDoubleDataset as _cpxdoubleds
 import org.eclipse.january.dataset.CompoundFloatDataset as _cpdfloatds
 import org.eclipse.january.dataset.CompoundDoubleDataset as _cpddoubleds
 import org.eclipse.january.dataset.DateDataset as _dateds
 import org.eclipse.january.dataset.StringDataset as _stringds
 
 import org.eclipse.january.dataset.DatasetUtils as _dsutils
 import org.eclipse.january.dataset.InterfaceUtils as _ifutils
+import org.eclipse.january.dataset.ShapeUtils as _shutils
 from uk.ac.diamond.scisoft.python.PythonUtils import convertToJava as _cvt2j
 from uk.ac.diamond.scisoft.python.PythonUtils import getSlice as _getslice
 from uk.ac.diamond.scisoft.python.PythonUtils import setSlice as _setslice
 from uk.ac.diamond.scisoft.python.PythonUtils import convertToSlice as _cvt2js
 from uk.ac.diamond.scisoft.python.PythonUtils import getInterfaceFromObject as _getdt
 from uk.ac.diamond.scisoft.python.PythonUtils import createFromObject as _create
+from uk.ac.diamond.scisoft.python.PythonUtils import callIBArgsMethod as _callIB
+from uk.ac.diamond.scisoft.python.PythonUtils import callIBBArgsMethod as _callIBB
+from uk.ac.diamond.scisoft.python.PythonUtils import concatenate as _concatenate
 
 import org.apache.commons.math3.complex.Complex as _jcomplex #@UnresolvedImport
 
 import Jama.Matrix as _matrix #@UnresolvedImport
 
 import inspect
 
 import java.lang.ArrayIndexOutOfBoundsException as _jarrayindex_exception #@UnresolvedImport
 import java.lang.IllegalArgumentException as _jillegalargument_exception #@UnresolvedImport
 
 from functools import wraps
 
+class AxisError(ValueError):
+    pass
+
 def quieten_logging(netty_only=True):
     '''
     Quieten logging to warnings and above
     
     :param netty_only: True then only quieten messages from Netty's DefaultChannelPipeline
     '''
     try:
@@ -428,15 +435,15 @@
 def _keepdims(func):
     '''
     Retain dimensions of output array
     '''
     @wraps(func)
     def new_f(*args, **kwargs):
         keepdims = kwargs.get('keepdims', False)
-        axis = kwargs.get('axis', None)    
+        axis = kwargs.get('axis', None)
         if keepdims:
             if axis is None:
                 dimensionality = (1,) * len(args[0].shape)
             elif isinstance(axis, int):
                 dimensionality = list(args[0].shape)
                 dimensionality[axis] = 1
             elif isinstance(axis, tuple):
@@ -589,37 +596,46 @@
             return obj.cast(dtype.value)
 
     if not isinstance(obj, list):
         if isinstance(obj, _matrix): # cope with JAMA matrices
             if dtype is None:
                 dtype = float64
             obj = obj.getArray()
-    elif len(obj) == 0 and dtype is None:
-        dtype = float64
 
     obj = _cvt2j(obj)
     try:
         iter(obj)
     except:
         if not force:
             if isinstance(obj, complex):
                 return _jcomplex(obj.real, obj.imag)
             return obj
 
     if dtype is None:
-        dtype = _getdtypefromobj(obj)
+        dtype = float64 if _shutils.isZeroSize(_shutils.getShapeFromObject(obj)) else _getdtypefromobj(obj)
 
     return _create(dtype.value, obj)
 
 # prevent incorrect coercion of Python booleans causing trouble with overloaded Java methods
 import java.lang.Boolean as _jbool #@UnresolvedImport
 _jtrue = _jbool(1)
 _jfalse = _jbool(0)
+_jatrue = _array((True,), 'z')
+_jafalse = _array((False,), 'z')
 import java.lang.Integer as _jint
 
+def _jintarray(*ij):
+    if len(ij) == 1:
+        i = ij[0]
+        if i is None:
+            return None
+        if isinstance(i, (tuple, list)):
+            ij = ij[0]
+    return _array(ij, 'i')
+
 from . import jymaths as _maths
 from . import jycomparisons as _cmps
 
 _jempty = tuple()
 
 class lazyarray(object):
     def __init__(self, dataset, shape=None, dtype=None, maxshape=None, attrs={}, parent=None):
@@ -948,129 +964,71 @@
     # MISSING: searchsorted
     # MISSING: compress, diagonal
 
     #  calculation
     @_wrapout
     @_keepdims
     def max(self, axis=None, ignore_nans=False, keepdims=False): #@ReservedAssignment
-        if axis is None:
-            if ignore_nans:
-                return self.__dataset.max(_jtrue)
-            return self.__dataset.max(_empty_boolean_array)
-        elif isinstance(axis, int):
-            if ignore_nans:
-                return self.__dataset.max(_jint(axis), _jtrue)
-            return self.__dataset.max(_jint(axis))
-        elif isinstance(axis, tuple):
-            if ignore_nans:
-                return self.__dataset.max(asarray([_jint(x) for x in axis]), _jtrue)
-            return self.__dataset.max(asarray([_jint(x) for x in axis]))
+        return _callIB(self.__dataset, "max", _jintarray(axis), _jatrue if ignore_nans else None)
 
     @_wrapout
     @_keepdims
     def min(self, axis=None, ignore_nans=False, keepdims=False): #@ReservedAssignment
-        if axis is None:
-            if ignore_nans:
-                return self.__dataset.min(_jtrue)
-            return self.__dataset.min(_empty_boolean_array)
-        elif isinstance(axis, int):
-            if ignore_nans:
-                return self.__dataset.min(_jint(axis), _jtrue)
-            return self.__dataset.min(_jint(axis))
-        elif isinstance(axis, tuple):
-            if ignore_nans:
-                return self.__dataset.min(asarray([_jint(x) for x in axis]), _jtrue)
-            return self.__dataset.min(asarray([_jint(x) for x in axis]))
+        return _callIB(self.__dataset, "min", _jintarray(axis), _jatrue if ignore_nans else None)
 
     @_wrapout
     def argmax(self, axis=None, ignore_nans=False):
-        if axis is None:
-            if ignore_nans:
-                return self.__dataset.argMax(_jtrue)
-            return self.__dataset.argMax(_empty_boolean_array)
-        else:
-            if ignore_nans:
-                return self.__dataset.argMax(_jint(axis), _jtrue)
-            return self.__dataset.argMax(_jint(axis))
+        return _callIB(self.__dataset, "argMax", _jintarray(axis), _jatrue if ignore_nans else None)
 
     @_wrapout
     def argmin(self, axis=None, ignore_nans=False):
-        if axis is None:
-            if ignore_nans:
-                return self.__dataset.argMin(_jtrue)
-            return self.__dataset.argMin(_empty_boolean_array)
-        else:
-            if ignore_nans:
-                return self.__dataset.argMin(_jint(axis), _jtrue)
-            return self.__dataset.argMin(_jint(axis))
+        return _callIB(self.__dataset, "argMin", _jintarray(axis), _jatrue if ignore_nans else None)
 
     @_wrapout
     @_keepdims
-    def ptp(self, axis=None, keepdims=False):
-        if axis is None:
-            return self.__dataset.peakToPeak(_empty_boolean_array)
-        elif isinstance(axis, int):
-            return self.__dataset.peakToPeak(_jint(axis))
-        elif isinstance(axis, tuple):
-            return self.__dataset.peakToPeak(asarray([_jint(x) for x in axis]))
+    def ptp(self, axis=None, ignore_nans=False, keepdims=False):
+        return _callIB(self.__dataset, "peakToPeak", _jintarray(axis), _jatrue if ignore_nans else None)
 
     def clip(self, a_min, a_max):
         return _maths.clip(self, a_min, a_max)
 
     def conj(self):
         return _maths.conj(self)
 
     # MISSING: round, trace
     @_wrapout
     def sum(self, axis=None, dtype=None, keepdims=False):
-        return _maths.sum(self, axis, dtype, keepdims=keepdims)
+        return _maths.sum(self, axis=axis, dtype=dtype, keepdims=keepdims)
 
     def cumsum(self, axis=None, dtype=None):
         return _maths.cumsum(self, axis, dtype, keepdims=keepdims)
 
     @_wrapout
     @_keepdims
     def mean(self, axis=None, keepdims=False):
-        if axis is None:
-            return self.__dataset.mean(_empty_boolean_array)
-        elif isinstance(axis, int):
-            return self.__dataset.mean(_jint(axis))
-        elif isinstance(axis, tuple):
-            return self.__dataset.mean(asarray([_jint(x) for x in axis]))
+        return _callIB(self.__dataset, "mean", _jintarray(axis), None)
 
     @_wrapout
     @_keepdims
     def var(self, axis=None, ddof=0, keepdims=False):
         is_pop = _jbool(ddof == 0)
-        if axis is None:
-            return self.__dataset.variance(is_pop)
-        elif isinstance(axis, int):
-            return self.__dataset.variance(_jint(axis), is_pop)
-        elif isinstance(axis, tuple):
-            return self.__dataset.variance(asarray([_jint(x) for x in axis]), is_pop)
+        return _callIBB(self.__dataset, "variance", _jintarray(axis), is_pop, None)
 
     @_wrapout
     @_keepdims
     def std(self, axis=None, ddof=0, keepdims=False):
         is_pop = _jbool(ddof == 0)
-        if axis is None:
-            return self.__dataset.stdDeviation(is_pop)
-        elif isinstance(axis, int):
-            return self.__dataset.stdDeviation(_jint(axis), is_pop)
-        elif isinstance(axis, tuple):
-            return self.__dataset.stdDeviation(asarray([_jint(x) for x in axis]), is_pop)
+        return _callIBB(self.__dataset, "stdDeviation", _jintarray(axis), is_pop, None)
 
     @_wrapout
     def rms(self, axis=None):
-        if axis is None:
-            return self.__dataset.rootMeanSquare()
-        return self.__dataset.rootMeanSquare(_jint(axis))
+        return _callIB(self.__dataset, "rootMeanSquare", _jintarray(axis), None)
 
     def prod(self, axis=None, dtype=None, keepdims=False):
-        return _maths.prod(self, axis, dtype, keepdims=keepdims)
+        return _maths.prod(self, axis=axis, dtype=dtype, keepdims=keepdims)
 
     def cumprod(self, axis=None, dtype=None):
         return _maths.cumprod(self, axis, dtype)
 
     @_wrapout
     @_keepdims
     def all(self, axis=None, keepdims=False): #@ReservedAssignment
@@ -1348,47 +1306,47 @@
     def __init__(self, shape=None, dtype=None, buffer=None, copy=False): #@ReservedAssignment
         super(ndarrayRGB, self).__init__(shape=shape, dtype=dtype, buffer=buffer, copy=copy)
 
     @_wrapout
     def get_red(self, dtype=None):
         dtype = _translatenativetype(dtype)
         if dtype is None:
-            dtype = int16
-        if dtype != int16:
+            dtype = int8
+        if dtype != int8:
             return self._jdataset().createRedDataset(dtype.value)
         return self._jdataset().getRedView()
 
     @_wrapout
     def get_green(self, dtype=None):
         dtype = _translatenativetype(dtype)
         if dtype is None:
-            dtype = int16
-        if dtype != int16:
+            dtype = int8
+        if dtype != int8:
             return self._jdataset().createGreenDataset(dtype.value)
         return self._jdataset().getGreenView()
 
     @_wrapout
     def get_blue(self, dtype=None):
         dtype = _translatenativetype(dtype)
         if dtype is None:
-            dtype = int16
-        if dtype != int16:
+            dtype = int8
+        if dtype != int8:
             return self._jdataset().createBlueDataset(dtype.value)
         return self._jdataset().getBlueView()
 
     @_wrapout
     def get_grey(self, cweights=None, dtype=None):
         '''Get grey image
         
         Arguments:
         cweights -- optional set of weight for combining the colour channel
         dtype    -- optional dataset type (default is int16)'''
         dtype = _translatenativetype(dtype)
         if dtype is None:
-            dtype = int16
+            dtype = int8
         if cweights:
             cweights = asIterable(cweights)
             if len(cweights) != 3:
                 raise ValueError("three colour channel weights needed")
             csum = float(sum(cweights))
             return self._jdataset().createGreyDataset(dtype.value, cweights[0]/csum, cweights[1]/csum, cweights[2]/csum)
         return self._jdataset().createGreyDataset(dtype.value)
@@ -1657,39 +1615,75 @@
 
 @_wrapout
 def atleast_3d(*arrays):
     '''Return list of datasets that are at least 3d'''
     res = _jatleast_3d(arrays)
     return res if len(res) > 1 else res[0]
 
+def expand_dims(a, axis):
+    '''Expand dimensions by inserting 1s in shape'''
+    if isinstance(axis, int):
+        axis = [axis,]
+    else:
+        axis = list(axis)
+    
+    r = a.ndim + len(axis)
+    for n,i in enumerate(axis):
+        if i < -r or i >= r:
+            raise AxisError('Axis value %d must be in [%d, %d)' % (i, -r, r))
+        if i < 0:
+            axis[n] = i + r
+
+    # i = 0
+    # ashape = a.shape
+    # shape = []
+    # for ax in range(r):
+    #     if ax in axis:
+    #         j = 1
+    #     else:
+    #         j = ashape[i]
+    #         i += 1
+    #     shape.append(j)
+    sit = iter(a.shape)
+    shape = [1 if ax in axis else next(sit) for ax in range(r)]
+    return a.reshape(shape)
+
 @_wrapout
 def concatenate(a, axis=0):
     a = [array(arr_like) if (not isinstance(arr_like, ndarray)) else arr_like for arr_like in a]
     a = [_jinput(arr) for arr in a]
-    return _dsutils.concatenate(a, axis)
+    return _concatenate(a, axis)
+
+@_wrapout
+def stack(a, axis=0):
+    if not isinstance(axis, int):
+        raise A('axis must be an integer')
+    a = [array(arr_like) if (not isinstance(arr_like, ndarray)) else arr_like for arr_like in a]
+    a = [_jinput(expand_dims(arr, axis)) for arr in a]
+    return _concatenate(a, axis)
 
 @_wrapout
 def vstack(tup):
     arr = [atleast_2d(t)._jdataset() for t in tup ]
-    return _dsutils.concatenate(arr, 0)
+    return _concatenate(arr, 0)
 
 @_wrapout
 def hstack(tup):
     arr = _jatleast_1d(toList(tup))
-    return _dsutils.concatenate(arr, 0) if arr[0].getRank() == 1 else _dsutils.concatenate(arr, 1)
+    return _concatenate(arr, 0 if arr[0].getRank() == 1 else 1)
 
 @_wrapout
 def dstack(tup):
     arr = [atleast_3d(t)._jdataset() for t in tup ]
-    return _dsutils.concatenate(arr, 2)
+    return _concatenate(arr, 2)
 
 @_wrapout
 def column_stack(tup):
     arr = [t._jdataset() if t.ndim >= 2 else atleast_2d(t).T._jdataset() for t in tup ]
-    return _dsutils.concatenate(arr, 1)
+    return _concatenate(arr, 1)
 
 @_wrap
 def split(ary, indices_or_sections, axis=0):
     return _dsutils.split(ary, indices_or_sections, axis, True)
 
 @_wrap
 def array_split(ary, indices_or_sections, axis=0):
@@ -1718,15 +1712,15 @@
 def tile(a, reps):
     return _dsutils.tile(a, _as_int_array(reps))
 
 @_wrap('a')
 def repeat(a, repeats, axis=None):
     if axis is None:
         axis = -1
-    if a.getRank() == 0: # FIXME bug in january 2.2
+    if a.getRank() == 0: # FIXME bug in january 2.3
         a = a.reshape(1)
     return _dsutils.repeat(a, asIterable(repeats), axis)
 
 @_wrap('arr', 'values')
 def append(arr, values, axis=None):
     '''Append values to end of array
     Keyword argument:
@@ -1771,27 +1765,29 @@
 
 @_wrap('a')
 def swapaxes(a, axis1, axis2):
     return _dsutils.swapAxes(a, axis1, axis2)
 
 @_argsToArrayType('a')
 def amax(a, axis=None, keepdims=False):
-    return a.max(axis, keepdims=keepdims)
+    '''Maximum of input'''
+    return a.max(axis=axis, keepdims=keepdims)
 
 @_argsToArrayType('a')
 def amin(a, axis=None, keepdims=False):
-    return a.min(axis, keepdims=keepdims)
+    '''Minimum of input'''
+    return a.min(axis=axis, keepdims=keepdims)
 
 @_argsToArrayType('a')
 def nanmax(a, axis=None, keepdims=False):
-    return a.max(axis, ignore_nans=True, keepdims=keepdims)
+    return a.max(axis=axis, ignore_nans=True, keepdims=keepdims)
 
 @_argsToArrayType('a')
 def nanmin(a, axis=None, keepdims=False):
-    return a.min(axis, ignore_nans=True, keepdims=keepdims)
+    return a.min(axis=axis, ignore_nans=True, keepdims=keepdims)
 
 @_argsToArrayType('a')
 def argmax(a, axis=None):
     return a.argmax(axis)
 
 @_argsToArrayType('a')
 def argmin(a, axis=None):
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jycrystallography.py` & `scisoftpy-2.29.0/scisoftpy/jython/jycrystallography.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jydata.py` & `scisoftpy-2.29.0/scisoftpy/jython/jydata.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jydiffraction.py` & `scisoftpy-2.29.0/scisoftpy/jython/jydiffraction.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyfft.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyfft.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyflatten.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyflatten.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyhdf5io.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyhdf5io.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             return True, key
         return False, (key,)
 
     return _isslice(rank, key), key
 
 
 class SDS(_hdataset):
-    def __init__(self, dataset, attrs, parent):
+    def __init__(self, dataset, attrs, parent, warn):
         if isinstance(dataset, _jdnode):
             if dataset.isString() or not dataset.isSupported():
                 dataset = asarray(dataset.getString())
                 shape = None
                 dtype = None
                 maxshape = None
                 self.rank = dataset.ndim
@@ -88,15 +88,15 @@
         else:
             dataset = asarray(dataset)
             shape = None
             dtype = None
             maxshape = None
             self.rank = dataset.ndim
 
-        _hdataset.__init__(self, dataset, shape, dtype, maxshape, attrs, parent)
+        _hdataset.__init__(self, dataset, shape, dtype, maxshape, attrs, parent, warn)
 
     @_wrapout
     def __getitem__(self, key):
         data = self._getdata()
         if isinstance(data, _ldataset):
             isslice, key = _toslice(self.rank, key)
             if not isslice: # single item
@@ -113,15 +113,15 @@
     def __init__(self, name):
         if _hdf5loader is None:
             raise io_exception("HDf5 loader could not be imported")
         self.ldr = _hdf5loader(name)
 
     def load(self, warn=True):
         tree = self._load_tree()
-
+        self.warn = warn
         if tree is None:
             raise io_exception("No tree found")
 
         # convert tree to own tree
         r = tree.getNodeLink()
         pool = dict()
         return self._copynode(pool, r, tree)
@@ -140,18 +140,18 @@
 
         return tree
 
     def _mkgroup(self, name, link, attrs, parent):
         if isinstance(parent, _jtree):
             src = parent.getFilename() if isinstance(parent, _jtreefile) else parent.getSourceURI()
             return _tree(src, attrs, parent)
-        return _group(attrs, parent)
+        return _group(attrs, parent, self.warn)
 
     def _mkdataset(self, dataset, attrs, parent):
-        return SDS(dataset, attrs, parent)
+        return SDS(dataset, attrs, parent, self.warn)
 
     def _copynode(self, pool, link, parent=None):
         node = link.getDestination()
         nid = node.getID()
 #        print link.getName(), nid
         if nid in pool:
             return pool[nid]
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyimage.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyimage.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyio.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyio.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jylinalg.py` & `scisoftpy-2.29.0/scisoftpy/jython/jylinalg.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jymaths.py` & `scisoftpy-2.29.0/scisoftpy/jython/jymaths.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###
+from scisoftpy.jython.jycore import _jintarray
 
 '''
 Maths package
 '''
 
 import org.eclipse.january.dataset.Dataset as _ds
 import org.eclipse.january.dataset.Maths as _maths
 import org.eclipse.january.dataset.Stats as _stats
+from uk.ac.diamond.scisoft.python.PythonUtils import callIBArgsMethod as _callIB
+from uk.ac.diamond.scisoft.python.PythonUtils import callDIBArgsStaticMethod as _callDIBStatic
 
 from math import pi as _ppi
 from math import e as _e
 from java.lang.Double import POSITIVE_INFINITY as _jinf #@UnresolvedImport
 from java.lang.Double import MAX_VALUE as _jmax #@UnresolvedImport
 from java.lang.Double import NaN as _jnan #@UnresolvedImport
 
@@ -35,82 +38,59 @@
 
 floatmax = _jmax # maximum float value (use sys.float_info.max for 2.6+)
 
 from .jycore import _wrap, _jint, _argsToArrayType, _keepdims
 from .jycore import asarray as _asarray
 from .jycore import float64 as _f64
 from .jycore import _translatenativetype, _empty_boolean_array
+from .jycore import toList as _toList
 
 # these functions can call (wrapped) instance methods
 @_keepdims
 @_wrap('a')
 def prod(a, axis=None, dtype=None, keepdims=False):
     '''Product of input'''
     if dtype is None:
-        if axis is None:
-            return a.product(_empty_boolean_array)
-        elif isinstance(axis, int):
-            return a.product(_jint(axis))
-        elif isinstance(axis, tuple):
-            return a.product([_jint(x) for x in axis])
+        return _callIB(a, "product", _jintarray(axis), None)
     dtval = _translatenativetype(dtype).value
     if axis is None:
         return _stats.typedProduct(a, dtval)
     return _stats.typedProduct(a, dtval, axis)
 
 @_keepdims
 @_wrap('a')
 def sum(a, axis=None, dtype=None, keepdims=False): #@ReservedAssignment
     '''Sum of input'''
     if dtype is not None:
         dtval = _translatenativetype(dtype).value
         a = a.cast(dtval)
 
-    if axis is None:
-        return a.sum(_empty_boolean_array)
-    elif isinstance(axis, int):
-        return a.sum(_jint(axis))
-    elif isinstance(axis, tuple):
-        return a.sum([_jint(x) for x in axis])
+    return _callIB(a, "sum", _jintarray(axis), None)
+
+# TODO add nansum, etc
 
-@_keepdims
 @_argsToArrayType('a')
 def mean(a, axis=None, keepdims=False):
     '''Arithmetic mean of input'''
-    return a.mean(axis)
+    return a.mean(axis=axis, keepdims=keepdims)
 
-@_keepdims
 @_argsToArrayType('a')
 def std(a, axis=None, ddof=0, keepdims=False):
     '''Standard deviation of input'''
-    return a.std(axis, ddof)
+    return a.std(axis=axis, ddof=ddof, keepdims=keepdims)
 
-@_keepdims
 @_argsToArrayType('a')
 def var(a, axis=None, ddof=0, keepdims=False):
     '''Variance of input'''
-    return a.var(axis, ddof)
+    return a.var(axis=axis, ddof=ddof, keepdims=keepdims)
 
-@_keepdims
 @_argsToArrayType('a')
 def ptp(a, axis=None, keepdims=False):
     '''Peak-to-peak of input'''
-    return a.ptp(axis)
-
-@_keepdims
-@_argsToArrayType('a')
-def amax(a, axis=None, keepdims=False):
-    '''Maximum of input'''
-    return a.max(axis)
-
-@_keepdims
-@_argsToArrayType('a')
-def amin(a, axis=None, keepdims=False):
-    '''Minimum of input'''
-    return a.min(axis)
+    return a.ptp(axis=axis, keepdims=keepdims)
 
 @_argsToArrayType('a')
 def real(a):
     '''Real part of input'''
     return _asarray(a).real
 
 @_argsToArrayType('a')
@@ -399,34 +379,56 @@
     '''Median of input'''
     if axis is None:
         return _stats.median(a)
     else:
         return _stats.median(a, axis)
 
 @_wrap('a')
+def quantile(a, q, axis=None):
+    '''Quantile (or inverse cumulative distribution) function based on input
+
+    a -- data
+    q -- probability value(s)
+    axis -- can be None'''
+    q = _toList(q)
+    if axis is None:
+        if len(q) == 1:
+            return _stats.quantile(a, q)[0]
+        return _stats.quantile(a, q)
+    else:
+        if len(q) == 1:
+            return _stats.quantile(a, axis, q)[0]
+        return _stats.quantile(a, axis, q)
+
+@_wrap('a')
+def precentile(a, p, axis=None):
+    '''Quantile (or inverse cumulative distribution) function based on input
+    a -- data
+    p -- percentile value(s), must be between 0 and 100 inclusive
+    axis -- can be None'''
+    q = [ i / 100. for i in _toList(p) ]
+    return quantile(a, q, axis)
+
+@_wrap('a')
 def cumprod(a, axis=None, dtype=None):
     '''Cumulative product of input'''
     dtype = _translatenativetype(dtype)
     if dtype is not None:
         a = a.cast(_translatenativetype(dtype).value)
-    if axis is None:
-        return _stats.cumulativeProduct(a)
-    else:
-        return _stats.cumulativeProduct(a, _jint(axis))
+    return _callDIBStatic(_stats, "cumulativeProduct", a, _jintarray(axis), None)
 
 @_wrap('a')
 def cumsum(a, axis=None, dtype=None):
     '''Cumulative sum of input'''
     dtype = _translatenativetype(dtype)
     if dtype is not None:
         a = a.cast(_translatenativetype(dtype).value)
-    if axis is None:
-        return _stats.cumulativeSum(a)
-    else:
-        return _stats.cumulativeSum(a, _jint(axis))
+    return _callDIBStatic(_stats, "cumulativeSum", a, _jintarray(axis), None)
+
+# TODO nancumsum, etc
 
 @_wrap('a')
 def diff(a, order=1, axis=-1):
     '''Difference of input'''
     return _maths.difference(a, order, axis)
 
 import uk.ac.diamond.scisoft.analysis.dataset.function.Histogram as _histo
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jynxio.py` & `scisoftpy-2.29.0/scisoftpy/jython/jynxio.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 
 class NXLoader(_h5loader):
     def _mkgroup(self, name, link, attrs, parent):
         cls = link.getDestination().getAttribute('NX_class')
         if cls is not None:
             cls = cls.getFirstElement()
             if cls in _nx.NX_CLASSES:
-                g = _nx.NX_CLASSES[cls](attrs, parent)
+                g = _nx.NX_CLASSES[cls](attrs, parent, self.warn)
             else:
                 if cls:
                     print("Unknown Nexus class: %s" % cls)
                 g = super(NXLoader, self)._mkgroup(name, link, attrs, parent)
         elif name == '/' or isinstance(parent, _jtree):
             src = parent.getFilename() if isinstance(parent, _jtreefile) else parent.getSourceURI()
-            g = _nx.NXroot(src, attrs, parent)
+            g = _nx.NXroot(src, attrs, parent, self.warn)
         else:
-            g = _nx.NXobject(attrs, parent)
+            g = _nx.NXobject(attrs, parent, self.warn)
 
         return g
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyplot.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,20 +129,19 @@
             else:
                 l = None
             v = l
         nb[k] = v
     return nb
 
 def _unwrap_gui_bean(ob, nb):
-    for k in ob:
-        v = ob[k]
+    for k, v in ob.items():
         if k == _jyparams.roilist:
             if isinstance(v, _roi_list):
                 v = v._jroilist()
-        nb[k] = v
+        nb.put(k, v) # need to use Java method to convert None
     return nb
 
 def plot_getbean(name):
     jb = _plotter.getGuiBean(name)
     if jb is not None:
         return _wrap_gui_bean(jb, _guibean())
     return jb
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyplottingsystem.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyplottingsystem.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyrandom.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyrandom.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyroi.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyroi.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###
 
 from uk.ac.diamond.scisoft.analysis.roi import ROIProfile as _profile
-from org.eclipse.dawnsci.analysis.api.roi import IROI as _iroi
 import org.eclipse.dawnsci.analysis.dataset.roi as _roi
 from .jycore import _wrap
 
-_jroi = _iroi
 
 # base class for implementing point property
 class _iroi(object):
+    def _initstate(self, jroi, point, plot, fixed):
+        self._roi = jroi
+        if point is not None:
+            self.point = point
+        if plot is not None:
+            self.plot = plot
+        if fixed is not None:
+            self.fixed = fixed
+
     def _jroi(self):
         return self._roi
 
     def getPoint(self):
         return self._roi.getPoint()
  
     def setPoint(self, pt):
@@ -46,14 +53,22 @@
         return self._roi.isPlot()
  
     def setPlot(self, p):
         self._roi.setPlot(bool(p))
 
     plot = property(isPlot, setPlot)
 
+    def isFixed(self):
+        return self._roi.isFixed()
+
+    def setFixed(self, f):
+        self._roi.setFixed(bool(f))
+
+    fixed = property(isFixed, setFixed)
+
     def __repr__(self):
         return "%s(%s)" % (self.__class__.__name__, self._roi.toString())
 
     def copy(self):
         from copy import copy
         c = copy(self)
         c._roi = self._roi.copy()
@@ -73,65 +88,54 @@
         return self._roi.getAngleDegrees()
   
     def setAngleDegrees(self, ang):
         self._roi.setAngleDegrees(float(ang))
 
     angledegrees = property(getAngleDegrees, setAngleDegrees)
 
-class roibase(_iroi):
-    pass
-
 class point(_iroi):
-    def __init__(self, jroi=None, point=None, **kwargs):
+    def __init__(self, jroi=None, point=None, plot=None, fixed=None, **kwargs):
         if jroi is None:
             jroi = _roi.PointROI(**kwargs)
-        self._roi = jroi
-        if point is not None:
-            self.point = point
+        self._initstate(jroi, point, plot, fixed)
 
 class line(_iroi, _angleprop):
-    def __init__(self, jroi=None, point=None, **kwargs):
+    def __init__(self, jroi=None, point=None, plot=None, fixed=None, **kwargs):
         if jroi is None:
             jroi = _roi.LinearROI(**kwargs)
-        self._roi = jroi
-        if point is not None:
-            self.point = point
+        self._initstate(jroi, point, plot, fixed)
 
     def getLength(self):
         return self._roi.getLength()
   
     def setLength(self, ang):
         self._roi.setLength(float(ang))
 
     length = property(getLength, setLength)
 
 
 class rectangle(_iroi, _angleprop):
-    def __init__(self, jroi=None, point=None, **kwargs):
+    def __init__(self, jroi=None, point=None, plot=None, fixed=None, **kwargs):
         if jroi is None:
             jroi = _roi.RectangularROI(**kwargs)
-        self._roi = jroi
-        if point is not None:
-            self.point = point
+        self._initstate(jroi, point, plot, fixed)
 
     def getLengths(self):
         return self._roi.getLengths()
   
     def setLengths(self, lens):
         self._roi.setLengths([float(l) for l in lens])
 
     lengths = property(getLengths, setLengths)
 
 class sector(_iroi):
-    def __init__(self, jroi=None, point=None, **kwargs):
+    def __init__(self, jroi=None, point=None, plot=None, fixed=None, **kwargs):
         if jroi is None:
             jroi = _roi.SectorROI(**kwargs)
-        self._roi = jroi
-        if point is not None:
-            self.point = point
+        self._initstate(jroi, point, plot, fixed)
 
     def getRadii(self):
         return self._roi.getRadii()
   
     def setRadii(self, rads):
         self._roi.setRadii([float(r) for r in rads])
 
@@ -150,36 +154,32 @@
  
     def setAnglesDegrees(self, angs):
         self._roi.setAnglesDegrees([float(a) for a in angs])
 
     anglesdegrees = property(getAnglesDegrees, setAnglesDegrees)
 
 class circle(_iroi):
-    def __init__(self, jroi=None, point=None, **kwargs):
+    def __init__(self, jroi=None, point=None, plot=None, fixed=None, **kwargs):
         if jroi is None:
             jroi = _roi.CircularROI(**kwargs)
-        self._roi = jroi
-        if point is not None:
-            self.point = point
+        self._initstate(jroi, point, plot, fixed)
 
     def getRadius(self):
         return self._roi.getRadius()
   
     def setRadius(self, rad):
         self._roi.setRadius(float(rad))
 
     radius = property(getRadius, setRadius)
 
 class ellipse(_iroi, _angleprop):
-    def __init__(self, jroi=None, point=None, **kwargs):
+    def __init__(self, jroi=None, point=None, plot=None, fixed=None, **kwargs):
         if jroi is None:
             jroi = _roi.EllipticalROI(**kwargs)
-        self._roi = jroi
-        if point is not None:
-            self.point = point
+        self._initstate(jroi, point, plot, fixed)
 
     def getSemiAxes(self):
         return self._roi.getSemiAxes()
   
     def setSemiAxes(self, axes):
         self._roi.setSemiAxes([float(a) for a in axes])
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyrpc.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyrpc.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jyscisoft.py` & `scisoftpy-2.29.0/scisoftpy/jython/jyscisoft.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,31 +65,14 @@
 def iqr(a, axis=None):
     '''Interquartile range of input'''
     if axis is None:
         return _stats.iqr(a)
     else:
         return _stats.iqr(a, axis)
 
-@_wrap('a')
-def quantile(a, q, axis=None):
-    '''Quantile (or inverse cumulative distribution) function based on input
-
-    a -- data
-    q -- probability value(s)
-    axis -- can be None'''
-    q = _toList(q)
-    if axis is None:
-        if len(q) == 1:
-            return _stats.quantile(a, q)[0]
-        return _stats.quantile(a, q)
-    else:
-        if len(q) == 1:
-            return _stats.quantile(a, axis, q)[0]
-        return _stats.quantile(a, axis, q)
-
 @_wrapin('a', 'b')
 def residual(a, b, weight=None):
     '''Residual (sum of squared difference) of two inputs with optional weighting'''
     if weight is None:
         return _stats.residual(a, b)
     return _stats.weightedResidual(a, b, weight)
 
@@ -115,9 +98,8 @@
 @_wrap('weights')
 def centroid(weights, coords=None):
     '''Calculate the centroid of an array with its (half) indexes or
     coordinates (list of 1D arrays), if given, and returns it as a list
     '''
     if coords is None:
         return _dsutils.centroid(weights)
-    from .jycore import toList
-    return _dsutils.centroid(weights, toList(coords))
+    return _dsutils.centroid(weights, _toList(coords))
```

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jysignal.py` & `scisoftpy-2.29.0/scisoftpy/jython/jysignal.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/jython/jywrapper.py` & `scisoftpy-2.29.0/scisoftpy/jython/jywrapper.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/linalg.py` & `scisoftpy-2.29.0/scisoftpy/linalg.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/nexus/__init__.py` & `scisoftpy-2.29.0/scisoftpy/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/nexus/hdf5.py` & `scisoftpy-2.29.0/scisoftpy/nexus/hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 
 '''
 '''
 
 from scisoftpy.dictutils import ListDict as _ldict
 
 class HDF5node(object):
-    def __init__(self, attrs={}, parent=None):
+    def __init__(self, attrs={}, parent=None, warn=True):
         '''
         '''
-        super(HDF5node, self).__setattr__('attrs', _ldict(attrs, lock=True))
+        super(HDF5node, self).__setattr__('attrs', _ldict(attrs, lock=True, warn=warn))
         super(HDF5node, self).__setattr__('__parent', parent)
 
     def _getparent(self):
         return super(HDF5node, self).__getattribute__('__parent')
 
     def _setparent(self, parent):
         super(HDF5node, self).__setattr__('__parent', parent)
 
 class HDF5dataset(HDF5node):
-    def __init__(self, dataset, shape=None, dtype=None, maxshape=None, attrs={}, parent=None):
+    def __init__(self, dataset, shape=None, dtype=None, maxshape=None, attrs={}, parent=None, warn=True):
         '''
         '''
-        HDF5node.__init__(self, attrs, parent)
+        HDF5node.__init__(self, attrs, parent, warn)
         self.__data = dataset
 
         if shape is None:
             shape = dataset.shape
         self.__shape = shape
 
         if dtype is None:
@@ -75,17 +75,17 @@
             s += "   @%s = %s\n" % (a, self.attrs[a]) 
         return s
 
     def _getdata(self):
         return self.__data
 
 class HDF5group(_ldict, HDF5node):
-    def __init__(self, attrs={}, parent=None):
-        _ldict.__init__(self)
-        HDF5node.__init__(self, attrs, parent)
+    def __init__(self, attrs={}, parent=None, warn=True):
+        _ldict.__init__(self, warn=warn)
+        HDF5node.__init__(self, attrs, parent, warn)
 
     def __getitem__(self, key):
         if isinstance(key, str):
             return self.__findnode(key)
         return _ldict.__getitem__(self, key)
 
     def __findroot(self):
@@ -155,16 +155,16 @@
     def create_group(self):
         pass
 
     def create_dataset(self):
         pass
 
 class HDF5tree(HDF5group):
-    def __init__(self, filename, attrs={}, native=None):
-        HDF5group.__init__(self, attrs)
+    def __init__(self, filename, attrs={}, native=None, warn=True):
+        HDF5group.__init__(self, attrs, warn=warn)
         super(HDF5tree, self).__setattr__('__filename', filename)
         self.__native = native
 
     def _getnative(self):
         return self.__native
 
     def getnodes(self, name, group=True, data=True):
```

### Comparing `scisoftpy-2.23.1/scisoftpy/nexus/nxclasses.py` & `scisoftpy-2.29.0/scisoftpy/nexus/nxclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,31 +31,31 @@
     '''NeXus Error'''
     pass
 
 class NXobject(_group):
     '''
     NXobject is the base object of NeXus and is a group
     '''
-    def __init__(self, attrs={}, parent=None):
-        _group.__init__(self, attrs, parent)
+    def __init__(self, attrs={}, parent=None, warn=True):
+        _group.__init__(self, attrs, parent, warn)
         self.nxname = self.__class__.__name__
 
     def init_group(self, nodes):
         n = self.nxname
         _group.init_group(self, nodes)
         self.nxname = n
 
 class NXroot(_tree):
     '''
     NXroot node. This is a subclass of the NXobject class.
     
     See the NXobject documentation for more details.
     '''
-    def __init__(self, filename, attrs={}, native=None):
-        _tree.__init__(self, filename, attrs, native)
+    def __init__(self, filename, attrs={}, native=None, warn=True):
+        _tree.__init__(self, filename, attrs, native, warn)
         self.nxname = self.__class__.__name__
 
     def init_group(self, nodes):
         n = self.nxname
         _tree.init_group(self, nodes)
         self.nxname = n
```

### Comparing `scisoftpy-2.23.1/scisoftpy/nexus/utils.py` & `scisoftpy-2.29.0/scisoftpy/nexus/utils.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/plot.py` & `scisoftpy-2.29.0/scisoftpy/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -715,26 +715,38 @@
 
 def setbean(bean, name=None, warn=True):
     '''Set GUI bean
 
     Arguments:
     bean -- GUI bean
     name -- name of plot view to use (if None, use default name)
+    warn -- if True, warn of any issues
     '''
     if name is None:
         name = _PVNAME
     if bean is not None:
-        if parameters.roi in bean:
+        cr = bean.get(parameters.roi)
+        if cr:
             # ensure current roi is in list
             nbean = _guibean(bean)
-            cr = bean[parameters.roi]
-            nbean[parameters.roi] = cr.name
-            if not parameters.roilist in nbean or not nbean[parameters.roilist]:
-                nbean[parameters.roilist] = roi._create_list(cr)
-            _set_roi(nbean[parameters.roilist], cr, warn)
+            rl = bean.get(parameters.roilist)
+            if not rl:
+                rl = roi._create_list(cr)
+                nbean[parameters.roilist] = rl
+            n = cr.name
+            if not n: # add unique name if missing
+                nl = [ r.name for r in rl if r.name ]
+                np = cr.__class__.__name__ 
+                for i in range(max(1,len(nl))):
+                    n = '%s-%d' % (np, i)
+                    if not n in nl:
+                        break
+                cr.name = n
+            nbean[parameters.roi] = n
+            _set_roi(rl, cr, warn)
             bean = nbean
 
         _plot_setbean(name, bean)
 
 def getdatabean(name=None):
     '''Get data bean (contains data from named view)
 
@@ -774,58 +786,79 @@
     r = bean[parameters.roi]
     if roi is None:
         return r
     if r is None or not isinstance(r, roi):
         return None
     return r
 
-def setroi(bean, roi=None, send=False, name=None):
+def setroi(bean, roi=None, send=False, name=None, warn=True):
     '''Set region of interest in bean
 
     Arguments:
     bean -- GUI bean
     roi  -- ROI to set (if None, then use first arg as roi and retrieve bean from and update to plot view of given name)
     send -- flag to update plot
     name -- name of plot view to use (if None, use default name)
+    warn -- if True, warn of any issues
     '''
     if name is None:
         name = _PVNAME
-    warn = True
     if roi is None:
         roi = bean
         send = True
         bean = getbean(name)
     if isinstance(bean, _guibean):
         bean[parameters.roi] = roi
-        warn = False
+
     if send:
         setbean(bean, name, warn=warn)
     return bean
 
-def delroi(bean=None, roi=None, send=False, name=None):
+def delroi(bean=None, roi=None, send=False, name=None, warn=True):
     '''Delete region of interest from bean
 
     Arguments:
     bean -- GUI bean (if None, retrieve from and update to plot view of given name)
     roi  -- class of ROI to remove. If None, then remove anyway
     send -- flag to update plot
     name -- name of plot view to use (if None, use default name)
+    warn -- if True, warn of any issues
     '''
     if name is None:
         name = _PVNAME
     if bean is None:
         send = True
         bean = getbean(name)
-        
-    if parameters.roi in bean:
-        if roi is None or isinstance(bean[parameters.roi], roi):
+
+    r = bean.get(parameters.roi)
+    if r:
+        dr = None
+        if roi:
+            if not issubclass(roi, _iroi):
+                raise ValueError("roi should be a subclass of ROI")
+            if isinstance(r, roi):
+                bean[parameters.roi] = None
+                dr = r
+        else:
             bean[parameters.roi] = None
-            # TODO remove from ROI list?
+            dr = r
+        if dr:
+            dn = dr.name
+            rl = bean.get(parameters.roilist)
+            if rl:
+                if dn:
+                    for i in range(len(rl)):
+                        if dn == rl[i].name:
+                            rl.pop(i)
+                            break
+                else:
+                    rl.remove(dr)
+
     if send:
-        setbean(bean, name)
+        setbean(bean, name, warn=warn)
     return bean
 
 from scisoftpy.dictutils import ListDict
 
 class roi_list(ListDict):
     def __init__(self, data=[]):
         super(roi_list, self).__init__(data=data, warn=False, lock=False, interactive=False)
@@ -841,109 +874,122 @@
     if name is None:
         name = _PVNAME
     if bean is None:
         bean = getbean(name)
     if not parameters.roilist in bean:
         return None
     rs = bean[parameters.roilist]
-    if rs is None or len(rs) == 0:
+    if not rs:
         return None
     try:
         iter(rs)
     except:
         rs = [rs]
     if roi is None:
         rl = [(r.name, r) for r in rs]
     else:
         rl = [(r.name, r) for r in rs if isinstance(r, roi)]
     return roi_list(rl)
 
-def setrois(bean, roilist=None, send=False, name=None):
+def _to_roilist(roilist):
+    if not roilist:
+        return None
+
+    if isinstance(roilist, (roi.point_list, roi.line_list, roi.rectangle_list, roi.sector_list, roi.ellipse_list, roi.circle_list)):
+        return roilist
+
+    r = roilist[0]
+    if isinstance(r, roi.point):
+        rtype = roi.point
+        nlist = roi.point_list()
+    elif isinstance(r, roi.line):
+        rtype = roi.line
+        nlist = roi.line_list()
+    elif isinstance(r, roi.rectangle):
+        rtype = roi.rectangle
+        nlist = roi.rectangle_list()
+    elif isinstance(r, roi.sector):
+        rtype = roi.sector
+        nlist = roi.sector_list()
+    elif isinstance(r, roi.ellipse):
+        rtype = roi.ellipse
+        nlist = roi.ellipse_list()
+    elif isinstance(r, roi.circle):
+        rtype = roi.circle
+        nlist = roi.circle_list()
+    else:
+        raise TypeError("Type of first item not supported")
+
+    if isinstance(roilist, roi_list):
+        for k in roilist:
+            r = roilist[k]
+            if isinstance(r, rtype):
+                nlist.append(r)
+    else:
+        for r in roilist:
+            if isinstance(r, rtype):
+                nlist.append(r)
+    return nlist
+
+
+def setrois(bean, roilist=None, send=False, name=None, warn=True):
     '''Set list/dict of regions of interest in bean
     Arguments:
     bean -- GUI bean
     roilist  -- ROI list to set (if None, then use first arg as roilist and retrieve bean from and update to plot view of given name)
     send    -- flag to update plot
     name    -- name of plot view to use (if None, use default name)
+    warn -- if True, warn of any issues
     '''
     if name is None:
         name = _PVNAME
+
     if roilist is None:
         roilist = bean
         send = True
         bean = getbean(name)
 
-    if not isinstance(roilist, (roi.point_list, roi.line_list, roi.rectangle_list, roi.sector_list, roi.ellipse_list, roi.circle_list)):
-        r = roilist[0]
-        if isinstance(r, roi.point):
-            rtype = roi.point
-            nlist = roi.point_list()
-        elif isinstance(r, roi.line):
-            rtype = roi.line
-            nlist = roi.line_list()
-        elif isinstance(r, roi.rectangle):
-            rtype = roi.rectangle
-            nlist = roi.rectangle_list()
-        elif isinstance(r, roi.sector):
-            rtype = roi.sector
-            nlist = roi.sector_list()
-        elif isinstance(r, roi.ellipse):
-            rtype = roi.ellipse
-            nlist = roi.ellipse_list()
-        elif isinstance(r, roi.circle):
-            rtype = roi.circle
-            nlist = roi.circle_list()
-        else:
-            raise TypeError("Type of first item not supported")
-
-        if isinstance(roilist, roi_list):
-            for k in roilist:
-                r = roilist[k]
-                if isinstance(r, rtype):
-                    nlist.append(r)
-        else:
-            for r in roilist:
-                if isinstance(r, rtype):
-                    nlist.append(r)
-        roilist = nlist
-
+    roilist = _to_roilist(roilist)
     bean[parameters.roilist] = roilist
-    if parameters.roi in bean: # replace current ROI with one from list
-        cr = bean[parameters.roi]
+    cr = bean.get(parameters.roi)
+    if cr: # replace current ROI with one from list
         cname = cr.name
         for r in roilist:
             if r.name == cname:
                 bean[parameters.roi] = r
                 break
+    elif roilist:
+        bean[parameters.roi] = roilist[0]
 
     if send:
-        setbean(bean, name)
+        setbean(bean, name, warn=warn)
     return bean
 
-def delrois(bean=None, roi=None, send=False, name=None):
+def delrois(bean=None, roi=None, send=False, name=None, warn=True):
     '''Delete list/dict of regions of interest from bean
 
     Arguments:
     bean -- GUI bean (if None, retrieve from and update to plot view of given name)
     roi  -- class of ROI or ROI list to remove. If None, then remove anyway
     send -- flag to update plot
     name -- name of plot view to use (if None, use default name)
+    warn -- if True, warn of any issues
     '''
     if name is None:
         name = _PVNAME
     if bean is None:
         send = True
         bean = getbean(name)
 
     if parameters.roilist in bean:
         rl = bean[parameters.roilist]
-        if roi is None or isinstance(rl, roi) or isinstance(rl[0], roi):
+        if roi is None or rl is None or isinstance(rl, roi) or isinstance(rl[0], roi):
             bean[parameters.roilist] = None
     if send:
-        setbean(bean, name)
+        setbean(bean, name, warn=warn)
     return bean
 
 def getline(bean=None, name=None):
     '''Get linear region of interest'''
     if name is None:
         name = _PVNAME
     return getroi(bean, roi=roi.line, name=name)
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pybeans.py` & `scisoftpy-2.29.0/scisoftpy/python/pybeans.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         
     def get(self, modename):
         '''Return the GuiPlotMode with the given name, or return None for no matching'''
         return self._str_to_modes.get(modename)
 
 plotmode = _plotmode()
 
-class axismapbean(object):   
+class axismapbean(object):
     _AXIS_ID = 'axisID'
     _AXIS_NAMES = 'axisNames'
     
     DIRECT = 0
     FULL = 1
 
     XAXIS = "X-Axis"
@@ -195,8 +195,8 @@
         return True
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __repr__(self):
         return self.__dict__.__repr__()
-    
+
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pycomparisons.py` & `scisoftpy-2.29.0/scisoftpy/python/pycomparisons.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pycore.py` & `scisoftpy-2.29.0/scisoftpy/python/pycore.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 
 import numpy as _np #@UnresolvedImport
 
 from distutils.version import LooseVersion
 
 _np_version_cur = LooseVersion(_np.version.version)
 _is_np_version_ge_1_8 = _np_version_cur >= LooseVersion('1.8')
+_is_np_version_ge_1_18 = _np_version_cur >= LooseVersion('1.18')
 
 newaxis = _np.newaxis
 
 ndarray = _np.ndarray
 generic = ndgeneric = _np.generic
-bool = _np.bool #@ReservedAssignment
+bool = _np.bool_ #@ReservedAssignment
 int8 = _np.int8
 _uint8 = _np.uint8 # used for PIL saving
 _uint16 = _np.uint16 # used for PIL saving and fixing a PIL bug
 int16 = _np.int16
 int32 = _np.int32
 int64 = _np.int64
 cint8 = lambda e : _np.dtype([('', _np.int8)]*e)
@@ -41,28 +42,27 @@
 cint64 = lambda e : _np.dtype([('', _np.int64)]*e)
 float32 = _np.float32
 float64 = _np.float64
 cfloat32 = lambda e : _np.dtype([('', _np.float32)]*e)
 cfloat64 = lambda e : _np.dtype([('', _np.float64)]*e)
 complex64 = _np.complex64
 complex128 = _np.complex128
-rgb = _np.dtype([('r', int16), ('g', int16), ('b', int16)])
+rgb = _np.dtype([('r', _uint8), ('g', _uint8), ('b', _uint8)])
 
-_pyint = int
-_pyfloat = float
-_pycomplex = complex
-int_ = int64
-int = int_ #@ReservedAssignment
-float_ = float64
-float = float_ #@ReservedAssignment
-complex_ = complex128
-complex = complex_ #@ReservedAssignment
+int_ = _np.int_
+int = _np.int_ #@ReservedAssignment
+float_ = _np.float_
+float = _np.float_ #@ReservedAssignment
+complex_ = _np.complex_
+complex = _np.complex_ #@ReservedAssignment
 
 import types as _types
 
+AxisError = _np.AxisError
+
 def asIterable(items):
     '''
     Ensure entity is an iterable by making it a tuple if not
     '''
     if isinstance(items, (list, tuple)):
         pass
     elif isinstance(items, dict):
@@ -162,14 +162,18 @@
 
 atleast_2d = _np.atleast_2d
 
 atleast_3d = _np.atleast_3d
 
 concatenate = _np.concatenate
 
+expand_dims = _np.expand_dims
+
+stack = _np.stack # 1.10+
+
 vstack = _np.vstack
 
 hstack = _np.hstack
 
 dstack = _np.dstack
 
 column_stack = _np.column_stack
@@ -210,18 +214,26 @@
 
 swapaxes = _np.swapaxes
 
 amax = _np.amax
 
 amin = _np.amin
 
+nanmax = _np.nanmax
+
+nanmin = _np.nanmin
+
 argmax = _np.argmax
 
 argmin = _np.argmin
 
+nanargmax = _np.nanargmax
+
+nanargmin = _np.nanargmin
+
 meshgrid = _np.meshgrid
 
 indices = _np.indices
 
 ix_ = _np.ix_
 
 # need to define r_, c_, s_, index_exp objects
@@ -330,38 +342,38 @@
         super(ndarrayRGB, self).shape = shape
         self._oldshape = shape
     shape = property(__get_shape, __set_shape) # python 2.5 rather than using @shape.setter
 
 
     def get_red(self, dtype=None):
         if dtype is None:
-            dtype = int16
+            dtype = _uint8
 #        return self['r'].astype(dtype)
-        return self.view(int16)[..., 0].astype(dtype)
+        return self.view(_uint8)[..., 0].astype(dtype)
 
     def get_green(self, dtype=None):
         if dtype is None:
-            dtype = int16
+            dtype = _uint8
 #        return self['g'].astype(dtype)
         return self.view(int16)[..., 1].astype(dtype)
 
     def get_blue(self, dtype=None):
         if dtype is None:
             dtype = int16
 #        return self['b'].astype(dtype)
-        return self.view(int16)[..., 2].astype(dtype)
+        return self.view(_uint8)[..., 2].astype(dtype)
 
     def get_grey(self, cweights=None, dtype=None):
         '''Get grey image
         
         Arguments:
         cweights -- optional set of weight for combining the colour channel
         dtype    -- optional dataset type (default is int16)'''
         if dtype is None:
-            dtype = int16
+            dtype = _uint8
         if cweights is None:
             cweights = [0.299, 0.587, 0.114]
         else:
             cweights = asIterable(cweights)
             if len(cweights) != 3:
                 raise ValueError("three colour channel weights needed")
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyflatten.py` & `scisoftpy-2.29.0/scisoftpy/python/pyflatten.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 continue
             v = unflatten(v)
             unflattenedObj[k] = v
         return self.typeObj(**unflattenedObj)
 
     @staticmethod
     def getROIBaseHelper():
-        return roiHelper(_roi.roibase, "org.eclipse.dawnsci.analysis.dataset.roi.ROIBase")
+        return roiHelper(_roi._iroi, "org.eclipse.dawnsci.analysis.dataset.roi.ROIBase")
         
     @staticmethod
     def getPointHelper():
         return roiHelper(_roi.point, "org.eclipse.dawnsci.analysis.dataset.roi.PointROI")
         
     @staticmethod
     def getRectangleHelper():
@@ -596,15 +596,15 @@
                 out = traceback.format_list([x[:4] for x in stackTrace]) # clip for formatter
                 excmsg += "".join(out)
             e = Exception(excmsg)
             e.flatten_traceback = stackTrace
             return e
         else:
             return Exception(excheader)
-    
+
 helpers = [noneHelper(), roiListHelper.getLineListHelper(), roiListHelper.getPointListHelper(),
            roiListHelper.getSectorListHelper(), roiListHelper.getRectangleListHelper(),
            roiListHelper.getCircleListHelper(), roiListHelper.getEllipseListHelper(),
            roiHelper.getRectangleHelper(), roiHelper.getSectorHelper(),
            roiHelper.getCircleHelper(), roiHelper.getEllipseHelper(),
            roiHelper.getLineHelper(), roiHelper.getPointHelper(), roiHelper.getROIBaseHelper(), 
            ndArrayHelper(), guiBeanHelper(),
@@ -635,12 +635,9 @@
     return False
         
 def canunflatten(obj):
     for thisHelper in helpers:
         if thisHelper.canunflatten(obj):
             return True
     return False
-        
-
-
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyh5py.py` & `scisoftpy-2.29.0/scisoftpy/python/pyh5py.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 from __future__ import print_function
 import h5py #@UnresolvedImport
 
 if h5py.version.version_tuple[0] < 2:
     raise ImportError("Installed h5py is too old - it must be at least version 2")
 elif h5py.version.version_tuple[0] > 2:
-    print("Warning string datasets in HDF5 files now return bytes objects (use .decode() to convert to strings)", file=sys.stderr)
+    import sys
+    if hasattr(sys, 'ps1'):
+        print("Warning string datasets in HDF5 files now return bytes objects (use .decode() to convert to strings)", file=sys.stderr)
 
 from ..nexus.hdf5 import HDF5tree as _tree
 from ..nexus.hdf5 import HDF5group as _group
 from ..nexus.hdf5 import HDF5dataset as _dataset
 from ..nexus import nxclasses as _nx
 io_exception = IOError
 
@@ -130,22 +132,22 @@
             v[tuple(dst_pos)] = ds[tuple(src_pos)]
 
         fh.close()
         return v.reshape(nshape)
 
 
 class SDS(_dataset):
-    def __init__(self, dataset, attrs={}, parent=None):
+    def __init__(self, dataset, attrs={}, parent=None, warn=True):
         '''Make a SDS
         
         dataset can be a ndarray or HDF5Dataset when created from a file
         '''
         if not isinstance(dataset, (_lazydataset, ndarray, h5py.Dataset)):
             dataset = asarray(dataset)
-        _dataset.__init__(self, dataset, attrs=attrs, parent=parent)
+        _dataset.__init__(self, dataset, attrs=attrs, parent=parent, warn=warn)
 #        self.__data = dataset
 #        if not isinstance(dataset, ndarray):
 #            self.__shape = tuple(dataset.shape)
 #            self.__maxshape = tuple(dataset.maxshape)
 #        else:
 #            self.__shape = self.__maxshape = tuple(dataset.shape)
 
@@ -164,29 +166,30 @@
             raise io_exception(e)
         finally:
             pass
 
         if fh is None:
             raise io_exception("No tree found")
 
+        self.warn = warn
         # convert tree to own tree
         pool = dict()
         t = self._copynode(pool, fh)
         pool.clear()
         fh.close()
         return t
 
     def _mkgroup(self, node, attrs, parent):
         if parent is None:
             return _tree(node.filename, attrs)
-        return _group(attrs, parent)
+        return _group(attrs, parent, self.warn)
 
     def _mkdataset(self, node, attrs, link, parent):
         d = _lazydataset(node, isinstance(link, h5py.ExternalLink))
-        return _dataset(d, attrs=attrs, parent=parent)
+        return _dataset(d, attrs=attrs, parent=parent, warn=self.warn)
 
     def _copynode(self, pool, node, link=None, parent=None):
         if node.id in pool:
             return pool[node.id]
 
         attrs = []
         for k,v in node.attrs.items():
@@ -208,14 +211,17 @@
         if isinstance(node, h5py.Group):
             g = self._mkgroup(node, attrs, parent)
             pool[node.id] = g
             nodes = []
             for k in node.keys():
                 n = node.get(k)
                 l = node.get(k, getlink=True)
+                if n is None:
+                    print('Missing node "' + k + '" with link', l)
+                    continue
                 try:
                     nodes.append((k, self._copynode(pool, n, l, g)))
                 except Exception as e:
                     print(k, n, e)
             g.init_group(nodes)
             return g
         elif isinstance(node, h5py.Dataset):
@@ -234,22 +240,22 @@
             cls = node.attrs['NX_class']
         except KeyError:
             cls = None
         if cls is not None:
             if not isinstance(cls, str):
                 cls = str(cls, 'utf-8')
             if cls in _nx.NX_CLASSES:
-                g = _nx.NX_CLASSES[cls](attrs, parent)
+                g = _nx.NX_CLASSES[cls](attrs, parent, self.warn)
             else:
                 print("Unknown Nexus class: %s" % cls)
                 g = super(NXLoader, self)._mkgroup(node, attrs, parent)
         elif node.name == '/':
-            g = _nx.NXroot(node.filename, attrs)
+            g = _nx.NXroot(node.filename, attrs, warn=self.warn)
         else:
-            g = _nx.NXobject(attrs, parent)
+            g = _nx.NXobject(attrs, parent, self.warn)
 
         return g
 
     def _mkdataset(self, dataset, attrs, link, parent):
         d = _lazydataset(dataset, isinstance(link, h5py.ExternalLink))
-        return SDS(d, attrs, parent)
+        return SDS(d, attrs, parent, self.warn)
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyhdf5io.py` & `scisoftpy-2.29.0/scisoftpy/python/pyhdf5io.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyio.py` & `scisoftpy-2.29.0/scisoftpy/python/pyio.py`

 * *Files 3% similar despite different names*

```diff
@@ -442,70 +442,79 @@
 try:
     import tifffile as _tf
 except:
     print("Could not import tiff file package", file=sys.stderr)
     _tf = None
 
 class TIFFfileLoader(PythonLoader):
-    def load(self, warn=True):
+    def load(self, warn=True, stack=True):
+        '''
+        stack -- if True, stack up images to a single array
+        '''
         if _tf is None:
             raise NotImplementedError
 
         data = []
         if self.load_metadata:
             metadata = dict()
         else:
             metadata = None
 
         t = _tf.TiffFile(self.name)
-        for i, p in enumerate(t.pages):
-            d = p.asarray()
-            if p.photometric == p.photometric.RGB:
-                # convert to an rgb dataset
-                d = _core.asarray(d, dtype=_core.int16).view(_RGB)
 
+        if stack:
+            data.append(("stack", t.asarray()))
+        else:
+            for i, p in enumerate(t.pages):
+                d = p.asarray()
+                data.append(("image-%02d" % (i+1,), d))
+                if self.load_metadata:
+                    for k,v in p.tags.items():
+                        metadata[k] = v.value
+
+        pho = t.pages[0].photometric
+        if pho == pho.RGB:
+            # convert to an rgb dataset
+            for i, d in enumerate(data):
+                di = _core.asarray(d[1], dtype=_core.int16).view(_RGB)
                 if not self.ascolour:
-                    d = d.get_grey()
-
-            data.append(("image-%02d" % (i+1,), d))
-            if self.load_metadata:
-                for k,v in p.tags.items():
-                    metadata[k] = v.value
-
-        if len(data) < 1:
-            pass
+                    di = di.get_grey()
+                data[i] = (d[0], di)
         return DataHolder(data, metadata, warn)
 
 if _tf is None:
     TIFFLoader = ImageLoader
 else:
     TIFFLoader = TIFFfileLoader
 
 try:
     import pycbf as _cbf  # @UnresolvedImport
     import numpy  # @UnresolvedImport
+    def _str(v): # needed until https://github.com/dials/pycbf/pull/2 is merged
+        return v.decode() if isinstance(v, bytes) else v
+
     class CBFLoader(PythonLoader):
         def getvalue(self, h):
-            vtype = h.get_typeofvalue()
-            if "bnry" not in vtype:
-                return h.get_value()
+            vtype = _str(h.get_typeofvalue())
+            if "bnry" != vtype:
+                return _str(h.get_value())
             try:
                 (_compression, _binaryid, _elsize, _elsigned, \
                     _elunsigned, _elements, _minelement, _maxelement, \
                     _byteorder, dimfast, dimmid, dimslow, _padding) = \
                     h.get_integerarrayparameters_wdims()
                 isreal = False
             except:
                 try:
                     (_compression, _binaryid, _elsize, _elements, \
                         _byteorder, dimfast, dimmid, dimslow, _padding) = \
                         h.get_doublearrayparameters_wdims()
                     isreal = True
                 except:
-                    return h.get_value()
+                    return _str(h.get_value())
                     
             if dimfast == 0:
                 dimfast = 1
             if dimmid == 0:
                 dimmid = 1
             if dimslow == 0:
                 dimslow = 1
@@ -521,63 +530,88 @@
 #             print "byteorder", _byteorder
 #             print "dimfast", dimfast
 #             print "dimmid", dimmid
 #             print "dimslow",dimslow
 #             print "padding", _padding
             if isreal:
                 s = h.get_doublearray_as_string()
-                print(type(s))
                 d = numpy.frombuffer(s, numpy.float64)
             else:
                 s = h.get_integerarray_as_string()
-                print(type(s))
-                d = numpy.frombuffer(s, numpy.uint32)
-#             print d.shape
-#             print d[0:10], d[d.shape[0]/2], d[-1]
-            d.shape = (dimfast, dimmid)
+                d = numpy.frombuffer(s, numpy.int32)
+            if d.size == dimmid * dimfast:
+                d.shape = (dimmid, dimfast)
             return d
 
         def load(self, warn=True):
             data = []
             metadata = []
+            from scisoftpy.dictutils import ListDict
             try:
                 h = _cbf.cbf_handle_struct()
                 h.read_widefile(self.name, _cbf.MSG_DIGEST)
                 h.rewind_datablock()
                 for nd in range(h.count_datablocks()):
                     h.select_datablock(nd)
 #                     db_name = h.datablock_name()
 #                     print "DBl: %d, %s" % (nd, db_name)
                     h.rewind_category()
                     for nc in range(h.count_categories()):
                         h.select_category(nc)
-#                         ct_name = h.category_name()
+                        ct_name = _str(h.category_name())
+                        ct_md = []
 #                         print "  Cat: %d, %s" % (nc, ct_name)
                         h.rewind_column()
                         colnames = []
                         for nv in range(h.count_columns()):
                             h.select_column(nv)
-                            cl_name = h.column_name()
+                            cl_name = _str(h.column_name())
                             colnames.append(cl_name)
+                            ct_md.append([])
 #                             print "    Col: %d, %s" % (nv, cl_name)
                         h.rewind_row()
                         for nh in range(h.count_rows()):
                             h.select_row(nh)
                             h.rewind_column()
                             for nv in range(h.count_columns()):
                                 h.select_column(nv)
                                 v = self.getvalue(h)
 #                                 print "    %d %d: " % (nh, nv), v
-                                item = "%s-%d" % (colnames[nv], nh), v
                                 if isinstance(v, numpy.ndarray):
+                                    item = "%s-%d" % (colnames[nv], nh), v
                                     data.append(item)
                                 else:
-                                    metadata.append(item)
+                                    ct_md[nv].append(v)
+                        if ct_md:
+                            ct_md = list(zip(colnames,ct_md))
+                        metadata.append((ct_name, ListDict(ct_md)))
             finally:
                 del(h)
+
+            shape = None
+            for n,v in metadata:
+                if n == 'array_structure_list':
+                    for an,ai in enumerate(v['index']):
+                        if ai == '1':
+                            xn = an
+                            break
+                    fn = 1 - xn if v['precedence'][xn] == '1' else xn
+                    is_f_incr = v['direction'][fn] == 'increasing'
+                    is_s_incr = v['direction'][1 - fn] == 'increasing'
+                    shape = int(v['dimension'][1 - fn]), int(v['dimension'][fn])
+                    break
+
+            if shape is not None:
+                for n,v in data:
+                    if v.ndim == 1:
+                        v.shape = shape
+                    if not is_f_incr or not is_s_incr:
+                        flip = slice(None, None, -1)
+                        data[n] = v[None if is_s_incr else flip, None if is_f_incr else flip]
+            
             return DataHolder(data, metadata, warn)
 except:
     CBFLoader = None
 
 PNGLoader = ImageLoader
 JPEGLoader = ImageLoader
 TIFFLoader = TIFFLoader
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pymaths.py` & `scisoftpy-2.29.0/scisoftpy/python/pymaths.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,22 +34,21 @@
 
 import sys
 floatmax = sys.float_info.max # maximum float value #@UndefinedVariable
 
 prod = _np.prod
 sum = _np.sum #@ReservedAssignment
 
+# TODO add nansum, etc
+
 mean = _np.mean
 std = _np.std
 var = _np.var
 ptp = _np.ptp
 
-amax = _np.amax
-amin = _np.amin
-
 real = _np.real
 imag = _np.imag
 
 abs = _np.abs #@ReservedAssignment
 
 absolute = _np.absolute
 
@@ -134,18 +133,23 @@
 sign = _np.sign
 negative = _np.negative
 
 clip = _np.clip
 maximum = _np.maximum
 minimum = _np.minimum
 
-median = _np.median
 cumprod = _np.cumprod
 cumsum = _np.cumsum
 
+median = _np.median
+percentile = _np.percentile
+quantile = _np.quantile
+
+# TODO nancumsum, etc
+
 diff = _np.diff
 
 histogram = _np.histogram
 histogram2d = _np.histogram2d
 histogramdd = _np.histogramdd
 bincount = _np.bincount
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pynxio.py` & `scisoftpy-2.29.0/scisoftpy/python/pynxio.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyplot.py` & `scisoftpy-2.29.0/scisoftpy/python/pyplot.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyplottingsystem.py` & `scisoftpy-2.29.0/scisoftpy/python/pyplottingsystem.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyroi.py` & `scisoftpy-2.29.0/scisoftpy/python/pyroi.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###
 
 import math as _math
 
 class _iroi(object):
-    pass
-
-class roibase(_iroi):
     _NAME = "name"
     _SPT = "spt"
     _PLOT = "plot"
+    _FIXED = "fixed"
 
-    def __init__(self, name='', point=[0.0,0.0], spt=None, plot=False, **kwargs):
-        super(roibase, self).__init__()
+    def __init__(self, name='', point=[0.0,0.0], spt=None, plot=False, fixed=False, **kwargs):
         self.name = name
         self.spt = [float(p) for p in spt] if spt is not None else [float(p) for p in point]
         self.plot = plot
+        self.fixed = fixed
 
     # rois are not hashable because they are mutable
     __hash__ = None
     
     def __eq__(self, other):
         return (isinstance(other, self.__class__)
             and self.__dict__ == other.__dict__)
@@ -53,23 +51,29 @@
 
     def isPlot(self):
         return self.plot
 
     def setPlot(self, p):
         self.plot = bool(p)
 
+    def isFixed(self):
+        return self.fixed
+
+    def setFixed(self, f):
+        self.fixed = bool(f)
+
     def copy(self):
         from copy import deepcopy
         return deepcopy(self)
 
-class point(roibase):
+class point(_iroi):
     def __init__(self, **kwargs):
         super(point, self).__init__(**kwargs)
 
-class line(roibase):
+class line(_iroi):
     _LEN = "len"
     _ANG = "ang"
     _CROSS_HAIR = "crossHair"
 
     def __init__(self, length=0.0, len=None, angle=0.0, ang=None, angledegrees=None, crossHair=False, **kwargs): #@ReservedAssignment
         super(line, self).__init__(**kwargs)
         self.len = float(len) if len is not None else float(length)
@@ -98,15 +102,15 @@
         return _math.degrees(self.ang)
 
     def setAngleDegrees(self, angle):
         self.ang = _math.radians(angle)
 
     angledegrees = property(getAngleDegrees, setAngleDegrees)
 
-class rectangle(roibase):
+class rectangle(_iroi):
     _LEN = "len"
     _ANG = "ang"
     _CLIPPING_COMPENSATION = "clippingCompensation"
     
     def __init__(self, lengths=[0.0,0.0], len=None, angle=0.0, ang=None, angledegrees=None, clippingCompensation=False, **kwargs): #@ReservedAssignment
         super(rectangle, self).__init__(**kwargs)
         self.len = [float(l) for l in len] if len is not None else [float(l) for l in lengths]
@@ -135,15 +139,15 @@
         return _math.degrees(self.ang)
 
     def setAngleDegrees(self, angle):
         self.ang = _math.radians(angle)
 
     angledegrees = property(getAngleDegrees, setAngleDegrees)
 
-class sector(roibase):
+class sector(_iroi):
     _ANG = "ang"
     _RAD = "rad"
     _CLIPPING_COMPENSATION = "clippingCompensation"
     _SYMMETRY = "symmetry"
     _COMBINE_SYMMETRY = "combineSymmetry"
     _AVERAGE_AREA = "averageArea"
     
@@ -209,30 +213,30 @@
 
     def setAnglesDegrees(self, angle):
         self.ang = [_math.radians(a) for a in angle]
         self._chkAngles()
 
     anglesdegrees = property(getAnglesDegrees, setAnglesDegrees)
 
-class circle(roibase):
+class circle(_iroi):
     _RAD = "rad"
     
     def __init__(self, radius=1.0, rad=None, **kwargs): #@ReservedAssignment
         super(circle, self).__init__(**kwargs)
         self.rad = float(rad) if rad is not None else float(radius)
 
     def getRadius(self):
         return self.rad
 
     def setRadius(self, radius):
         self.rad = float(radius)
 
     radius = property(getRadius, setRadius)
 
-class ellipse(roibase):
+class ellipse(_iroi):
     _SAXIS = "saxis"
     _ANG = "ang"
     
     def __init__(self, semiaxes=[0.0,0.0], saxis=None, angle=0.0, ang=None, angledegrees=None, **kwargs): #@ReservedAssignment
         super(ellipse, self).__init__(**kwargs)
         self.saxis = [float(l) for l in saxis] if saxis is not None else [float(l) for l in semiaxes]
         self.ang = float(ang) if ang is not None else float(angle)
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyrpc.py` & `scisoftpy-2.29.0/scisoftpy/python/pyrpc.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pyscisoft.py` & `scisoftpy-2.29.0/scisoftpy/python/pyscisoft.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,48 +59,17 @@
     raise NotImplementedError
 
 
 def kurtosis(a, axis=None):
     '''Kurtosis of input'''
     raise NotImplementedError
 
-def quantile(a, q, axis=None):
-    '''Quantile (or inverse cumulative distribution) function based on input
-
-    a -- data
-    q -- probability value(s)
-    axis -- can be None'''
-    from .pycore import toList
-    from math import floor
-    q = toList(q)
-    sa = _np.sort(a, axis=axis)
-    if axis is None:
-        size = sa.size
-    else:
-        size = sa.shape[axis]
-
-    x = [ (size - 1)*p for p in q ]
-    n = [ int(floor(f)) for f in x ]
-    x = [ f - i for f, i in zip(x,n) ]
-    if axis is None:
-        return [ sa[i]*(1-f) + sa[i+1]*f for f, i in zip(x,n) ]
-    else:
-        slices = [ slice(d) for d in sa.shape ]
-        result = []
-        for f, i in zip(x, n):
-            slices[axis] = i
-            r = sa[slices]*(1-f)
-            slices[axis] = i+1
-            r += sa[slices]*f
-            result.append(r)
-        return result
-
 def iqr(a, axis=None):
     '''Interquartile range of input'''
-    result = quantile(a, [0.25, 0.75], axis=axis)
+    result = _np.quantile(a, [0.25, 0.75], axis=axis)
     return result[1] - result[0]
 
 def residual(a, b, weight=None):
     '''Residual (sum of squared difference) of two inputs with optional weighting'''
     r = _np.square(a-b)
     if weight is None:
         return r
@@ -116,15 +85,15 @@
     return False
 
 def centroid(weights, coords=None):
     '''Calculate the centroid of an array with its (half) indexes or
     coordinates (list of 1D arrays), if given, and returns it as a list
     '''
     if coords is None:
-        coords = [ _np.arange(d, dtype=_np.float) + 0.5 for d in weights.shape ]
+        coords = [ _np.arange(d, dtype=_np.float_) + 0.5 for d in weights.shape ]
     else:
         from .pycore import toList
         coords = toList(coords)
 
     rank = weights.ndim
     if rank > len(coords):
         raise ValueError("Number of coordinate arrays must match rank")
```

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pysignal.py` & `scisoftpy-2.29.0/scisoftpy/python/pysignal.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/python/pywrapper.py` & `scisoftpy-2.29.0/scisoftpy/python/pywrapper.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/random.py` & `scisoftpy-2.29.0/scisoftpy/random.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/roi.py` & `scisoftpy-2.29.0/scisoftpy/roi.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     from .jython import jyroi as _roi #@UnusedImport
 else:
     from .python import pyroi as _roi #@Reimport
 
  
 
 _iroi = _roi._iroi
-_roibase = _roi.roibase
 
 point = _roi.point
 line = _roi.line
 rectangle = rect = _roi.rectangle
 sector = sect = _roi.sector
 circle = _roi.circle
 ellipse = _roi.ellipse
```

### Comparing `scisoftpy-2.23.1/scisoftpy/rpc.py` & `scisoftpy-2.29.0/scisoftpy/rpc.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy/signal.py` & `scisoftpy-2.29.0/scisoftpy/signal.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.23.1/scisoftpy.egg-info/PKG-INFO` & `scisoftpy-2.29.0/scisoftpy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: scisoftpy
-Version: 2.23.1
+Version: 2.29.0
 Summary: DAWN Python Extensions
 Home-page: https://gerrit.diamond.ac.uk/plugins/gitiles/scisoft/scisoft-core
 Author: Peter Chang
-Author-email: scientificsoftware@diamond.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: dataanalysis@diamond.ac.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-
-UNKNOWN
-
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `scisoftpy-2.23.1/scisoftpy.egg-info/SOURCES.txt` & `scisoftpy-2.29.0/scisoftpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+pyproject.toml
 setup.cfg
 setup.py
 scisoftpy/__init__.py
 scisoftpy/crystallography.py
 scisoftpy/data.py
 scisoftpy/dictutils.py
 scisoftpy/diffraction.py
```

