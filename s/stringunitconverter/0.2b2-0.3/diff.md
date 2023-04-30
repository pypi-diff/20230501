# Comparing `tmp/stringunitconverter-0.2b2.tar.gz` & `tmp/stringunitconverter-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringunitconverter-0.2b2.tar", last modified: Tue Feb  7 21:53:45 2023, max compression
+gzip compressed data, was "stringunitconverter-0.3.tar", last modified: Sun Apr 30 23:46:12 2023, max compression
```

## Comparing `stringunitconverter-0.2b2.tar` & `stringunitconverter-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-02-07 21:53:45.055225 stringunitconverter-0.2b2/
--rw-rw-r--   0 arend     (1000) arend     (1000)     1112 2023-02-07 21:45:17.000000 stringunitconverter-0.2b2/LICENSE.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)     5444 2023-02-07 21:53:45.055225 stringunitconverter-0.2b2/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)     4589 2023-02-07 21:41:23.000000 stringunitconverter-0.2b2/README.md
--rw-rw-r--   0 arend     (1000) arend     (1000)       86 2022-03-13 18:39:33.000000 stringunitconverter-0.2b2/pyproject.toml
--rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-02-07 21:53:45.055225 stringunitconverter-0.2b2/setup.cfg
--rw-rw-r--   0 arend     (1000) arend     (1000)     1243 2023-02-07 21:50:15.000000 stringunitconverter-0.2b2/setup.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-02-07 21:53:45.055225 stringunitconverter-0.2b2/src/
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-02-07 21:53:45.055225 stringunitconverter-0.2b2/src/stringunitconverter/
--rw-rw-r--   0 arend     (1000) arend     (1000)       76 2022-03-13 20:47:38.000000 stringunitconverter-0.2b2/src/stringunitconverter/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3941 2023-02-07 21:46:45.000000 stringunitconverter-0.2b2/src/stringunitconverter/core.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      273 2022-04-04 23:30:44.000000 stringunitconverter-0.2b2/src/stringunitconverter/prefixes.json
--rw-rw-r--   0 arend     (1000) arend     (1000)      608 2023-02-07 21:40:49.000000 stringunitconverter-0.2b2/src/stringunitconverter/units.json
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-02-07 21:53:45.055225 stringunitconverter-0.2b2/src/stringunitconverter.egg-info/
--rw-rw-r--   0 arend     (1000) arend     (1000)     5444 2023-02-07 21:53:45.000000 stringunitconverter-0.2b2/src/stringunitconverter.egg-info/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)      438 2023-02-07 21:53:45.000000 stringunitconverter-0.2b2/src/stringunitconverter.egg-info/SOURCES.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-02-07 21:53:45.000000 stringunitconverter-0.2b2/src/stringunitconverter.egg-info/dependency_links.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)       25 2023-02-07 21:53:45.000000 stringunitconverter-0.2b2/src/stringunitconverter.egg-info/requires.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)       20 2023-02-07 21:53:45.000000 stringunitconverter-0.2b2/src/stringunitconverter.egg-info/top_level.txt
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-02-07 21:53:45.055225 stringunitconverter-0.2b2/tests/
--rw-rw-r--   0 arend     (1000) arend     (1000)     1718 2022-05-23 20:58:17.000000 stringunitconverter-0.2b2/tests/test_all.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.326774 stringunitconverter-0.3/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1112 2023-02-07 21:57:17.000000 stringunitconverter-0.3/LICENSE.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)     6011 2023-04-30 23:46:12.326774 stringunitconverter-0.3/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5157 2023-04-30 23:33:33.000000 stringunitconverter-0.3/README.md
+-rw-rw-r--   0 arend     (1000) arend     (1000)       86 2022-03-13 18:39:33.000000 stringunitconverter-0.3/pyproject.toml
+-rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-04-30 23:46:12.326774 stringunitconverter-0.3/setup.cfg
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1212 2023-04-30 23:43:42.000000 stringunitconverter-0.3/setup.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.322775 stringunitconverter-0.3/src/
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.322775 stringunitconverter-0.3/src/stringunitconverter/
+-rw-rw-r--   0 arend     (1000) arend     (1000)       76 2022-03-13 20:47:38.000000 stringunitconverter-0.3/src/stringunitconverter/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     3941 2023-02-07 21:46:45.000000 stringunitconverter-0.3/src/stringunitconverter/core.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      273 2022-04-04 23:30:44.000000 stringunitconverter-0.3/src/stringunitconverter/prefixes.json
+-rw-rw-r--   0 arend     (1000) arend     (1000)      608 2023-02-07 21:40:49.000000 stringunitconverter-0.3/src/stringunitconverter/units.json
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.326774 stringunitconverter-0.3/src/stringunitconverter.egg-info/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     6011 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)      438 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/SOURCES.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/dependency_links.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)       20 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/requires.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)       20 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/top_level.txt
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.326774 stringunitconverter-0.3/tests/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1718 2022-05-23 20:58:17.000000 stringunitconverter-0.3/tests/test_all.py
```

### Comparing `stringunitconverter-0.2b2/LICENSE.txt` & `stringunitconverter-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stringunitconverter-0.2b2/PKG-INFO` & `stringunitconverter-0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: stringunitconverter
-Version: 0.2b2
+Version: 0.3
 Summary: Unit converter: Returns multiplier for unit conversion, with units defined as strings.
 Home-page: https://gitlab.com/abaeyens/stringunitconverter
