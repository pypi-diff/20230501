# Comparing `tmp/CUQIpy-CIL-0.3.0.tar.gz` & `tmp/CUQIpy-CIL-0.3.0.post0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-CIL-0.3.0.tar", last modified: Wed Feb 22 09:53:06 2023, max compression
+gzip compressed data, was "CUQIpy-CIL-0.3.0.post0.dev2.tar", last modified: Mon May  1 06:34:22 2023, max compression
```

## Comparing `CUQIpy-CIL-0.3.0.tar` & `CUQIpy-CIL-0.3.0.post0.dev2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:53:06.327410 CUQIpy-CIL-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:53:06.323410 CUQIpy-CIL-0.3.0/CUQIpy_CIL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-02-22 09:53:06.000000 CUQIpy-CIL-0.3.0/CUQIpy_CIL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-22 09:53:06.000000 CUQIpy-CIL-0.3.0/CUQIpy_CIL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:53:06.000000 CUQIpy-CIL-0.3.0/CUQIpy_CIL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 09:53:06.000000 CUQIpy-CIL-0.3.0/CUQIpy_CIL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 09:53:06.000000 CUQIpy-CIL-0.3.0/CUQIpy_CIL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-02-22 09:53:06.327410 CUQIpy-CIL-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:53:06.327410 CUQIpy-CIL-0.3.0/cuqipy_cil/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/cuqipy_cil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-22 09:53:06.327410 CUQIpy-CIL-0.3.0/cuqipy_cil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/cuqipy_cil/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/cuqipy_cil/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/cuqipy_cil/testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:53:06.327410 CUQIpy-CIL-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:53:06.327410 CUQIpy-CIL-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-22 09:52:51.000000 CUQIpy-CIL-0.3.0/tests/test_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/tests/test_testproblem.py
```

### Comparing `CUQIpy-CIL-0.3.0/CUQIpy_CIL.egg-info/PKG-INFO` & `CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-CIL
-Version: 0.3.0
+Version: 0.3.0.post0.dev2
 Summary: CUQIpy plugin for CIL
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -228,15 +228,15 @@
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 import cuqi
 import cuqipy_cil
 
 # Load a CT forward model and data from testproblem library
-A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2DProblem.get_components(
+A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2D.get_components(
     im_size=(128, 128),
     det_count=128,
     angles=np.linspace(0, np.pi, 180),
     phantom="shepp-logan"
 )
 
 # Set up Bayesian model
```

### Comparing `CUQIpy-CIL-0.3.0/LICENSE` & `CUQIpy-CIL-0.3.0.post0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0/PKG-INFO` & `CUQIpy-CIL-0.3.0.post0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-CIL
-Version: 0.3.0
+Version: 0.3.0.post0.dev2
 Summary: CUQIpy plugin for CIL
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -228,15 +228,15 @@
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 import cuqi
 import cuqipy_cil
 
 # Load a CT forward model and data from testproblem library
-A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2DProblem.get_components(
+A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2D.get_components(
     im_size=(128, 128),
     det_count=128,
     angles=np.linspace(0, np.pi, 180),
     phantom="shepp-logan"
 )
 
 # Set up Bayesian model
```

### Comparing `CUQIpy-CIL-0.3.0/README.md` & `CUQIpy-CIL-0.3.0.post0.dev2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 import cuqi
 import cuqipy_cil
 
 # Load a CT forward model and data from testproblem library
-A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2DProblem.get_components(
+A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2D.get_components(
     im_size=(128, 128),
     det_count=128,
     angles=np.linspace(0, np.pi, 180),
     phantom="shepp-logan"
 )
 
 # Set up Bayesian model
```

### Comparing `CUQIpy-CIL-0.3.0/cuqipy_cil/config.py` & `CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0/cuqipy_cil/model.py` & `CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0/cuqipy_cil/testproblem.py` & `CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/testproblem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import cuqi
 import numpy as np
 import cuqipy_cil
 
 #=============================================================================
-class ParallelBeam2DProblem(cuqi.problem.BayesianProblem):
+class ParallelBeam2D(cuqi.problem.BayesianProblem):
     """ 2D parallel-beam Computed Tomography test problem using CIL.
 
     Parameters
     ----------
     im_size : tuple of ints
         Dimensions of image in pixels.
```

### Comparing `CUQIpy-CIL-0.3.0/pyproject.toml` & `CUQIpy-CIL-0.3.0.post0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0/tests/test_model.py` & `CUQIpy-CIL-0.3.0.post0.dev2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0/tests/test_testproblem.py` & `CUQIpy-CIL-0.3.0.post0.dev2/tests/test_testproblem.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 import cuqi
 import numpy as np
 import matplotlib.pyplot as plt
 
 def test_testproblem_simple():
     # Create simple testproblem
-    TP = cuqipy_cil.testproblem.ParallelBeam2DProblem()
+    TP = cuqipy_cil.testproblem.ParallelBeam2D()
 
     # First check dimension of model matches dimension of image + data
     assert TP.model.domain_dim == TP.exactSolution.geometry.par_dim
 
     # Check that the output is the correct shape
     assert TP.model.range_dim == TP.exactData.geometry.par_dim
 
@@ -33,24 +33,24 @@
         (cuqi.data.grains(size=128)),
         ("shepp_logan"),
         ("p_power"),
         ("grains"),
     ])
 def test_testproblem_phantom(phantom):
     # Create simple testproblem
-    TP = cuqipy_cil.testproblem.ParallelBeam2DProblem(im_size=(128,128), phantom=phantom)
+    TP = cuqipy_cil.testproblem.ParallelBeam2D(im_size=(128,128), phantom=phantom)
 
     if isinstance(phantom, str): # If phantom is a string, it should be a valid phantom name
         phantom = cuqi.data.__dict__[phantom](size=TP.model.domain_geometry.fun_shape[0])
 
     assert np.allclose(TP.exactSolution, cuqi.data.imresize(phantom, TP.model.domain_geometry.fun_shape))
 
 def test_testproblem_set_prior():
     """ Test if one can set a prior after creating a testproblem """
-    TP = cuqipy_cil.testproblem.ParallelBeam2DProblem(
+    TP = cuqipy_cil.testproblem.ParallelBeam2D(
         im_size=(256, 256),
         det_count=256,
         angles=np.linspace(0, np.pi, 180),
         phantom="shepp-logan",
     )
 
     # Cauchy difference prior
@@ -65,15 +65,15 @@
 
     # Plot sample mean and ci
     samples.plot_ci()
 
 def test_testproblem_from_readme():
 
     # Load a CT forward model and data from testproblem library
-    A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2DProblem.get_components(
+    A, y_data, info = cuqipy_cil.testproblem.ParallelBeam2D.get_components(
         im_size=(128, 128),
         det_count=128,
         angles=np.linspace(0, np.pi, 180),
         phantom="shepp-logan"
     )
 
     # Set up Bayesian model
```

