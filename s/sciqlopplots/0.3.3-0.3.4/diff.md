# Comparing `tmp/sciqlopplots-0.3.3.tar.gz` & `tmp/sciqlopplots-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciqlopplots-0.3.3.tar", last modified: Tue Apr 25 08:27:59 2023, max compression
+gzip compressed data, was "sciqlopplots-0.3.4.tar", last modified: Mon May  1 08:53:17 2023, max compression
```

## Comparing `sciqlopplots-0.3.3.tar` & `sciqlopplots-0.3.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.clang-format
--rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.github/workflows/pythonpublish-linux.yml
--rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.github/workflows/pythonpublish-osx.yml
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.github/workflows/pythonpublish-win.yml
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.gitignore
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/COPYING
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/README.md
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/__init__.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/_QCustomPlot.hpp
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/bindings.h
--rw-r--r--   0        0        0    17049 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/bindings.xml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
--rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/src_list.py
--rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/snippets.cpp
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/meson.build
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMap.hpp
--rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMapResampler.hpp
--rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraph.hpp
--rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraphResampler.hpp
--rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlot.hpp
--rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlotItem.hpp
--rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopVerticalSpan.hpp
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/constants.hpp
--rw-r--r--   0        0        0     6070 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/numpy_wrappers.hpp
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/meson.build
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/meson_options.txt
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/pyproject.toml
--rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/GPL.txt
--rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/changelog.txt
--rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.cpp
--rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.h
--rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/setup.cfg
--rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopColorMap.cpp
--rw-r--r--   0        0        0     5102 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopGraph.cpp
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopPlot.cpp
--rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopPlotItem.cpp
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopVerticalSpan.cpp
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/numpy_wrappers.cpp
--rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/subprojects/cpp_utils.wrap
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/subprojects/hedley.wrap
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/QCP_Examples/plots/main.py
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/SciQLopColorMap/main.py
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/SciQLopGraph/main.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/SciQLopVerticalSpan/main.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/StackedGraphs/main.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/meson.build
--rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/meson.build
--rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/.clang-format
+-rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/.github/workflows/pythonpublish-linux.yml
+-rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/.github/workflows/pythonpublish-osx.yml
+-rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/.github/workflows/pythonpublish-win.yml
+-rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/COPYING
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/README.md
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/__init__.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/_QCustomPlot.hpp
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/bindings.h
+-rw-r--r--   0        0        0    17049 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/bindings.xml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
+-rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/src_list.py
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/bindings/snippets.cpp
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/SciQLopPlots/meson.build
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopColorMap.hpp
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopColorMapResampler.hpp
+-rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopGraph.hpp
+-rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopGraphResampler.hpp
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopPlot.hpp
+-rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopPlotItem.hpp
+-rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopVerticalSpan.hpp
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/constants.hpp
+-rw-r--r--   0        0        0     6070 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/include/SciQLopPlots/numpy_wrappers.hpp
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/meson.build
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/meson_options.txt
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/pyproject.toml
+-rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/qcustomplot-source/GPL.txt
+-rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/qcustomplot-source/changelog.txt
+-rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/qcustomplot-source/qcustomplot.cpp
+-rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/qcustomplot-source/qcustomplot.h
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/setup.cfg
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/src/SciQLopColorMap.cpp
+-rw-r--r--   0        0        0     5102 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/src/SciQLopGraph.cpp
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/src/SciQLopPlot.cpp
+-rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/src/SciQLopPlotItem.cpp
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/src/SciQLopVerticalSpan.cpp
+-rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/src/numpy_wrappers.cpp
+-rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/subprojects/cpp_utils.wrap
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/subprojects/hedley.wrap
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/tests/manual-tests/QCP_Examples/plots/main.py
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/tests/manual-tests/SciQLopColorMap/main.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/tests/manual-tests/SciQLopGraph/main.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/tests/manual-tests/SciQLopVerticalSpan/main.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/tests/manual-tests/StackedGraphs/main.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/tests/manual-tests/meson.build
+-rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/tests/meson.build
+-rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.3.4/PKG-INFO
```

### Comparing `sciqlopplots-0.3.3/.clang-format` & `sciqlopplots-0.3.4/.clang-format`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/.github/workflows/pythonpublish-linux.yml` & `sciqlopplots-0.3.4/.github/workflows/pythonpublish-linux.yml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/.github/workflows/pythonpublish-osx.yml` & `sciqlopplots-0.3.4/.github/workflows/pythonpublish-osx.yml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/.github/workflows/pythonpublish-win.yml` & `sciqlopplots-0.3.4/.github/workflows/pythonpublish-win.yml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/COPYING` & `sciqlopplots-0.3.4/COPYING`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/_QCustomPlot.hpp` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/_QCustomPlot.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/bindings.xml` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/bindings.xml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/rpath-helper.py` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/rpath-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/src_list.py` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/helper_scripts/src_list.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/bindings/snippets.cpp` & `sciqlopplots-0.3.4/SciQLopPlots/bindings/snippets.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 %CPPSELF.%FUNCTION_NAME (%1,%2,&a,&b);
 %PYARG_0 = PyTuple_New(2);
 PyTuple_SET_ITEM(%PYARG_0, 0, %CONVERTTOPYTHON[int](a));
 PyTuple_SET_ITEM(%PYARG_0, 1, %CONVERTTOPYTHON[int](b));
 // @snippet QCPColorMapData-coordToCell
 
 // @snippet SciQLopGraph-setData
