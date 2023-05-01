# Comparing `tmp/abba_python-0.1.3.tar.gz` & `tmp/abba_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-dafhehj7\abba_python-0.1.3.tar", last modified: Mon May  1 13:40:32 2023, max compression
+gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-s2h3a4xa\abba_python-0.1.4.tar", last modified: Mon May  1 14:59:30 2023, max compression
```

## Comparing `abba_python-0.1.3.tar` & `abba_python-0.1.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/
--rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.3/HISTORY.rst
--rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1876 2023-05-01 13:40:32.000000 abba_python-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/docs/
--rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/Makefile
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/authors.rst
--rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.3/docs/conf.py
--rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/history.rst
--rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/index.rst
--rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.3/docs/usage.rst
--rw-rw-rw-   0        0        0      621 2023-05-01 13:40:32.000000 abba_python-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1386 2023-05-01 13:40:08.000000 abba_python-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python/
--rw-rw-rw-   0        0        0      175 2023-05-01 13:40:08.000000 abba_python-0.1.3/src/abba_python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python/abba_private/
--rw-rw-rw-   0        0        0     1810 2023-03-22 16:22:22.000000 abba_python-0.1.3/src/abba_python/abba_private/AbbaAtlas.py
--rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.3/src/abba_python/abba_private/AbbaMap.py
--rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.3/src/abba_python/abba_private/AbbaOntology.py
--rw-rw-rw-   0        0        0     2115 2023-03-22 16:24:20.000000 abba_python-0.1.3/src/abba_python/abba_private/DeepSliceProcessor.py
--rw-rw-rw-   0        0        0      230 2023-02-13 21:48:20.000000 abba_python-0.1.3/src/abba_python/abba_private/__init__.py
--rw-rw-rw-   0        0        0    38829 2023-05-01 12:05:50.000000 abba_python-0.1.3/src/abba_python/abba_python.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python/deepslice/
--rw-rw-rw-   0        0        0    20688 2023-03-22 15:57:33.000000 abba_python-0.1.3/src/abba_python/deepslice/DeepSlice.py
--rw-rw-rw-   0        0        0       48 2023-03-22 15:57:33.000000 abba_python-0.1.3/src/abba_python/deepslice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python/deepslice/utilities/
--rw-rw-rw-   0        0        0     5025 2022-09-25 13:45:55.000000 abba_python-0.1.3/src/abba_python/deepslice/utilities/QuickNII_functions.py
--rw-rw-rw-   0        0        0        0 2023-01-07 21:45:39.000000 abba_python-0.1.3/src/abba_python/deepslice/utilities/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-03-22 15:57:33.000000 abba_python-0.1.3/src/abba_python/deepslice/utilities/neuron_tools.py
--rw-rw-rw-   0        0        0    12364 2022-09-25 13:45:55.000000 abba_python-0.1.3/src/abba_python/deepslice/utilities/plane_alignment.py
--rw-rw-rw-   0        0        0    13145 2022-09-25 13:45:55.000000 abba_python-0.1.3/src/abba_python/deepslice/utilities/plane_alignment_rat.py
--rw-rw-rw-   0        0        0        0 2022-09-25 13:45:55.000000 abba_python-0.1.3/src/abba_python/deepslice/utilities/render_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python/itk/
--rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.3/src/abba_python/itk/__init__.py
--rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.3/src/abba_python/itk/abba_itk.py
--rw-rw-rw-   0        0        0     2827 2023-05-01 12:36:39.000000 abba_python-0.1.3/src/abba_python/run-abba-local-fiji.py
--rw-rw-rw-   0        0        0     2418 2023-03-22 16:04:53.000000 abba_python-0.1.3/src/abba_python/run-abba.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python/scijava_python_command/
--rw-rw-rw-   0        0        0      308 2022-10-31 22:05:25.000000 abba_python-0.1.3/src/abba_python/scijava_python_command/__init__.py
--rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.3/src/abba_python/scijava_python_command/command.py
--rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.3/src/abba_python/scijava_python_command/jupyter_ui.py
--rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.3/src/abba_python/scijava_python_command/magic.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1543 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.3/src/abba_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 13:40:32.000000 abba_python-0.1.3/src/abba_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 13:40:32.000000 abba_python-0.1.3/tests/
--rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.3/tests/test_abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/
+-rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.4/HISTORY.rst
+-rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1876 2023-05-01 14:59:30.000000 abba_python-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/docs/
+-rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/authors.rst
+-rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.4/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.4/docs/usage.rst
+-rw-rw-rw-   0        0        0      621 2023-05-01 14:59:30.000000 abba_python-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1386 2023-05-01 14:59:11.000000 abba_python-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python/
+-rw-rw-rw-   0        0        0      175 2023-05-01 14:59:11.000000 abba_python-0.1.4/src/abba_python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python/abba_private/
+-rw-rw-rw-   0        0        0     1810 2023-03-22 16:22:22.000000 abba_python-0.1.4/src/abba_python/abba_private/AbbaAtlas.py
+-rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.4/src/abba_python/abba_private/AbbaMap.py
+-rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.4/src/abba_python/abba_private/AbbaOntology.py
+-rw-rw-rw-   0        0        0     2115 2023-03-22 16:24:20.000000 abba_python-0.1.4/src/abba_python/abba_private/DeepSliceProcessor.py
+-rw-rw-rw-   0        0        0      230 2023-02-13 21:48:20.000000 abba_python-0.1.4/src/abba_python/abba_private/__init__.py
+-rw-rw-rw-   0        0        0    40376 2023-05-01 14:50:10.000000 abba_python-0.1.4/src/abba_python/abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python/deepslice/
+-rw-rw-rw-   0        0        0    20688 2023-03-22 15:57:33.000000 abba_python-0.1.4/src/abba_python/deepslice/DeepSlice.py
+-rw-rw-rw-   0        0        0       48 2023-03-22 15:57:33.000000 abba_python-0.1.4/src/abba_python/deepslice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python/deepslice/utilities/
+-rw-rw-rw-   0        0        0     5025 2022-09-25 13:45:55.000000 abba_python-0.1.4/src/abba_python/deepslice/utilities/QuickNII_functions.py
+-rw-rw-rw-   0        0        0        0 2023-01-07 21:45:39.000000 abba_python-0.1.4/src/abba_python/deepslice/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-03-22 15:57:33.000000 abba_python-0.1.4/src/abba_python/deepslice/utilities/neuron_tools.py
+-rw-rw-rw-   0        0        0    12364 2022-09-25 13:45:55.000000 abba_python-0.1.4/src/abba_python/deepslice/utilities/plane_alignment.py
+-rw-rw-rw-   0        0        0    13145 2022-09-25 13:45:55.000000 abba_python-0.1.4/src/abba_python/deepslice/utilities/plane_alignment_rat.py
+-rw-rw-rw-   0        0        0        0 2022-09-25 13:45:55.000000 abba_python-0.1.4/src/abba_python/deepslice/utilities/render_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python/itk/
+-rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.4/src/abba_python/itk/__init__.py
+-rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.4/src/abba_python/itk/abba_itk.py
+-rw-rw-rw-   0        0        0     2839 2023-05-01 14:31:10.000000 abba_python-0.1.4/src/abba_python/run-abba-local-fiji.py
+-rw-rw-rw-   0        0        0      995 2023-05-01 14:58:40.000000 abba_python-0.1.4/src/abba_python/run-abba.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python/scijava_python_command/
+-rw-rw-rw-   0        0        0      308 2022-10-31 22:05:25.000000 abba_python-0.1.4/src/abba_python/scijava_python_command/__init__.py
+-rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.4/src/abba_python/scijava_python_command/command.py
+-rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.4/src/abba_python/scijava_python_command/jupyter_ui.py
+-rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.4/src/abba_python/scijava_python_command/magic.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python.egg-info/
+-rw-rw-rw-   0        0        0     1876 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1543 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.4/src/abba_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 14:59:30.000000 abba_python-0.1.4/src/abba_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:30.000000 abba_python-0.1.4/tests/
+-rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.4/tests/test_abba_python.py
```

### Comparing `abba_python-0.1.3/CONTRIBUTING.rst` & `abba_python-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/LICENSE` & `abba_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/PKG-INFO` & `abba_python-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba_python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.3/README.rst` & `abba_python-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/docs/Makefile` & `abba_python-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/docs/conf.py` & `abba_python-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/docs/installation.rst` & `abba_python-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/docs/make.bat` & `abba_python-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/setup.cfg` & `abba_python-0.1.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.3
+current_version = 0.1.4
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `abba_python-0.1.3/setup.py` & `abba_python-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='abba_python',
     name='abba_python',
     packages=find_packages(include=['abba_python', 'abba_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nicoKiaru/abba_python',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

### Comparing `abba_python-0.1.3/src/abba_python/abba_private/AbbaAtlas.py` & `abba_python-0.1.4/src/abba_python/abba_private/AbbaAtlas.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/abba_private/AbbaMap.py` & `abba_python-0.1.4/src/abba_python/abba_private/AbbaMap.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/abba_private/AbbaOntology.py` & `abba_python-0.1.4/src/abba_python/abba_private/AbbaOntology.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/abba_private/DeepSliceProcessor.py` & `abba_python-0.1.4/src/abba_python/abba_private/DeepSliceProcessor.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/abba_python.py` & `abba_python-0.1.4/src/abba_python/abba_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Main module."""
 
-
 # Core
 import os
 import tempfile
 
 # BrainGlobe
 from bg_atlasapi import BrainGlobeAtlas
 from bg_atlasapi.list_atlases import get_all_atlases_lastversions, get_downloaded_atlases, get_local_atlas_version
@@ -14,26 +13,71 @@
 from scyjava import jimport
 import imagej
 
 # JPype
 from jpype.types import JString, JArray
 
 
+def start_imagej(headless: bool = False):
+    mode = "headless"
+    if not headless:
+        mode = "interactive"
+    ij = imagej.init(get_java_dependencies(), mode=mode)
+    enable_python_hooks(ij)
+    add_brainglobe_atlases(ij)
+
+    from scyjava import jimport
+    from jpype.types import JString
+
+    # loci.common.DebugTools.enableLogging("OFF");
+    DebugTools = jimport('loci.common.DebugTools')
+    # DebugTools.enableLogging('OFF')
+    DebugTools.enableLogging("INFO");
+    # DebugTools.enableLogging("DEBUG");
+
+    import platform
+    if platform.system() == 'Windows':
+        File = jimport('java.io.File')
+        # Now let's set the atlas folder location in a folder with all users access
+
+        AtlasLocationHelper = jimport('ch.epfl.biop.atlas.AtlasLocationHelper')
+        directory = os.path.join(os.environ['ProgramData'], 'abba-atlas')
+
+        # create the directory with write access for all users
+        try:
+            print('Attempt to set ABBA Atlas cache directory to ' + directory)
+            os.makedirs(directory, exist_ok=True)
+            atlasPath = str(directory)
+            AtlasLocationHelper.defaultCacheDir = File(JString(atlasPath))
+            print('ABBA Atlas cache directory set to ' + directory)
+        except OSError:
+            print('ERROR! Could not set ABBA Atlas cache dir')
+            # directory already exists ?
+            pass
+    else:
+        print('ERROR! ' + platform.system() + ' OS not supported yet.')
+    pass
+
+    if not headless:
+        ij.ui().showUI()
+
+
 def get_java_dependencies():
     """
     Returns the jar files that need to be included into the classpath
     of an imagej object in order to have a functional ABBA app
     these jars should be available in https://maven.scijava.org/
     :return:
     """
     imagej_core_dep = 'net.imagej:imagej:2.9.0'
     imagej_legacy_dep = 'net.imagej:imagej-legacy:0.39.3'
     abba_dep = 'ch.epfl.biop:ImageToAtlasRegister:0.5.3'
     return [imagej_core_dep, imagej_legacy_dep, abba_dep]
 
+
 def add_brainglobe_atlases(ij):
     # TODO : check connection available or not
     try:
         check_internet_connection()
         available_atlases = get_all_atlases_lastversions()
     except ConnectionError:
         available_atlases_nodict = get_downloaded_atlases()
@@ -42,14 +86,15 @@
             print(atlas)
             available_atlases[atlas] = get_local_atlas_version(atlas)
 
     AtlasChooserCommand = jimport('ch.epfl.biop.atlas.scijava.AtlasChooserCommand')
     from abba_private.AbbaAtlas import AbbaAtlas  # delayed import because the jvm should be set first
     from jpype import JImplements, JOverride
     Supplier = jimport('java.util.function.Supplier')
+
     # initialized
 
     @JImplements(Supplier)
     class AtlasSupplier(object):
 
         def __init__(self, atlas_name, ij):
             self.atlas_name = atlas_name
@@ -62,36 +107,39 @@
             current_atlas.initialize(None, None)
             Abba.opened_atlases[self.atlas_name] = current_atlas
             return current_atlas
 
     for atlas_name in available_atlases.keys():
         AtlasChooserCommand.registerAtlas(atlas_name, AtlasSupplier(atlas_name, ij))
 
+
 def enable_python_hooks(ij):
     from jpype import JImplements, JOverride
     PyPostprocessor = jimport('org.scijava.processor.PyPostprocessor')
     Supplier = jimport('java.util.function.Supplier')
     Consumer = jimport('java.util.function.Consumer')
     import logging
 
     logger = logging.getLogger('ABBAPostprocessor')
+
     @JImplements(Consumer)
     class IPyWidgetCommandPostProcessor(object):
 
         @JOverride
         def accept(self, module):
             self.module = module
             outputs = module.getOutputs()
             logger.debug('ABBA post-processing, module ' + str(module))
             print('ABBA post-processing, module ' + str(module))
             for output_key in outputs.keySet():
                 if not module.isOutputResolved(output_key):
                     logger.debug('Unresolved output: ' + str(output_key))
                     print('Unresolved output: ' + str(output_key))
-                    if str(module.getInfo().getOutput(output_key).getType()) == 'class ch.epfl.biop.atlas.aligner.gui.bdv.BdvMultislicePositionerView':
+                    if str(module.getInfo().getOutput(
+                        output_key).getType()) == 'class ch.epfl.biop.atlas.aligner.gui.bdv.BdvMultislicePositionerView':
                         print('MultiSlicePositionerView found')
                         view = module.getOutputs().get(output_key)
                         print(str(view.msp.getAtlas().getName()))
                         if str(view.msp.getAtlas().getName()) == 'Adult Mouse Brain - Allen Brain Atlas V3p1':
                             print('Adult Mouse Brain - Allen Brain Atlas V3p1 detected, installing DeepSlice module')
                             BdvScijavaHelper = jimport('sc.fiji.bdvpg.scijava.BdvScijavaHelper')
                             from jpype import JImplements, JOverride
@@ -110,36 +158,34 @@
 
                                 @JOverride
                                 def run(self):
                                     RegisterSlicesDeepSliceCommand = jimport(
                                         'ch.epfl.biop.atlas.aligner.command.RegisterSlicesDeepSliceCommand')
                                     # Any missing input parameter will lead to a popup window asking the missing argument to the user
                                     self.dsp.ij.command().run(RegisterSlicesDeepSliceCommand, True,
-                                                               "image_name_prefix", JString('Section'),
-                                                               "mp", view.msp,
-                                                               "deepSliceProcessor", self.dsp._run_deep_slice,
-                                                               "dataset_folder", JString(self.dsp.temp_folder)
-                                                               )
+                                                              "image_name_prefix", JString('Section'),
+                                                              "mp", view.msp,
+                                                              "deepSliceProcessor", self.dsp._run_deep_slice,
+                                                              "dataset_folder", JString(self.dsp.temp_folder)
+                                                              )
 
                             BdvScijavaHelper.addActionToBdvHandleMenu(view.getBdvh(),
                                                                       "Align>ABBA - DeepSlice Registration (Python)", 0,
                                                                       ExecuteDeepSlicePython(DSPlaceHolder(ij)))
 
-
-
     @JImplements(Supplier)
     class IPyWidgetCommandPreprocessorSupplier(object):
         @JOverride
         def get(self):
             return IPyWidgetCommandPostProcessor()
 
-
     PyPostprocessor.register(IPyWidgetCommandPreprocessorSupplier())
     print('ABBA Python hooks enabled')
 
+
 def prepare_deepslice_temp_folder(self):
     if not hasattr(self, '_run_deep_slice'):
         from src.abba_python.abba_private.DeepSliceProcessor import DeepSliceProcessor
         self._run_deep_slice = DeepSliceProcessor()
 
     # TODO : fix potential multiple running instance issues
     temp_folder = tempfile.gettempdir() + '/temp/deepslice/'
@@ -157,14 +203,15 @@
             # elif os.path.isdir(file_path):
             #    shutil.rmtree(file_path)
         except Exception as e:
             print('Failed to delete %s. Reason: %s' % (file_path, e))
     # print('Temp folder = '+str(temp_folder))
     return temp_folder
 
+
 class Abba:
     """Abba object which can be used to register sections to a BrainGlobe atlas object
     Parameters
     ----------
     atlas_name :
         Name of the atlas to be used, should be either:
          - available in BrainGlobe
