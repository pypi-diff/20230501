# Comparing `tmp/abba_python-0.1.0.tar.gz` & `tmp/abba_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-e3ztzxe1\abba_python-0.1.0.tar", last modified: Wed Mar 22 16:38:48 2023, max compression
+gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-spk5vkga\abba_python-0.1.2.tar", last modified: Mon May  1 13:18:36 2023, max compression
```

## Comparing `abba_python-0.1.0.tar` & `abba_python-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 16:38:48.000000 abba_python-0.1.0/
--rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1876 2023-03-22 16:38:48.000000 abba_python-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-22 16:38:48.000000 abba_python-0.1.0/docs/
--rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.0/docs/usage.rst
--rw-rw-rw-   0        0        0      617 2023-03-22 16:38:48.000000 abba_python-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-03-22 13:49:35.000000 abba_python-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 16:38:48.000000 abba_python-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 16:38:48.000000 abba_python-0.1.0/src/abba_python.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-03-22 16:38:48.000000 abba_python-0.1.0/src/abba_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-03-22 16:38:48.000000 abba_python-0.1.0/src/abba_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 16:38:48.000000 abba_python-0.1.0/src/abba_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.0/src/abba_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-03-22 16:38:48.000000 abba_python-0.1.0/src/abba_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 16:38:48.000000 abba_python-0.1.0/src/abba_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 16:38:48.000000 abba_python-0.1.0/tests/
--rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.0/tests/test_abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/
+-rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1876 2023-05-01 13:18:36.000000 abba_python-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/docs/
+-rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.2/docs/usage.rst
+-rw-rw-rw-   0        0        0      621 2023-05-01 13:18:36.000000 abba_python-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-05-01 13:18:14.000000 abba_python-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python/
+-rw-rw-rw-   0        0        0      175 2023-05-01 13:18:14.000000 abba_python-0.1.2/src/abba_python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python/abba_private/
+-rw-rw-rw-   0        0        0     1810 2023-03-22 16:22:22.000000 abba_python-0.1.2/src/abba_python/abba_private/AbbaAtlas.py
+-rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.2/src/abba_python/abba_private/AbbaMap.py
+-rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.2/src/abba_python/abba_private/AbbaOntology.py
+-rw-rw-rw-   0        0        0     2115 2023-03-22 16:24:20.000000 abba_python-0.1.2/src/abba_python/abba_private/DeepSliceProcessor.py
+-rw-rw-rw-   0        0        0      230 2023-02-13 21:48:20.000000 abba_python-0.1.2/src/abba_python/abba_private/__init__.py
+-rw-rw-rw-   0        0        0    38829 2023-05-01 12:05:50.000000 abba_python-0.1.2/src/abba_python/abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python/deepslice/
+-rw-rw-rw-   0        0        0    20688 2023-03-22 15:57:33.000000 abba_python-0.1.2/src/abba_python/deepslice/DeepSlice.py
+-rw-rw-rw-   0        0        0       48 2023-03-22 15:57:33.000000 abba_python-0.1.2/src/abba_python/deepslice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python/deepslice/utilities/
+-rw-rw-rw-   0        0        0     5025 2022-09-25 13:45:55.000000 abba_python-0.1.2/src/abba_python/deepslice/utilities/QuickNII_functions.py
+-rw-rw-rw-   0        0        0        0 2023-01-07 21:45:39.000000 abba_python-0.1.2/src/abba_python/deepslice/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-03-22 15:57:33.000000 abba_python-0.1.2/src/abba_python/deepslice/utilities/neuron_tools.py
+-rw-rw-rw-   0        0        0    12364 2022-09-25 13:45:55.000000 abba_python-0.1.2/src/abba_python/deepslice/utilities/plane_alignment.py
+-rw-rw-rw-   0        0        0    13145 2022-09-25 13:45:55.000000 abba_python-0.1.2/src/abba_python/deepslice/utilities/plane_alignment_rat.py
+-rw-rw-rw-   0        0        0        0 2022-09-25 13:45:55.000000 abba_python-0.1.2/src/abba_python/deepslice/utilities/render_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python/itk/
+-rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.2/src/abba_python/itk/__init__.py
+-rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.2/src/abba_python/itk/abba_itk.py
+-rw-rw-rw-   0        0        0     2827 2023-05-01 12:36:39.000000 abba_python-0.1.2/src/abba_python/run-abba-local-fiji.py
+-rw-rw-rw-   0        0        0     2418 2023-03-22 16:04:53.000000 abba_python-0.1.2/src/abba_python/run-abba.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python/scijava_python_command/
+-rw-rw-rw-   0        0        0      308 2022-10-31 22:05:25.000000 abba_python-0.1.2/src/abba_python/scijava_python_command/__init__.py
+-rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.2/src/abba_python/scijava_python_command/command.py
+-rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.2/src/abba_python/scijava_python_command/jupyter_ui.py
+-rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.2/src/abba_python/scijava_python_command/magic.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python.egg-info/
+-rw-rw-rw-   0        0        0     1876 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1505 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.2/src/abba_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-01 13:18:36.000000 abba_python-0.1.2/src/abba_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 13:18:36.000000 abba_python-0.1.2/tests/
+-rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.2/tests/test_abba_python.py
```

### Comparing `abba_python-0.1.0/CONTRIBUTING.rst` & `abba_python-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.0/LICENSE` & `abba_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.0/PKG-INFO` & `abba_python-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba_python
-Version: 0.1.0
+Version: 0.1.2
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.0/README.rst` & `abba_python-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.0/docs/Makefile` & `abba_python-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.0/docs/conf.py` & `abba_python-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.0/docs/installation.rst` & `abba_python-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.0/docs/make.bat` & `abba_python-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.0/setup.cfg` & `abba_python-0.1.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
-[bumpversion:file:abba_python/__init__.py]
+[bumpversion:file:src/abba_python/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 exclude = docs
 
 [options]
+package_dir = 
+	=src
 packages = find:
+
+[options.packages.find]
+where = src
 install_requires = 
 	numpy
 	pandas
 	pyimagej
 	bg-atlasapi
 python_requires = >=3.7
 include_package_data = True
-package_dir = 
-	=src
-
-[options.packages.find]
-where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `abba_python-0.1.0/setup.py` & `abba_python-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='abba_python',
     name='abba_python',
     packages=find_packages(include=['abba_python', 'abba_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nicoKiaru/abba_python',
-    version='0.1.0',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `abba_python-0.1.0/src/abba_python.egg-info/PKG-INFO` & `abba_python-0.1.2/src/abba_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba-python
-Version: 0.1.0
+Version: 0.1.2
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

