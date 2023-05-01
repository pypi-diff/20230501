# Comparing `tmp/radbelt-0.1.0.tar.gz` & `tmp/radbelt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radbelt-0.1.0.tar", last modified: Thu Apr  8 18:38:49 2021, max compression
+gzip compressed data, was "radbelt-0.1.3.tar", last modified: Mon May  1 14:02:38 2023, max compression
```

## Comparing `radbelt-0.1.0.tar` & `radbelt-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-08 18:38:49.972616 radbelt-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      667 2021-04-08 18:38:49.972616 radbelt-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2606 2021-04-08 18:38:36.000000 radbelt-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      133 2021-04-08 18:38:36.000000 radbelt-0.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-08 18:38:49.968616 radbelt-0.1.0/radbelt/
--rw-r--r--   0 root         (0) root         (0)     2545 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1849 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/core.f
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-08 18:38:49.968616 radbelt-0.1.0/radbelt/extern/
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-08 18:38:49.972616 radbelt-0.1.0/radbelt/extern/aep8/
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/aep8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    83596 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/aep8/ae8max.asc
--rw-r--r--   0 root         (0) root         (0)    81254 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/aep8/ae8min.asc
--rw-r--r--   0 root         (0) root         (0)   100542 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/aep8/ap8max.asc
--rw-r--r--   0 root         (0) root         (0)   102318 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/aep8/ap8min.asc
--rw-r--r--   0 root         (0) root         (0)    14732 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/aep8/trmfun.f
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-08 18:38:49.972616 radbelt-0.1.0/radbelt/extern/igrf/
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1945.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1950.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1955.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1960.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1965.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1970.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1975.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1980.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1985.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1990.dat
--rw-r--r--   0 root         (0) root         (0)     1590 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf1995.dat
--rw-r--r--   0 root         (0) root         (0)     1655 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf2000.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf2005.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf2010.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/dgrf2015.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/igrf2020.dat
--rw-r--r--   0 root         (0) root         (0)     1786 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/igrf2020s.dat
--rw-r--r--   0 root         (0) root         (0)    43035 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/extern/igrf/shellig.f
--rw-r--r--   0 root         (0) root         (0)      611 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/paths.py
--rw-r--r--   0 root         (0) root         (0)      493 2021-04-08 18:38:36.000000 radbelt-0.1.0/radbelt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-08 18:38:49.968616 radbelt-0.1.0/radbelt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      667 2021-04-08 18:38:49.000000 radbelt-0.1.0/radbelt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1121 2021-04-08 18:38:49.000000 radbelt-0.1.0/radbelt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-08 18:38:49.000000 radbelt-0.1.0/radbelt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-08 18:38:49.000000 radbelt-0.1.0/radbelt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2021-04-08 18:38:49.000000 radbelt-0.1.0/radbelt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-08 18:38:49.000000 radbelt-0.1.0/radbelt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-08 18:38:49.972616 radbelt-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1218 2021-04-08 18:38:36.000000 radbelt-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)    12693 2023-05-01 14:02:23.000000 radbelt-0.1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-05-01 14:02:38.213750 radbelt-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-05-01 14:02:23.000000 radbelt-0.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-05-01 14:02:23.000000 radbelt-0.1.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt/
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt/_version.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/core.f
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.209750 radbelt-0.1.3/radbelt/extern/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt/extern/aep8/
+-rw-r--r--   0 root         (0) root         (0)    14732 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/extern/aep8/trmfun.f
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt/extern/igrf/
+-rw-r--r--   0 root         (0) root         (0)    43035 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/extern/igrf/shellig.f
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/paths.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 14:02:38.213750 radbelt-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      322 2023-05-01 14:02:23.000000 radbelt-0.1.3/setup.py
```

### Comparing `radbelt-0.1.0/README.md` & `radbelt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.0/radbelt/__init__.py` & `radbelt-0.1.3/radbelt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #
 # SPDX-License-Identifier: NASA-1.3
 #
 
 from astropy import units as u
 import numpy as np
 
+from ._version import version as __version__
 from .core import igrf as _igrf, aep8 as _aep8
 from .paths import IGRF_DATA_PATH, AEP8_DATA_PATH
 from .util import working_directory
 
 
 @working_directory(IGRF_DATA_PATH)
 @np.vectorize
```

### Comparing `radbelt-0.1.0/radbelt/core.f` & `radbelt-0.1.3/radbelt/core.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.0/radbelt/extern/aep8/trmfun.f` & `radbelt-0.1.3/radbelt/extern/aep8/trmfun.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.0/radbelt/extern/igrf/shellig.f` & `radbelt-0.1.3/radbelt/extern/igrf/shellig.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.0/radbelt/paths.py` & `radbelt-0.1.3/radbelt/paths.py`

 * *Files identical despite different names*