-Author: abaeyens
-Author-email: 2arne.baeyens@gmail.com
+Author: Arne Baeyens
+Author-email: mail@arnebaeyens.com
 Keywords: unit conversion,conversion
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,20 +16,28 @@
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # stringunitconverter
+[![PyPI version](https://badge.fury.io/py/stringunitconverter.svg)](https://badge.fury.io/py/stringunitconverter)
+![coverage](https://gitlab.com/abaeyens/stringunitconverter/badges/master/coverage.svg)
 
 ## Goal
 Get the multiplication factor
 required to convert from one unit to another,
 with the units being given as strings.
+In short:
+make it easy to convert between units.
 
+## Get it
+Install with pip using `pip install stringunitconverter`.
+For more information,
+please see the [PyPI page](https://pypi.org/project/stringunitconverter/).
 
 ## Main concepts
 - Use strings to specify units
   (e.g. 'kN').
 - Allow quasi all mathematical combinations of units
   (e.g. 'N/m^2').
   Math execution order rules should be respected.
@@ -91,14 +99,17 @@
 10.0
 >>> suc.multiplier('1/kPa', '1/(N/m^2)')
 0.001
 ```
 
 
 ## Contribution and development
+The Git remote repository is hosted on
+[GitLab](https://gitlab.com/abaeyens/stringunitconverter).
+
 ### Testing
 Tests are in the directory `tests`
 in the root directory.
 To run the tests, navigate to the root directory
 and run
 `pytest`.
 
@@ -148,12 +159,14 @@
 for example a stable version from PyPi
 and a development version from a local install,
 it may be useful to use
 [Python virtual environments](https://docs.python.org/3/tutorial/venv.html).
 
 
 ## Contact
-Have a question, suggestion, ... ? Send an email to
+Have a question, suggestion, ... ?
+Your feedback on this project is always appreciated!
+Send an email to
 [2arne.baeyens@gmail.com](mailto:2arne.baeyens@gmail.com).
 
 It is also possible to use the [GitLab issues webpage](
   https://gitlab.com/abaeyens/stringunitconverter/-/issues).
```

### Comparing `stringunitconverter-0.2b2/README.md` & `stringunitconverter-0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # stringunitconverter
+[![PyPI version](https://badge.fury.io/py/stringunitconverter.svg)](https://badge.fury.io/py/stringunitconverter)
+![coverage](https://gitlab.com/abaeyens/stringunitconverter/badges/master/coverage.svg)
 
 ## Goal
 Get the multiplication factor
 required to convert from one unit to another,
 with the units being given as strings.
+In short:
+make it easy to convert between units.
 
+## Get it
+Install with pip using `pip install stringunitconverter`.
+For more information,
+please see the [PyPI page](https://pypi.org/project/stringunitconverter/).
 
 ## Main concepts
 - Use strings to specify units
   (e.g. 'kN').
 - Allow quasi all mathematical combinations of units
   (e.g. 'N/m^2').
   Math execution order rules should be respected.
@@ -70,14 +78,17 @@
 10.0
 >>> suc.multiplier('1/kPa', '1/(N/m^2)')
 0.001
 ```
 
 
 ## Contribution and development
+The Git remote repository is hosted on
+[GitLab](https://gitlab.com/abaeyens/stringunitconverter).
+
 ### Testing
 Tests are in the directory `tests`
 in the root directory.
 To run the tests, navigate to the root directory
 and run
 `pytest`.
 
@@ -127,12 +138,14 @@
 for example a stable version from PyPi
 and a development version from a local install,
 it may be useful to use
 [Python virtual environments](https://docs.python.org/3/tutorial/venv.html).
 
 
 ## Contact
-Have a question, suggestion, ... ? Send an email to
+Have a question, suggestion, ... ?
+Your feedback on this project is always appreciated!
+Send an email to
 [2arne.baeyens@gmail.com](mailto:2arne.baeyens@gmail.com).
 
 It is also possible to use the [GitLab issues webpage](
   https://gitlab.com/abaeyens/stringunitconverter/-/issues).
```

### Comparing `stringunitconverter-0.2b2/setup.py` & `stringunitconverter-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stringunitconverter",
-    version="0.2b2",
-    author="abaeyens",
-    author_email="2arne.baeyens@gmail.com",
+    version="0.3",
+    author="Arne Baeyens",
+    author_email="mail@arnebaeyens.com",
     description="Unit converter: Returns multiplier for unit conversion, with units defined as strings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/abaeyens/stringunitconverter",
     keywords='unit conversion, conversion',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     package_data={'': ['*.json']},
-    install_requires=['json',
-                      'importlib_resources',
+    install_requires=['importlib_resources',
                       ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "Intended Audience :: Manufacturing",
         "License :: OSI Approved :: MIT License",
```

### Comparing `stringunitconverter-0.2b2/src/stringunitconverter/core.py` & `stringunitconverter-0.3/src/stringunitconverter/core.py`

 * *Files identical despite different names*

### Comparing `stringunitconverter-0.2b2/src/stringunitconverter/units.json` & `stringunitconverter-0.3/src/stringunitconverter/units.json`

 * *Files identical despite different names*

### Comparing `stringunitconverter-0.2b2/src/stringunitconverter.egg-info/PKG-INFO` & `stringunitconverter-0.3/src/stringunitconverter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: stringunitconverter
-Version: 0.2b2
+Version: 0.3
 Summary: Unit converter: Returns multiplier for unit conversion, with units defined as strings.
 Home-page: https://gitlab.com/abaeyens/stringunitconverter
-Author: abaeyens
-Author-email: 2arne.baeyens@gmail.com
+Author: Arne Baeyens
+Author-email: mail@arnebaeyens.com
 Keywords: unit conversion,conversion
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,20 +16,28 @@
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # stringunitconverter
+[![PyPI version](https://badge.fury.io/py/stringunitconverter.svg)](https://badge.fury.io/py/stringunitconverter)
+![coverage](https://gitlab.com/abaeyens/stringunitconverter/badges/master/coverage.svg)
 
 ## Goal
 Get the multiplication factor
 required to convert from one unit to another,
 with the units being given as strings.
+In short:
+make it easy to convert between units.
 
+## Get it
+Install with pip using `pip install stringunitconverter`.
+For more information,
+please see the [PyPI page](https://pypi.org/project/stringunitconverter/).
 
 ## Main concepts
 - Use strings to specify units
   (e.g. 'kN').
 - Allow quasi all mathematical combinations of units
   (e.g. 'N/m^2').
   Math execution order rules should be respected.
@@ -91,14 +99,17 @@
 10.0
 >>> suc.multiplier('1/kPa', '1/(N/m^2)')
 0.001
 ```
 
 
 ## Contribution and development
+The Git remote repository is hosted on
+[GitLab](https://gitlab.com/abaeyens/stringunitconverter).
+
 ### Testing
 Tests are in the directory `tests`
 in the root directory.
 To run the tests, navigate to the root directory
 and run
 `pytest`.
 
@@ -148,12 +159,14 @@
 for example a stable version from PyPi
 and a development version from a local install,
 it may be useful to use
 [Python virtual environments](https://docs.python.org/3/tutorial/venv.html).
 
 
 ## Contact
-Have a question, suggestion, ... ? Send an email to
+Have a question, suggestion, ... ?
+Your feedback on this project is always appreciated!
+Send an email to
 [2arne.baeyens@gmail.com](mailto:2arne.baeyens@gmail.com).
 
 It is also possible to use the [GitLab issues webpage](
   https://gitlab.com/abaeyens/stringunitconverter/-/issues).
```

### Comparing `stringunitconverter-0.2b2/tests/test_all.py` & `stringunitconverter-0.3/tests/test_all.py`

 * *Files identical despite different names*

