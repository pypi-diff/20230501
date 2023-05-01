# Comparing `tmp/pandas_streaming-0.3.218.tar.gz` & `tmp/pandas_streaming-0.3.239.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_streaming-0.3.218.tar", last modified: Tue Oct 26 12:08:51 2021, max compression
+gzip compressed data, was "pandas_streaming-0.3.239.tar", last modified: Mon May  1 07:02:02 2023, max compression
```

## Comparing `pandas_streaming-0.3.218.tar` & `pandas_streaming-0.3.239.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2021-10-26 12:08:51.851583 pandas_streaming-0.3.218/
--rw-rw-rw-   0        0        0     1083 2021-01-01 01:08:49.000000 pandas_streaming-0.3.218/LICENSE.txt
--rw-rw-rw-   0        0        0      104 2020-05-16 12:59:24.000000 pandas_streaming-0.3.218/MANIFEST.in
--rw-rw-rw-   0        0        0     5686 2021-10-26 12:08:51.851583 pandas_streaming-0.3.218/PKG-INFO
--rw-rw-rw-   0        0        0     4196 2021-08-20 23:20:27.000000 pandas_streaming-0.3.218/README.rst
-drwxrwxrwx   0        0        0        0 2021-10-26 12:08:51.773476 pandas_streaming-0.3.218/pandas_streaming/
--rw-rw-rw-   0        0        0     1535 2021-10-26 12:08:05.000000 pandas_streaming-0.3.218/pandas_streaming/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-26 12:08:51.773476 pandas_streaming-0.3.218/pandas_streaming/data/
--rw-rw-rw-   0        0        0       92 2017-09-21 21:46:39.000000 pandas_streaming-0.3.218/pandas_streaming/data/__init__.py
--rw-rw-rw-   0        0        0      885 2021-10-16 10:25:43.000000 pandas_streaming-0.3.218/pandas_streaming/data/dummy.py
-drwxrwxrwx   0        0        0        0 2021-10-26 12:08:51.820341 pandas_streaming-0.3.218/pandas_streaming/df/
--rw-rw-rw-   0        0        0      393 2018-05-17 08:24:44.000000 pandas_streaming-0.3.218/pandas_streaming/df/__init__.py
--rw-rw-rw-   0        0        0    20132 2021-10-16 10:25:43.000000 pandas_streaming-0.3.218/pandas_streaming/df/connex_split.py
--rw-rw-rw-   0        0        0    50018 2021-10-26 00:28:26.000000 pandas_streaming-0.3.218/pandas_streaming/df/dataframe.py
--rw-rw-rw-   0        0        0    18476 2021-07-10 22:49:08.000000 pandas_streaming-0.3.218/pandas_streaming/df/dataframe_helpers.py
--rw-rw-rw-   0        0        0     4426 2021-10-16 10:25:43.000000 pandas_streaming-0.3.218/pandas_streaming/df/dataframe_io.py
--rw-rw-rw-   0        0        0    16036 2021-10-26 11:55:25.000000 pandas_streaming-0.3.218/pandas_streaming/df/dataframe_io_helpers.py
--rw-rw-rw-   0        0        0    11247 2021-07-05 21:17:13.000000 pandas_streaming-0.3.218/pandas_streaming/df/dataframe_split.py
-drwxrwxrwx   0        0        0        0 2021-10-26 12:08:51.835961 pandas_streaming-0.3.218/pandas_streaming/exc/
--rw-rw-rw-   0        0        0      105 2017-09-21 21:24:00.000000 pandas_streaming-0.3.218/pandas_streaming/exc/__init__.py
--rw-rw-rw-   0        0        0      537 2021-10-16 10:25:43.000000 pandas_streaming-0.3.218/pandas_streaming/exc/exc_streaming.py
-drwxrwxrwx   0        0        0        0 2021-10-26 12:08:51.851583 pandas_streaming-0.3.218/pandas_streaming.egg-info/
--rw-rw-rw-   0        0        0     5686 2021-10-26 12:08:51.000000 pandas_streaming-0.3.218/pandas_streaming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2021-10-26 12:08:51.000000 pandas_streaming-0.3.218/pandas_streaming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-26 12:08:51.000000 pandas_streaming-0.3.218/pandas_streaming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2021-10-26 12:08:51.000000 pandas_streaming-0.3.218/pandas_streaming.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2021-10-26 12:08:51.000000 pandas_streaming-0.3.218/pandas_streaming.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-10-26 12:08:51.851583 pandas_streaming-0.3.218/setup.cfg
--rw-rw-rw-   0        0        0     1633 2021-10-26 12:06:31.000000 pandas_streaming-0.3.218/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:02:02.043985 pandas_streaming-0.3.239/
+-rw-rw-rw-   0        0        0     1065 2023-01-01 14:07:59.000000 pandas_streaming-0.3.239/LICENSE.txt
+-rw-rw-rw-   0        0        0      104 2020-05-16 12:59:24.000000 pandas_streaming-0.3.239/MANIFEST.in
+-rw-rw-rw-   0        0        0     4611 2023-05-01 07:02:02.043985 pandas_streaming-0.3.239/PKG-INFO
+-rw-rw-rw-   0        0        0     3917 2023-01-28 18:06:36.000000 pandas_streaming-0.3.239/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 07:02:01.965879 pandas_streaming-0.3.239/pandas_streaming/
+-rw-rw-rw-   0        0        0     1535 2023-05-01 06:55:03.000000 pandas_streaming-0.3.239/pandas_streaming/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:02:01.965879 pandas_streaming-0.3.239/pandas_streaming/data/
+-rw-rw-rw-   0        0        0       92 2017-09-21 21:46:39.000000 pandas_streaming-0.3.239/pandas_streaming/data/__init__.py
+-rw-rw-rw-   0        0        0      867 2022-07-19 23:52:06.000000 pandas_streaming-0.3.239/pandas_streaming/data/dummy.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:02:01.981500 pandas_streaming-0.3.239/pandas_streaming/df/
+-rw-rw-rw-   0        0        0      393 2018-05-17 08:24:44.000000 pandas_streaming-0.3.239/pandas_streaming/df/__init__.py
+-rw-rw-rw-   0        0        0    20484 2022-11-24 23:22:42.000000 pandas_streaming-0.3.239/pandas_streaming/df/connex_split.py
+-rw-rw-rw-   0        0        0    50894 2023-05-01 06:55:38.000000 pandas_streaming-0.3.239/pandas_streaming/df/dataframe.py
+-rw-rw-rw-   0        0        0    18909 2023-05-01 06:36:59.000000 pandas_streaming-0.3.239/pandas_streaming/df/dataframe_helpers.py
+-rw-rw-rw-   0        0        0     4381 2022-07-19 23:52:06.000000 pandas_streaming-0.3.239/pandas_streaming/df/dataframe_io.py
+-rw-rw-rw-   0        0        0    16405 2022-11-26 22:45:01.000000 pandas_streaming-0.3.239/pandas_streaming/df/dataframe_io_helpers.py
+-rw-rw-rw-   0        0        0    10983 2022-11-26 23:31:34.000000 pandas_streaming-0.3.239/pandas_streaming/df/dataframe_split.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:02:01.981500 pandas_streaming-0.3.239/pandas_streaming/exc/
+-rw-rw-rw-   0        0        0      105 2017-09-21 21:24:00.000000 pandas_streaming-0.3.239/pandas_streaming/exc/__init__.py
+-rw-rw-rw-   0        0        0      528 2022-07-19 23:52:06.000000 pandas_streaming-0.3.239/pandas_streaming/exc/exc_streaming.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:02:02.043985 pandas_streaming-0.3.239/pandas_streaming.egg-info/
+-rw-rw-rw-   0        0        0     4611 2023-05-01 07:02:01.000000 pandas_streaming-0.3.239/pandas_streaming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2023-05-01 07:02:01.000000 pandas_streaming-0.3.239/pandas_streaming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:02:01.000000 pandas_streaming-0.3.239/pandas_streaming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-01 07:02:01.000000 pandas_streaming-0.3.239/pandas_streaming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 07:02:01.000000 pandas_streaming-0.3.239/pandas_streaming.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 07:02:02.059606 pandas_streaming-0.3.239/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2022-07-19 23:52:06.000000 pandas_streaming-0.3.239/setup.py
```

### Comparing `pandas_streaming-0.3.218/PKG-INFO` & `pandas_streaming-0.3.239/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,116 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pandas_streaming
-Version: 0.3.218
+Version: 0.3.239
 Summary: Streaming operations with pandas.
 Home-page: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html
+Download-URL: https://github.com/sdpython/pandas_streaming/
 Author: Xavier Dupré
 Author-email: xavier.dupre@gmail.com
 License: MIT
-Download-URL: https://github.com/sdpython/pandas_streaming/
-Description: 
-        .. image:: https://github.com/sdpython/pandas_streaming/blob/master/_doc/sphinxdoc/source/phdoc_static/project_ico.png?raw=true
-            :target: https://github.com/sdpython/pandas_streaming/
-        
-        .. _l-README:
-        
-        pandas_streaming: streaming API over pandas
-        ===========================================
-        
-        .. image:: https://travis-ci.com/sdpython/pandas_streaming.svg?branch=master
-            :target: https://app.travis-ci.com/github/sdpython/pandas_streaming
-            :alt: Build status
-        
-        .. image:: https://ci.appveyor.com/api/projects/status/4te066r8ne1ymmhy?svg=true
-            :target: https://ci.appveyor.com/project/sdpython/pandas-streaming
-            :alt: Build Status Windows
-        
-        .. image:: https://circleci.com/gh/sdpython/pandas_streaming/tree/master.svg?style=svg
-            :target: https://circleci.com/gh/sdpython/pandas_streaming/tree/master
-        
-        .. image:: https://dev.azure.com/xavierdupre3/pandas_streaming/_apis/build/status/sdpython.pandas_streaming
-            :target: https://dev.azure.com/xavierdupre3/pandas_streaming/
-        
-        .. image:: https://badge.fury.io/py/pandas_streaming.svg
-            :target: http://badge.fury.io/py/pandas_streaming
-        
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :alt: MIT License
-            :target: http://opensource.org/licenses/MIT
-        
-        .. image:: https://codecov.io/github/sdpython/pandas_streaming/coverage.svg?branch=master
-            :target: https://codecov.io/github/sdpython/pandas_streaming?branch=master
-        
-        .. image:: http://img.shields.io/github/issues/sdpython/pandas_streaming.png
-            :alt: GitHub Issues
-            :target: https://github.com/sdpython/pandas_streaming/issues
-        
-        .. image:: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/_images/nbcov.png
-            :target: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/all_notebooks_coverage.html
-            :alt: Notebook Coverage
-        
-        .. image:: https://api.codacy.com/project/badge/Grade/f53b7f4d6a0447aa9ce0c4ad5df659ef
-            :target: https://www.codacy.com/app/sdpython/pandas_streaming?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=sdpython/pandas_streaming&amp;utm_campaign=Badge_Grade
-        
-        .. image:: https://pepy.tech/badge/pandas_streaming/month
-            :target: https://pepy.tech/project/pandas_streaming/month
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/github/forks/sdpython/pandas_streaming.svg
-            :target: https://github.com/sdpython/pandas_streaming/
-            :alt: Forks
-        
-        .. image:: https://img.shields.io/github/stars/sdpython/pandas_streaming.svg
-            :target: https://github.com/sdpython/pandas_streaming/
-            :alt: Stars
-        
-        .. image:: https://img.shields.io/github/repo-size/sdpython/pandas_streaming
-            :target: https://github.com/sdpython/pandas_streaming/
-            :alt: size
-        
-        `pandas_streaming <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
-        aims at processing big files with `pandas <http://pandas.pydata.org/>`_,
-        too big to hold in memory, too small to be parallelized with a significant gain.
-        The module replicates a subset of `pandas <http://pandas.pydata.org/>`_ API
-        and implements other functionalities for machine learning.
-        
-        ::
-        
-            from pandas_streaming.df import StreamingDataFrame
-            sdf = StreamingDataFrame.read_csv("filename", sep="\t", encoding="utf-8")
-        
-            for df in sdf:
-                # process this chunk of data
-                # df is a dataframe
-                print(df)
-        
-        The module can also stream an existing dataframe.
-        
-        ::
-        
-            import pandas
-            df = pandas.DataFrame([dict(cf=0, cint=0, cstr="0"),
-                                   dict(cf=1, cint=1, cstr="1"),
-                                   dict(cf=3, cint=3, cstr="3")])
-        
-            from pandas_streaming.df import StreamingDataFrame
-            sdf = StreamingDataFrame.read_df(df)
-        
-            for df in sdf:
-                # process this chunk of data
-                # df is a dataframe
-                print(df)
-        
-        It contains other helpers to split datasets into
-        train and test with some weird constraints.
-        
-        **Links:**
-        
-        * `GitHub/pandas_streaming <https://github.com/sdpython/pandas_streaming/>`_
-        * `documentation <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
-        * `Blog <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/blog/main_0000.html#ap-main-0>`_
-        
-Keywords: pandas_streaming,Xavier Dupré
-Platform: UNKNOWN
+Keywords: pandas_streaming,Xavier Dupré,pandas,streaming
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
+License-File: LICENSE.txt
+
+
+.. image:: https://github.com/sdpython/pandas_streaming/blob/master/_doc/sphinxdoc/source/_static/project_ico.png?raw=true
+    :target: https://github.com/sdpython/pandas_streaming/
+
+.. _l-README:
+
+pandas_streaming: streaming API over pandas
+===========================================
+
+.. image:: https://travis-ci.com/sdpython/pandas_streaming.svg?branch=master
+    :target: https://app.travis-ci.com/github/sdpython/pandas_streaming
+    :alt: Build status
+
+.. image:: https://ci.appveyor.com/api/projects/status/4te066r8ne1ymmhy?svg=true
+    :target: https://ci.appveyor.com/project/sdpython/pandas-streaming
+    :alt: Build Status Windows
+
+.. image:: https://circleci.com/gh/sdpython/pandas_streaming/tree/master.svg?style=svg
+    :target: https://circleci.com/gh/sdpython/pandas_streaming/tree/master
+
+.. image:: https://dev.azure.com/xavierdupre3/pandas_streaming/_apis/build/status/sdpython.pandas_streaming
+    :target: https://dev.azure.com/xavierdupre3/pandas_streaming/
+
+.. image:: https://badge.fury.io/py/pandas_streaming.svg
+    :target: http://badge.fury.io/py/pandas_streaming
+
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :alt: MIT License
+    :target: http://opensource.org/licenses/MIT
+
+.. image:: https://codecov.io/github/sdpython/pandas_streaming/coverage.svg?branch=master
+    :target: https://codecov.io/github/sdpython/pandas_streaming?branch=master
+
+.. image:: http://img.shields.io/github/issues/sdpython/pandas_streaming.png
+    :alt: GitHub Issues
+    :target: https://github.com/sdpython/pandas_streaming/issues
+
+.. image:: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/_images/nbcov.png
+    :target: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/all_notebooks_coverage.html
+    :alt: Notebook Coverage
+
+.. image:: https://pepy.tech/badge/pandas_streaming/month
+    :target: https://pepy.tech/project/pandas_streaming/month
+    :alt: Downloads
+
+.. image:: https://img.shields.io/github/forks/sdpython/pandas_streaming.svg
+    :target: https://github.com/sdpython/pandas_streaming/
+    :alt: Forks
+
+.. image:: https://img.shields.io/github/stars/sdpython/pandas_streaming.svg
+    :target: https://github.com/sdpython/pandas_streaming/
+    :alt: Stars
+
+.. image:: https://img.shields.io/github/repo-size/sdpython/pandas_streaming
+    :target: https://github.com/sdpython/pandas_streaming/
+    :alt: size
+
+`pandas_streaming <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
+aims at processing big files with `pandas <http://pandas.pydata.org/>`_,
+too big to hold in memory, too small to be parallelized with a significant gain.
+The module replicates a subset of `pandas <http://pandas.pydata.org/>`_ API
+and implements other functionalities for machine learning.
+
+::
+
+    from pandas_streaming.df import StreamingDataFrame
+    sdf = StreamingDataFrame.read_csv("filename", sep="\t", encoding="utf-8")
+
+    for df in sdf:
+        # process this chunk of data
+        # df is a dataframe
+        print(df)
+
+The module can also stream an existing dataframe.
+
+::
+
+    import pandas
+    df = pandas.DataFrame([dict(cf=0, cint=0, cstr="0"),
+                           dict(cf=1, cint=1, cstr="1"),
+                           dict(cf=3, cint=3, cstr="3")])
+
+    from pandas_streaming.df import StreamingDataFrame
+    sdf = StreamingDataFrame.read_df(df)
+
+    for df in sdf:
+        # process this chunk of data
+        # df is a dataframe
+        print(df)
+
+It contains other helpers to split datasets into
+train and test with some weird constraints.
+
+**Links:**
+
+* `GitHub/pandas_streaming <https://github.com/sdpython/pandas_streaming/>`_
+* `documentation <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
+* `Blog <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/blog/main_0000.html#ap-main-0>`_
```

### Comparing `pandas_streaming-0.3.218/README.rst` & `pandas_streaming-0.3.239/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-.. image:: https://github.com/sdpython/pandas_streaming/blob/master/_doc/sphinxdoc/source/phdoc_static/project_ico.png?raw=true
+.. image:: https://github.com/sdpython/pandas_streaming/blob/master/_doc/sphinxdoc/source/_static/project_ico.png?raw=true
     :target: https://github.com/sdpython/pandas_streaming/
 
 .. _l-README:
 
 pandas_streaming: streaming API over pandas
 ===========================================
 
