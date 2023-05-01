# Comparing `tmp/maddaq-0.7.5.tar.gz` & `tmp/maddaq-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maddaq-0.7.5.tar", last modified: Mon Apr 24 11:18:08 2023, max compression
+gzip compressed data, was "maddaq-0.7.6.tar", last modified: Mon May  1 16:24:23 2023, max compression
```

## Comparing `maddaq-0.7.5.tar` & `maddaq-0.7.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.080302 maddaq-0.7.5/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-24 11:18:08.079809 maddaq-0.7.5/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.5/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.073951 maddaq-0.7.5/maddaq/
--rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.5/maddaq/GTimer.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.5/maddaq/MadDAQData.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.5/maddaq/MadDAQModule.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.5/maddaq/Progress.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.5/maddaq/ScanManager.py
--rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-04-24 11:13:35.000000 maddaq-0.7.5/maddaq/__init__.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.079262 maddaq-0.7.5/maddaq/cmmds/
--rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.5/maddaq/cmmds/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.5/maddaq/cmmds/analyze_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.5/maddaq/cmmds/file_info.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.5/maddaq/cmmds/fit_utils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     6170 2023-04-24 11:10:08.000000 maddaq-0.7.5/maddaq/cmmds/getSpectrum.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.5/maddaq/cmmds/read_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.5/maddaq/cmmds/show_data.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.076372 maddaq-0.7.5/maddaq.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-24 11:13:35.000000 maddaq-0.7.5/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-24 11:18:08.080406 maddaq-0.7.5/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-01 16:24:23.413336 maddaq-0.7.6/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-05-01 16:24:23.412930 maddaq-0.7.6/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.6/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-01 16:24:23.406991 maddaq-0.7.6/maddaq/
+-rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.6/maddaq/GTimer.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.6/maddaq/MadDAQData.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.6/maddaq/MadDAQModule.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.6/maddaq/Progress.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.6/maddaq/ScanManager.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-05-01 16:22:54.000000 maddaq-0.7.6/maddaq/__init__.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-01 16:24:23.412429 maddaq-0.7.6/maddaq/cmmds/
+-rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.6/maddaq/cmmds/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.6/maddaq/cmmds/analyze_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.6/maddaq/cmmds/file_info.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.6/maddaq/cmmds/fit_utils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     6571 2023-05-01 16:20:25.000000 maddaq-0.7.6/maddaq/cmmds/getSpectrum.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.6/maddaq/cmmds/read_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.6/maddaq/cmmds/show_data.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-01 16:24:23.409554 maddaq-0.7.6/maddaq.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-05-01 16:24:23.000000 maddaq-0.7.6/maddaq.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-05-01 16:24:23.000000 maddaq-0.7.6/maddaq.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-01 16:24:23.000000 maddaq-0.7.6/maddaq.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-05-01 16:24:23.000000 maddaq-0.7.6/maddaq.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-05-01 16:24:23.000000 maddaq-0.7.6/maddaq.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-05-01 16:24:23.000000 maddaq-0.7.6/maddaq.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-05-01 16:22:54.000000 maddaq-0.7.6/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-01 16:24:23.413453 maddaq-0.7.6/setup.cfg
```

### Comparing `maddaq-0.7.5/PKG-INFO` & `maddaq-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.5
+Version: 0.7.6
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.5/README.md` & `maddaq-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/GTimer.py` & `maddaq-0.7.6/maddaq/GTimer.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/MadDAQData.py` & `maddaq-0.7.6/maddaq/MadDAQData.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/MadDAQModule.py` & `maddaq-0.7.6/maddaq/MadDAQModule.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/Progress.py` & `maddaq-0.7.6/maddaq/Progress.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/ScanManager.py` & `maddaq-0.7.6/maddaq/ScanManager.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/cmmds/analyze_data.py` & `maddaq-0.7.6/maddaq/cmmds/analyze_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/cmmds/file_info.py` & `maddaq-0.7.6/maddaq/cmmds/file_info.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/cmmds/fit_utils.py` & `maddaq-0.7.6/maddaq/cmmds/fit_utils.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/cmmds/getSpectrum.py` & `maddaq-0.7.6/maddaq/cmmds/getSpectrum.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 """Open data file and get spectrum."""
 import os
 import sys
