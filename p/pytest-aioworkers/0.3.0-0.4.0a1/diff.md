# Comparing `tmp/pytest-aioworkers-0.3.0.tar.gz` & `tmp/pytest_aioworkers-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-aioworkers-0.3.0.tar", last modified: Wed Dec  4 09:43:16 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytest-aioworkers-0.3.0.tar` & `pytest_aioworkers-0.4.0a1.tar`

### file list

```diff
@@ -1,15 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-04 09:43:16.866282 pytest-aioworkers-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (115)    11358 2019-12-04 09:43:02.000000 pytest-aioworkers-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)       97 2019-12-04 09:43:02.000000 pytest-aioworkers-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)     3382 2019-12-04 09:43:16.866282 pytest-aioworkers-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1793 2019-12-04 09:43:02.000000 pytest-aioworkers-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-04 09:43:16.866282 pytest-aioworkers-0.3.0/pytest_aioworkers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     3382 2019-12-04 09:43:16.000000 pytest-aioworkers-0.3.0/pytest_aioworkers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      318 2019-12-04 09:43:16.000000 pytest-aioworkers-0.3.0/pytest_aioworkers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-12-04 09:43:16.000000 pytest-aioworkers-0.3.0/pytest_aioworkers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       43 2019-12-04 09:43:16.000000 pytest-aioworkers-0.3.0/pytest_aioworkers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)       40 2019-12-04 09:43:16.000000 pytest-aioworkers-0.3.0/pytest_aioworkers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       18 2019-12-04 09:43:16.000000 pytest-aioworkers-0.3.0/pytest_aioworkers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)     1911 2019-12-04 09:43:02.000000 pytest-aioworkers-0.3.0/pytest_aioworkers.py
--rw-r--r--   0 runner    (1001) docker     (115)      352 2019-12-04 09:43:16.866282 pytest-aioworkers-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1519 2019-12-04 09:43:02.000000 pytest-aioworkers-0.3.0/setup.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pytest_aioworkers/__init__.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pytest_aioworkers/plugin.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pytest_aioworkers/utils.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/README.rst
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/PKG-INFO
```

### Comparing `pytest-aioworkers-0.3.0/LICENSE` & `pytest_aioworkers-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-aioworkers-0.3.0/PKG-INFO` & `pytest_aioworkers-0.4.0a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,98 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-aioworkers
-Version: 0.3.0
+Version: 0.4.0a1
 Summary: A plugin to test aioworkers project with pytest