@@ -35,17 +35,14 @@
     :alt: GitHub Issues
     :target: https://github.com/sdpython/pandas_streaming/issues
 
 .. image:: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/_images/nbcov.png
     :target: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/all_notebooks_coverage.html
     :alt: Notebook Coverage
 
-.. image:: https://api.codacy.com/project/badge/Grade/f53b7f4d6a0447aa9ce0c4ad5df659ef
-    :target: https://www.codacy.com/app/sdpython/pandas_streaming?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=sdpython/pandas_streaming&amp;utm_campaign=Badge_Grade
-
 .. image:: https://pepy.tech/badge/pandas_streaming/month
     :target: https://pepy.tech/project/pandas_streaming/month
     :alt: Downloads
 
 .. image:: https://img.shields.io/github/forks/sdpython/pandas_streaming.svg
     :target: https://github.com/sdpython/pandas_streaming/
     :alt: Forks
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/__init__.py` & `pandas_streaming-0.3.239/pandas_streaming/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @file
 @brief Module *pandas_streaming*.
 Processes large datasets with :epkg:`pandas` by
 reimplementing streeaming versions of
 :epkg:`pandas` functionalites.
 """
 
-__version__ = "0.3.218"
+__version__ = "0.3.239"
 __author__ = "Xavier Dupré"
 __github__ = "https://github.com/sdpython/pandas_streaming"
 __url__ = "http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html"
 __license__ = "MIT License"
 __blog__ = """
 <?xml version="1.0" encoding="UTF-8"?>
 <opml version="1.0">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- """ @file @brief Module *pandas_streaming*. Processes
 large datasets with :epkg:`pandas` by reimplementing streeaming versions of :
-epkg:`pandas` functionalites. """ __version__ = "0.3.218" __author__ = "Xavier
+epkg:`pandas` functionalites. """ __version__ = "0.3.239" __author__ = "Xavier
 DuprÃ©" __github__ = "https://github.com/sdpython/pandas_streaming" __url__ =
 "http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html"
 __license__ = "MIT License" __blog__ = """ <?xml version="1.0" encoding="UTF-
 8"?>
  """ def check(log=False): """ Checks the library is working. It raises an
 exception. If you want to disable the logs: :param log: if True, display
 information, otherwise none :return: 0 or exception """ return True def
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/data/dummy.py` & `pandas_streaming-0.3.239/pandas_streaming/data/dummy.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,14 @@
     :param chunksize: chunk size
     :param asfloat: use random float and not random int
     :param cols: additional columns
     :return: a @see cl StreamingDataFrame
     """
     if asfloat:
         df = DataFrame(dict(cfloat=[_ + 0.1 for _ in range(0, n)], cstr=[
-                       "s{0}".format(i) for i in range(0, n)]))
+                       f"s{i}" for i in range(0, n)]))
     else:
         df = DataFrame(dict(cint=list(range(0, n)), cstr=[
-                       "s{0}".format(i) for i in range(0, n)]))
+                       f"s{i}" for i in range(0, n)]))
     for k, v in cols.items():
         df[k] = v
     return StreamingDataFrame.read_df(df, chunksize=chunksize)
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/df/connex_split.py` & `pandas_streaming-0.3.239/pandas_streaming/df/connex_split.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,505 +1,501 @@
-# -*- coding: utf-8 -*-
-"""
-@file
-@brief Implements a connex split between train and test.
-"""
-from collections import Counter
-import pandas
-import numpy
-from sklearn.model_selection import train_test_split
-from .dataframe_helpers import dataframe_shuffle
-
-
-class ImbalancedSplitException(Exception):
-    """
-    Raised when an imbalanced split is detected.
-    """
-    pass
-
-
-def train_test_split_weights(df, weights=None, test_size=0.25, train_size=None,
-                             shuffle=True, fail_imbalanced=0.05, random_state=None):
-    """
-    Splits a database in train/test given, every row
-    can have a different weight.
-
-    @param  df              :epkg:`pandas:DataFrame` or @see cl StreamingDataFrame
-    @param  weights         None or weights or weights column name
-    @param  test_size       ratio for the test partition (if *train_size* is not specified)
-    @param  train_size      ratio for the train partition
-    @param  shuffle         shuffles before the split
-    @param  fail_imbalanced raises an exception if relative weights difference is higher than this value
-    @param  random_state    seed for random generators
-    @return                 train and test :epkg:`pandas:DataFrame`
-
-    If the dataframe is not shuffled first, the function
-    will produce two datasets which are unlikely to be randomized
-    as the function tries to keep equal weights among both paths
-    without using randomness.
-    """
-    if hasattr(df, 'iter_creation'):
-        raise NotImplementedError(  # pragma: no cover
-            'Not implemented yet for StreamingDataFrame.')
-    if isinstance(df, numpy.ndarray):
-        raise NotImplementedError(  # pragma: no cover
-            "Not implemented on numpy arrays.")
-    if shuffle:
-        df = dataframe_shuffle(df, random_state=random_state)
-    if weights is None:
-        if test_size == 0 or train_size == 0:
-            raise ValueError(
-                "test_size={0} or train_size={1} cannot be null (1)."
-                "".format(test_size, train_size))
-        return train_test_split(df, test_size=test_size,
-                                train_size=train_size,
-                                random_state=random_state)
-
-    if isinstance(weights, pandas.Series):
-        weights = list(weights)
-    elif isinstance(weights, str):
-        weights = list(df[weights])
-    if len(weights) != df.shape[0]:
-        raise ValueError(
-            "Dimension mismatch between weights and dataframe "
-            "{0} != {1}".format(df.shape[0], len(weights)))
-
-    p = (1 - test_size) if test_size else None
-    if train_size is not None:
-        p = train_size
-        test_size = 1 - p
-    if p is None or min(test_size, p) <= 0:
-        raise ValueError(
-            "test_size={0} or train_size={1} cannot be null (2)."
-            "".format(test_size, train_size))
-    ratio = test_size / p
-
-    if random_state is None:
-        randint = numpy.random.randint
-    else:
-        state = numpy.random.RandomState(random_state)
-        randint = state.randint
-
-    balance = 0
-    train_ids = []
-    test_ids = []
-    test_weights = 0
-    train_weights = 0
-    for i in range(0, df.shape[0]):
-        w = weights[i]
-        if balance == 0:
-            h = randint(0, 1)
-            totest = h == 0
-        else:
-            totest = balance < 0
-        if totest:
-            test_ids.append(i)
-            balance += w
-            test_weights += w
-        else:
-            train_ids.append(i)
-            balance -= w * ratio
-            train_weights += w * ratio
-
-    r = abs(train_weights - test_weights) / \
-        (1.0 * (train_weights + test_weights))
-    if r >= fail_imbalanced:
-        raise ImbalancedSplitException(  # pragma: no cover
-            "Split is imbalanced: train_weights={0} test_weights={1} r={2}."
-            "".format(train_weights, test_weights, r))
-
-    return df.iloc[train_ids, :], df.iloc[test_ids, :]
-
-
-def train_test_connex_split(df, groups, test_size=0.25, train_size=None,
-                            stratify=None, hash_size=9, unique_rows=False,
-                            shuffle=True, fail_imbalanced=0.05, keep_balance=None,
-                            stop_if_bigger=None, return_cnx=False,
-                            must_groups=None, random_state=None, fLOG=None):
-    """
-    This split is for a specific case where data is linked
-    in many ways. Let's assume we have three ids as we have
-    for online sales: *(product id, user id, card id)*.
-    As we may need to compute aggregated features,
-    we need every id not to be present in both train and
-    test set. The function computes the connected components
-    and breaks each of them in two parts for train and test.
-
-    @param  df              :epkg:`pandas:DataFrame`
-    @param  groups          columns name for the ids
-    @param  test_size       ratio for the test partition (if *train_size* is not specified)
-    @param  train_size      ratio for the train partition
-    @param  stratify        column holding the stratification
-    @param  hash_size       size of the hash to cache information about partition
-    @param  unique_rows     ensures that rows are unique
-    @param  shuffle         shuffles before the split
-    @param  fail_imbalanced raises an exception if relative weights difference
-                            is higher than this value
-    @param  stop_if_bigger  (float) stops a connected components from being
-                            bigger than this ratio of elements, this should not be used
-                            unless a big components emerges, the algorithm stops merging
-                            but does not guarantee it returns the best cut,
-                            the value should be close to 0
-    @param  keep_balance    (float), if not None, does not merge connected components
-                            if their relative sizes are too different, the value should be
-                            close to 1
-    @param  return_cnx      returns connected components as a third results
-    @param  must_groups     column name for ids which must not be shared by
-                            train/test partitions
-    @param  random_state    seed for random generator
-    @param  fLOG            logging function
-    @return                 Two @see cl StreamingDataFrame, one
-                            for train, one for test.
-
-    The list of ids must hold in memory.
-    There is no streaming implementation for the ids.
-
-    .. exref::
-        :title: Splits a dataframe, keep ids in separate partitions
-        :tag: dataframe
-
-        In some data science problems, rows are not independant
-        and share common value, most of the time ids. In some
-        specific case, multiple ids from different columns are
-        connected and must appear in the same partition.
-        Testing that each id column is evenly split and do not
-        appear in both sets in not enough. Connected components
-        are needed.
-
-        .. runpython::
-            :showcode:
-
-            from pandas import DataFrame
-            from pandas_streaming.df import train_test_connex_split
-
-            df = DataFrame([dict(user="UA", prod="PAA", card="C1"),
-                            dict(user="UA", prod="PB", card="C1"),
-                            dict(user="UB", prod="PC", card="C2"),
-                            dict(user="UB", prod="PD", card="C2"),
-                            dict(user="UC", prod="PAA", card="C3"),
-                            dict(user="UC", prod="PF", card="C4"),
-                            dict(user="UD", prod="PG", card="C5"),
-                            ])
-
-            train, test = train_test_connex_split(
-                df, test_size=0.5, groups=['user', 'prod', 'card'],
-                fail_imbalanced=0.6)
-
-            print(train)
-            print(test)
-
-    If *return_cnx* is True, the third results contains:
-
-    * connected components for each id
-    * the dataframe with connected components as a new column
-
-    .. runpython::
-        :showcode:
-
-        from pandas import DataFrame
-        from pandas_streaming.df import train_test_connex_split
-
-        df = DataFrame([dict(user="UA", prod="PAA", card="C1"),
-                        dict(user="UA", prod="PB", card="C1"),
-                        dict(user="UB", prod="PC", card="C2"),
-                        dict(user="UB", prod="PD", card="C2"),
-                        dict(user="UC", prod="PAA", card="C3"),
-                        dict(user="UC", prod="PF", card="C4"),
-                        dict(user="UD", prod="PG", card="C5"),
-                        ])
-
-        train, test, cnx = train_test_connex_split(
-            df, test_size=0.5, groups=['user', 'prod', 'card'],
-            fail_imbalanced=0.6, return_cnx=True)
-
-        print(cnx[0])
-        print(cnx[1])
-    """
-    if stratify is not None:
-        raise NotImplementedError(  # pragma: no cover
-            "Option stratify is not implemented.")
-    if groups is None or len(groups) == 0:
-        raise ValueError(  # pragma: no cover
-            "groups is empty. Use regular train_test_split.")
-    if hasattr(df, 'iter_creation'):
-        raise NotImplementedError(  # pragma: no cover
-            'Not implemented yet for StreamingDataFrame.')
-    if isinstance(df, numpy.ndarray):
-        raise NotImplementedError(  # pragma: no cover
-            "Not implemented on numpy arrays.")
-    if shuffle:
-        df = dataframe_shuffle(df, random_state=random_state)
-
-    dfids = df[groups].copy()
-    if must_groups is not None:
-        dfids_must = df[must_groups].copy()
-
-    name = "connex"
-    while name in dfids.columns:
-        name += "_"
-    one = "weight"
-    while one in dfids.columns:
-        one += "_"
-
-    # Connected components.
-    elements = list(range(dfids.shape[0]))
-    counts_cnx = {i: {i} for i in elements}
-    connex = {}
-    avoids_merge = {}
-
-    def do_connex_components(dfrows, local_groups, kb, sib):
-        "run connected components algorithms"
-        itern = 0
-        modif = 1
-
-        while modif > 0 and itern < len(elements):
-            if fLOG and df.shape[0] > 10000:
-                fLOG("[train_test_connex_split] iteration={0}-#nb connect={1} - "
-                     "modif={2}".format(iter, len(set(elements)), modif))
-            modif = 0
-            itern += 1
-            for i, row in enumerate(dfrows.itertuples(index=False, name=None)):
-                vals = [val for val in zip(local_groups, row) if not isinstance(
-                    val[1], float) or not numpy.isnan(val[1])]
-
-                c = elements[i]
-
-                for val in vals:
-                    if val not in connex:
-                        connex[val] = c
-                        modif += 1
-
-                set_c = set(connex[val] for val in vals)
-                set_c.add(c)
-                new_c = min(set_c)
-
-                add_pair_c = []
-                for c in set_c:
-                    if c == new_c or (new_c, c) in avoids_merge:
-                        continue
-                    if kb is not None:
-                        maxi = min(len(counts_cnx[new_c]), len(counts_cnx[c]))
-                        if maxi > 5:
-                            diff = len(counts_cnx[new_c]) + \
-                                len(counts_cnx[c]) - maxi
-                            r = diff / float(maxi)
-                            if r > kb:
-                                if fLOG:  # pragma: no cover
-                                    fLOG('[train_test_connex_split]    balance '
-                                         'r={0:0.00000}>{1:0.00}, #[{2}]={3}, '
-                                         '#[{4}]={5}'.format(r, kb, new_c,
-                                                             len(counts_cnx[new_c]),
-                                                             c, len(counts_cnx[c])))
-                                continue
-
-                    if sib is not None:
-                        r = (len(counts_cnx[new_c]) +
-                             len(counts_cnx[c])) / float(len(elements))
-                        if r > sib:
-                            if fLOG:  # pragma: no cover
-                                fLOG('[train_test_connex_split]    no merge '
-                                     'r={0:0.00000}>{1:0.00}, #[{2}]={3}, #[{4}]={5}'
-                                     ''.format(r, sib, new_c, len(counts_cnx[new_c]),
-                                               c, len(counts_cnx[c])))
-                            avoids_merge[new_c, c] = i
-                            continue
-
-                    add_pair_c.append(c)
-
-                if len(add_pair_c) > 0:
-                    for c in add_pair_c:
-                        modif += len(counts_cnx[c])
-                        for ii in counts_cnx[c]:
-                            elements[ii] = new_c
-                        counts_cnx[new_c] = counts_cnx[new_c].union(
-                            counts_cnx[c])
-                        counts_cnx[c] = set()
-
-                        keys = list(vals)
-                        for val in keys:
-                            if connex[val] == c:
-                                connex[val] = new_c
-                                modif += 1
-
-    if must_groups:
-        do_connex_components(dfids_must, must_groups, None, None)
-    do_connex_components(dfids, groups, keep_balance, stop_if_bigger)
-
-    # final
-    dfids[name] = elements
-    dfids[one] = 1
-    grsum = dfids[[name, one]].groupby(name, as_index=False).sum()
-    if fLOG:
-        for g in groups:
-            fLOG("[train_test_connex_split]     #nb in '{0}': {1}".format(
-                g, len(set(dfids[g]))))
-        fLOG(
-            "[train_test_connex_split] #connex {0}/{1}".format(
-                grsum.shape[0], dfids.shape[0]))
-    if grsum.shape[0] <= 1:
-        raise ValueError(  # pragma: no cover
-            "Every element is in the same connected components.")
-
-    # Statistics: top connected components
-    if fLOG:
-        # Global statistics
-        counts = Counter(elements)
-        cl = [(v, k) for k, v in counts.items()]
-        cum = 0
-        maxc = None
-        fLOG("[train_test_connex_split] number of connected components: {0}"
-             "".format(len(set(elements))))
-        for i, (v, k) in enumerate(sorted(cl, reverse=True)):
-            if i == 0:
-                maxc = k, v
-            if i >= 10:
-                break
-            cum += v
-            fLOG("[train_test_connex_split]     c={0} #elements={1} cumulated"
-                 "={2}/{3}".format(k, v, cum, len(elements)))
-
-        # Most important component
-        fLOG('[train_test_connex_split] first row of the biggest component '
-             '{0}'.format(maxc))
-        tdf = dfids[dfids[name] == maxc[0]]
-        fLOG('[train_test_connex_split] \n{0}'.format(tdf.head(n=10)))
-
-    # Splits.
-    train, test = train_test_split_weights(
-        grsum, weights=one, test_size=test_size, train_size=train_size,
-        shuffle=shuffle, fail_imbalanced=fail_imbalanced,
-        random_state=random_state)
-    train.drop(one, inplace=True, axis=1)
-    test.drop(one, inplace=True, axis=1)
-
-    # We compute the final dataframe.
-    def double_merge(d):
-        "merge twice"
-        merge1 = dfids.merge(d, left_on=name, right_on=name)
-        merge2 = df.merge(merge1, left_on=groups, right_on=groups)
-        return merge2
-
-    train_f = double_merge(train)
-    test_f = double_merge(test)
-    if return_cnx:
-        return train_f, test_f, (connex, dfids)
-    else:
-        return train_f, test_f
-
-
-def train_test_apart_stratify(df, group, test_size=0.25, train_size=None,
-                              stratify=None, force=False, random_state=None,
-                              fLOG=None):
-    """
-    This split is for a specific case where data is linked
-    in one way. Let's assume we have two ids as we have
-    for online sales: *(product id, category id)*.
-    A product can have multiple categories. We need to have
-    distinct products on train and test but common categories
-    on both sides.
-
-    @param  df              :epkg:`pandas:DataFrame`
-    @param  group           columns name for the ids
-    @param  test_size       ratio for the test partition
-                            (if *train_size* is not specified)
-    @param  train_size      ratio for the train partition
-    @param  stratify        column holding the stratification
-    @param  force           if True, tries to get at least one example on the test side
-                            for each value of the column *stratify*
-    @param  random_state    seed for random generators
-    @param  fLOG            logging function
-    @return                 Two @see cl StreamingDataFrame, one
-                            for train, one for test.
-
-    .. index:: multi-label
-
-    The list of ids must hold in memory.
-    There is no streaming implementation for the ids.
-    This split was implemented for a case of a multi-label
-    classification. A category (*stratify*) is not exclusive
-    and an observation can be assigned to multiple
-    categories. In that particular case, the method
-    `train_test_split <http://scikit-learn.org/stable/modules/generated/
-    sklearn.model_selection.train_test_split.html>`_
-    can not directly be used.
-
-    .. runpython::
-        :showcode:
-
-        import pandas
-        from pandas_streaming.df import train_test_apart_stratify
-
-        df = pandas.DataFrame([dict(a=1, b="e"),
-                               dict(a=1, b="f"),
-                               dict(a=2, b="e"),
-                               dict(a=2, b="f")])
-
-        train, test = train_test_apart_stratify(
-            df, group="a", stratify="b", test_size=0.5)
-        print(train)
-        print('-----------')
-        print(test)
-    """
-    if stratify is None:
-        raise ValueError(  # pragma: no cover
-            "stratify must be specified.")
-    if group is None:
-        raise ValueError(  # pragma: no cover
-            "group must be specified.")
-    if hasattr(df, 'iter_creation'):
-        raise NotImplementedError(
-            'Not implemented yet for StreamingDataFrame.')
-    if isinstance(df, numpy.ndarray):
-        raise NotImplementedError("Not implemented on numpy arrays.")
-
-    p = (1 - test_size) if test_size else None
-    if train_size is not None:
-        p = train_size
-    test_size = 1 - p
-    if p is None or min(test_size, p) <= 0:
-        raise ValueError(  # pragma: no cover
-            "test_size={0} or train_size={1} cannot be null".format(
-                test_size, train_size))
-
-    couples = df[[group, stratify]].itertuples(name=None, index=False)
-    hist = Counter(df[stratify])
-    sorted_hist = [(v, k) for k, v in hist.items()]
-    sorted_hist.sort()
-    ids = {c: set() for c in hist}
-
-    for g, s in couples:
-        ids[s].add(g)
-
-    if random_state is None:
-        permutation = numpy.random.permutation
-    else:
-        state = numpy.random.RandomState(random_state)
-        permutation = state.permutation
-
-    split = {}
-    for _, k in sorted_hist:
-        not_assigned = [c for c in ids[k] if c not in split]
-        if len(not_assigned) == 0:
-            continue
-        assigned = [c for c in ids[k] if c in split]
-        nb_test = sum(split[c] for c in assigned)
-        expected = min(len(ids[k]), int(
-            test_size * len(ids[k]) + 0.5)) - nb_test
-        if force and expected == 0 and nb_test == 0:
-            nb_train = len(assigned) - nb_test
-            if nb_train > 0 or len(not_assigned) > 1:
-                expected = min(1, len(not_assigned))
-        if expected > 0:
-            permutation(not_assigned)
-            for e in not_assigned[:expected]:
-                split[e] = 1
-            for e in not_assigned[expected:]:
-                split[e] = 0
-        else:
-            for c in not_assigned:
-                split[c] = 0
-
-    train_set = set(k for k, v in split.items() if v == 0)
-    test_set = set(k for k, v in split.items() if v == 1)
-    train_df = df[df[group].isin(train_set)]
-    test_df = df[df[group].isin(test_set)]
-    return train_df, test_df
+# -*- coding: utf-8 -*-
+"""
+@file
+@brief Implements a connex split between train and test.
+"""
+from collections import Counter
+import pandas
+import numpy
+from sklearn.model_selection import train_test_split
+from .dataframe_helpers import dataframe_shuffle
+
+
+class ImbalancedSplitException(Exception):
+    """
+    Raised when an imbalanced split is detected.
+    """
+    pass
+
+
+def train_test_split_weights(df, weights=None, test_size=0.25, train_size=None,
+                             shuffle=True, fail_imbalanced=0.05, random_state=None):
+    """
+    Splits a database in train/test given, every row
+    can have a different weight.
+
+    @param  df              :epkg:`pandas:DataFrame` or @see cl StreamingDataFrame
+    @param  weights         None or weights or weights column name
+    @param  test_size       ratio for the test partition (if *train_size* is not specified)
+    @param  train_size      ratio for the train partition
+    @param  shuffle         shuffles before the split
+    @param  fail_imbalanced raises an exception if relative weights difference is higher than this value
+    @param  random_state    seed for random generators
+    @return                 train and test :epkg:`pandas:DataFrame`
+
+    If the dataframe is not shuffled first, the function
+    will produce two datasets which are unlikely to be randomized
+    as the function tries to keep equal weights among both paths
+    without using randomness.
+    """
+    if hasattr(df, 'iter_creation'):
+        raise NotImplementedError(  # pragma: no cover
+            'Not implemented yet for StreamingDataFrame.')
+    if isinstance(df, numpy.ndarray):
+        raise NotImplementedError(  # pragma: no cover
+            "Not implemented on numpy arrays.")
+    if shuffle:
+        df = dataframe_shuffle(df, random_state=random_state)
+    if weights is None:
+        if test_size == 0 or train_size == 0:
+            raise ValueError(
+                f"test_size={test_size} or train_size={train_size} cannot be null (1).")
+        return train_test_split(df, test_size=test_size,
+                                train_size=train_size,
+                                random_state=random_state)
+
+    if isinstance(weights, pandas.Series):
+        weights = list(weights)
+    elif isinstance(weights, str):
+        weights = list(df[weights])
+    if len(weights) != df.shape[0]:
+        raise ValueError(
+            "Dimension mismatch between weights and dataframe "
+            "{0} != {1}".format(df.shape[0], len(weights)))
+
+    p = (1 - test_size) if test_size else None
+    if train_size is not None:
+        p = train_size
+        test_size = 1 - p
+    if p is None or min(test_size, p) <= 0:
+        raise ValueError(
+            f"test_size={test_size} or train_size={train_size} cannot be null (2).")
+    ratio = test_size / p
+
+    if random_state is None:
+        randint = numpy.random.randint
+    else:
+        state = numpy.random.RandomState(random_state)
+        randint = state.randint
+
+    balance = 0
+    train_ids = []
+    test_ids = []
+    test_weights = 0
+    train_weights = 0
+    for i in range(0, df.shape[0]):
+        w = weights[i]
+        if balance == 0:
+            h = randint(0, 1)
+            totest = h == 0
+        else:
+            totest = balance < 0
+        if totest:
+            test_ids.append(i)
+            balance += w
+            test_weights += w
+        else:
+            train_ids.append(i)
+            balance -= w * ratio
+            train_weights += w * ratio
+
+    r = abs(train_weights - test_weights) / \
+        (1.0 * (train_weights + test_weights))
+    if r >= fail_imbalanced:
+        raise ImbalancedSplitException(  # pragma: no cover
+            "Split is imbalanced: train_weights={0} test_weights={1} r={2}."
+            "".format(train_weights, test_weights, r))
+
+    return df.iloc[train_ids, :], df.iloc[test_ids, :]
+
+
+def train_test_connex_split(df, groups, test_size=0.25, train_size=None,
+                            stratify=None, hash_size=9, unique_rows=False,
+                            shuffle=True, fail_imbalanced=0.05, keep_balance=None,
+                            stop_if_bigger=None, return_cnx=False,
+                            must_groups=None, random_state=None, fLOG=None):
+    """
+    This split is for a specific case where data is linked
+    in many ways. Let's assume we have three ids as we have
+    for online sales: *(product id, user id, card id)*.
+    As we may need to compute aggregated features,
+    we need every id not to be present in both train and
+    test set. The function computes the connected components
+    and breaks each of them in two parts for train and test.
+
+    @param  df              :epkg:`pandas:DataFrame`
+    @param  groups          columns name for the ids
+    @param  test_size       ratio for the test partition (if *train_size* is not specified)
+    @param  train_size      ratio for the train partition
+    @param  stratify        column holding the stratification
+    @param  hash_size       size of the hash to cache information about partition
+    @param  unique_rows     ensures that rows are unique
+    @param  shuffle         shuffles before the split
+    @param  fail_imbalanced raises an exception if relative weights difference
+                            is higher than this value
+    @param  stop_if_bigger  (float) stops a connected components from being
+                            bigger than this ratio of elements, this should not be used
+                            unless a big components emerges, the algorithm stops merging
+                            but does not guarantee it returns the best cut,
+                            the value should be close to 0
+    @param  keep_balance    (float), if not None, does not merge connected components
+                            if their relative sizes are too different, the value should be
+                            close to 1
+    @param  return_cnx      returns connected components as a third results
+    @param  must_groups     column name for ids which must not be shared by
+                            train/test partitions
+    @param  random_state    seed for random generator
+    @param  fLOG            logging function
+    @return                 Two @see cl StreamingDataFrame, one
+                            for train, one for test.
+
+    The list of ids must hold in memory.
+    There is no streaming implementation for the ids.
+
+    .. exref::
+        :title: Splits a dataframe, keep ids in separate partitions
+        :tag: dataframe
+
+        In some data science problems, rows are not independant
+        and share common value, most of the time ids. In some
+        specific case, multiple ids from different columns are
+        connected and must appear in the same partition.
+        Testing that each id column is evenly split and do not
+        appear in both sets in not enough. Connected components
+        are needed.
+
+        .. runpython::
+            :showcode:
+
+            from pandas import DataFrame
+            from pandas_streaming.df import train_test_connex_split
+
+            df = DataFrame([dict(user="UA", prod="PAA", card="C1"),
+                            dict(user="UA", prod="PB", card="C1"),
+                            dict(user="UB", prod="PC", card="C2"),
+                            dict(user="UB", prod="PD", card="C2"),
+                            dict(user="UC", prod="PAA", card="C3"),
+                            dict(user="UC", prod="PF", card="C4"),
+                            dict(user="UD", prod="PG", card="C5"),
+                            ])
+
+            train, test = train_test_connex_split(
+                df, test_size=0.5, groups=['user', 'prod', 'card'],
+                fail_imbalanced=0.6)
+
+            print(train)
+            print(test)
+
+    If *return_cnx* is True, the third results contains:
+
+    * connected components for each id
+    * the dataframe with connected components as a new column
+
+    .. runpython::
+        :showcode:
+
+        from pandas import DataFrame
+        from pandas_streaming.df import train_test_connex_split
+
+        df = DataFrame([dict(user="UA", prod="PAA", card="C1"),
+                        dict(user="UA", prod="PB", card="C1"),
+                        dict(user="UB", prod="PC", card="C2"),
+                        dict(user="UB", prod="PD", card="C2"),
+                        dict(user="UC", prod="PAA", card="C3"),
+                        dict(user="UC", prod="PF", card="C4"),
+                        dict(user="UD", prod="PG", card="C5"),
+                        ])
+
+        train, test, cnx = train_test_connex_split(
+            df, test_size=0.5, groups=['user', 'prod', 'card'],
+            fail_imbalanced=0.6, return_cnx=True)
+
+        print(cnx[0])
+        print(cnx[1])
+    """
+    if stratify is not None:
+        raise NotImplementedError(  # pragma: no cover
+            "Option stratify is not implemented.")
+    if groups is None or len(groups) == 0:
+        raise ValueError(  # pragma: no cover
+            "groups is empty. Use regular train_test_split.")
+    if hasattr(df, 'iter_creation'):
+        raise NotImplementedError(  # pragma: no cover
+            'Not implemented yet for StreamingDataFrame.')
+    if isinstance(df, numpy.ndarray):
+        raise NotImplementedError(  # pragma: no cover
+            "Not implemented on numpy arrays.")
+    if shuffle:
+        df = dataframe_shuffle(df, random_state=random_state)
+
+    dfids = df[groups].copy()
+    if must_groups is not None:
+        dfids_must = df[must_groups].copy()
+
+    name = "connex"
+    while name in dfids.columns:
+        name += "_"
+    one = "weight"
+    while one in dfids.columns:
+        one += "_"
+
+    # Connected components.
+    elements = list(range(dfids.shape[0]))
+    counts_cnx = {i: {i} for i in elements}
+    connex = {}
+    avoids_merge = {}
+
+    def do_connex_components(dfrows, local_groups, kb, sib):
+        "run connected components algorithms"
+        itern = 0
+        modif = 1
+
+        while modif > 0 and itern < len(elements):
+            if fLOG and df.shape[0] > 10000:
+                fLOG("[train_test_connex_split] iteration={0}-#nb connect={1} - "
+                     "modif={2}".format(iter, len(set(elements)), modif))
+            modif = 0
+            itern += 1
+            for i, row in enumerate(dfrows.itertuples(index=False, name=None)):
+                vals = [val for val in zip(local_groups, row) if not isinstance(
+                    val[1], float) or not numpy.isnan(val[1])]
+
+                c = elements[i]
+
+                for val in vals:
+                    if val not in connex:
+                        connex[val] = c
+                        modif += 1
+
+                set_c = set(connex[val] for val in vals)
+                set_c.add(c)
+                new_c = min(set_c)
+
+                add_pair_c = []
+                for c in set_c:
+                    if c == new_c or (new_c, c) in avoids_merge:
+                        continue
+                    if kb is not None:
+                        maxi = min(len(counts_cnx[new_c]), len(counts_cnx[c]))
+                        if maxi > 5:
+                            diff = len(counts_cnx[new_c]) + \
+                                len(counts_cnx[c]) - maxi
+                            r = diff / float(maxi)
+                            if r > kb:
+                                if fLOG:  # pragma: no cover
+                                    fLOG('[train_test_connex_split]    balance '
+                                         'r={0:0.00000}>{1:0.00}, #[{2}]={3}, '
+                                         '#[{4}]={5}'.format(r, kb, new_c,
+                                                             len(counts_cnx[new_c]),
+                                                             c, len(counts_cnx[c])))
+                                continue
+
+                    if sib is not None:
+                        r = (len(counts_cnx[new_c]) +
+                             len(counts_cnx[c])) / float(len(elements))
+                        if r > sib:
+                            if fLOG:  # pragma: no cover
+                                fLOG('[train_test_connex_split]    no merge '
+                                     'r={0:0.00000}>{1:0.00}, #[{2}]={3}, #[{4}]={5}'
+                                     ''.format(r, sib, new_c, len(counts_cnx[new_c]),
+                                               c, len(counts_cnx[c])))
+                            avoids_merge[new_c, c] = i
+                            continue
+
+                    add_pair_c.append(c)
+
+                if len(add_pair_c) > 0:
+                    for c in add_pair_c:
+                        modif += len(counts_cnx[c])
+                        for ii in counts_cnx[c]:
+                            elements[ii] = new_c
+                        counts_cnx[new_c] = counts_cnx[new_c].union(
+                            counts_cnx[c])
+                        counts_cnx[c] = set()
+
+                        keys = list(vals)
+                        for val in keys:
+                            if connex[val] == c:
+                                connex[val] = new_c
+                                modif += 1
+
+    if must_groups:
+        do_connex_components(dfids_must, must_groups, None, None)
+    do_connex_components(dfids, groups, keep_balance, stop_if_bigger)
+
+    # final
+    dfids[name] = elements
+    dfids[one] = 1
+    grsum = dfids[[name, one]].groupby(name, as_index=False).sum()
+    if fLOG:
+        for g in groups:
+            fLOG(
+                f"[train_test_connex_split]     #nb in '{g}': {len(set(dfids[g]))}")
+        fLOG(
+            f"[train_test_connex_split] #connex {grsum.shape[0]}/{dfids.shape[0]}")
+    if grsum.shape[0] <= 1:
+        raise ValueError(  # pragma: no cover
+            "Every element is in the same connected components.")
+
+    # Statistics: top connected components
+    if fLOG:
+        # Global statistics
+        counts = Counter(elements)
+        cl = [(v, k) for k, v in counts.items()]
+        cum = 0
+        maxc = None
+        fLOG("[train_test_connex_split] number of connected components: {0}"
+             "".format(len(set(elements))))
+        for i, (v, k) in enumerate(sorted(cl, reverse=True)):
+            if i == 0:
+                maxc = k, v
+            if i >= 10:
+                break
+            cum += v
+            fLOG("[train_test_connex_split]     c={0} #elements={1} cumulated"
+                 "={2}/{3}".format(k, v, cum, len(elements)))
+
+        # Most important component
+        fLOG(
+            f'[train_test_connex_split] first row of the biggest component {maxc}')
+        tdf = dfids[dfids[name] == maxc[0]]
+        fLOG(f'[train_test_connex_split] \n{tdf.head(n=10)}')
+
+    # Splits.
+    train, test = train_test_split_weights(
+        grsum, weights=one, test_size=test_size, train_size=train_size,
+        shuffle=shuffle, fail_imbalanced=fail_imbalanced,
+        random_state=random_state)
+    train.drop(one, inplace=True, axis=1)
+    test.drop(one, inplace=True, axis=1)
+
+    # We compute the final dataframe.
+    def double_merge(d):
+        "merge twice"
+        merge1 = dfids.merge(d, left_on=name, right_on=name)
+        merge2 = df.merge(merge1, left_on=groups, right_on=groups)
+        return merge2
+
+    train_f = double_merge(train)
+    test_f = double_merge(test)
+    if return_cnx:
+        return train_f, test_f, (connex, dfids)
+    else:
+        return train_f, test_f
+
+
+def train_test_apart_stratify(df, group, test_size=0.25, train_size=None,
+                              stratify=None, force=False, random_state=None,
+                              fLOG=None):
+    """
+    This split is for a specific case where data is linked
+    in one way. Let's assume we have two ids as we have
+    for online sales: *(product id, category id)*.
+    A product can have multiple categories. We need to have
+    distinct products on train and test but common categories
+    on both sides.
+
+    @param  df              :epkg:`pandas:DataFrame`
+    @param  group           columns name for the ids
+    @param  test_size       ratio for the test partition
+                            (if *train_size* is not specified)
+    @param  train_size      ratio for the train partition
+    @param  stratify        column holding the stratification
+    @param  force           if True, tries to get at least one example on the test side
+                            for each value of the column *stratify*
+    @param  random_state    seed for random generators
+    @param  fLOG            logging function
+    @return                 Two @see cl StreamingDataFrame, one
+                            for train, one for test.
+
+    .. index:: multi-label
+
+    The list of ids must hold in memory.
+    There is no streaming implementation for the ids.
+    This split was implemented for a case of a multi-label
+    classification. A category (*stratify*) is not exclusive
+    and an observation can be assigned to multiple
+    categories. In that particular case, the method
+    `train_test_split <http://scikit-learn.org/stable/modules/generated/
+    sklearn.model_selection.train_test_split.html>`_
+    can not directly be used.
+
+    .. runpython::
+        :showcode:
+
+        import pandas
+        from pandas_streaming.df import train_test_apart_stratify
+
+        df = pandas.DataFrame([dict(a=1, b="e"),
+                               dict(a=1, b="f"),
+                               dict(a=2, b="e"),
+                               dict(a=2, b="f")])
+
+        train, test = train_test_apart_stratify(
+            df, group="a", stratify="b", test_size=0.5)
+        print(train)
+        print('-----------')
+        print(test)
+    """
+    if stratify is None:
+        raise ValueError(  # pragma: no cover
+            "stratify must be specified.")
+    if group is None:
+        raise ValueError(  # pragma: no cover
+            "group must be specified.")
+    if hasattr(df, 'iter_creation'):
+        raise NotImplementedError(
+            'Not implemented yet for StreamingDataFrame.')
+    if isinstance(df, numpy.ndarray):
+        raise NotImplementedError("Not implemented on numpy arrays.")
+
+    p = (1 - test_size) if test_size else None
+    if train_size is not None:
+        p = train_size
+    test_size = 1 - p
+    if p is None or min(test_size, p) <= 0:
+        raise ValueError(  # pragma: no cover
+            f"test_size={test_size} or train_size={train_size} cannot be null")
+
+    couples = df[[group, stratify]].itertuples(name=None, index=False)
+    hist = Counter(df[stratify])
+    sorted_hist = [(v, k) for k, v in hist.items()]
+    sorted_hist.sort()
+    ids = {c: set() for c in hist}
+
+    for g, s in couples:
+        ids[s].add(g)
+
+    if random_state is None:
+        permutation = numpy.random.permutation
+    else:
+        state = numpy.random.RandomState(random_state)
+        permutation = state.permutation
+
+    split = {}
+    for _, k in sorted_hist:
+        not_assigned = [c for c in ids[k] if c not in split]
+        if len(not_assigned) == 0:
+            continue
+        assigned = [c for c in ids[k] if c in split]
+        nb_test = sum(split[c] for c in assigned)
+        expected = min(len(ids[k]), int(
+            test_size * len(ids[k]) + 0.5)) - nb_test
+        if force and expected == 0 and nb_test == 0:
+            nb_train = len(assigned) - nb_test
+            if nb_train > 0 or len(not_assigned) > 1:
+                expected = min(1, len(not_assigned))
+        if expected > 0:
+            permutation(not_assigned)
+            for e in not_assigned[:expected]:
+                split[e] = 1
+            for e in not_assigned[expected:]:
+                split[e] = 0
+        else:
+            for c in not_assigned:
+                split[c] = 0
+
+    train_set = set(k for k, v in split.items() if v == 0)
+    test_set = set(k for k, v in split.items() if v == 1)
+    train_df = df[df[group].isin(train_set)]
+    test_df = df[df[group].isin(test_set)]
+    return train_df, test_df
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/df/dataframe.py` & `pandas_streaming-0.3.239/pandas_streaming/df/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -*- coding: utf-8 -*-
+# pylint: disable=W0102
 """
 @file
 @brief Defines a streaming dataframe.
 """
 import pickle
 import os
 from io import StringIO, BytesIO
 from inspect import isfunction
 import numpy
 import numpy.random as nrandom
 import pandas
 from pandas.testing import assert_frame_equal
