# Comparing `tmp/sarcgraph-0.1.0.tar.gz` & `tmp/sarcgraph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcgraph-0.1.0.tar", last modified: Fri Mar  3 23:17:23 2023, max compression
+gzip compressed data, was "sarcgraph-0.1.1.tar", last modified: Mon May  1 17:13:39 2023, max compression
```

## Comparing `sarcgraph-0.1.0.tar` & `sarcgraph-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 23:17:23.160000 sarcgraph-0.1.0/
--rw-rw-rw-   0        0        0     1088 2022-12-30 17:23:44.000000 sarcgraph-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    10474 2023-03-03 23:17:24.000000 sarcgraph-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9769 2023-03-03 22:50:10.000000 sarcgraph-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 23:17:23.170000 sarcgraph-0.1.0/sarcgraph/
--rw-rw-rw-   0        0        0        0 2023-02-19 08:05:22.000000 sarcgraph-0.1.0/sarcgraph/__init__.py
--rw-rw-rw-   0        0        0    38189 2023-03-03 07:27:34.000000 sarcgraph-0.1.0/sarcgraph/sg.py
--rw-rw-rw-   0        0        0    60155 2023-03-03 07:29:26.000000 sarcgraph-0.1.0/sarcgraph/sg_tools.py
-drwxrwxrwx   0        0        0        0 2023-03-03 23:17:23.180000 sarcgraph-0.1.0/sarcgraph.egg-info/
--rw-rw-rw-   0        0        0    10474 2023-03-03 23:17:24.000000 sarcgraph-0.1.0/sarcgraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-03-03 23:17:24.000000 sarcgraph-0.1.0/sarcgraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 23:17:24.000000 sarcgraph-0.1.0/sarcgraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-24 08:59:34.000000 sarcgraph-0.1.0/sarcgraph.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-03-03 23:17:24.000000 sarcgraph-0.1.0/sarcgraph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-03 23:17:24.000000 sarcgraph-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-03-03 23:17:10.000000 sarcgraph-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 17:13:39.210000 sarcgraph-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    10473 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9768 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 17:13:39.220000 sarcgraph-0.1.1/sarcgraph/
+-rw-rw-rw-   0        0        0        0 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/sarcgraph/__init__.py
+-rw-rw-rw-   0        0        0    38694 2023-04-27 23:54:10.000000 sarcgraph-0.1.1/sarcgraph/sg.py
+-rw-rw-rw-   0        0        0    60155 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/sarcgraph/sg_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 17:13:39.230000 sarcgraph-0.1.1/sarcgraph.egg-info/
+-rw-rw-rw-   0        0        0    10473 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 17:07:28.000000 sarcgraph-0.1.1/sarcgraph.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      149 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2023-05-01 17:10:10.000000 sarcgraph-0.1.1/setup.py
```

### Comparing `sarcgraph-0.1.0/LICENSE` & `sarcgraph-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcgraph-0.1.0/PKG-INFO` & `sarcgraph-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcgraph
-Version: 0.1.0
+Version: 0.1.1
 Summary: A software for sarcomere detection and tracking
 Home-page: https://pypi.org/project/sarcgraph/
 Author: Saeed Mohammadzadeh
 Author-email: saeedmhz@bu.edu
 Maintainer: [('Saeed Mohammadzadeh', 'saeedmhz@bu.edu'), ('Emma Lejeune', 'elejeune@bu.edu')]
 License: MIT
 Project-URL: Source, https://github.com/Sarc-Graph/sarcgraph
@@ -61,15 +61,15 @@
 
 1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
 
 2. Open a terminal and move to the directory of the ``sarcgraph`` repository. Then, type the following command in terminal to create a virtual envirnoment and install the required packages:
 
 ```bash
 cd sarcgraph
-conda env create --file=environments.yml
+conda env create --file=environment.yml
 ```
 
 3. Activate your virtual environment.
 
 ```bash
 conda activate sarcgraph
 ```
```

### Comparing `sarcgraph-0.1.0/README.md` & `sarcgraph-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
 
 2. Open a terminal and move to the directory of the ``sarcgraph`` repository. Then, type the following command in terminal to create a virtual envirnoment and install the required packages:
 
 ```bash
 cd sarcgraph
-conda env create --file=environments.yml
+conda env create --file=environment.yml
 ```
 
 3. Activate your virtual environment.
 
 ```bash
 conda activate sarcgraph
 ```
```

### Comparing `sarcgraph-0.1.0/sarcgraph/sg.py` & `sarcgraph-0.1.1/sarcgraph/sg.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,24 @@
         ----------
         filtered_frames : np.ndarray, shape=(frames, dim_1, dim_2)
         min_length : int
             Zdisc contours shorter than ``min_length`` pixels will be ignored.
         save_output : bool
             by default True
 
+        Notes
+        -----
+        .. warning::
+            Here we use the ``skimage.measure.find_contours`` function to find
+            contours. This function returns contours with coordinates in
+            ``(row, column)`` order, which corresponds to ``(y, x)`` in
+            Cartesian coordinates. Therefore, in the rest of the code, we use
+            ``y`` for the first dimension and ``x`` for the second dimension.
+            For example, for plotting we use ``plt.plot(y, x)``.
+
         Returns
         -------
         List[np.ndarray]
         """
         if filtered_frames.ndim != 3:
             raise ValueError(
                 "The input must be a 3d numpy array: (frames, " "dim 1, dim 2)"
```

### Comparing `sarcgraph-0.1.0/sarcgraph/sg_tools.py` & `sarcgraph-0.1.1/sarcgraph/sg_tools.py`

 * *Files identical despite different names*

### Comparing `sarcgraph-0.1.0/sarcgraph.egg-info/PKG-INFO` & `sarcgraph-0.1.1/sarcgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcgraph
-Version: 0.1.0
+Version: 0.1.1
 Summary: A software for sarcomere detection and tracking
 Home-page: https://pypi.org/project/sarcgraph/
 Author: Saeed Mohammadzadeh
 Author-email: saeedmhz@bu.edu
 Maintainer: [('Saeed Mohammadzadeh', 'saeedmhz@bu.edu'), ('Emma Lejeune', 'elejeune@bu.edu')]
 License: MIT
 Project-URL: Source, https://github.com/Sarc-Graph/sarcgraph
@@ -61,15 +61,15 @@
 
 1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
 
 2. Open a terminal and move to the directory of the ``sarcgraph`` repository. Then, type the following command in terminal to create a virtual envirnoment and install the required packages:
 
 ```bash
 cd sarcgraph
-conda env create --file=environments.yml
+conda env create --file=environment.yml
 ```
 
 3. Activate your virtual environment.
 
 ```bash
 conda activate sarcgraph
 ```
```

### Comparing `sarcgraph-0.1.0/setup.py` & `sarcgraph-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sarcgraph",
-    version="0.1.0",
+    version="0.1.1",
     author="Saeed Mohammadzadeh",
     author_email="saeedmhz@bu.edu",
     description="A software for sarcomere detection and tracking",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/sarcgraph/",
     project_urls={
@@ -23,9 +23,20 @@
     packages=["sarcgraph"],
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
+    install_requires=[
+        "matplotlib==3.5.2",
+        "networkx==2.8.4",
+        "numpy==1.23.5",
+        "pandas==1.5.2",
+        "scikit-image==0.19.3",
+        "scikit-learn==1.2.1",
+        "scipy==1.10.0",
+        "sk-video==1.1.10",
+        "trackpy==0.6.1",
+    ],
     zip_safe=False,
 )
```

