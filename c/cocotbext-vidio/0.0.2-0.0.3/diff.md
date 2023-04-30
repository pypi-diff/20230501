# Comparing `tmp/cocotbext-vidio-0.0.2.tar.gz` & `tmp/cocotbext-vidio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocotbext-vidio-0.0.2.tar", last modified: Sat Apr 22 02:37:01 2023, max compression
+gzip compressed data, was "cocotbext-vidio-0.0.3.tar", last modified: Sun Apr 30 22:25:47 2023, max compression
```

## Comparing `cocotbext-vidio-0.0.2.tar` & `cocotbext-vidio-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-22 02:37:01.984484 cocotbext-vidio-0.0.2/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1075 2023-04-22 00:20:30.000000 cocotbext-vidio-0.0.2/LICENSE
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1726 2023-04-22 02:37:01.984484 cocotbext-vidio-0.0.2/PKG-INFO
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      819 2023-04-22 00:15:53.000000 cocotbext-vidio-0.0.2/README.md
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-22 02:37:01.984484 cocotbext-vidio-0.0.2/cocotbext/
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-22 02:37:01.984484 cocotbext-vidio-0.0.2/cocotbext/vidio/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)        0 2023-04-22 00:15:53.000000 cocotbext-vidio-0.0.2/cocotbext/vidio/__init__.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       79 2023-04-22 00:15:53.000000 cocotbext-vidio-0.0.2/cocotbext/vidio/csc.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     2054 2023-04-22 02:36:04.000000 cocotbext-vidio-0.0.2/cocotbext/vidio/tpg.py
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       87 2023-04-22 02:36:04.000000 cocotbext-vidio-0.0.2/cocotbext/vidio/utils.py
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-22 02:37:01.984484 cocotbext-vidio-0.0.2/cocotbext_vidio.egg-info/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1726 2023-04-22 02:37:01.000000 cocotbext-vidio-0.0.2/cocotbext_vidio.egg-info/PKG-INFO
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      347 2023-04-22 02:37:01.000000 cocotbext-vidio-0.0.2/cocotbext_vidio.egg-info/SOURCES.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)        1 2023-04-22 02:37:01.000000 cocotbext-vidio-0.0.2/cocotbext_vidio.egg-info/dependency_links.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       72 2023-04-22 02:37:01.000000 cocotbext-vidio-0.0.2/cocotbext_vidio.egg-info/requires.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       10 2023-04-22 02:37:01.000000 cocotbext-vidio-0.0.2/cocotbext_vidio.egg-info/top_level.txt
--rw-rw-r--   0 nkm       (1000) nkm       (1000)     1097 2023-04-22 02:37:01.984484 cocotbext-vidio-0.0.2/setup.cfg
--rw-rw-r--   0 nkm       (1000) nkm       (1000)       79 2023-04-22 02:36:04.000000 cocotbext-vidio-0.0.2/setup.py
-drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-22 02:37:01.984484 cocotbext-vidio-0.0.2/tests/
--rw-rw-r--   0 nkm       (1000) nkm       (1000)      366 2023-04-22 02:36:04.000000 cocotbext-vidio-0.0.2/tests/test_tpg.py
+drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)     1075 2023-04-30 22:02:02.000000 cocotbext-vidio-0.0.3/LICENSE
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)     1634 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/PKG-INFO
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)      727 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/README.md
+drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/cocotbext/
+drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/cocotbext/vidio/
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)       87 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/__init__.py
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)    10699 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/colorconv.py
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)      295 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/constants.py
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)      609 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/csc.py
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)     2054 2023-04-30 22:03:53.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/tpg.py
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)     2034 2023-04-30 22:05:53.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/utils.py
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)       21 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/version.py
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)     1895 2023-04-30 22:02:11.000000 cocotbext-vidio-0.0.3/cocotbext/vidio/vidio.py
+drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)     1634 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/PKG-INFO
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)      457 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/SOURCES.txt
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)        1 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/dependency_links.txt
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)       72 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/requires.txt
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)       10 2023-04-30 22:25:47.000000 cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/top_level.txt
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)     1133 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/setup.cfg
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)       78 2023-04-30 22:04:31.000000 cocotbext-vidio-0.0.3/setup.py
+drwxrwxr-x   0 nkm       (1000) nkm       (1000)        0 2023-04-30 22:25:47.746376 cocotbext-vidio-0.0.3/tests/
+-rw-rw-r--   0 nkm       (1000) nkm       (1000)      396 2023-04-30 22:05:46.000000 cocotbext-vidio-0.0.3/tests/test_tpg.py
```

### Comparing `cocotbext-vidio-0.0.2/LICENSE` & `cocotbext-vidio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cocotbext-vidio-0.0.2/PKG-INFO` & `cocotbext-vidio-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotbext-vidio
-Version: 0.0.2
+Version: 0.0.3
 Summary: AXIS video subsystem for cocotb
 Home-page: https://github.com/nitheeshkm/cocotbext-vidio
 Download-URL: https://github.com/nitheeshkm/cocotbext-vidio/tarball/main
 Author: Nitheesh Manjunath
 Author-email: nitheesh2013@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nitheeshkm/cocotbext-vidio/issues