-from pandas.io.json import json_normalize
+try:
+    from pandas import json_normalize
+except ImportError:
+    from pandas.io.json import json_normalize
 from .dataframe_split import sklearn_train_test_split, sklearn_train_test_split_streaming
 from .dataframe_io_helpers import enumerate_json_items, JsonIterator2Stream
 
 
 class StreamingDataFrameSchemaError(Exception):
     """
     Reveals an issue with inconsistant schemas.
@@ -284,15 +288,16 @@
         if chunksize is None:
             return StreamingDataFrame(
                 lambda: pandas.read_json(
                     st, *args, chunksize=chunksize, lines=True, **kwargs),
                 **kwargs_create)
 
         def fct3(st=st, args=args, chunksize=chunksize, kw=kwargs.copy()):
-            st.seek(0)
+            if hasattr(st, 'seek'):
+                st.seek(0)
             for r in pandas.read_json(
                     st, *args, chunksize=chunksize, nrows=chunksize,
                     lines=True, **kw):
                 yield r
         return StreamingDataFrame(fct3, **kwargs_create)
 
     @staticmethod
@@ -350,22 +355,21 @@
         @return                     iterator on @see cl StreamingDataFrame
         """
         if chunksize is None:
             if hasattr(df, 'shape'):
                 chunksize = df.shape[0]
             else:
                 raise NotImplementedError(
-                    "Cannot retrieve size to infer chunksize for type={0}"
-                    ".".format(type(df)))
+                    f"Cannot retrieve size to infer chunksize for type={type(df)}.")
 
         if hasattr(df, 'shape'):
             size = df.shape[0]
         else:
             raise NotImplementedError(  # pragma: no cover
-                "Cannot retrieve size for type={0}.".format(type(df)))
+                f"Cannot retrieve size for type={type(df)}.")
 
         def local_iterator():
             "local iterator"
             for i in range(0, size, chunksize):
                 end = min(size, i + chunksize)
                 yield df[i:end].copy()
         return StreamingDataFrame(local_iterator, check_schema=check_schema)