@@ -185,20 +232,20 @@
         TO IMPROVE : test how well this matches with the BrainGlobe API
 
     """
 
     opened_atlases: dict = {}
 
     def __init__(
-            self,
-            atlas_name: str = 'Adult Mouse Brain - Allen Brain Atlas V3',
-            ij=None,
-            slicing_mode: str = 'coronal',  # or sagittal or horizontal
-            headless: bool = False,
-            enable_jupyter_ui: bool = False
+        self,
+        atlas_name: str = 'Adult Mouse Brain - Allen Brain Atlas V3',
+        ij=None,
+        slicing_mode: str = 'coronal',  # or sagittal or horizontal
+        headless: bool = False,
+        enable_jupyter_ui: bool = False
     ):
         if ij is None:
             if headless:
                 ij = imagej.init(get_java_dependencies())
                 if enable_jupyter_ui:
                     # below : experimental UI, uses ipywidgets instead of ImageJ's swing UI (very partial functionality)
                     from src.abba_python.scijava_python_command import enable_jupyter_ui
@@ -207,16 +254,14 @@
                 ij = imagej.init(get_java_dependencies(), mode='interactive')
                 ij.ui().showUI()
             self.ij = ij
         else:
             print('ij was provided, headless argument ignored')
             self.ij = ij
 
-
-
         # Look in object service to see if the atlas is not already opened by any chance
         # in java TODO
 
         # or in python
         if atlas_name not in Abba.opened_atlases:
             if atlas_name == 'Adult Mouse Brain - Allen Brain Atlas V3':
                 atlas_name = 'Adult Mouse Brain - Allen Brain Atlas V3p1'
@@ -230,15 +275,16 @@
             elif atlas_name == 'Rat - Waxholm Sprague Dawley V4p1':
                 WaxholmSpragueDawleyRatV4Command = jimport(
                     'ch.epfl.biop.atlas.rat.waxholm.spraguedawley.v4p1.command.WaxholmSpragueDawleyRatV4p1Command')
                 atlas = ij.command().run(WaxholmSpragueDawleyRatV4Command, True).get().getOutput("ba")
                 Abba.opened_atlases[atlas_name] = atlas
             else:
                 bg_atlas = BrainGlobeAtlas(atlas_name)
-                from src.abba_python.abba_private.AbbaAtlas import AbbaAtlas  # delayed import because the jvm should be correctly
+                from src.abba_python.abba_private.AbbaAtlas import \
+                    AbbaAtlas  # delayed import because the jvm should be correctly
                 # initialized
                 atlas = AbbaAtlas(bg_atlas, ij)
                 atlas.initialize(None, None)
                 Abba.opened_atlases[atlas_name] = atlas
                 ij.object().addObject(atlas, atlas_name)  # store it in java's object service
 
         self.atlas = Abba.opened_atlases[atlas_name]
@@ -282,15 +328,14 @@
                 if self.slicing_mode == 'coronal':
                     self.install_deepslice_bdv_ui()
                     pass
         else:
             # TODO: make sure it is visible
             pass
 
-
     def install_deepslice_bdv_ui(self):
 
         BdvScijavaHelper = jimport('sc.fiji.bdvpg.scijava.BdvScijavaHelper')
 
         from jpype import JImplements, JOverride
 
         Runnable = jimport('java.lang.Runnable')
@@ -317,15 +362,15 @@
         BdvScijavaHelper.addActionToBdvHandleMenu(self.bdv_view.getBdvh(),
                                                   "Align>ABBA - DeepSlice Registration (Python)", 0,
                                                   ExecuteDeepSlicePython(self))
 
     def get_bdv_view(self):
         return self.bdv_view
 
-    def prepare_deepslice_temp_folder(self): # TODO : remove
+    def prepare_deepslice_temp_folder(self):  # TODO : remove
         if not hasattr(self, '_run_deep_slice'):
             from src.abba_python.abba_private.DeepSliceProcessor import DeepSliceProcessor
             self._run_deep_slice = DeepSliceProcessor()
 
         # TODO : fix potential multiple running instance issues
         temp_folder = tempfile.gettempdir() + '/temp/deepslice/'
 
@@ -342,15 +387,14 @@
                 # elif os.path.isdir(file_path):
                 #    shutil.rmtree(file_path)
             except Exception as e:
                 print('Failed to delete %s. Reason: %s' % (file_path, e))
         # print('Temp folder = '+str(temp_folder))
         return temp_folder
 
-
     # ------------------------ IMPORT
     def import_from_files(self, filepaths, z_location=0, z_increment=0.02, split_rgb=False):
         """
 
         :param z_location:
             initial location in mm along the atlas cutting axis
         :param z_increment:
