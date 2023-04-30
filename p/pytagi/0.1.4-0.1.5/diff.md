# Comparing `tmp/pytagi-0.1.4.tar.gz` & `tmp/pytagi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytagi-0.1.4.tar", last modified: Sun Mar 12 19:21:28 2023, max compression
+gzip compressed data, was "pytagi-0.1.5.tar", last modified: Sun Apr 30 22:33:42 2023, max compression
```

## Comparing `pytagi-0.1.4.tar` & `pytagi-0.1.5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.798773 pytagi-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-03-12 19:21:14.000000 pytagi-0.1.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-03-12 19:21:14.000000 pytagi-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-03-12 19:21:14.000000 pytagi-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-03-12 19:21:28.798773 pytagi-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14111 2023-03-12 19:21:14.000000 pytagi-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-03-12 19:21:14.000000 pytagi-0.1.4/RELEASES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.778773 pytagi-0.1.4/extern/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.786773 pytagi-0.1.4/extern/action_scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-03-12 19:21:15.000000 pytagi-0.1.4/extern/action_scripts/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (122)     5786 2023-03-12 19:21:15.000000 pytagi-0.1.4/extern/action_scripts/install_cuda_ubuntu.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.786773 pytagi-0.1.4/extern/pybind11/
--rw-r--r--   0 runner    (1001) docker     (122)    10999 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.778773 pytagi-0.1.4/extern/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.790773 pytagi-0.1.4/extern/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (122)    23979 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (122)     7069 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (122)    65705 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (122)     8458 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (122)    28337 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (122)    49082 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (122)    17981 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (122)    24008 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (122)    42266 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (122)    31971 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (122)    11735 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (122)     4695 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (122)    79251 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (122)     9051 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (122)   126295 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (122)    90338 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (122)    14556 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (122)    27013 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    20608 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (122)     1163 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.794773 pytagi-0.1.4/extern/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.798773 pytagi-0.1.4/extern/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     2350 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (122)    10890 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (122)     1423 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1282 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (122)    13487 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     6930 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     7711 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-03-12 19:21:17.000000 pytagi-0.1.4/extern/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-03-12 19:21:15.000000 pytagi-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.798773 pytagi-0.1.4/pytagi/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-03-12 19:21:15.000000 pytagi-0.1.4/pytagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-03-12 19:21:15.000000 pytagi-0.1.4/pytagi/__version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-03-12 19:21:15.000000 pytagi-0.1.4/pytagi/metric.py
--rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-03-12 19:21:15.000000 pytagi-0.1.4/pytagi/tagi_network.py
--rw-r--r--   0 runner    (1001) docker     (122)    11314 2023-03-12 19:21:15.000000 pytagi-0.1.4/pytagi/tagi_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-12 19:21:15.000000 pytagi-0.1.4/pytagi/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 19:21:28.798773 pytagi-0.1.4/pytagi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-03-12 19:21:28.000000 pytagi-0.1.4/pytagi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-03-12 19:21:28.000000 pytagi-0.1.4/pytagi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-12 19:21:28.000000 pytagi-0.1.4/pytagi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-12 19:21:28.000000 pytagi-0.1.4/pytagi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-03-12 19:21:28.798773 pytagi-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5619 2023-03-12 19:21:15.000000 pytagi-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.440460 pytagi-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     6250 2023-04-30 22:33:21.000000 pytagi-0.1.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-30 22:33:21.000000 pytagi-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-30 22:33:21.000000 pytagi-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-30 22:33:42.440460 pytagi-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14111 2023-04-30 22:33:21.000000 pytagi-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-30 22:33:21.000000 pytagi-0.1.5/RELEASES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.432460 pytagi-0.1.5/extern/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.432460 pytagi-0.1.5/extern/action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-30 22:33:22.000000 pytagi-0.1.5/extern/action_scripts/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5786 2023-04-30 22:33:22.000000 pytagi-0.1.5/extern/action_scripts/install_cuda_ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.432460 pytagi-0.1.5/extern/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (122)    10999 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.432460 pytagi-0.1.5/extern/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (122)    23979 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7069 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (122)    65705 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8458 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (122)    28337 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (122)    49082 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17981 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (122)    24008 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (122)    42266 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (122)    31971 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (122)    11735 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4695 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (122)    79251 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (122)     9051 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (122)   126295 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (122)    90338 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14556 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    27013 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    20608 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (122)     1163 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.436460 pytagi-0.1.5/extern/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.440460 pytagi-0.1.5/extern/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     2350 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)    10890 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1423 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1282 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13487 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     6930 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     7711 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-30 22:33:24.000000 pytagi-0.1.5/extern/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-30 22:33:22.000000 pytagi-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.440460 pytagi-0.1.5/pytagi/
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-30 22:33:22.000000 pytagi-0.1.5/pytagi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-04-30 22:33:22.000000 pytagi-0.1.5/pytagi/__version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-30 22:33:22.000000 pytagi-0.1.5/pytagi/metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-04-30 22:33:22.000000 pytagi-0.1.5/pytagi/tagi_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11314 2023-04-30 22:33:22.000000 pytagi-0.1.5/pytagi/tagi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-30 22:33:22.000000 pytagi-0.1.5/pytagi/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 22:33:42.440460 pytagi-0.1.5/pytagi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-30 22:33:42.000000 pytagi-0.1.5/pytagi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-04-30 22:33:42.000000 pytagi-0.1.5/pytagi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 22:33:42.000000 pytagi-0.1.5/pytagi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-30 22:33:42.000000 pytagi-0.1.5/pytagi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-30 22:33:42.440460 pytagi-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5619 2023-04-30 22:33:22.000000 pytagi-0.1.5/setup.py
```

### Comparing `pytagi-0.1.4/CMakeLists.txt` & `pytagi-0.1.5/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -126,21 +126,25 @@
   src/task_cpu.cpp
   src/user_input.cpp
   src/utils.cpp
   src/feature_availability.cpp
   src/derivative_calcul_cpu.cpp
   src/tagi_network_cpu.cpp
   src/tagi_network_base.cpp
