# Comparing `tmp/streamlit_controllerDF-0.1.2.tar.gz` & `tmp/streamlit_controllerDF-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_controllerDF-0.1.2.tar", last modified: Fri Apr 28 19:04:18 2023, max compression
+gzip compressed data, was "streamlit_controllerDF-0.1.3.tar", last modified: Mon May  1 18:51:50 2023, max compression
```

## Comparing `streamlit_controllerDF-0.1.2.tar` & `streamlit_controllerDF-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 19:04:18.015235 streamlit_controllerDF-0.1.2/
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5463 2023-04-28 19:04:18.015235 streamlit_controllerDF-0.1.2/PKG-INFO
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     4332 2023-04-28 19:02:15.000000 streamlit_controllerDF-0.1.2/README.md
-drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 19:04:18.011902 streamlit_controllerDF-0.1.2/SCDF/
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       16 2023-04-24 18:44:49.000000 streamlit_controllerDF-0.1.2/SCDF/UnitTests.py
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       30 2023-04-24 18:44:49.000000 streamlit_controllerDF-0.1.2/SCDF/__init__.py
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     7227 2023-04-28 06:01:41.000000 streamlit_controllerDF-0.1.2/SCDF/streamlit_controllerDF.py
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       38 2023-04-28 19:04:18.015235 streamlit_controllerDF-0.1.2/setup.cfg
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     1759 2023-04-28 19:02:35.000000 streamlit_controllerDF-0.1.2/setup.py
-drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-04-28 19:04:18.015235 streamlit_controllerDF-0.1.2/streamlit_controllerDF.egg-info/
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5463 2023-04-28 19:04:17.000000 streamlit_controllerDF-0.1.2/streamlit_controllerDF.egg-info/PKG-INFO
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)      313 2023-04-28 19:04:17.000000 streamlit_controllerDF-0.1.2/streamlit_controllerDF.egg-info/SOURCES.txt
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)        1 2023-04-28 19:04:17.000000 streamlit_controllerDF-0.1.2/streamlit_controllerDF.egg-info/dependency_links.txt
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)       34 2023-04-28 19:04:17.000000 streamlit_controllerDF-0.1.2/streamlit_controllerDF.egg-info/requires.txt
--rw-r--r--   0 sunjet    (1000) sunjet    (1000)        5 2023-04-28 19:04:17.000000 streamlit_controllerDF-0.1.2/streamlit_controllerDF.egg-info/top_level.txt
+drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-05-01 18:51:50.611338 streamlit_controllerDF-0.1.3/
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5463 2023-05-01 18:51:50.608004 streamlit_controllerDF-0.1.3/PKG-INFO
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     4332 2023-04-28 19:02:15.000000 streamlit_controllerDF-0.1.3/README.md
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       38 2023-05-01 18:51:50.611338 streamlit_controllerDF-0.1.3/setup.cfg
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     1759 2023-05-01 18:51:31.000000 streamlit_controllerDF-0.1.3/setup.py
+drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-05-01 18:51:50.608004 streamlit_controllerDF-0.1.3/streamlit_controllerDF/
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       16 2023-04-24 18:44:49.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF/UnitTests.py
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       60 2023-05-01 18:48:03.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF/__init__.py
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     7227 2023-04-28 06:01:41.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF/streamlit_controllerDF.py
+drwxr-xr-x   0 sunjet    (1000) sunjet    (1000)        0 2023-05-01 18:51:50.608004 streamlit_controllerDF-0.1.3/streamlit_controllerDF.egg-info/
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)     5463 2023-05-01 18:51:50.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF.egg-info/PKG-INFO
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)      367 2023-05-01 18:51:50.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF.egg-info/SOURCES.txt
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)        1 2023-05-01 18:51:50.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF.egg-info/dependency_links.txt
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       34 2023-05-01 18:51:50.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF.egg-info/requires.txt
+-rw-r--r--   0 sunjet    (1000) sunjet    (1000)       23 2023-05-01 18:51:50.000000 streamlit_controllerDF-0.1.3/streamlit_controllerDF.egg-info/top_level.txt
```

### Comparing `streamlit_controllerDF-0.1.2/PKG-INFO` & `streamlit_controllerDF-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_controllerDF
-Version: 0.1.2
+Version: 0.1.3
 Summary: A solid base for controlling your data frame, getting quick metrics, and data visualizations using streamlit, pandas, numpy and matplotlib.
 Home-page: https://github.com/joshjetson/SCDF/
 Author: Joshua Dario
 Author-email: joshuajdr@gmail.com
 License: MIT
 Keywords: Python,streamlit,dataframe,data frame,data set,visualization,automatic,widgets,automation,machine learning,quick,controller,controllerdf,controllerDF,streamlit controller,streamlit data frame,streamlit controllerDF
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlit_controllerDF Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: streamlit_controllerDF Version: 0.1.3 Summary: A
 solid base for controlling your data frame, getting quick metrics, and data
 visualizations using streamlit, pandas, numpy and matplotlib. Home-page: https:
 //github.com/joshjetson/SCDF/ Author: Joshua Dario Author-email:
 joshuajdr@gmail.com License: MIT Keywords: Python,streamlit,dataframe,data
 frame,data set,visualization,automatic,widgets,automation,machine
 learning,quick,controller,controllerdf,controllerDF,streamlit
 controller,streamlit data frame,streamlit controllerDF Classifier: Intended
```

### Comparing `streamlit_controllerDF-0.1.2/README.md` & `streamlit_controllerDF-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_controllerDF-0.1.2/SCDF/streamlit_controllerDF.py` & `streamlit_controllerDF-0.1.3/streamlit_controllerDF/streamlit_controllerDF.py`

 * *Files identical despite different names*

### Comparing `streamlit_controllerDF-0.1.2/setup.py` & `streamlit_controllerDF-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="streamlit_controllerDF",
-    version="0.1.2",
+    version="0.1.3",
     description="A solid base for controlling your data frame, getting quick metrics, and data visualizations using streamlit, pandas, numpy and matplotlib.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/joshjetson/SCDF/",
     author="Joshua Dario",
     author_email="joshuajdr@gmail.com",
     license="MIT",
```

### Comparing `streamlit_controllerDF-0.1.2/streamlit_controllerDF.egg-info/PKG-INFO` & `streamlit_controllerDF-0.1.3/streamlit_controllerDF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-controllerDF
-Version: 0.1.2
+Version: 0.1.3
 Summary: A solid base for controlling your data frame, getting quick metrics, and data visualizations using streamlit, pandas, numpy and matplotlib.
 Home-page: https://github.com/joshjetson/SCDF/
 Author: Joshua Dario
 Author-email: joshuajdr@gmail.com
 License: MIT
 Keywords: Python,streamlit,dataframe,data frame,data set,visualization,automatic,widgets,automation,machine learning,quick,controller,controllerdf,controllerDF,streamlit controller,streamlit data frame,streamlit controllerDF
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlit-controllerDF Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: streamlit-controllerDF Version: 0.1.3 Summary: A
 solid base for controlling your data frame, getting quick metrics, and data
 visualizations using streamlit, pandas, numpy and matplotlib. Home-page: https:
 //github.com/joshjetson/SCDF/ Author: Joshua Dario Author-email:
 joshuajdr@gmail.com License: MIT Keywords: Python,streamlit,dataframe,data
 frame,data set,visualization,automatic,widgets,automation,machine
 learning,quick,controller,controllerdf,controllerDF,streamlit
 controller,streamlit data frame,streamlit controllerDF Classifier: Intended
```