@@ -604,14 +608,32 @@
                             buffer.clear()
             if len(buffer) > 0:
                 yield pandas.DataFrame(buffer)
 
         return StreamingDataFrame(
             lambda: reservoir_iterate(sdf=self, indices=indices, chunksize=1000))
 
+    def drop(self, labels=None, *, axis=0, index=None, columns=None, level=None,
+             inplace=False, errors='raise') -> 'StreamingDataFrame':
+        """
+        Applies :epkg:`pandas:DataFrame:drop`.
+        This function returns a @see cl StreamingDataFrame.
+        """
+        if axis == 0:
+            raise NotImplementedError(
+                f"drop is not implemented for axis={axis}.")
+        if inplace:
+            raise NotImplementedError(
+                f"drop is not implemented for inplace={inplace}.")
+        return StreamingDataFrame(
+            lambda: map(lambda df: df.drop(
+                labels, axis=axis, index=index, columns=columns,
+                level=level, inplace=False, errors=errors), self),
+            **self.get_kwargs())
+
     def apply(self, *args, **kwargs) -> 'StreamingDataFrame':
         """
         Applies :epkg:`pandas:DataFrame:apply`.
         This function returns a @see cl StreamingDataFrame.
         """
         return StreamingDataFrame(
             lambda: map(lambda df: df.apply(*args, **kwargs), self),
@@ -691,18 +713,18 @@
                 yield df
             for obj in lothers:
                 check = True
                 for i, df in enumerate(obj):
                     if check:
                         if list(columns) != list(df.columns):
                             raise ValueError(
-                                "Frame others[{0}] do not have the same column names or the same order.".format(i))
+                                f"Frame others[{i}] do not have the same column names or the same order.")
                         if list(dtypes) != list(df.dtypes):
                             raise ValueError(
-                                "Frame others[{0}] do not have the same column types.".format(i))
+                                f"Frame others[{i}] do not have the same column types.")
                         check = False
                     yield df
 
         if isinstance(others, pandas.DataFrame):
             others = [others]
         elif isinstance(others, StreamingDataFrame):
             others = [others]
@@ -891,15 +913,15 @@
                 for df in self:
                     gr = df.groupby(by=by, **ckw)
                     gragg = lambda_agg(gr)
                     yield lambda_agg(gragg.groupby(by=by, **kwargs))
             return StreamingDataFrame(lambda: iterate_streaming(), **self.get_kwargs())
 
         raise ValueError(  # pragma: no cover
-            "Unknown strategy '{0}'".format(strategy))
+            f"Unknown strategy '{strategy}'")
 
     def ensure_dtype(self, df, dtypes):
         """
         Ensures the :epkg:`dataframe` *df* has types indicated in dtypes.
         Changes it if not.
 
         :param df: dataframe
@@ -917,15 +939,16 @@
 
     def __getitem__(self, *args):
         """
         Implements some of the functionalities :epkg:`pandas`
         offers for the operator ``[]``.
         """
         if len(args) != 1:
-            raise NotImplementedError("Only a list of columns is supported.")
+            raise NotImplementedError(  # pragma: no cover
+                "Only a list of columns is supported.")
         cols = args[0]
         if isinstance(cols, str):
             # One column.
             iter_creation = self.iter_creation
 
             def iterate_col():
                 "iterate on one column"
@@ -946,15 +969,15 @@
 
     def __setitem__(self, index, value):
         """
         Limited set of operators are supported.
         """
         if not isinstance(index, str):
             raise ValueError(
-                "Only column affected are supported but index=%r." % index)
+                f"Only column affected are supported but index={index!r}.")
         if isinstance(value, (int, float, numpy.number, str)):
             # Is is equivalent to add_column.
             iter_creation = self.iter_creation
 
             def iterate_fct():
                 "iterate on rows"
                 iters = iter_creation()
@@ -1017,15 +1040,15 @@
                 print(sdf2.to_dataframe())
 
                 sdf2 = sdf.add_column("d", lambda row: int(1))
                 print(sdf2.to_dataframe())
 
         """
         if not isinstance(col, str):
-            raise NotImplementedError(
+            raise NotImplementedError(  # pragma: no cover
                 "Only a column as a string is supported.")
 
         if isfunction(value):
             def iterate_fct(self, value, col):
                 "iterate on rows"
                 for df in self:
                     dfc = df.copy()
@@ -1072,34 +1095,36 @@
             else:
                 for df in self:
                     yield df.fillna(**kwargs)
 
         return StreamingDataFrame(
             lambda: iterate_na(self, **kwargs), **self.get_kwargs())
 
-    def describe(self, percentiles=None, include=None, exclude=None,
-                 datetime_is_numeric=False):
+    def describe(self, percentiles=None, include=None, exclude=None):
         """
         Calls :epkg:`pandas:DataFrame:describe` on every piece
         of the datasets. *percentiles* are not really accurate
         but just an indication.
 
         :param percentiles: see :epkg:`pandas:DataFrame:describe`
         :param include: see :epkg:`pandas:DataFrame:describe`
         :param exclude: see :epkg:`pandas:DataFrame:describe`
-        :param datetime_is_numeric: see :epkg:`pandas:DataFrame:describe`
         :return: :epkg:`pandas:DataFrame:describe`
+
+        .. versionchanged:: 0.3.219
+
+            Parameter *datetime_is_numeric* was removed
+            (see :epkg:`pandas:DataFrame:describe`).
         """
         merged = None
         stack = []
         notper = ['count', 'mean', 'std']
         for df in self:
             desc = df.describe(
-                percentiles=percentiles, include=include, exclude=exclude,
-                datetime_is_numeric=datetime_is_numeric)
+                percentiles=percentiles, include=include, exclude=exclude)
             count = desc.loc['count', :]
             rows = [name for name in desc.index if name not in notper]
             stack.append(desc.loc[rows, :])
             if merged is None:
                 merged = desc
                 merged.loc['std', :] = (
                     merged.loc['std', :] ** 2 + merged.loc['mean', :] ** 2) * count
@@ -1114,16 +1139,15 @@
                 merged.loc['min', :] = numpy.maximum(
                     merged.loc['min', :], desc.loc['min', :])
         merged.loc['mean', :] /= merged.loc['count', :]
         merged.loc['std', :] = (
             merged.loc['std', :] / merged.loc['count', :] -
             merged.loc['mean', :] ** 2) ** 0.5
         values = pandas.concat(stack)