+  test/act_func/test_act_func_cpu.cpp
+  test/fnn/test_fnn_cpu.cpp
+  test/fnn_heteros/test_fnn_heteros_cpu.cpp
+  test/fnn_full_cov/test_fnn_full_cov_cpu.cpp
+  test/fnn_derivatives/test_fnn_derivatives_cpu.cpp
+  test/lstm/test_lstm_cpu.cpp
+  test/test_lstm.cpp
   test/test_lstm_cpu.cpp
   test/test_cpu.cpp
   test/test_regression.cpp
   test/test_dataloader.cpp
-  test/fnn/test_fnn_cpu.cpp
-  test/fnn_heteros/test_fnn_heteros_cpu.cpp
-  test/fnn_full_cov/test_fnn_full_cov_cpu.cpp
 )
 
 # Sources code for CUDA
 set(GPU_SOURCES
   ${CPU_SOURCES}
   src/data_transfer.cu
   src/global_param_update.cu
@@ -150,14 +154,20 @@
   src/derivative_calcul.cu
   src/lstm_feed_forward.cu
   src/lstm_feed_backward.cu
   src/activation_fun.cu
   src/task.cu
   src/tagi_network.cu
   src/gpu_debug_utils.cpp
+  test/test_gpu.cu
+  test/autoencoder/test_autoencoder_gpu.cu
+  test/cnn/test_cnn_gpu.cu
+  test/cnn_batch_norm/test_cnn_batch_norm_gpu.cu
+  test/test_classification.cu
+  test/test_autoencoder.cu
 )
 
 # Output binary folder der for different mode
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY_RELEASE ${CMAKE_BINARY_DIR})
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY_RELWITHDEBINFO ${CMAKE_BINARY_DIR})
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY_MINSIZEREL ${CMAKE_BINARY_DIR})
@@ -175,14 +185,15 @@
   # Executablecode i.e. application
   add_executable(main main.cu)
 
   # Python wrapper for C++/CUDA code
   pybind11_add_module(cutagi "src/python_api.cu")
 else()
   add_library(cutagi_lib STATIC ${CPU_SOURCES})