-Home-page: https://github.com/aioworkers/pytest-aioworkers
-Author: Alexander Malev
-Author-email: malev@somedev.ru
-Maintainer: Alexander Malev
-Maintainer-email: malev@somedev.ru
-License: Apache Software License 2.0
-Description: =================
-        pytest-aioworkers
-        =================
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-aioworkers.svg
-            :target: https://pypi.org/project/pytest-aioworkers
-            :alt: PyPI version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/pytest-aioworkers.svg
-            :target: https://pypi.org/project/pytest-aioworkers
-            :alt: Python versions
-        
-        .. image:: https://travis-ci.org/aioworkers/pytest-aioworkers.svg?branch=master
-            :target: https://travis-ci.org/aioworkers/pytest-aioworkers
-            :alt: See Build Status on Travis CI
-        
-        .. image:: https://ci.appveyor.com/api/projects/status/github/aioworkers/pytest-aioworkers?branch=master
-            :target: https://ci.appveyor.com/project/aioworkers/pytest-aioworkers/branch/master
-            :alt: See Build Status on AppVeyor
-        
-        A plugin to test aioworkers projects with pytest
-        
-        
-        
-        Features
-        --------
-        
-        * fixtures
-        
-        
-        Requirements
-        ------------
-        
-        * pytest
-        * aioworkers
-        
-        
-        Installation
-        ------------
-        
-        You can install "pytest-aioworkers" via `pip`_ from `PyPI`_::
-        
-            $ pip install pytest-aioworkers
-        
-        
-        Contributing
-        ------------
-        Contributions are very welcome. Tests can be run with `tox`_, please ensure
-        the coverage at least stays the same before you submit a pull request.
-        
-        License
-        -------
-        
-        Distributed under the terms of the `Apache Software License 2.0`_ license, "pytest-aioworkers" is free and open source software
-        
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please `file an issue`_ along with a detailed description.
-        
-        .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
-        .. _`file an issue`: https://github.com/aioworkers/pytest-aioworkers/issues
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`tox`: https://tox.readthedocs.io/en/latest/
-        .. _`pip`: https://pypi.org/project/pip/
-        .. _`PyPI`: https://pypi.org/project
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Project-URL: GitHub, https://github.com/aioworkers/pytest-aioworkers
+Project-URL: Homepage, https://github.com/aioworkers/pytest-aioworkers
+Author-email: Alexander Malev <malev@somedev.ru>
+License-Expression: Apache-2.0
+License-File: LICENSE
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.5.3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Testing
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Requires-Dist: aioworkers
+Requires-Dist: pytest>=6.1.0
+Provides-Extra: aiohttp
+Requires-Dist: pytest-aiohttp; extra == 'aiohttp'
+Provides-Extra: asyncio
+Requires-Dist: pytest-asyncio; extra == 'asyncio'
+Description-Content-Type: text/x-rst
+
+=================
+pytest-aioworkers
+=================
+
+.. image:: https://github.com/aioworkers/pytest-aioworkers/workflows/Tests/badge.svg
+  :target: https://github.com/aioworkers/pytest-aioworkers/actions?query=workflow%3ATests
+
+.. image:: https://codecov.io/gh/aioworkers/pytest-aioworkers/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/aioworkers/pytest-aioworkers
+
+.. image:: https://img.shields.io/pypi/v/pytest-aioworkers.svg
+  :target: https://pypi.org/project/pytest-aioworkers
+  :alt: PyPI version
+
+.. image:: https://img.shields.io/pypi/pyversions/pytest-aioworkers.svg
+  :target: https://pypi.org/project/pytest-aioworkers
+  :alt: Python versions
+
+.. image:: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
+   :alt: Hatch project
+   :target: https://github.com/pypa/hatch
+
+A plugin to test aioworkers projects with pytest
+
+
+
+Features
+--------
+
+* fixtures
+
+
+Requirements
+------------
+
+* pytest
+* aioworkers
+
+
+Installation
+------------
+
+You can install "pytest-aioworkers" via `pip`_ from `PyPI`_::
+
+    $ pip install pytest-aioworkers
+
+
+Contributing
+------------
+Contributions are very welcome. Tests can be run with `tox`_, please ensure
+the coverage at least stays the same before you submit a pull request.
+
+License
+-------
+
+Distributed under the terms of the `Apache Software License 2.0`_ license, "pytest-aioworkers" is free and open source software
+
+
+Issues
+------
+
+If you encounter any problems, please `file an issue`_ along with a detailed description.
+
+.. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
+.. _`file an issue`: https://github.com/aioworkers/pytest-aioworkers/issues
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`tox`: https://tox.readthedocs.io/en/latest/
+.. _`pip`: https://pypi.org/project/pip/
+.. _`PyPI`: https://pypi.org/project
```

### Comparing `pytest-aioworkers-0.3.0/README.rst` & `pytest_aioworkers-0.4.0a1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 =================
 pytest-aioworkers
 =================
 
+.. image:: https://github.com/aioworkers/pytest-aioworkers/workflows/Tests/badge.svg
+  :target: https://github.com/aioworkers/pytest-aioworkers/actions?query=workflow%3ATests
+
+.. image:: https://codecov.io/gh/aioworkers/pytest-aioworkers/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/aioworkers/pytest-aioworkers
+
 .. image:: https://img.shields.io/pypi/v/pytest-aioworkers.svg
-    :target: https://pypi.org/project/pytest-aioworkers
-    :alt: PyPI version
+  :target: https://pypi.org/project/pytest-aioworkers
+  :alt: PyPI version
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-aioworkers.svg
-    :target: https://pypi.org/project/pytest-aioworkers
-    :alt: Python versions
+  :target: https://pypi.org/project/pytest-aioworkers
+  :alt: Python versions
 
-.. image:: https://travis-ci.org/aioworkers/pytest-aioworkers.svg?branch=master
-    :target: https://travis-ci.org/aioworkers/pytest-aioworkers
-    :alt: See Build Status on Travis CI
-
-.. image:: https://ci.appveyor.com/api/projects/status/github/aioworkers/pytest-aioworkers?branch=master
-    :target: https://ci.appveyor.com/project/aioworkers/pytest-aioworkers/branch/master
-    :alt: See Build Status on AppVeyor
+.. image:: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
+   :alt: Hatch project
+   :target: https://github.com/pypa/hatch
 
 A plugin to test aioworkers projects with pytest
 
 
 
 Features
 --------
```