@@ -20,28 +20,28 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # vidio (video io)
 
-This was built to generate simulation model similar to AMD-Xilinx Test Pattern Generator IP but can be used with cocotb
+This generates the AXIStream frame for video subsystems to be used with cocotb.  
 
-Implemented
-- Generates an AXI stream of one RGB video frame with specfied resolution, pixel-width and pattern. 
+Functions:
+- GenRGBAXIStream: Generates an AXIS frame
+- ConvertAXIStreamCS: Converts color space RGB to YUV [In development] 
 
 Roadmap:
 - AXIS to matrix
 - Matrix to AXIS
 - Generate color bars AXIS/matrix, supporting ITU-R BT.601-7, ITU-R BT.709-5
 - Color convertion
 - Chroma convertion
 - Video to SMPTE-2110 packet
 
 References:
 - [Xilinx TPG](https://www.xilinx.com/content/dam/xilinx/support/documents/ip_documentation/v_tpg/v8_1/pg103-v-tpg.pdf)
 - [cocotb](https://docs.cocotb.org/en/stable/)
 - [cocotbext-axi](https://github.com/alexforencich/cocotbext-axi)
-- [vlc python bindings](https://wiki.videolan.org/python_bindings)
 
 #
 <!-- <https://docs.cocotb.org/en/stable/extensions.html -->
```

### Comparing `cocotbext-vidio-0.0.2/cocotbext/vidio/tpg.py` & `cocotbext-vidio-0.0.3/cocotbext/vidio/tpg.py`

 * *Files identical despite different names*

### Comparing `cocotbext-vidio-0.0.2/cocotbext_vidio.egg-info/PKG-INFO` & `cocotbext-vidio-0.0.3/cocotbext_vidio.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotbext-vidio
-Version: 0.0.2
+Version: 0.0.3
 Summary: AXIS video subsystem for cocotb
 Home-page: https://github.com/nitheeshkm/cocotbext-vidio
 Download-URL: https://github.com/nitheeshkm/cocotbext-vidio/tarball/main
 Author: Nitheesh Manjunath
 Author-email: nitheesh2013@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nitheeshkm/cocotbext-vidio/issues
@@ -20,28 +20,28 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # vidio (video io)
 
-This was built to generate simulation model similar to AMD-Xilinx Test Pattern Generator IP but can be used with cocotb
+This generates the AXIStream frame for video subsystems to be used with cocotb.  
 
-Implemented
-- Generates an AXI stream of one RGB video frame with specfied resolution, pixel-width and pattern. 
+Functions:
+- GenRGBAXIStream: Generates an AXIS frame
+- ConvertAXIStreamCS: Converts color space RGB to YUV [In development] 
 
 Roadmap:
 - AXIS to matrix
 - Matrix to AXIS
 - Generate color bars AXIS/matrix, supporting ITU-R BT.601-7, ITU-R BT.709-5
 - Color convertion
 - Chroma convertion
 - Video to SMPTE-2110 packet
 
 References:
 - [Xilinx TPG](https://www.xilinx.com/content/dam/xilinx/support/documents/ip_documentation/v_tpg/v8_1/pg103-v-tpg.pdf)
 - [cocotb](https://docs.cocotb.org/en/stable/)
 - [cocotbext-axi](https://github.com/alexforencich/cocotbext-axi)
-- [vlc python bindings](https://wiki.videolan.org/python_bindings)
 
 #
 <!-- <https://docs.cocotb.org/en/stable/extensions.html -->
```

### Comparing `cocotbext-vidio-0.0.2/setup.cfg` & `cocotbext-vidio-0.0.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cocotbext-vidio
-version = 0.0.2
+version = attr: cocotbext.vidio.version.__version__
 author = Nitheesh Manjunath
 author_email = nitheesh2013@gmail.com
 description = AXIS video subsystem for cocotb
 keywords = axi, cocotb
 license = MIT
 url = https://github.com/nitheeshkm/cocotbext-vidio
 project_urls =
```