+  target_link_libraries(cutagi_lib ${CMAKE_DL_LIBS})
 
   # Executable code i.e. application
   add_executable(main main.cpp)
 
   # Python wrapper for C++/CUDA code
   pybind11_add_module(cutagi "src/python_api_cpu.cpp")
 endif()
```

### Comparing `pytagi-0.1.4/LICENSE` & `pytagi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/PKG-INFO` & `pytagi-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytagi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tractable Approximate Gaussian Inference
 Home-page: https://github.com/lhnguyen102/cuTAGI
 Author: Luong-Ha Nguyen and James-A. Goulet
 Author-email: luongha.nguyen@gmail.com, james.goulet@polymtl.ca
 License: MIT
 Project-URL: Download_url, https://github.com/lhnguyen102/cuTAGI
 Keywords: Bayesian,Neural Networks,Machine Learning,Tractability,C++11,CUDA
```

### Comparing `pytagi-0.1.4/README.md` & `pytagi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/RELEASES.md` & `pytagi-0.1.5/RELEASES.md`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/action_scripts/LICENSE` & `pytagi-0.1.5/extern/action_scripts/LICENSE`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/action_scripts/install_cuda_ubuntu.sh` & `pytagi-0.1.5/extern/action_scripts/install_cuda_ubuntu.sh`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/LICENSE` & `pytagi-0.1.5/extern/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/attr.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/buffer_info.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/cast.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/chrono.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/complex.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/detail/class.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/detail/common.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/detail/descr.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/detail/init.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/detail/internals.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/detail/type_caster_base.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/detail/typeid.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/eigen.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/embed.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/eval.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/functional.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/gil.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/iostream.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/numpy.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/operators.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/options.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/pybind11.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/pytypes.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/stl/filesystem.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/stl.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/include/pybind11/stl_bind.h` & `pytagi-0.1.5/extern/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tests/test_embed/CMakeLists.txt` & `pytagi-0.1.5/extern/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/FindCatch.cmake` & `pytagi-0.1.5/extern/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/FindEigen3.cmake` & `pytagi-0.1.5/extern/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/FindPythonLibsNew.cmake` & `pytagi-0.1.5/extern/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/check-style.sh` & `pytagi-0.1.5/extern/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/cmake_uninstall.cmake.in` & `pytagi-0.1.5/extern/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/libsize.py` & `pytagi-0.1.5/extern/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/make_changelog.py` & `pytagi-0.1.5/extern/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/pybind11Common.cmake` & `pytagi-0.1.5/extern/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/pybind11Config.cmake.in` & `pytagi-0.1.5/extern/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/pybind11NewTools.cmake` & `pytagi-0.1.5/extern/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/pybind11Tools.cmake` & `pytagi-0.1.5/extern/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/setup_global.py.in` & `pytagi-0.1.5/extern/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/extern/pybind11/tools/setup_main.py.in` & `pytagi-0.1.5/extern/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/pytagi/metric.py` & `pytagi-0.1.5/pytagi/metric.py`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/pytagi/tagi_network.py` & `pytagi-0.1.5/pytagi/tagi_network.py`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/pytagi/tagi_utils.py` & `pytagi-0.1.5/pytagi/tagi_utils.py`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/pytagi.egg-info/PKG-INFO` & `pytagi-0.1.5/pytagi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytagi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tractable Approximate Gaussian Inference
 Home-page: https://github.com/lhnguyen102/cuTAGI
 Author: Luong-Ha Nguyen and James-A. Goulet
 Author-email: luongha.nguyen@gmail.com, james.goulet@polymtl.ca
 License: MIT
 Project-URL: Download_url, https://github.com/lhnguyen102/cuTAGI
 Keywords: Bayesian,Neural Networks,Machine Learning,Tractability,C++11,CUDA
```

### Comparing `pytagi-0.1.4/pytagi.egg-info/SOURCES.txt` & `pytagi-0.1.5/pytagi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/setup.cfg` & `pytagi-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytagi-0.1.4/setup.py` & `pytagi-0.1.5/setup.py`

 * *Files identical despite different names*