+from pathlib import Path
 from argparse import Action
 from argparse import ArgumentParser
 
 import matplotlib.pyplot as plt
 import numpy as np
 from maddaq.cmmds.fit_utils import draw_best_fit, fit_gaussian, fit_two_peaks
 from maddaq import MadDAQData
@@ -86,36 +87,44 @@
     print("Noise mean {:.1f} std {:.1f}".format(mnoise, stnoise))
 
 
 def do_getSpectrum(files, options):
     """Main entry."""
     
     amplitudes = []
+    names = []
     for fnam in files:
         # Check that the file exists
         if not os.path.exists(fnam):
             print("Input file", fnam, "does not exist")
             continue
         
+        i1 = fnam.rfind('/')
+        i2 = fnam.rfind('_')
+        nam = fnam[i1+1:i2] 
+        names.append(nam)
+        
         # We open here the file with MadDAQData
+        print("\n\n### Opening {}".format(Path(fnam).name))
         maddaq = MadDAQData(fnam)
         maddaq.show_info(True)
 
         # Find the module
         keys = list(maddaq.modules.keys())
         if options.mid in keys:
             mid = options.mid
         else:
             mid = keys[0]
 
         print("\n## Looking at data from module {}.".format(mid))
         md = maddaq.modules[mid]
 
         # Show pedeswtals and noise
-        show_pedestals(md)
+        if options.show_ped:
+            show_pedestals(md)
 
         # Create the iterator
         if options.scan_point is not None:
             maddaq_iter = maddaq.create_iterator_at_scanpoint(options.scan_point, [mid])
         elif options.start_time is not None:
             maddaq_iter = maddaq.create_iterator_at_time(options.start_time, [mid])
         elif options.start_evt is not None:
@@ -138,15 +147,15 @@
 
         amplitudes.append(amplitude)
         prg.stop()
         print("")
         
     # Draw the signal
     fig, ax = plt.subplots(1, 1)
-    n, bins, *_ = ax.hist(amplitudes, bins=options.nbin)
+    n, bins, *_ = ax.hist(amplitudes, bins=options.nbin, label=names)
     legends = []
     if options.fit:
         for amplitude in amplitudes:
             mean = np.mean(amplitude)
             std = np.std(amplitude)
             if options.two_peaks:
                 result, out, legend = fit_two_peaks(mean, std, std, n, bins)
@@ -154,14 +163,16 @@
             else:
                 result, out, legend = fit_gaussian(n, bins, mean, width=std)
 
             draw_best_fit(ax, result, bins)
             legends.append(legend)
             
         ax.legend(legends, loc=1)
+    else:
+        ax.legend(names, loc=1)
 
     ax.set_title("Signal")
     ax.set_xlabel("Charge (ADC)")
     if options.logY:
         ax.set_yscale("log")
 
     plt.show()
@@ -188,14 +199,15 @@
     parser.add_argument("--scan-point", dest="scan_point", type=int, default=None,
                         help="Scan point number to visit")
     parser.add_argument("--nbin", default=50, type=int, help="Number of bins in histogram.")
     parser.add_argument("--logY", default=False, action="store_true", help="Log axis")
     parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
     parser.add_argument("--two_peaks", default=False, action="store_true", help="Min E to show in histogram")
     parser.add_argument("--no-fit", dest="fit", default=True, action="store_false")
+    parser.add_argument("--show-ped", action="store_true", default=False, dest="show_ped")
     parser.add_argument("--mid", dest="mid", default=-1,
                         type=int, help="The module ID")
 
     options = parser.parse_args()
 
     if len(options.files) == 0:
         print("I need an input file")
```

### Comparing `maddaq-0.7.5/maddaq/cmmds/read_data.py` & `maddaq-0.7.6/maddaq/cmmds/read_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq/cmmds/show_data.py` & `maddaq-0.7.6/maddaq/cmmds/show_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/maddaq.egg-info/PKG-INFO` & `maddaq-0.7.6/maddaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.5
+Version: 0.7.6
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.5/maddaq.egg-info/SOURCES.txt` & `maddaq-0.7.6/maddaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.5/pyproject.toml` & `maddaq-0.7.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maddaq"
-version = "0.7.5"
+version = "0.7.6"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to access maddaq data."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

