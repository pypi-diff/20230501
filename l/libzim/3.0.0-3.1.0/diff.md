# Comparing `tmp/libzim-3.0.0.tar.gz` & `tmp/libzim-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libzim-3.0.0.tar", last modified: Thu Mar 16 16:32:55 2023, max compression
+gzip compressed data, was "libzim-3.1.0.tar", last modified: Mon May  1 15:36:32 2023, max compression
```

## Comparing `libzim-3.0.0.tar` & `libzim-3.1.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 16:32:55.238546 libzim-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-03-16 16:32:29.000000 libzim-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-03-16 16:32:29.000000 libzim-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6040 2023-03-16 16:32:55.238546 libzim-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-03-16 16:32:29.000000 libzim-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 16:32:55.218546 libzim-3.0.0/lib/
--rwxr-xr-x   0 runner    (1001) docker     (122) 19948552 2022-11-30 17:21:47.000000 libzim-3.0.0/lib/libzim.so.8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 16:32:55.238546 libzim-3.0.0/libzim/
--rw-r--r--   0 runner    (1001) docker     (122)     6532 2023-03-16 16:32:29.000000 libzim-3.0.0/libzim/libwrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11058 2023-03-16 16:32:29.000000 libzim-3.0.0/libzim/libwrapper.h
--rw-r--r--   0 runner    (1001) docker     (122)  1411006 2023-03-16 16:32:37.000000 libzim-3.0.0/libzim/libzim.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1695 2023-03-16 16:32:37.000000 libzim-3.0.0/libzim/libzim.h
--rw-r--r--   0 runner    (1001) docker     (122)    44667 2023-03-16 16:32:29.000000 libzim-3.0.0/libzim/libzim.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     6350 2023-03-16 16:32:37.000000 libzim-3.0.0/libzim/libzim_api.h
--rw-r--r--   0 runner    (1001) docker     (122)     7746 2023-03-16 16:32:29.000000 libzim-3.0.0/libzim/zim.pxd
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 16:32:55.238546 libzim-3.0.0/libzim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-03-16 16:32:55.000000 libzim-3.0.0/libzim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-03-16 16:32:29.000000 libzim-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-03-16 16:32:29.000000 libzim-3.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-03-16 16:32:55.238546 libzim-3.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-03-16 16:32:29.000000 libzim-3.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     3655 2023-03-16 16:32:29.000000 libzim-3.0.0/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 16:32:55.238546 libzim-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    25520 2023-03-16 16:32:29.000000 libzim-3.0.0/tests/test_libzim_creator.py
--rw-r--r--   0 runner    (1001) docker     (122)    18261 2023-03-16 16:32:29.000000 libzim-3.0.0/tests/test_libzim_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      884 2023-03-16 16:32:29.000000 libzim-3.0.0/tests/test_libzim_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:32.867163 libzim-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 15:36:18.000000 libzim-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-01 15:36:18.000000 libzim-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-01 15:36:32.867163 libzim-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-01 15:36:18.000000 libzim-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:32.867163 libzim-3.1.0/libzim/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-01 15:36:18.000000 libzim-3.1.0/libzim/libwrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-01 15:36:18.000000 libzim-3.1.0/libzim/libwrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)  1412078 2023-05-01 15:36:32.000000 libzim-3.1.0/libzim/libzim.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-01 15:36:32.000000 libzim-3.1.0/libzim/libzim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44667 2023-05-01 15:36:18.000000 libzim-3.1.0/libzim/libzim.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-01 15:36:32.000000 libzim-3.1.0/libzim/libzim_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-01 15:36:18.000000 libzim-3.1.0/libzim/zim.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:32.867163 libzim-3.1.0/libzim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 15:36:32.000000 libzim-3.1.0/libzim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-01 15:36:18.000000 libzim-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-01 15:36:18.000000 libzim-3.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-01 15:36:32.867163 libzim-3.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15741 2023-05-01 15:36:18.000000 libzim-3.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-01 15:36:18.000000 libzim-3.1.0/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:32.867163 libzim-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-05-01 15:36:18.000000 libzim-3.1.0/tests/test_libzim_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18261 2023-05-01 15:36:18.000000 libzim-3.1.0/tests/test_libzim_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-01 15:36:18.000000 libzim-3.1.0/tests/test_libzim_version.py
```

### Comparing `libzim-3.0.0/LICENSE` & `libzim-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libzim-3.0.0/libzim/libwrapper.cpp` & `libzim-3.1.0/libzim/libwrapper.cpp`

 * *Files identical despite different names*

### Comparing `libzim-3.0.0/libzim/libwrapper.h` & `libzim-3.1.0/libzim/libwrapper.h`

 * *Files identical despite different names*

### Comparing `libzim-3.0.0/libzim/libzim.cpp` & `libzim-3.1.0/libzim/libzim.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=c++11",
             "-Wall",
             "-Wextra"
         ],
         "include_dirs": [
-            "libzim",
             "include"
         ],
         "language": "c++",
         "libraries": [
             "zim"
         ],
         "library_dirs": [
-            "lib"
+            "libzim"
         ],
         "name": "libzim",
