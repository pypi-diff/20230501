# Comparing `tmp/stissplice-1.0.3.tar.gz` & `tmp/stissplice-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stissplice-1.0.3.tar", last modified: Fri Apr 28 17:41:57 2023, max compression
+gzip compressed data, was "stissplice-1.0.4.tar", last modified: Mon May  1 19:13:32 2023, max compression
```

## Comparing `stissplice-1.0.3.tar` & `stissplice-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:57.794852 stissplice-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 17:41:44.000000 stissplice-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:41:57.794852 stissplice-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-28 17:41:44.000000 stissplice-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:41:57.794852 stissplice-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 17:41:44.000000 stissplice-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:57.794852 stissplice-1.0.3/stissplice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:44.000000 stissplice-1.0.3/stissplice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32529 2023-04-28 17:41:44.000000 stissplice-1.0.3/stissplice/splicer.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-28 17:41:44.000000 stissplice-1.0.3/stissplice/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:57.794852 stissplice-1.0.3/stissplice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:13:32.075539 stissplice-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 19:13:20.000000 stissplice-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-01 19:13:32.075539 stissplice-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-01 19:13:20.000000 stissplice-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:13:32.075539 stissplice-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-01 19:13:20.000000 stissplice-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:13:32.071539 stissplice-1.0.4/stissplice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:13:20.000000 stissplice-1.0.4/stissplice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32535 2023-05-01 19:13:20.000000 stissplice-1.0.4/stissplice/splicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-01 19:13:20.000000 stissplice-1.0.4/stissplice/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:13:32.071539 stissplice-1.0.4/stissplice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-01 19:13:32.000000 stissplice-1.0.4/stissplice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-01 19:13:32.000000 stissplice-1.0.4/stissplice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:13:32.000000 stissplice-1.0.4/stissplice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 19:13:32.000000 stissplice-1.0.4/stissplice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 19:13:32.000000 stissplice-1.0.4/stissplice.egg-info/top_level.txt
```

### Comparing `stissplice-1.0.3/LICENSE` & `stissplice-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.3/PKG-INFO` & `stissplice-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stissplice
-Version: 1.0.3
+Version: 1.0.4
 Summary: Splicer of STIS Echelle Spectra from Hubble Space Telescope
 Home-page: https://github.com/ladsantos/stissplice
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stissplice-1.0.3/README.md` & `stissplice-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.3/setup.py` & `stissplice-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist upload")
     sys.exit()
 
 setup(
     name="stissplice",
-    version="1.0.3",
+    version="1.0.4",
     author="Leonardo dos Santos",
     author_email="ldsantos@stsci.edu",
     packages=["stissplice"],
     url="https://github.com/ladsantos/stissplice",
     license="MIT",
     description="Splicer of STIS Echelle Spectra from Hubble Space Telescope",
     install_requires=[line.strip() for line in
```

### Comparing `stissplice-1.0.3/stissplice/splicer.py` & `stissplice-1.0.4/stissplice/splicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
 
     # First we need to determine which spectrum has a higher sensitivity
     avg_sensitivity = np.array([np.nanmean(ok['net'] / ok['flux'])
                                 for ok in overlap_sections])
 
     # We interpolate the lower-SNR spectra to the wavelength bins of the higher
     # SNR spectrum.
-    max_sens_idx = np.where(avg_sensitivity == max(avg_sensitivity))[0][0]
+    max_sens_idx = np.where(avg_sensitivity == np.nanmax(avg_sensitivity))[0][0]
     overlap_ref = overlap_sections.pop(max_sens_idx)
 
     f_interp = []
     err_interp = []
     net_interp = []
     for i in range(n_overlaps - 1):
         # Since we cannot really interpolate DQ flags, before we do the
```

### Comparing `stissplice-1.0.3/stissplice/tools.py` & `stissplice-1.0.4/stissplice/tools.py`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.3/stissplice.egg-info/PKG-INFO` & `stissplice-1.0.4/stissplice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stissplice
-Version: 1.0.3
+Version: 1.0.4
 Summary: Splicer of STIS Echelle Spectra from Hubble Space Telescope
 Home-page: https://github.com/ladsantos/stissplice
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