-        summary = values.describe(percentiles=percentiles,
-                                  datetime_is_numeric=datetime_is_numeric)
+        summary = values.describe(percentiles=percentiles)
         merged = merged.loc[notper, :]
         rows = [name for name in summary.index if name not in notper]
         summary = summary.loc[rows, :]
         return pandas.concat([merged, summary])
 
     def sort_values(self, by, axis=0, ascending=True, kind='quicksort',
                     na_position='last',
@@ -1139,16 +1163,16 @@
             without storing intermediate results on disk
             unless it can fit into the memory, but in that case,
             it is easier to convert the streaming database into
             a dataframe and sort it
         :return: streaming database
         """
         if not isinstance(by, str):
-            raise NotImplementedError(
-                "Only one column can be used to sort not %r." % by)
+            raise NotImplementedError(  # pragma: no cover
+                f"Only one column can be used to sort not {by!r}.")
         keys = {}
         nans = []
         indices = []
         with open(temp_file, 'wb') as f:
             for df in self:
                 dfs = df.sort_values(by, ascending=ascending, kind=kind,
                                      na_position=na_position)
@@ -1218,16 +1242,17 @@
     Seens as a @see cl StreamingDataFrame of one column.
     """
 
     def __init__(self, iter_creation, check_schema=True, stable=True):
         StreamingDataFrame.__init__(
             self, iter_creation, check_schema=check_schema, stable=stable)
         if len(self.columns) != 1:
-            raise RuntimeError(
-                "A series can contain only one column not %r." % len(self.columns))
+            raise RuntimeError(  # pragma: no cover
+                f"A series can contain only one column not "
+                f"{len(self.columns)!r}.")
 
     def apply(self, *args, **kwargs) -> 'StreamingDataFrame':
         """
         Applies :epkg:`pandas:Series:apply`.
         This function returns a @see cl StreamingSeries.
         """
         return StreamingSeries(
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/df/dataframe_helpers.py` & `pandas_streaming-0.3.239/pandas_streaming/df/dataframe_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @file
 @brief Helpers for dataframes.
 """
 import hashlib
 import struct
 import warnings
 import numpy
-from pandas import DataFrame, Index
+from pandas import DataFrame, Index, Series
 
 
 def numpy_types():
     """
     Returns the list of :epkg:`numpy` available types.
 
     :return: list of types
@@ -45,15 +45,15 @@
     @param      c               value to hash
     @param      hash_length     hash_length
     @return                     string
     """
     if isinstance(c, float):
         if numpy.isnan(c):
             return c
-        raise ValueError("numpy.nan expected, not {0}".format(c))
+        raise ValueError(f"numpy.nan expected, not {c}")
     m = hashlib.sha256()
     m.update(c.encode("utf-8"))
     r = m.hexdigest()
     if len(r) >= hash_length:
         return r[:hash_length]
     return r
 
@@ -66,15 +66,15 @@
     @param      hash_length     hash_length
     @return                     int
     """
     if isinstance(c, float):
         if numpy.isnan(c):
             return c
         else:
-            raise ValueError("numpy.nan expected, not {0}".format(c))
+            raise ValueError(f"numpy.nan expected, not {c}")
     else:
         b = struct.pack("i", c)
         m = hashlib.sha256()
         m.update(b)
         r = m.hexdigest()
         if len(r) >= hash_length:
             r = r[:hash_length]
@@ -162,16 +162,16 @@
         elif t == numpy.int64:
             df[c] = df[c].apply(lambda x: numpy.int64(hash_intl(x)))
         elif t == float:
             df[c] = df[c].apply(hash_floatl)
         elif t == object:
             df[c] = df[c].apply(hash_strl)
         else:
-            raise NotImplementedError(
-                "Conversion of type {0} in column '{1}' is not implemented".format(t, c))
+            raise NotImplementedError(  # pragma: no cover
+                f"Conversion of type {t} in column '{c}' is not implemented")
 
     return df
 
 
 def dataframe_unfold(df, col, new_col=None, sep=","):
     """
     One column may contain concatenated values.
@@ -385,14 +385,26 @@
                     dict(a=2, ind="a"),
                     dict(a=3, ind="b"),
                     dict(a=30)]
             df = DataFrame(data)
             gr2 = pandas_groupby_nan(df, ["ind"]).sum()
             print(gr2)
     """
+    if nanback and suffix is None:
+        try:
+            res = df.groupby(by, axis=axis, as_index=as_index,
+                             dropna=False, **kwargs)
+        except TypeError:
+            # old version of pandas
+            res = None
+        if res is not None:
+            if suffix is None:
+                return res
+            res.index = Series(res.index).replace(numpy.nan, suffix)
+            return res
     if axis != 0:
         raise NotImplementedError("axis should be 0")
     if as_index:
         raise NotImplementedError("as_index must be False")
     if isinstance(by, tuple):
         raise TypeError("by should be of list not tuple")
     if not isinstance(by, list):
@@ -409,15 +421,15 @@
             if not nanback:
                 dummy = DataFrame([{"a": "a"}])
                 do = dummy.dtypes[0]
                 typ = {c: t for c, t in zip(  # pylint: disable=R1721
                     df.columns, df.dtypes)}  # pylint: disable=R1721
                 if typ[by[0]] != do:
                     warnings.warn(  # pragma: no cover
-                        "[pandas_groupby_nan] NaN value: {0}".format(rep))
+                        f"[pandas_groupby_nan] NaN value: {rep}")
                 return res
             for b in by:
                 fnan = rep[b]
                 if fnan in res.grouper.groups:
                     res.grouper.groups[numpy.nan] = res.grouper.groups[fnan]
                     del res.grouper.groups[fnan]
                 new_val = list((numpy.nan if b == fnan else b)
@@ -448,31 +460,31 @@
                                 new_index = numpy.array(index)
                                 for i in range(0, len(new_index)):  # pylint: disable=C0200
                                     if new_index[i] == key:
                                         new_index[i] = numpy.nan
                                 res.grouper.groupings[0]._cache['result_index'] = (
                                     index.__class__(new_index))
                             else:
-                                raise NotImplementedError(
+                                raise NotImplementedError(  # pragma: no cover
                                     "NaN values not implemented for multiindex.")
                     else:
-                        raise NotImplementedError(
+                        raise NotImplementedError(  # pragma: no cover
                             "Not implemented for type: {0}".format(
                                 type(res.grouper.groupings[0].grouper)))
                 res.grouper._cache['result_index'] = res.grouper.groupings[0]._group_index
         else:
             if not nanback:
                 dummy = DataFrame([{"a": "a"}])
                 do = dummy.dtypes[0]
                 typ = {c: t for c, t in zip(  # pylint: disable=R1721
                     df.columns, df.dtypes)}  # pylint: disable=R1721
                 for b in by:
                     if typ[b] != do:
                         warnings.warn(  # pragma: no cover
-                            "[pandas_groupby_nan] NaN values: {0}".format(rep))
+                            f"[pandas_groupby_nan] NaN values: {rep}")
                         break
                 return res
             raise NotImplementedError(
                 "Not yet implemented. Replacing pseudo nan values by real nan "
                 "values is not as easy as it looks. Use nanback=False")
 
             # keys = list(res.grouper.groups.keys())
@@ -515,9 +527,8 @@
             #         if isinstance(grou.grouper, numpy.ndarray):
             #             grou.grouper = numpy.array(new_val)
             #         else:
             #             raise NotImplementedError(
             #                 "Not implemented for type: {0}".format(type(grou.grouper)))
             #     del res.grouper._cache
         return res
-    else:
-        return df.groupby(by, axis=axis, **kwargs)
+    return df.groupby(by, axis=axis, **kwargs)
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/df/dataframe_io.py` & `pandas_streaming-0.3.239/pandas_streaming/df/dataframe_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,30 +75,30 @@
         ext = os.path.splitext(zname)[-1]
         if ext != '.npy':
             raise ValueError(  # pragma: no cover
                 "Extension '.npy' is required when saving a numpy array.")
         numpy.save(stb, df, **kwargs)
     else:
         raise TypeError(  # pragma: no cover
-            "Type not handled {0}".format(type(df)))
+            f"Type not handled {type(df)}")
     text = stb.getvalue()
 
     if isinstance(zipfilename, str):
         ext = os.path.splitext(zipfilename)[-1]
         if ext != '.zip':
             raise NotImplementedError(  # pragma: no cover
-                "Only zip file are implemented not '{0}'.".format(ext))
+                f"Only zip file are implemented not '{ext}'.")
         zf = zipfile.ZipFile(zipfilename, 'w')  # pylint: disable=R1732
         close = True
     elif isinstance(zipfilename, zipfile.ZipFile):
         zf = zipfilename
         close = False
     else:
         raise TypeError(  # pragma: no cover
-            "No implementation for type '{0}'".format(type(zipfilename)))
+            f"No implementation for type '{type(zipfilename)}'")
 
     zf.writestr(zname, text)
     if close:
         zf.close()
 
 
 def read_zip(zipfilename, zname=None, **kwargs):
