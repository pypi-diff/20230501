# Comparing `tmp/ec_ecology_toolbox-0.0.3.tar.gz` & `tmp/ec_ecology_toolbox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec_ecology_toolbox-0.0.3.tar", last modified: Thu Apr 13 18:09:31 2023, max compression
+gzip compressed data, was "ec_ecology_toolbox-0.0.4.tar", last modified: Mon May  1 18:20:36 2023, max compression
```

## Comparing `ec_ecology_toolbox-0.0.3.tar` & `ec_ecology_toolbox-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:31.383500 ec_ecology_toolbox-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 18:09:09.000000 ec_ecology_toolbox-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 18:09:31.383500 ec_ecology_toolbox-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 18:09:09.000000 ec_ecology_toolbox-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:31.383500 ec_ecology_toolbox-0.0.3/ec_ecology_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 18:09:31.000000 ec_ecology_toolbox-0.0.3/ec_ecology_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-13 18:09:31.000000 ec_ecology_toolbox-0.0.3/ec_ecology_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:09:31.000000 ec_ecology_toolbox-0.0.3/ec_ecology_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:09:31.000000 ec_ecology_toolbox-0.0.3/ec_ecology_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 18:09:31.000000 ec_ecology_toolbox-0.0.3/ec_ecology_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 18:09:31.000000 ec_ecology_toolbox-0.0.3/ec_ecology_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 18:09:09.000000 ec_ecology_toolbox-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-13 18:09:31.383500 ec_ecology_toolbox-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-13 18:09:09.000000 ec_ecology_toolbox-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:31.383500 ec_ecology_toolbox-0.0.3/source/
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-13 18:09:09.000000 ec_ecology_toolbox-0.0.3/source/wrapper.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:31.383500 ec_ecology_toolbox-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-13 18:09:09.000000 ec_ecology_toolbox-0.0.3/tests/test_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/source/wrapper.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/tests/test_toolbox.py
```

### Comparing `ec_ecology_toolbox-0.0.3/LICENSE` & `ec_ecology_toolbox-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ec_ecology_toolbox-0.0.3/README.md` & `ec_ecology_toolbox-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 # EC Ecology Toolbox
 
 [![C/C++ CI](https://github.com/emilydolson/ec_ecology_toolbox/actions/workflows/c-cpp.yml/badge.svg)](https://github.com/emilydolson/ec_ecology_toolbox/actions/workflows/c-cpp.yml) 
 [![Python CI](https://github.com/emilydolson/ec_ecology_toolbox/actions/workflows/python_ci.yml/badge.svg)](https://github.com/emilydolson/ec_ecology_toolbox/actions/workflows/python_ci.yml)
 [![codecov](https://codecov.io/gh/emilydolson/ec_ecology_toolbox/branch/master/graph/badge.svg)](https://codecov.io/gh/emilydolson/ec_ecology_toolbox)
 [![PyPi Package Version](https://img.shields.io/pypi/v/ec-ecology-toolbox.svg)](https://pypi.python.org/pypi/ec-ecology-toolbox)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/ec-ecology-toolbox)
+[![Documentation Status](https://readthedocs.org/projects/ec-ecology-toolbox/badge/?version=latest)](https://ec-ecology-toolbox.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `ec_ecology_toolbox-0.0.3/setup.py` & `ec_ecology_toolbox-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `ec_ecology_toolbox-0.0.3/source/wrapper.cc` & `ec_ecology_toolbox-0.0.4/source/wrapper.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 #include "interaction_networks.hpp"
+#include "Evolve/NK.hpp"
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 namespace py = pybind11;
 
 PYBIND11_MODULE(ec_ecology_toolbox, m) {
     m.doc() = "Tools for measuring the ecology of various evolutionary algorithms"; 
@@ -97,8 +98,15 @@
 
             Returns
             -------
             List of floats
               The probabilities of each individual in pop being selected.            
             )mydelimiter",
           py::arg("pop"), py::arg("t_size") = 2);
+
+    py::class_<emp::Random>(m, "Random")
+      .def(py::init<int>());
+
+    py::class_<emp::NKLandscape>(m, "NKLandscape")
+      .def(py::init<size_t, size_t, emp::Random&>())
+      .def("GetFitness", static_cast<double (emp::NKLandscape::*)(size_t, size_t) const>(&emp::NKLandscape::GetFitness));
 }
```

### Comparing `ec_ecology_toolbox-0.0.3/tests/test_toolbox.py` & `ec_ecology_toolbox-0.0.4/tests/test_toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,7 +70,13 @@
     assert result[0] == pytest.approx(3/9)
     assert result[1] == pytest.approx(3/9)
 
     result = eco.TournamentFitness([[1, 2, 3], [2, 1, 3], [3, 3, 1]], t_size=3)
     assert result[2] == pytest.approx(1 - (2/3)**3)
     assert result[0] == pytest.approx(((2/3)**3)/2)
     assert result[1] == pytest.approx(((2/3)**3)/2)
+
+
+def test_nk():
+    r = eco.Random(-1)
+    nk = eco.NKLandscape(8, 2, r)
+    print(nk.GetFitness(0, 1))
```

