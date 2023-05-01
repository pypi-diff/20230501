# Comparing `tmp/silabeador-1.1.8.tar.gz` & `tmp/silabeador-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silabeador-1.1.8.tar", last modified: Tue Jun  7 14:37:49 2022, max compression
+gzip compressed data, was "silabeador-1.1.9.tar", last modified: Tue Jun  7 14:40:33 2022, max compression
```

## Comparing `silabeador-1.1.8.tar` & `silabeador-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-06-07 14:37:49.279044 silabeador-1.1.8/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     7848 2022-06-07 14:37:49.279044 silabeador-1.1.8/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)     6007 2022-06-07 14:37:07.000000 silabeador-1.1.8/README.md
--rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2022-06-07 14:37:49.279044 silabeador-1.1.8/setup.cfg
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1480 2022-06-07 14:37:01.000000 silabeador-1.1.8/setup.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-06-07 14:37:49.279044 silabeador-1.1.8/silabeador/
--rw-r--r--   0 fernando  (1000) fernando  (1000)       26 2021-05-29 07:18:15.000000 silabeador-1.1.8/silabeador/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     8238 2022-06-07 14:36:24.000000 silabeador-1.1.8/silabeador/silabeador.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-06-07 14:37:49.279044 silabeador-1.1.8/silabeador.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     7848 2022-06-07 14:37:49.000000 silabeador-1.1.8/silabeador.egg-info/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)      239 2022-06-07 14:37:49.000000 silabeador-1.1.8/silabeador.egg-info/SOURCES.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2022-06-07 14:37:49.000000 silabeador-1.1.8/silabeador.egg-info/dependency_links.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       57 2022-06-07 14:37:49.000000 silabeador-1.1.8/silabeador.egg-info/entry_points.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       11 2022-06-07 14:37:49.000000 silabeador-1.1.8/silabeador.egg-info/top_level.txt
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-06-07 14:40:33.115584 silabeador-1.1.9/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     7848 2022-06-07 14:40:33.115584 silabeador-1.1.9/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     6007 2022-06-07 14:40:03.000000 silabeador-1.1.9/README.md
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2022-06-07 14:40:33.115584 silabeador-1.1.9/setup.cfg
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     1480 2022-06-07 14:39:59.000000 silabeador-1.1.9/setup.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-06-07 14:40:33.115584 silabeador-1.1.9/silabeador/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       26 2021-05-29 07:18:15.000000 silabeador-1.1.9/silabeador/__init__.py
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     8274 2022-06-07 14:39:46.000000 silabeador-1.1.9/silabeador/silabeador.py
+drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2022-06-07 14:40:33.115584 silabeador-1.1.9/silabeador.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     7848 2022-06-07 14:40:32.000000 silabeador-1.1.9/silabeador.egg-info/PKG-INFO
+-rw-r--r--   0 fernando  (1000) fernando  (1000)      239 2022-06-07 14:40:32.000000 silabeador-1.1.9/silabeador.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2022-06-07 14:40:32.000000 silabeador-1.1.9/silabeador.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       57 2022-06-07 14:40:32.000000 silabeador-1.1.9/silabeador.egg-info/entry_points.txt
+-rw-r--r--   0 fernando  (1000) fernando  (1000)       11 2022-06-07 14:40:32.000000 silabeador-1.1.9/silabeador.egg-info/top_level.txt
```

### Comparing `silabeador-1.1.8/PKG-INFO` & `silabeador-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: silabeador
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python library of methods and functions for syllabic division and prosodic stress detecting for Spanish
 Home-page: https://github.com/fsanzl/silabeador
 Author: Fernando Sanz-Lázaro
 Author-email: fsanzl@gmail.com
 License: LGPL
 Project-URL: Source, https://github.com/fsanzl/silabeador/
 Project-URL: Tracker, https://github.com/fsanzl/silabeador/issues
 Description: [![License: LGPL](https://img.shields.io/github/license/fsanzl/silabeador)](https://opensource.org/licenses/LGPL-2.1)
-        [![Version: 1.1.8](https://img.shields.io/github/v/release/fsanzl/silabeador?include_prereleases)](https://pypi.org/project/silabeador/)
+        [![Version: 1.1.9](https://img.shields.io/github/v/release/fsanzl/silabeador?include_prereleases)](https://pypi.org/project/silabeador/)
         [![Python versions: 3.5, 3.6, 3.7, 3.8, 3.9](https://img.shields.io/pypi/pyversions/silabeador)](https://pypi.org/project/silabeador/)
         
         
         <h2 align="center">Silabeador</h2>
         
         <h3 align="center">A Python library for syllabic division and stress detection for Spanish</h2>
```

### Comparing `silabeador-1.1.8/README.md` & `silabeador-1.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![License: LGPL](https://img.shields.io/github/license/fsanzl/silabeador)](https://opensource.org/licenses/LGPL-2.1)
-[![Version: 1.1.8](https://img.shields.io/github/v/release/fsanzl/silabeador?include_prereleases)](https://pypi.org/project/silabeador/)
+[![Version: 1.1.9](https://img.shields.io/github/v/release/fsanzl/silabeador?include_prereleases)](https://pypi.org/project/silabeador/)
 [![Python versions: 3.5, 3.6, 3.7, 3.8, 3.9](https://img.shields.io/pypi/pyversions/silabeador)](https://pypi.org/project/silabeador/)
 
 
 <h2 align="center">Silabeador</h2>
 
 <h3 align="center">A Python library for syllabic division and stress detection for Spanish</h2>
```

### Comparing `silabeador-1.1.8/setup.py` & `silabeador-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work #
 setup(
     name="silabeador",
-    version="1.1.8",
+    version="1.1.9",
     python_requires='>=3.5',
     description="A Python library of methods and functions for syllabic division and prosodic stress detecting for Spanish",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/fsanzl/silabeador",
     project_urls={
         'Source': 'https://github.com/fsanzl/silabeador/',
```

### Comparing `silabeador-1.1.8/silabeador/silabeador.py` & `silabeador-1.1.9/silabeador/silabeador.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,17 +156,18 @@
                 word += [onset[-1] + letter]
                 onset = ''
             else:
                 word[-1] += onset[:media]
                 word += [onset[media:] + letter]
                 onset = ''
         if onset:
+            print(word, onset)
             if onset.endswith('y') and len(onset) == 1:
                 word[-1] += onset
-            elif len(onset) > 1:
+            elif onset.endswith('y'):
                 word[-1] += onset[:-2]
                 word += [onset[-2:]]
             else:
                 word[-1] += onset
         return word
```

### Comparing `silabeador-1.1.8/silabeador.egg-info/PKG-INFO` & `silabeador-1.1.9/silabeador.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: silabeador
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python library of methods and functions for syllabic division and prosodic stress detecting for Spanish
 Home-page: https://github.com/fsanzl/silabeador
 Author: Fernando Sanz-Lázaro
 Author-email: fsanzl@gmail.com
 License: LGPL
 Project-URL: Source, https://github.com/fsanzl/silabeador/
 Project-URL: Tracker, https://github.com/fsanzl/silabeador/issues
 Description: [![License: LGPL](https://img.shields.io/github/license/fsanzl/silabeador)](https://opensource.org/licenses/LGPL-2.1)
-        [![Version: 1.1.8](https://img.shields.io/github/v/release/fsanzl/silabeador?include_prereleases)](https://pypi.org/project/silabeador/)
+        [![Version: 1.1.9](https://img.shields.io/github/v/release/fsanzl/silabeador?include_prereleases)](https://pypi.org/project/silabeador/)
         [![Python versions: 3.5, 3.6, 3.7, 3.8, 3.9](https://img.shields.io/pypi/pyversions/silabeador)](https://pypi.org/project/silabeador/)
         
         
         <h2 align="center">Silabeador</h2>
         
         <h3 align="center">A Python library for syllabic division and stress detection for Spanish</h2>
```