@@ -111,23 +111,23 @@
     :param kwargs: parameters for :func:`pandas.read_csv`
     :return: :func:`pandas.DataFrame` or :epkg:`numpy:array`
     """
     if isinstance(zipfilename, str):
         ext = os.path.splitext(zipfilename)[-1]
         if ext != '.zip':
             raise NotImplementedError(  # pragma: no cover
-                "Only zip files are supported not '{0}'.".format(ext))
+                f"Only zip files are supported not '{ext}'.")
         zf = zipfile.ZipFile(zipfilename, 'r')  # pylint: disable=R1732
         close = True
     elif isinstance(zipfilename, zipfile.ZipFile):
         zf = zipfilename
         close = False
     else:
         raise TypeError(  # pragma: no cover
-            "No implementation for type '{0}'".format(type(zipfilename)))
+            f"No implementation for type '{type(zipfilename)}'")
 
     if zname is None:
         zname = zf.namelist()[0]
     content = zf.read(zname)
     stb = io.BytesIO(content)
     ext = os.path.splitext(zname)[-1]
     if ext == '.npy':
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/df/dataframe_io_helpers.py` & `pandas_streaming-0.3.239/pandas_streaming/df/dataframe_io_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,453 +1,452 @@
-# -*- coding: utf-8 -*-
-"""
-@file
-@brief Saves and reads a :epkg:`dataframe` into a :epkg:`zip` file.
-"""
-import os
-from io import StringIO, BytesIO
-try:
-    from ujson import dumps
-except ImportError:  # pragma: no cover
-    from json import dumps
-import ijson
-
-
-class JsonPerRowsStream:
-    """
-    Reads a :epkg:`json` streams and adds
-    ``,``, ``[``, ``]`` to convert a stream containing
-    one :epkg:`json` object per row into one single :epkg:`json` object.
-    It only implements method *readline*.
-
-    :param st: stream
-    """
-
-    def __init__(self, st):
-        self.st = st
-        self.begin = True
-        self.newline = False
-        self.end = True
-
-    def seek(self, offset):
-        """
-        Change the stream position to the given byte offset.
-
-        :param offset: offset, only 0 is implemented
-        """
-        self.st.seek(offset)
-
-    def readline(self, size=-1):
-        """
-        Reads a line, adds ``,``, ``[``, ``]`` if needed.
-        So the number of read characters is not recessarily
-        the requested one but could be greater.
-        """
-        text = self.st.readline(size)
-        if size == 0:
-            return text
-        if self.newline:
-            text = ',' + text
-            self.newline = False
-        elif self.begin:
-            text = '[' + text
-            self.begin = False
-
-        if text.endswith("\n"):
-            self.newline = True
-            return text
-        if len(text) == 0 or len(text) < size:
-            if self.end:
-                self.end = False
-                return text + ']'
-            return text
-        return text
-
-    def read(self, size=-1):
-        """
-        Reads characters, adds ``,``, ``[``, ``]`` if needed.
-        So the number of read characters is not recessarily
-        the requested one but could be greater.
-        """
-        text = self.st.read(size)
-        if isinstance(text, bytes):
-            cst = b"\n", b"\n,", b",", b"[", b"]"
-        else:
-            cst = "\n", "\n,", ",", "[", "]"
-        if size == 0:
-            return text
-        if len(text) > 1:
-            t1, t2 = text[:len(text) - 1], text[len(text) - 1:]
-            t1 = t1.replace(cst[0], cst[1])
-            text = t1 + t2
-
-        if self.newline:
-            text = cst[2] + text
-            self.newline = False
-        elif self.begin:
-            text = cst[3] + text
-            self.begin = False
-
-        if text.endswith(cst[0]):
-            self.newline = True
-            return text
-        if len(text) == 0 or len(text) < size:
-            if self.end:
-                self.end = False
-                return text + cst[4]
-            return text
-        return text
-
-    def getvalue(self):
-        """
-        Returns the whole stream content.
-        """
-        def byline():
-            line = self.readline()
-            while line:
-                yield line
-                line = self.readline()
-        return "".join(byline())
-
-
-def flatten_dictionary(dico, sep="_"):
-    """
-    Flattens a dictionary with nested structure to a dictionary with no
-    hierarchy.
-
-    :param dico: dictionary to flatten
-    :param sep: string to separate dictionary keys by
-    :return: flattened dictionary
-
-    Inspired from `flatten_json
-    <https://github.com/amirziai/flatten/blob/master/flatten_json.py>`_.
-    """
-    flattened_dict = {}
-
-    def _flatten(obj, key):
-        if obj is None:
-            flattened_dict[key] = obj
-        elif isinstance(obj, dict):
-            for k, v in obj.items():
-                if not isinstance(k, str):
-                    raise TypeError(
-                        "All keys must a string.")  # pragma: no cover
-                k2 = k if key is None else "{0}{1}{2}".format(key, sep, k)
-                _flatten(v, k2)
-        elif isinstance(obj, (list, set)):
-            for index, item in enumerate(obj):
-                k2 = k if key is None else "{0}{1}{2}".format(key, sep, index)
-                _flatten(item, k2)
-        else:
-            flattened_dict[key] = obj
-
-    _flatten(dico, None)
-    return flattened_dict
-
-
-def enumerate_json_items(filename, encoding=None, lines=False, flatten=False, fLOG=None):
-    """
-    Enumerates items from a :epkg:`JSON` file or string.
-
-    :param filename: filename or string or stream to parse
-    :param encoding: encoding
-    :param lines: one record per row
-    :param flatten: call @see fn flatten_dictionary
-    :param fLOG: logging function
-    :return: iterator on records at first level.
-
-    It assumes the syntax follows the format: ``[ {"id":1, ...}, {"id": 2, ...}, ...]``.
-    However, if option *lines* if true, the function considers that the
-    stream or file does have one record per row as follows:
-
-        {"id":1, ...}
-        {"id": 2, ...}
-
-    .. exref::
-        :title: Processes a json file by streaming.
-
-        The module :epkg:`ijson` can read a :epkg:`JSON` file by streaming.
-        This module is needed because a record can be written on multiple lines.
-        This function leverages it produces the following results.
-
-        .. runpython::
-            :showcode:
-
-            from pandas_streaming.df.dataframe_io_helpers import enumerate_json_items
-
-            text_json = b'''
-                [
-                {
-                    "glossary": {
-                        "title": "example glossary",
-                        "GlossDiv": {
-                            "title": "S",
-                            "GlossList": [{
-                                "GlossEntry": {
-                                    "ID": "SGML",
-                                    "SortAs": "SGML",
-                                    "GlossTerm": "Standard Generalized Markup Language",
-                                    "Acronym": "SGML",
-                                    "Abbrev": "ISO 8879:1986",
-                                    "GlossDef": {
-                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
-                                        "GlossSeeAlso": ["GML", "XML"]
-                                    },
-                                    "GlossSee": "markup"
-                                }
-                            }]
-                        }
-                    }
-                },
-                {
-                    "glossary": {
-                        "title": "example glossary",
-                        "GlossDiv": {
-                            "title": "S",
-                            "GlossList": {
-                                "GlossEntry": [{
-                                    "ID": "SGML",
-                                    "SortAs": "SGML",
-                                    "GlossTerm": "Standard Generalized Markup Language",
-                                    "Acronym": "SGML",
-                                    "Abbrev": "ISO 8879:1986",
-                                    "GlossDef": {
-                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
-                                        "GlossSeeAlso": ["GML", "XML"]
-                                    },
-                                    "GlossSee": "markup"
-                                }]
-                            }
-                        }
-                    }
-                }
-                ]
-            '''
-
-            for item in enumerate_json_items(text_json):
-                print(item)
-
-    The parsed json must have an empty line at the end otherwise
-    the following exception is raised:
-    `ijson.common.IncompleteJSONError: `
-    `parse error: unallowed token at this point in JSON text`.
-    """
-    if isinstance(filename, str):
-        if "{" not in filename and os.path.exists(filename):
-            with open(filename, "r", encoding=encoding) as f:
-                for el in enumerate_json_items(
-                        f, encoding=encoding, lines=lines,
-                        flatten=flatten, fLOG=fLOG):
-                    yield el
-        else:
-            st = StringIO(filename)
-            for el in enumerate_json_items(
-                    st, encoding=encoding, lines=lines,
-                    flatten=flatten, fLOG=fLOG):
-                yield el
-    elif isinstance(filename, bytes):
-        st = BytesIO(filename)
-        for el in enumerate_json_items(
-                st, encoding=encoding, lines=lines, flatten=flatten,
-                fLOG=fLOG):
-            yield el
-    elif lines:
-        for el in enumerate_json_items(
-                JsonPerRowsStream(filename),
-                encoding=encoding, lines=False, flatten=flatten, fLOG=fLOG):
-            yield el
-    else:
-        if hasattr(filename, 'seek'):
-            filename.seek(0)
-        parser = ijson.parse(filename)
-        current = None
-        curkey = None
-        stack = []
-        nbyield = 0
-        for i, (_, event, value) in enumerate(parser):
-            if i % 1000000 == 0 and fLOG is not None:
-                fLOG(  # pragma: no cover
-                    "[enumerate_json_items] i={0} yielded={1}"
-                    "".format(i, nbyield))
-            if event == "start_array":
-                if curkey is None:
-                    current = []
-                else:
-                    if not isinstance(current, dict):
-                        raise RuntimeError(  # pragma: no cover
-                            "Type issue {0}".format(type(current)))
-                    c = []
-                    current[curkey] = c  # pylint: disable=E1137
-                    current = c
-                curkey = None
-                stack.append(current)
-            elif event == "end_array":
-                stack.pop()
-                if len(stack) == 0:
-                    # We should be done.
-                    current = None
-                else:
-                    current = stack[-1]
-            elif event == "start_map":
-                c = {}
-                if curkey is None:
-                    if current is None:
-                        current = []
-                    current.append(c)
-                else:
-                    current[curkey] = c  # pylint: disable=E1137
-                stack.append(c)
-                current = c
-                curkey = None
-            elif event == "end_map":
-                stack.pop()
-                current = stack[-1]
-                if len(stack) == 1:
-                    nbyield += 1
-                    if flatten:
-                        yield flatten_dictionary(current[-1])
-                    else:
-                        yield current[-1]
-                    # We clear the memory.
-                    current.clear()
-            elif event == "map_key":
-                curkey = value
-            elif event in {"string", "number", "boolean"}:
-                if curkey is None:
-                    current.append(value)
-                else:
-                    current[curkey] = value  # pylint: disable=E1137
-                    curkey = None
-            elif event == "null":
-                if curkey is None:
-                    current.append(None)
-                else:
-                    current[curkey] = None  # pylint: disable=E1137
-                    curkey = None
-            else:
-                raise ValueError("Unknown event '{0}'".format(
-                    event))  # pragma: no cover
-
-
-class JsonIterator2Stream:
-    """
-    Transforms an iterator on :epkg:`JSON` items
-    into a stream which returns an items as a string every time
-    method *read* is called.
-    The iterator could be one returned by @see fn enumerate_json_items.
-
-    :param it: iterator
-    :param kwargs: arguments to :epkg:`*py:json:dumps`
-
-    .. exref::
-        :title: Reshape a json file
-
-        The function @see fn enumerate_json_items reads any
-        :epkg:`json` even if every record is split over
-        multiple lines. Class @see cl JsonIterator2Stream
-        mocks this iterator as a stream. Each row is a single item.
-
-        .. runpython::
-            :showcode:
-
-            from pandas_streaming.df.dataframe_io_helpers import enumerate_json_items, JsonIterator2Stream
-
-            text_json = b'''
-                [
-                {
-                    "glossary": {
-                        "title": "example glossary",
-                        "GlossDiv": {
-                            "title": "S",
-                            "GlossList": [{
-                                "GlossEntry": {
-                                    "ID": "SGML",
-                                    "SortAs": "SGML",
-                                    "GlossTerm": "Standard Generalized Markup Language",
-                                    "Acronym": "SGML",
-                                    "Abbrev": "ISO 8879:1986",
-                                    "GlossDef": {
-                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
-                                        "GlossSeeAlso": ["GML", "XML"]
-                                    },
-                                    "GlossSee": "markup"
-                                }
-                            }]
-                        }
-                    }
-                },
-                {
-                    "glossary": {
-                        "title": "example glossary",
-                        "GlossDiv": {
-                            "title": "S",
-                            "GlossList": {
-                                "GlossEntry": [{
-                                    "ID": "SGML",
-                                    "SortAs": "SGML",
-                                    "GlossTerm": "Standard Generalized Markup Language",
-                                    "Acronym": "SGML",
-                                    "Abbrev": "ISO 8879:1986",
-                                    "GlossDef": {
-                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
-                                        "GlossSeeAlso": ["GML", "XML"]
-                                    },
-                                    "GlossSee": "markup"
-                                }]
-                            }
-                        }
-                    }
-                }
-                ]
-            '''
-
-            for item in JsonIterator2Stream(lambda: enumerate_json_items(text_json)):
-                print(item)
-
-    .. versionchanged:: 0.3
-        The class takes a function which outputs an iterator and not an iterator.
-        `JsonIterator2Stream(enumerate_json_items(text_json))` needs to be rewritten
-        into JsonIterator2Stream(lambda: enumerate_json_items(text_json)).
-    """
-
-    def __init__(self, it, **kwargs):
-        self.it = it
-        self.kwargs = kwargs
-        self.it0 = it()
-
-    def seek(self, offset):
-        """
-        Change the stream position to the given byte offset.
-
-        :param offset: offset, only 0 is implemented
-        """
-        if offset != 0:
-            raise NotImplementedError(
-                "The iterator can only return at the beginning.")
-        self.it0 = self.it()
-
-    def write(self):
-        """
-        The class does not write.
-        """
-        raise NotImplementedError()
-
-    def read(self):
-        """
-        Reads the next item and returns it as a string.
-        """
-        try:
-            value = next(self.it0)
-            return dumps(value, **self.kwargs)
-        except StopIteration:
-            return None
-
-    def __iter__(self):
-        """
-        Iterates on each row. The behaviour is a bit tricky.
-        It is implemented to be swalled by :func:`pandas.read_json` which
-        uses :func:`itertools.islice` to go through the items.
-        It calls multiple times `__iter__` but does expect the
-        iterator to continue from where it stopped last time.
-        """
-        for value in self.it0:
-            yield dumps(value, **self.kwargs)
+# -*- coding: utf-8 -*-
+"""
+@file
+@brief Saves and reads a :epkg:`dataframe` into a :epkg:`zip` file.
+"""
+import os
+from io import StringIO, BytesIO
+try:
+    from ujson import dumps
+except ImportError:  # pragma: no cover
+    from json import dumps
+import ijson
+
+
+class JsonPerRowsStream:
+    """
+    Reads a :epkg:`json` streams and adds
+    ``,``, ``[``, ``]`` to convert a stream containing
+    one :epkg:`json` object per row into one single :epkg:`json` object.
+    It only implements method *readline*.
+
+    :param st: stream
+    """
+
+    def __init__(self, st):
+        self.st = st
+        self.begin = True
+        self.newline = False
+        self.end = True
+
+    def seek(self, offset):
+        """
+        Change the stream position to the given byte offset.
+
+        :param offset: offset, only 0 is implemented
+        """
+        self.st.seek(offset)
+
+    def readline(self, size=-1):
+        """
+        Reads a line, adds ``,``, ``[``, ``]`` if needed.
+        So the number of read characters is not recessarily
+        the requested one but could be greater.
+        """
+        text = self.st.readline(size)
+        if size == 0:
+            return text
+        if self.newline:
+            text = ',' + text
+            self.newline = False
+        elif self.begin:
+            text = '[' + text
+            self.begin = False
+
+        if text.endswith("\n"):
+            self.newline = True
+            return text
+        if len(text) == 0 or len(text) < size:
+            if self.end:
+                self.end = False
+                return text + ']'
+            return text
+        return text
+
+    def read(self, size=-1):
+        """
+        Reads characters, adds ``,``, ``[``, ``]`` if needed.
+        So the number of read characters is not recessarily
+        the requested one but could be greater.
+        """
+        text = self.st.read(size)
+        if isinstance(text, bytes):
+            cst = b"\n", b"\n,", b",", b"[", b"]"
+        else:
+            cst = "\n", "\n,", ",", "[", "]"
+        if size == 0:
+            return text
+        if len(text) > 1:
+            t1, t2 = text[:len(text) - 1], text[len(text) - 1:]
+            t1 = t1.replace(cst[0], cst[1])
+            text = t1 + t2
+
+        if self.newline:
+            text = cst[2] + text
+            self.newline = False
+        elif self.begin:
+            text = cst[3] + text
+            self.begin = False
+
+        if text.endswith(cst[0]):
+            self.newline = True
+            return text
+        if len(text) == 0 or len(text) < size:
+            if self.end:
+                self.end = False
+                return text + cst[4]
+            return text
+        return text
+
+    def getvalue(self):
+        """
+        Returns the whole stream content.
+        """
+        def byline():
+            line = self.readline()
+            while line:
+                yield line
+                line = self.readline()
+        return "".join(byline())
+
+
+def flatten_dictionary(dico, sep="_"):
+    """
+    Flattens a dictionary with nested structure to a dictionary with no
+    hierarchy.
+
+    :param dico: dictionary to flatten
+    :param sep: string to separate dictionary keys by
+    :return: flattened dictionary
+
+    Inspired from `flatten_json
+    <https://github.com/amirziai/flatten/blob/master/flatten_json.py>`_.
+    """
+    flattened_dict = {}
+
+    def _flatten(obj, key):
+        if obj is None:
+            flattened_dict[key] = obj
+        elif isinstance(obj, dict):
+            for k, v in obj.items():
+                if not isinstance(k, str):
+                    raise TypeError(
+                        "All keys must a string.")  # pragma: no cover
+                k2 = k if key is None else f"{key}{sep}{k}"
+                _flatten(v, k2)
+        elif isinstance(obj, (list, set)):
+            for index, item in enumerate(obj):
+                k2 = k if key is None else f"{key}{sep}{index}"
+                _flatten(item, k2)
+        else:
+            flattened_dict[key] = obj
+
+    _flatten(dico, None)
+    return flattened_dict
+
+
+def enumerate_json_items(filename, encoding=None, lines=False, flatten=False, fLOG=None):
+    """
+    Enumerates items from a :epkg:`JSON` file or string.
+
+    :param filename: filename or string or stream to parse
+    :param encoding: encoding
+    :param lines: one record per row
+    :param flatten: call @see fn flatten_dictionary
+    :param fLOG: logging function
+    :return: iterator on records at first level.
+
+    It assumes the syntax follows the format: ``[ {"id":1, ...}, {"id": 2, ...}, ...]``.
+    However, if option *lines* if true, the function considers that the
+    stream or file does have one record per row as follows:
+
+        {"id":1, ...}
+        {"id": 2, ...}
+
+    .. exref::
+        :title: Processes a json file by streaming.
+
+        The module :epkg:`ijson` can read a :epkg:`JSON` file by streaming.
+        This module is needed because a record can be written on multiple lines.
+        This function leverages it produces the following results.
+
+        .. runpython::
+            :showcode:
+
+            from pandas_streaming.df.dataframe_io_helpers import enumerate_json_items
+
+            text_json = b'''
+                [
+                {
+                    "glossary": {
+                        "title": "example glossary",
+                        "GlossDiv": {
+                            "title": "S",
+                            "GlossList": [{
+                                "GlossEntry": {
+                                    "ID": "SGML",
+                                    "SortAs": "SGML",
+                                    "GlossTerm": "Standard Generalized Markup Language",
+                                    "Acronym": "SGML",
+                                    "Abbrev": "ISO 8879:1986",
+                                    "GlossDef": {
+                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
+                                        "GlossSeeAlso": ["GML", "XML"]
+                                    },
+                                    "GlossSee": "markup"
+                                }
+                            }]
+                        }
+                    }
+                },
+                {
+                    "glossary": {
+                        "title": "example glossary",
+                        "GlossDiv": {
+                            "title": "S",
+                            "GlossList": {
+                                "GlossEntry": [{
+                                    "ID": "SGML",
+                                    "SortAs": "SGML",
+                                    "GlossTerm": "Standard Generalized Markup Language",
+                                    "Acronym": "SGML",
+                                    "Abbrev": "ISO 8879:1986",
+                                    "GlossDef": {
+                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
+                                        "GlossSeeAlso": ["GML", "XML"]
+                                    },
+                                    "GlossSee": "markup"
+                                }]
+                            }
+                        }
+                    }
+                }
+                ]
+            '''
+
+            for item in enumerate_json_items(text_json):
+                print(item)
+
+    The parsed json must have an empty line at the end otherwise
+    the following exception is raised:
+    `ijson.common.IncompleteJSONError: `
+    `parse error: unallowed token at this point in JSON text`.
+    """
+    if isinstance(filename, str):
+        if "{" not in filename and os.path.exists(filename):
+            with open(filename, "r", encoding=encoding) as f:
+                for el in enumerate_json_items(
+                        f, encoding=encoding, lines=lines,
+                        flatten=flatten, fLOG=fLOG):
+                    yield el
+        else:
+            st = StringIO(filename)
+            for el in enumerate_json_items(
+                    st, encoding=encoding, lines=lines,
+                    flatten=flatten, fLOG=fLOG):
+                yield el
+    elif isinstance(filename, bytes):
+        st = BytesIO(filename)
+        for el in enumerate_json_items(
+                st, encoding=encoding, lines=lines, flatten=flatten,
+                fLOG=fLOG):
+            yield el
+    elif lines:
+        for el in enumerate_json_items(
+                JsonPerRowsStream(filename),
+                encoding=encoding, lines=False, flatten=flatten, fLOG=fLOG):
+            yield el
+    else:
+        if hasattr(filename, 'seek'):
+            filename.seek(0)
+        parser = ijson.parse(filename)
+        current = None
+        curkey = None
+        stack = []
+        nbyield = 0
+        for i, (_, event, value) in enumerate(parser):
+            if i % 1000000 == 0 and fLOG is not None:
+                fLOG(  # pragma: no cover
+                    f"[enumerate_json_items] i={i} yielded={nbyield}")
+            if event == "start_array":
+                if curkey is None:
+                    current = []
+                else:
+                    if not isinstance(current, dict):
+                        raise RuntimeError(  # pragma: no cover
+                            f"Type issue {type(current)}")
+                    c = []
+                    current[curkey] = c  # pylint: disable=E1137
+                    current = c
+                curkey = None
+                stack.append(current)
+            elif event == "end_array":
+                stack.pop()
+                if len(stack) == 0:
+                    # We should be done.
+                    current = None
+                else:
+                    current = stack[-1]
+            elif event == "start_map":
+                c = {}
+                if curkey is None:
+                    if current is None:
+                        current = []
+                    current.append(c)
+                else:
+                    current[curkey] = c  # pylint: disable=E1137
+                stack.append(c)
+                current = c
+                curkey = None
+            elif event == "end_map":
+                stack.pop()
+                current = stack[-1]
+                if len(stack) == 1:
+                    nbyield += 1
+                    if flatten:
+                        yield flatten_dictionary(current[-1])
+                    else:
+                        yield current[-1]
+                    # We clear the memory.
+                    current.clear()
+            elif event == "map_key":
+                curkey = value
+            elif event in {"string", "number", "boolean"}:
+                if curkey is None:
+                    current.append(value)
+                else:
+                    current[curkey] = value  # pylint: disable=E1137
+                    curkey = None
+            elif event == "null":
+                if curkey is None:
+                    current.append(None)
+                else:
+                    current[curkey] = None  # pylint: disable=E1137
+                    curkey = None
+            else:
+                raise ValueError(
+                    f"Unknown event '{event}'")  # pragma: no cover
+
+
+class JsonIterator2Stream:
+    """
+    Transforms an iterator on :epkg:`JSON` items
+    into a stream which returns an items as a string every time
+    method *read* is called.
+    The iterator could be one returned by @see fn enumerate_json_items.
+
+    :param it: iterator
+    :param kwargs: arguments to :epkg:`*py:json:dumps`
+
+    .. exref::
+        :title: Reshape a json file
+
+        The function @see fn enumerate_json_items reads any
+        :epkg:`json` even if every record is split over
+        multiple lines. Class @see cl JsonIterator2Stream
+        mocks this iterator as a stream. Each row is a single item.
+
+        .. runpython::
+            :showcode:
+
+            from pandas_streaming.df.dataframe_io_helpers import enumerate_json_items, JsonIterator2Stream
+
+            text_json = b'''
+                [
+                {
+                    "glossary": {
+                        "title": "example glossary",
+                        "GlossDiv": {
+                            "title": "S",
+                            "GlossList": [{
+                                "GlossEntry": {
+                                    "ID": "SGML",
+                                    "SortAs": "SGML",
+                                    "GlossTerm": "Standard Generalized Markup Language",
+                                    "Acronym": "SGML",
+                                    "Abbrev": "ISO 8879:1986",
+                                    "GlossDef": {
+                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
+                                        "GlossSeeAlso": ["GML", "XML"]
+                                    },
+                                    "GlossSee": "markup"
+                                }
+                            }]
+                        }
+                    }
+                },
+                {
+                    "glossary": {
+                        "title": "example glossary",
+                        "GlossDiv": {
+                            "title": "S",
+                            "GlossList": {
+                                "GlossEntry": [{
+                                    "ID": "SGML",
+                                    "SortAs": "SGML",
+                                    "GlossTerm": "Standard Generalized Markup Language",
+                                    "Acronym": "SGML",
+                                    "Abbrev": "ISO 8879:1986",
+                                    "GlossDef": {
+                                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
+                                        "GlossSeeAlso": ["GML", "XML"]
+                                    },
+                                    "GlossSee": "markup"
+                                }]
+                            }
+                        }
+                    }
+                }
+                ]
+            '''
+
+            for item in JsonIterator2Stream(lambda: enumerate_json_items(text_json)):
+                print(item)
+
+    .. versionchanged:: 0.3
+        The class takes a function which outputs an iterator and not an iterator.
+        `JsonIterator2Stream(enumerate_json_items(text_json))` needs to be rewritten
+        into JsonIterator2Stream(lambda: enumerate_json_items(text_json)).
+    """
+
+    def __init__(self, it, **kwargs):
+        self.it = it
+        self.kwargs = kwargs
+        self.it0 = it()
+
+    def seek(self, offset):
+        """
+        Change the stream position to the given byte offset.
+
+        :param offset: offset, only 0 is implemented
+        """
+        if offset != 0:
+            raise NotImplementedError(
+                "The iterator can only return at the beginning.")
+        self.it0 = self.it()
+
+    def write(self):
+        """
+        The class does not write.
+        """
+        raise NotImplementedError()
+
+    def read(self):
+        """
+        Reads the next item and returns it as a string.
+        """
+        try:
+            value = next(self.it0)
+            return dumps(value, **self.kwargs)
+        except StopIteration:
+            return None
+
+    def __iter__(self):
+        """
+        Iterates on each row. The behaviour is a bit tricky.
+        It is implemented to be swalled by :func:`pandas.read_json` which
+        uses :func:`itertools.islice` to go through the items.
+        It calls multiple times `__iter__` but does expect the
+        iterator to continue from where it stopped last time.
+        """
+        for value in self.it0:
+            yield dumps(value, **self.kwargs)
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/df/dataframe_split.py` & `pandas_streaming-0.3.239/pandas_streaming/df/dataframe_split.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-# -*- coding: utf-8 -*-
-"""
-@file
-@brief Implements different methods to split a dataframe.
-"""
-import hashlib
-import pickle
-import random
-import warnings
-from io import StringIO
-import pandas
-
-
-def sklearn_train_test_split(self, path_or_buf=None, export_method="to_csv",
-                             names=None, **kwargs):
-    """
-    Randomly splits a dataframe into smaller pieces.
-    The function returns streams of file names.
-    The function relies on :epkg:`sklearn:model_selection:train_test_split`.
-    It does not handle stratified version of it.
-
-    @param  self            @see cl StreamingDataFrame
-    @param  path_or_buf     a string, a list of strings or buffers, if it is a
-                            string, it must contain ``{}`` like ``partition{}.txt``
-    @param  export_method   method used to store the partitions, by default
-                            :epkg:`pandas:DataFrame:to_csv`
-    @param  names           partitions names, by default ``('train', 'test')``
-    @param  kwargs          parameters for the export function and
-                            :epkg:`sklearn:model_selection:train_test_split`.
-    @return                 outputs of the exports functions
-
-    The function cannot return two iterators or two
-    @see cl StreamingDataFrame because running through one
-    means running through the other. We can assume both
-    splits do not hold in memory and we cannot run through
-    the same iterator again as random draws would be different.
-    We need to store the results into files or buffers.
-
-    .. warning::
-        The method *export_method* must write the data in
-        mode *append* and allows stream.
-    """
-    if kwargs.get("stratify") is not None:
-        raise NotImplementedError(
-            "No implementation yet for the stratified version.")
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=ImportWarning)
-        from sklearn.model_selection import train_test_split  # pylint: disable=C0415
-
-    opts = ['test_size', 'train_size',
-            'random_state', 'shuffle', 'stratify']
-    split_ops = {}
-    for o in opts:
-        if o in kwargs:
-            split_ops[o] = kwargs[o]
-            del kwargs[o]
-
-    exportf_ = getattr(pandas.DataFrame, export_method)
-    if export_method == 'to_csv' and 'mode' not in kwargs:
-        exportf = lambda *a, **kw: exportf_(*a, mode='a', **kw)
-    else:
-        exportf = exportf_
-
-    if isinstance(path_or_buf, str):
-        if "{}" not in path_or_buf:
-            raise ValueError(
-                "path_or_buf must contain {} to insert the partition name")
-        if names is None:
-            names = ['train', 'test']
-        elif len(names) != len(path_or_buf):
-            raise ValueError(  # pragma: no cover
-                'names and path_or_buf must have the same length')
-        path_or_buf = [path_or_buf.format(n) for n in names]
-    elif path_or_buf is None:
-        path_or_buf = [None, None]
-    else:
-        if not isinstance(path_or_buf, list):
-            raise TypeError(  # pragma: no cover
-                'path_or_buf must be a list or a string')
-
-    bufs = []
-    close = []
-    for p in path_or_buf:
-        if p is None:
-            st = StringIO()
-            cl = False
-        elif isinstance(p, str):
-            st = open(  # pylint: disable=R1732
-                p, "w", encoding=kwargs.get('encoding'))
-            cl = True
-        else:
-            st = p
-            cl = False
-        bufs.append(st)
-        close.append(cl)
-
-    for df in self:
-        train, test = train_test_split(df, **split_ops)
-        exportf(train, bufs[0], **kwargs)
-        exportf(test, bufs[1], **kwargs)
-        kwargs['header'] = False
-
-    for b, c in zip(bufs, close):
-        if c:
-            b.close()
-    return [st.getvalue() if isinstance(st, StringIO) else p
-            for st, p in zip(bufs, path_or_buf)]
-
-
-def sklearn_train_test_split_streaming(self, test_size=0.25, train_size=None,
-                                       stratify=None, hash_size=9, unique_rows=False):
-    """
-    Randomly splits a dataframe into smaller pieces.
-    The function returns streams of file names.
-    The function relies on :epkg:`sklearn:model_selection:train_test_split`.
-    It handles the stratified version of it.
-
-    @param  self            @see cl StreamingDataFrame
-    @param  test_size       ratio for the test partition (if *train_size* is not specified)
-    @param  train_size      ratio for the train partition
-    @param  stratify        column holding the stratification
-    @param  hash_size       size of the hash to cache information about partition
-    @param  unique_rows     ensures that rows are unique
-    @return                 Two @see cl StreamingDataFrame, one
-                            for train, one for test.
-
-    The function returns two iterators or two
-    @see cl StreamingDataFrame. It
-    tries to do everything without writing anything on disk
-    but it requires to store the repartition somehow.
-    This function hashes every row and maps the hash with a part
-    (train or test). This cache must hold in memory otherwise the
-    function fails. The two returned iterators must not be used
-    for the first time in the same time. The first time is used to
-    build the cache. The function changes the order of rows if
-    the parameter *stratify* is not null. The cache has a side effect:
-    every exact same row will be put in the same partition.
-    If that is not what you want, you should add an index column
-    or a random one.
-    """
-    p = (1 - test_size) if test_size else None
-    if train_size is not None:
-        p = train_size
-    n = 2 * max(1 / p, 1 / (1 - p))  # changement
-
-    static_schema = []
-
-    def iterator_rows():
-        "iterates on rows"
-        counts = {}
-        memory = {}
-        pos_col = None
-        for df in self:
-            if pos_col is None:
-                static_schema.append(list(df.columns))
-                static_schema.append(list(df.dtypes))
-                static_schema.append(df.shape[0])
-                if stratify is not None:
-                    pos_col = list(df.columns).index(stratify)
-                else:
-                    pos_col = -1
-
-            for obs in df.itertuples(index=False, name=None):
-                strat = 0 if stratify is None else obs[pos_col]
-                if strat not in memory:
-                    memory[strat] = []
-                memory[strat].append(obs)
-
-                for k, v in memory.items():
-                    if len(v) >= n + random.randint(0, 10):  # changement
-                        vr = list(range(len(v)))
-                        # on permute aléatoirement
-                        random.shuffle(vr)
-                        if (0, k) in counts:
-                            tt = counts[1, k] + counts[0, k]
-                            delta = - int(counts[0, k] - tt * p + 0.5)
-                        else:
-                            delta = 0
-                        i = int(len(v) * p + 0.5)
-                        i += delta
-                        i = max(0, min(len(v), i))
-                        one = set(vr[:i])
-                        for d, obs_ in enumerate(v):
-                            yield obs_, 0 if d in one else 1
-                        if (0, k) not in counts:
-                            counts[0, k] = i
-                            counts[1, k] = len(v) - i
-                        else:
-                            counts[0, k] += i
-                            counts[1, k] += len(v) - i
-                        # on efface de la mémoire les informations produites
-                        v.clear()
-
-        # Lorsqu'on a fini, il faut tout de même répartir les
-        # observations stockées.
-        for k, v in memory.items():
-            vr = list(range(len(v)))
-            # on permute aléatoirement
-            random.shuffle(vr)
-            if (0, k) in counts:
-                tt = counts[1, k] + counts[0, k]
-                delta = - int(counts[0, k] - tt * p + 0.5)
-            else:
-                delta = 0
-            i = int(len(v) * p + 0.5)
-            i += delta
-            i = max(0, min(len(v), i))
-            one = set(vr[:i])
-            for d, obs in enumerate(v):
-                yield obs, 0 if d in one else 1
-            if (0, k) not in counts:
-                counts[0, k] = i
-                counts[1, k] = len(v) - i
-            else:
-                counts[0, k] += i
-                counts[1, k] += len(v) - i
-
-    def h11(w):
-        "pickle and hash"
-        b = pickle.dumps(w)
-        return hashlib.md5(b).hexdigest()[:hash_size]
-
-    # We store the repartition in a cache.
-    cache = {}
-
-    def iterator_internal(part_requested):
-        "internal iterator on dataframes"
-        iy = 0
-        accumul = []
-        if len(cache) == 0:
-            for obs, part in iterator_rows():
-                h = h11(obs)
-                if unique_rows and h in cache:
-                    raise ValueError(  # pragma: no cover
-                        "A row or at least its hash is already cached. "
-                        "Increase hash_size or check for duplicates "
-                        "('{0}')\n{1}.".format(h, obs))
-                if h not in cache:
-                    cache[h] = part
-                else:
-                    part = cache[h]
-                if part == part_requested:
-                    accumul.append(obs)
-                    if len(accumul) >= static_schema[2]:
-                        dfo = pandas.DataFrame(
-                            accumul, columns=static_schema[0])
-                        self.ensure_dtype(dfo, static_schema[1])
-                        iy += dfo.shape[0]
-                        accumul.clear()
-                        yield dfo
-        else:
-            for df in self:
-                for obs in df.itertuples(index=False, name=None):
-                    h = h11(obs)
-                    part = cache.get(h)
-                    if part is None:
-                        raise ValueError(  # pragma: no cover
-                            "Second iteration. A row was never met in the first one\n{0}".format(obs))
-                    if part == part_requested:
-                        accumul.append(obs)
-                        if len(accumul) >= static_schema[2]:
-                            dfo = pandas.DataFrame(
-                                accumul, columns=static_schema[0])
-                            self.ensure_dtype(dfo, static_schema[1])
-                            iy += dfo.shape[0]
-                            accumul.clear()
-                            yield dfo
-        if len(accumul) > 0:
-            dfo = pandas.DataFrame(accumul, columns=static_schema[0])
-            self.ensure_dtype(dfo, static_schema[1])
-            iy += dfo.shape[0]
-            yield dfo
-
-    return (self.__class__(lambda: iterator_internal(0)),
-            self.__class__(lambda: iterator_internal(1)))
+# -*- coding: utf-8 -*-
+"""
+@file
+@brief Implements different methods to split a dataframe.
+"""
+import hashlib
+import pickle
+import random
+import warnings
+from io import StringIO
+import pandas
+
+
+def sklearn_train_test_split(self, path_or_buf=None, export_method="to_csv",
+                             names=None, **kwargs):
+    """
+    Randomly splits a dataframe into smaller pieces.
+    The function returns streams of file names.
+    The function relies on :epkg:`sklearn:model_selection:train_test_split`.
+    It does not handle stratified version of it.
+
+    @param  self            @see cl StreamingDataFrame
+    @param  path_or_buf     a string, a list of strings or buffers, if it is a
+                            string, it must contain ``{}`` like ``partition{}.txt``
+    @param  export_method   method used to store the partitions, by default
+                            :epkg:`pandas:DataFrame:to_csv`
+    @param  names           partitions names, by default ``('train', 'test')``
+    @param  kwargs          parameters for the export function and
+                            :epkg:`sklearn:model_selection:train_test_split`.
+    @return                 outputs of the exports functions
+
+    The function cannot return two iterators or two
+    @see cl StreamingDataFrame because running through one
+    means running through the other. We can assume both
+    splits do not hold in memory and we cannot run through
+    the same iterator again as random draws would be different.
+    We need to store the results into files or buffers.
+
+    .. warning::
+        The method *export_method* must write the data in
+        mode *append* and allows stream.
+    """
+    if kwargs.get("stratify") is not None:
+        raise NotImplementedError(  # pragma: no cover
+            "No implementation yet for the stratified version.")
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=ImportWarning)
+        from sklearn.model_selection import train_test_split  # pylint: disable=C0415
+
+    opts = ['test_size', 'train_size',
+            'random_state', 'shuffle', 'stratify']
+    split_ops = {}
+    for o in opts:
+        if o in kwargs:
+            split_ops[o] = kwargs[o]
+            del kwargs[o]
+
+    exportf_ = getattr(pandas.DataFrame, export_method)
+    if export_method == 'to_csv' and 'mode' not in kwargs:
+        exportf = lambda *a, **kw: exportf_(*a, mode='a', **kw)
+    else:
+        exportf = exportf_
+
+    if isinstance(path_or_buf, str):
+        if "{}" not in path_or_buf:
+            raise ValueError(
+                "path_or_buf must contain {} to insert the partition name")
+        if names is None:
+            names = ['train', 'test']
+        elif len(names) != len(path_or_buf):
+            raise ValueError(  # pragma: no cover
+                'names and path_or_buf must have the same length')
+        path_or_buf = [path_or_buf.format(n) for n in names]
+    elif path_or_buf is None:
+        path_or_buf = [None, None]
+    else:
+        if not isinstance(path_or_buf, list):
+            raise TypeError(  # pragma: no cover
+                'path_or_buf must be a list or a string')
+
+    bufs = []
+    close = []
+    for p in path_or_buf:
+        if p is None:
+            st = StringIO()
+            cl = False
+        elif isinstance(p, str):
+            st = open(  # pylint: disable=R1732
+                p, "w", encoding=kwargs.get('encoding'))
+            cl = True
+        else:
+            st = p
+            cl = False
+        bufs.append(st)
+        close.append(cl)
+
+    for df in self:
+        train, test = train_test_split(df, **split_ops)
+        exportf(train, bufs[0], **kwargs)
+        exportf(test, bufs[1], **kwargs)
+        kwargs['header'] = False
+
+    for b, c in zip(bufs, close):
+        if c:
+            b.close()
+    return [st.getvalue() if isinstance(st, StringIO) else p
+            for st, p in zip(bufs, path_or_buf)]
+
+
+def sklearn_train_test_split_streaming(self, test_size=0.25, train_size=None,
+                                       stratify=None, hash_size=9, unique_rows=False):
+    """
+    Randomly splits a dataframe into smaller pieces.
+    The function returns streams of file names.
+    The function relies on :epkg:`sklearn:model_selection:train_test_split`.
+    It handles the stratified version of it.
+
+    @param  self            @see cl StreamingDataFrame
+    @param  test_size       ratio for the test partition (if *train_size* is not specified)
+    @param  train_size      ratio for the train partition
+    @param  stratify        column holding the stratification
+    @param  hash_size       size of the hash to cache information about partition
+    @param  unique_rows     ensures that rows are unique
+    @return                 Two @see cl StreamingDataFrame, one
+                            for train, one for test.
+
+    The function returns two iterators or two
+    @see cl StreamingDataFrame. It
+    tries to do everything without writing anything on disk
+    but it requires to store the repartition somehow.
+    This function hashes every row and maps the hash with a part
+    (train or test). This cache must hold in memory otherwise the
+    function fails. The two returned iterators must not be used
+    for the first time in the same time. The first time is used to
+    build the cache. The function changes the order of rows if
+    the parameter *stratify* is not null. The cache has a side effect:
+    every exact same row will be put in the same partition.
+    If that is not what you want, you should add an index column
+    or a random one.
+    """
+    p = (1 - test_size) if test_size else None
+    if train_size is not None:
+        p = train_size
+    n = 2 * max(1 / p, 1 / (1 - p))  # changement
+
+    static_schema = []
+
+    def iterator_rows():
+        "iterates on rows"
+        counts = {}
+        memory = {}
+        pos_col = None
+        for df in self:
+            if pos_col is None:
+                static_schema.append(list(df.columns))
+                static_schema.append(list(df.dtypes))
+                static_schema.append(df.shape[0])
+                if stratify is not None:
+                    pos_col = list(df.columns).index(stratify)
+                else:
+                    pos_col = -1
+
+            for obs in df.itertuples(index=False, name=None):
+                strat = 0 if stratify is None else obs[pos_col]
+                if strat not in memory:
+                    memory[strat] = []
+                memory[strat].append(obs)
+
+                for k, v in memory.items():
+                    if len(v) >= n + random.randint(0, 10):  # changement
+                        vr = list(range(len(v)))
+                        # on permute aléatoirement
+                        random.shuffle(vr)
+                        if (0, k) in counts:
+                            tt = counts[1, k] + counts[0, k]
+                            delta = - int(counts[0, k] - tt * p + 0.5)
+                        else:
+                            delta = 0
+                        i = int(len(v) * p + 0.5)
+                        i += delta
+                        i = max(0, min(len(v), i))
+                        one = set(vr[:i])
+                        for d, obs_ in enumerate(v):
+                            yield obs_, 0 if d in one else 1
+                        if (0, k) not in counts:
+                            counts[0, k] = i
+                            counts[1, k] = len(v) - i
+                        else:
+                            counts[0, k] += i
+                            counts[1, k] += len(v) - i
+                        # on efface de la mémoire les informations produites
+                        v.clear()
+
+        # Lorsqu'on a fini, il faut tout de même répartir les
+        # observations stockées.
+        for k, v in memory.items():
+            vr = list(range(len(v)))
+            # on permute aléatoirement
+            random.shuffle(vr)
+            if (0, k) in counts:
+                tt = counts[1, k] + counts[0, k]
+                delta = - int(counts[0, k] - tt * p + 0.5)
+            else:
+                delta = 0
+            i = int(len(v) * p + 0.5)
+            i += delta
+            i = max(0, min(len(v), i))
+            one = set(vr[:i])
+            for d, obs in enumerate(v):
+                yield obs, 0 if d in one else 1
+            if (0, k) not in counts:
+                counts[0, k] = i
+                counts[1, k] = len(v) - i
+            else:
+                counts[0, k] += i
+                counts[1, k] += len(v) - i
+
+    def h11(w):
+        "pickle and hash"
+        b = pickle.dumps(w)
+        return hashlib.md5(b).hexdigest()[:hash_size]
+
+    # We store the repartition in a cache.
+    cache = {}
+
+    def iterator_internal(part_requested):
+        "internal iterator on dataframes"
+        iy = 0
+        accumul = []
+        if len(cache) == 0:
+            for obs, part in iterator_rows():
+                h = h11(obs)
+                if unique_rows and h in cache:
+                    raise ValueError(  # pragma: no cover
+                        "A row or at least its hash is already cached. "
+                        "Increase hash_size or check for duplicates "
+                        "('{0}')\n{1}.".format(h, obs))
+                if h not in cache:
+                    cache[h] = part
+                else:
+                    part = cache[h]
+                if part == part_requested:
+                    accumul.append(obs)
+                    if len(accumul) >= static_schema[2]:
+                        dfo = pandas.DataFrame(
+                            accumul, columns=static_schema[0])
+                        self.ensure_dtype(dfo, static_schema[1])
+                        iy += dfo.shape[0]
+                        accumul.clear()
+                        yield dfo
+        else:
+            for df in self:
+                for obs in df.itertuples(index=False, name=None):
+                    h = h11(obs)
+                    part = cache.get(h)
+                    if part is None:
+                        raise ValueError(  # pragma: no cover
+                            f"Second iteration. A row was never met in the first one\n{obs}")
+                    if part == part_requested:
+                        accumul.append(obs)
+                        if len(accumul) >= static_schema[2]:
+                            dfo = pandas.DataFrame(
+                                accumul, columns=static_schema[0])
+                            self.ensure_dtype(dfo, static_schema[1])
+                            iy += dfo.shape[0]
+                            accumul.clear()
+                            yield dfo
+        if len(accumul) > 0:
+            dfo = pandas.DataFrame(accumul, columns=static_schema[0])
+            self.ensure_dtype(dfo, static_schema[1])
+            iy += dfo.shape[0]
+            yield dfo
+
+    return (self.__class__(lambda: iterator_internal(0)),
+            self.__class__(lambda: iterator_internal(1)))
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming/exc/exc_streaming.py` & `pandas_streaming-0.3.239/pandas_streaming/exc/exc_streaming.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,8 +15,8 @@
         """
         This method is inefficient in streaming mode
         and not implemented.
 
         :param meth: inefficient method
         """
         Exception.__init__(
-            self, "{0} should not be done in streaming mode.".format(meth))
+            self, f"{meth} should not be done in streaming mode.")
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming.egg-info/PKG-INFO` & `pandas_streaming-0.3.239/pandas_streaming.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,116 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pandas-streaming
-Version: 0.3.218
+Version: 0.3.239
 Summary: Streaming operations with pandas.
 Home-page: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html
+Download-URL: https://github.com/sdpython/pandas_streaming/
 Author: Xavier Dupré
 Author-email: xavier.dupre@gmail.com
 License: MIT
-Download-URL: https://github.com/sdpython/pandas_streaming/
-Description: 
-        .. image:: https://github.com/sdpython/pandas_streaming/blob/master/_doc/sphinxdoc/source/phdoc_static/project_ico.png?raw=true
-            :target: https://github.com/sdpython/pandas_streaming/
-        
-        .. _l-README:
-        
-        pandas_streaming: streaming API over pandas
-        ===========================================
-        
-        .. image:: https://travis-ci.com/sdpython/pandas_streaming.svg?branch=master
-            :target: https://app.travis-ci.com/github/sdpython/pandas_streaming
-            :alt: Build status
-        
-        .. image:: https://ci.appveyor.com/api/projects/status/4te066r8ne1ymmhy?svg=true
-            :target: https://ci.appveyor.com/project/sdpython/pandas-streaming
-            :alt: Build Status Windows
-        
-        .. image:: https://circleci.com/gh/sdpython/pandas_streaming/tree/master.svg?style=svg
-            :target: https://circleci.com/gh/sdpython/pandas_streaming/tree/master
-        
-        .. image:: https://dev.azure.com/xavierdupre3/pandas_streaming/_apis/build/status/sdpython.pandas_streaming
-            :target: https://dev.azure.com/xavierdupre3/pandas_streaming/
-        
-        .. image:: https://badge.fury.io/py/pandas_streaming.svg
-            :target: http://badge.fury.io/py/pandas_streaming
-        
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :alt: MIT License
-            :target: http://opensource.org/licenses/MIT
-        
-        .. image:: https://codecov.io/github/sdpython/pandas_streaming/coverage.svg?branch=master
-            :target: https://codecov.io/github/sdpython/pandas_streaming?branch=master
-        
-        .. image:: http://img.shields.io/github/issues/sdpython/pandas_streaming.png
-            :alt: GitHub Issues
-            :target: https://github.com/sdpython/pandas_streaming/issues
-        
-        .. image:: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/_images/nbcov.png
-            :target: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/all_notebooks_coverage.html
-            :alt: Notebook Coverage
-        
-        .. image:: https://api.codacy.com/project/badge/Grade/f53b7f4d6a0447aa9ce0c4ad5df659ef
-            :target: https://www.codacy.com/app/sdpython/pandas_streaming?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=sdpython/pandas_streaming&amp;utm_campaign=Badge_Grade
-        
-        .. image:: https://pepy.tech/badge/pandas_streaming/month
-            :target: https://pepy.tech/project/pandas_streaming/month
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/github/forks/sdpython/pandas_streaming.svg
-            :target: https://github.com/sdpython/pandas_streaming/
-            :alt: Forks
-        
-        .. image:: https://img.shields.io/github/stars/sdpython/pandas_streaming.svg
-            :target: https://github.com/sdpython/pandas_streaming/
-            :alt: Stars
-        
-        .. image:: https://img.shields.io/github/repo-size/sdpython/pandas_streaming
-            :target: https://github.com/sdpython/pandas_streaming/
-            :alt: size
-        
-        `pandas_streaming <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
-        aims at processing big files with `pandas <http://pandas.pydata.org/>`_,
-        too big to hold in memory, too small to be parallelized with a significant gain.
-        The module replicates a subset of `pandas <http://pandas.pydata.org/>`_ API
-        and implements other functionalities for machine learning.
-        
-        ::
-        
-            from pandas_streaming.df import StreamingDataFrame
-            sdf = StreamingDataFrame.read_csv("filename", sep="\t", encoding="utf-8")
-        
-            for df in sdf:
-                # process this chunk of data
-                # df is a dataframe
-                print(df)
-        
-        The module can also stream an existing dataframe.
-        
-        ::
-        
-            import pandas
-            df = pandas.DataFrame([dict(cf=0, cint=0, cstr="0"),
-                                   dict(cf=1, cint=1, cstr="1"),
-                                   dict(cf=3, cint=3, cstr="3")])
-        
-            from pandas_streaming.df import StreamingDataFrame
-            sdf = StreamingDataFrame.read_df(df)
-        
-            for df in sdf:
-                # process this chunk of data
-                # df is a dataframe
-                print(df)
-        
-        It contains other helpers to split datasets into
-        train and test with some weird constraints.
-        
-        **Links:**
-        
-        * `GitHub/pandas_streaming <https://github.com/sdpython/pandas_streaming/>`_
-        * `documentation <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
-        * `Blog <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/blog/main_0000.html#ap-main-0>`_
-        
-Keywords: pandas_streaming,Xavier Dupré
-Platform: UNKNOWN
+Keywords: pandas_streaming,Xavier Dupré,pandas,streaming
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
+License-File: LICENSE.txt
+
+
+.. image:: https://github.com/sdpython/pandas_streaming/blob/master/_doc/sphinxdoc/source/_static/project_ico.png?raw=true
+    :target: https://github.com/sdpython/pandas_streaming/
+
+.. _l-README:
+
+pandas_streaming: streaming API over pandas
+===========================================
+
+.. image:: https://travis-ci.com/sdpython/pandas_streaming.svg?branch=master
+    :target: https://app.travis-ci.com/github/sdpython/pandas_streaming
+    :alt: Build status
+
+.. image:: https://ci.appveyor.com/api/projects/status/4te066r8ne1ymmhy?svg=true
+    :target: https://ci.appveyor.com/project/sdpython/pandas-streaming
+    :alt: Build Status Windows
+
+.. image:: https://circleci.com/gh/sdpython/pandas_streaming/tree/master.svg?style=svg
+    :target: https://circleci.com/gh/sdpython/pandas_streaming/tree/master
+
+.. image:: https://dev.azure.com/xavierdupre3/pandas_streaming/_apis/build/status/sdpython.pandas_streaming
+    :target: https://dev.azure.com/xavierdupre3/pandas_streaming/
+
+.. image:: https://badge.fury.io/py/pandas_streaming.svg
+    :target: http://badge.fury.io/py/pandas_streaming
+
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :alt: MIT License
+    :target: http://opensource.org/licenses/MIT
+
+.. image:: https://codecov.io/github/sdpython/pandas_streaming/coverage.svg?branch=master
+    :target: https://codecov.io/github/sdpython/pandas_streaming?branch=master
+
+.. image:: http://img.shields.io/github/issues/sdpython/pandas_streaming.png
+    :alt: GitHub Issues
+    :target: https://github.com/sdpython/pandas_streaming/issues
+
+.. image:: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/_images/nbcov.png
+    :target: http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/all_notebooks_coverage.html
+    :alt: Notebook Coverage
+
+.. image:: https://pepy.tech/badge/pandas_streaming/month
+    :target: https://pepy.tech/project/pandas_streaming/month
+    :alt: Downloads
+
+.. image:: https://img.shields.io/github/forks/sdpython/pandas_streaming.svg
+    :target: https://github.com/sdpython/pandas_streaming/
+    :alt: Forks
+
+.. image:: https://img.shields.io/github/stars/sdpython/pandas_streaming.svg
+    :target: https://github.com/sdpython/pandas_streaming/
+    :alt: Stars
+
+.. image:: https://img.shields.io/github/repo-size/sdpython/pandas_streaming
+    :target: https://github.com/sdpython/pandas_streaming/
+    :alt: size
+
+`pandas_streaming <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
+aims at processing big files with `pandas <http://pandas.pydata.org/>`_,
+too big to hold in memory, too small to be parallelized with a significant gain.
+The module replicates a subset of `pandas <http://pandas.pydata.org/>`_ API
+and implements other functionalities for machine learning.
+
+::
+
+    from pandas_streaming.df import StreamingDataFrame
+    sdf = StreamingDataFrame.read_csv("filename", sep="\t", encoding="utf-8")
+
+    for df in sdf:
+        # process this chunk of data
+        # df is a dataframe
+        print(df)
+
+The module can also stream an existing dataframe.
+
+::
+
+    import pandas
+    df = pandas.DataFrame([dict(cf=0, cint=0, cstr="0"),
+                           dict(cf=1, cint=1, cstr="1"),
+                           dict(cf=3, cint=3, cstr="3")])
+
+    from pandas_streaming.df import StreamingDataFrame
+    sdf = StreamingDataFrame.read_df(df)
+
+    for df in sdf:
+        # process this chunk of data
+        # df is a dataframe
+        print(df)
+
+It contains other helpers to split datasets into
+train and test with some weird constraints.
+
+**Links:**
+
+* `GitHub/pandas_streaming <https://github.com/sdpython/pandas_streaming/>`_
+* `documentation <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/index.html>`_
+* `Blog <http://www.xavierdupre.fr/app/pandas_streaming/helpsphinx/blog/main_0000.html#ap-main-0>`_
```

### Comparing `pandas_streaming-0.3.218/pandas_streaming.egg-info/SOURCES.txt` & `pandas_streaming-0.3.239/pandas_streaming.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandas_streaming-0.3.218/setup.py` & `pandas_streaming-0.3.239/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from pyquicksetup import read_version, read_readme, default_cmdclass
 
 #########
 # settings
 #########
 
 project_var_name = "pandas_streaming"
-versionPython = "%s.%s" % (sys.version_info.major, sys.version_info.minor)
+versionPython = f"{sys.version_info.major}.{sys.version_info.minor}"
 path = "Lib/site-packages/" + project_var_name
 readme = 'README.rst'
 history = "HISTORY.rst"
 requirements = None
 
-KEYWORDS = project_var_name + ', Xavier Dupré'
+KEYWORDS = [project_var_name, 'Xavier Dupré', 'pandas', 'streaming']
 DESCRIPTION = """Streaming operations with pandas."""
 CLASSIFIERS = [
     'Programming Language :: Python :: 3',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering',
     'Topic :: Education',
     'License :: OSI Approved :: MIT License',
```