+        "runtime_library_dirs": [
+            "$ORIGIN/libzim/"
+        ],
         "sources": [
             "libzim/libzim.pyx",
             "libzim/libwrapper.cpp"
         ]
     },
     "module_name": "libzim"
 }
@@ -35,16 +37,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -229,15 +231,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -268,15 +270,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1977,20 +1979,28 @@
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -25490,17 +25500,17 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
@@ -29137,28 +29147,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -30184,44 +30194,62 @@
     return -1;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `libzim-3.0.0/libzim/libzim.h` & `libzim-3.1.0/libzim/libzim.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef __PYX_HAVE__libzim
 #define __PYX_HAVE__libzim
 
 #include "Python.h"
 
 #ifndef __PYX_HAVE_API__libzim
```

### Comparing `libzim-3.0.0/libzim/libzim.pyx` & `libzim-3.1.0/libzim/libzim.pyx`

 * *Files identical despite different names*

### Comparing `libzim-3.0.0/libzim/libzim_api.h` & `libzim-3.1.0/libzim/libzim_api.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef __PYX_HAVE_API__libzim
 #define __PYX_HAVE_API__libzim
 #ifdef __MINGW64__
 #define MS_WIN64
 #endif
 #include "Python.h"
```

### Comparing `libzim-3.0.0/libzim/zim.pxd` & `libzim-3.1.0/libzim/zim.pxd`

 * *Files identical despite different names*

### Comparing `libzim-3.0.0/setup.cfg` & `libzim-3.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libzim
-version = 3.0.0
+version = 3.1.0
 url = https://github.com/openzim/python-libzim
 project_urls = 
 	Donate = https://www.kiwix.org/en/support-us/
 description = A python-facing API for creating and interacting with ZIM files
 author = Monadical Inc.
 author_email = jdc@monadical.com
 maintainer = openZIM
@@ -20,15 +20,14 @@
 	Topic :: System :: Archiving
 	Topic :: System :: Archiving :: Compression
 	Topic :: System :: Archiving :: Mirroring
 	Topic :: System :: Archiving :: Backup
 	Intended Audience :: Developers
 	Programming Language :: Cython
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Typing :: Stubs Only
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,20 +36,25 @@
 
 [options]
 include_package_data = True
 zim_safe = False
 packages = 
 	libzim
 python_requires = 
-	>=3.6,<3.12
+	>=3.7,<3.12
 setup_requires = 
-	cython >= 0.29.32,<0.30
+	cython >= 0.29.34,<0.30
 test_requires = 
 	pytest
 
+[options.package_data]
+libzim = 
+	libzim.8.dylib
+	libzim.so.8
+
 [isort]
 profile = black
 
 [flake8]
 max-line-length = 88
 
 [egg_info]
```

### Comparing `libzim-3.0.0/tests/test_libzim_creator.py` & `libzim-3.1.0/tests/test_libzim_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 import base64
 import datetime
 import itertools
+import os
 import pathlib
 import subprocess
 import sys
 from typing import Dict
 
 import pytest
 
@@ -770,14 +771,15 @@
 
     with Creator(fpath) as c:
         with pytest.raises(RuntimeError, match="TypeError: an integer is required"):
             c.add_item(AnItem())
 
 
 def test_creator_badfilename(tmpdir):
-    # lack of perm
-    with pytest.raises(IOError):
-        Creator("/root/test.zim")
+    if os.getuid() != 0:
+        # lack of perm
+        with pytest.raises(IOError):
+            Creator("/root/test.zim")
 
     # forward slash points to non-existing folder
     with pytest.raises(IOError):
         Creator(tmpdir / "test/test.zim")
```

### Comparing `libzim-3.0.0/tests/test_libzim_reader.py` & `libzim-3.1.0/tests/test_libzim_reader.py`

 * *Files identical despite different names*

### Comparing `libzim-3.0.0/tests/test_libzim_version.py` & `libzim-3.1.0/tests/test_libzim_version.py`

 * *Files identical despite different names*