+Py_BEGIN_ALLOW_THREADS
 %CPPSELF.setData(NpArray_view{pyArgs[0]}, NpArray_view{pyArgs[1]});
+Py_END_ALLOW_THREADS
 // @snippet SciQLopGraph-setData
 
 // @snippet SciQLopColorMap-setData
 Py_BEGIN_ALLOW_THREADS
 %CPPSELF.setData(NpArray_view{pyArgs[0]}, NpArray_view{pyArgs[1]}, NpArray_view{pyArgs[2]});
 Py_END_ALLOW_THREADS
 // @snippet SciQLopColorMap-setData
```

### Comparing `sciqlopplots-0.3.3/SciQLopPlots/meson.build` & `sciqlopplots-0.3.4/SciQLopPlots/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMap.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopColorMap.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMapResampler.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopColorMapResampler.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraph.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopGraph.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraphResampler.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopGraphResampler.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlot.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopPlot.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlotItem.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopPlotItem.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopVerticalSpan.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/SciQLopVerticalSpan.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/constants.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/constants.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/include/SciQLopPlots/numpy_wrappers.hpp` & `sciqlopplots-0.3.4/include/SciQLopPlots/numpy_wrappers.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/meson.build` & `sciqlopplots-0.3.4/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.3.3')
+project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.3.4')
 add_project_arguments(
             '-DCATCH_CONFIG_NO_POSIX_SIGNALS', # workaround for this https://github.com/catchorg/Catch2/issues/2192
             language: 'cpp',
             native: true
 )
 qt_sdk='qt6'
```

### Comparing `sciqlopplots-0.3.3/pyproject.toml` & `sciqlopplots-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/qcustomplot-source/GPL.txt` & `sciqlopplots-0.3.4/qcustomplot-source/GPL.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/qcustomplot-source/changelog.txt` & `sciqlopplots-0.3.4/qcustomplot-source/changelog.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.cpp` & `sciqlopplots-0.3.4/qcustomplot-source/qcustomplot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.h` & `sciqlopplots-0.3.4/qcustomplot-source/qcustomplot.h`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/src/SciQLopColorMap.cpp` & `sciqlopplots-0.3.4/src/SciQLopColorMap.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/src/SciQLopGraph.cpp` & `sciqlopplots-0.3.4/src/SciQLopGraph.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/src/SciQLopPlot.cpp` & `sciqlopplots-0.3.4/src/SciQLopPlot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/src/SciQLopPlotItem.cpp` & `sciqlopplots-0.3.4/src/SciQLopPlotItem.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/src/SciQLopVerticalSpan.cpp` & `sciqlopplots-0.3.4/src/SciQLopVerticalSpan.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/src/numpy_wrappers.cpp` & `sciqlopplots-0.3.4/src/numpy_wrappers.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/tests/manual-tests/QCP_Examples/plots/main.py` & `sciqlopplots-0.3.4/tests/manual-tests/QCP_Examples/plots/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/tests/manual-tests/SciQLopColorMap/main.py` & `sciqlopplots-0.3.4/tests/manual-tests/SciQLopColorMap/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/tests/manual-tests/SciQLopGraph/main.py` & `sciqlopplots-0.3.4/tests/manual-tests/SciQLopGraph/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/tests/manual-tests/SciQLopVerticalSpan/main.py` & `sciqlopplots-0.3.4/tests/manual-tests/SciQLopVerticalSpan/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/tests/manual-tests/StackedGraphs/main.py` & `sciqlopplots-0.3.4/tests/manual-tests/StackedGraphs/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/tests/manual-tests/meson.build` & `sciqlopplots-0.3.4/tests/manual-tests/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.3.3/PKG-INFO` & `sciqlopplots-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciqlopplots
-Version: 0.3.3
+Version: 0.3.4
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

