# Comparing `tmp/SpectroscopicBinarySystem-1.1.41.tar.gz` & `tmp/SpectroscopicBinarySystem-1.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.1.41.tar", last modified: Mon May  1 08:02:29 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.1.42.tar", last modified: Mon May  1 09:14:58 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.1.41.tar` & `SpectroscopicBinarySystem-1.1.42.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 08:02:29.299115 SpectroscopicBinarySystem-1.1.41/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.41/LICENSE
--rw-rw-rw-   0        0        0     4731 2023-05-01 08:02:29.299115 SpectroscopicBinarySystem-1.1.41/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2023-04-30 07:01:52.000000 SpectroscopicBinarySystem-1.1.41/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 08:02:29.287400 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4731 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.41/pyproject.toml
--rw-rw-rw-   0        0        0      725 2023-05-01 08:02:29.299115 SpectroscopicBinarySystem-1.1.41/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 08:02:29.295916 SpectroscopicBinarySystem-1.1.41/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    29368 2023-05-01 07:46:22.000000 SpectroscopicBinarySystem-1.1.41/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:14:58.923858 SpectroscopicBinarySystem-1.1.42/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.42/LICENSE
+-rw-rw-rw-   0        0        0     4732 2023-05-01 09:14:58.923858 SpectroscopicBinarySystem-1.1.42/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2023-05-01 08:09:46.000000 SpectroscopicBinarySystem-1.1.42/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 09:14:58.919834 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4732 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.42/pyproject.toml
+-rw-rw-rw-   0        0        0      725 2023-05-01 09:14:58.927845 SpectroscopicBinarySystem-1.1.42/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 09:14:58.923858 SpectroscopicBinarySystem-1.1.42/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    29374 2023-05-01 09:13:08.000000 SpectroscopicBinarySystem-1.1.42/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.1.41/LICENSE` & `SpectroscopicBinarySystem-1.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.41/PKG-INFO` & `SpectroscopicBinarySystem-1.1.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.41
+Version: 1.1.42
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.4)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.41)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.41/README.md` & `SpectroscopicBinarySystem-1.1.42/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.4)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.41)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.41
+Version: 1.1.42
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.4)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.41)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.41/setup.cfg` & `SpectroscopicBinarySystem-1.1.42/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 312e 3431 0d0a  rsion = 1.1.41..
+00000030: 7273 696f 6e20 3d20 312e 312e 3432 0d0a  rsion = 1.1.42..
 00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
 00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
 00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
 00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
 00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
 000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.1.41/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.1.42/spectroscopicbinarysystem/__init__.py`

 * *Files identical despite different names*

```diff
@@ -391,15 +391,15 @@
             self._t0 = self._orbital_solution[0][4] + 2400000
             self._v0 = 0
 
         period = self._orbital_solution[0][5]
         for s in self._sb_spectra:
             # compute phase of the sytem
             jd = s.getJD()
-            phase = self.__getPhase(float(t0), period, jd)
+            phase = self.__getPhase(float(self._t0), period, jd)
             s.setPhase(phase)
             if self._debug:
                 print(f"{s.getBaseName()} phase : {phase}")
 
         print(
             f'{self._object_name} orbital solution with {len(self._sb_spectra)} spectra',
             f'- γ = {params[0]} ± {err[0]}',
```