```

### Comparing `abba_python-0.1.3/src/abba_python/deepslice/DeepSlice.py` & `abba_python-0.1.4/src/abba_python/deepslice/DeepSlice.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/deepslice/utilities/QuickNII_functions.py` & `abba_python-0.1.4/src/abba_python/deepslice/utilities/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/deepslice/utilities/neuron_tools.py` & `abba_python-0.1.4/src/abba_python/deepslice/utilities/neuron_tools.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/deepslice/utilities/plane_alignment.py` & `abba_python-0.1.4/src/abba_python/deepslice/utilities/plane_alignment.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/deepslice/utilities/plane_alignment_rat.py` & `abba_python-0.1.4/src/abba_python/deepslice/utilities/plane_alignment_rat.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/itk/abba_itk.py` & `abba_python-0.1.4/src/abba_python/itk/abba_itk.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/run-abba-local-fiji.py` & `abba_python-0.1.4/src/abba_python/run-abba-local-fiji.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # core dependencies
 import time
 
-from abba_python import enable_python_hooks, add_brainglobe_atlases
+from abba_python.abba_python import enable_python_hooks, add_brainglobe_atlases
 # in order to wait for a jvm shutdown
 import jpype
 import imagej
 
 import os
 
 # THIS FILE SETS MANY PATHS EXPLICITLY WHEN ABBA IS INSTALLED FROM THE INSTALLER!
```

### Comparing `abba_python-0.1.3/src/abba_python/scijava_python_command/command.py` & `abba_python-0.1.4/src/abba_python/scijava_python_command/command.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/scijava_python_command/jupyter_ui.py` & `abba_python-0.1.4/src/abba_python/scijava_python_command/jupyter_ui.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python/scijava_python_command/magic.py` & `abba_python-0.1.4/src/abba_python/scijava_python_command/magic.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.3/src/abba_python.egg-info/PKG-INFO` & `abba_python-0.1.4/src/abba_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.3/src/abba_python.egg-info/SOURCES.txt` & `abba_python-0.1.4/src/abba_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

