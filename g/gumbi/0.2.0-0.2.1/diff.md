# Comparing `tmp/gumbi-0.2.0.tar.gz` & `tmp/gumbi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gumbi-0.2.0.tar", last modified: Mon May  1 01:04:32 2023, max compression
+gzip compressed data, was "gumbi-0.2.1.tar", last modified: Mon May  1 01:21:06 2023, max compression
```

## Comparing `gumbi-0.2.0.tar` & `gumbi-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.979941 gumbi-0.2.0/
--rw-r--r--   0 john      (1000) john      (1000)    11357 2022-10-14 20:45:47.000000 gumbi-0.2.0/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)      235 2022-10-14 20:45:47.000000 gumbi-0.2.0/MANIFEST.in
--rw-r--r--   0 john      (1000) john      (1000)     3045 2023-05-01 01:04:32.979941 gumbi-0.2.0/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     2225 2023-05-01 01:03:42.000000 gumbi-0.2.0/README.md
--rw-r--r--   0 john      (1000) john      (1000)        5 2023-05-01 01:03:42.000000 gumbi-0.2.0/VERSION
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.947441 gumbi-0.2.0/docs/
--rw-r--r--   0 john      (1000) john      (1000)      122 2023-05-01 01:03:42.000000 gumbi-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.958275 gumbi-0.2.0/docs/source/
--rw-r--r--   0 john      (1000) john      (1000)     2829 2023-05-01 01:03:42.000000 gumbi-0.2.0/docs/source/conf.py
--rw-r--r--   0 john      (1000) john      (1000)      620 2022-10-14 20:45:47.000000 gumbi-0.2.0/docs/source/index.rst
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.947441 gumbi-0.2.0/docs/source/notebooks/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.958275 gumbi-0.2.0/docs/source/notebooks/examples/
--rw-r--r--   0 john      (1000) john      (1000)  1505160 2023-05-01 01:03:42.000000 gumbi-0.2.0/docs/source/notebooks/examples/Cars_Dataset.ipynb
--rw-r--r--   0 john      (1000) john      (1000)  2084410 2023-05-01 01:03:42.000000 gumbi-0.2.0/docs/source/notebooks/examples/Latent_GP.ipynb
--rw-r--r--   0 john      (1000) john      (1000)   423694 2023-05-01 01:03:42.000000 gumbi-0.2.0/docs/source/notebooks/examples/Multioutput_Regression.ipynb
--rw-r--r--   0 john      (1000) john      (1000)   440843 2023-05-01 01:03:42.000000 gumbi-0.2.0/docs/source/notebooks/examples/Simple_Regression.ipynb
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.958275 gumbi-0.2.0/docs/source/notebooks/getting_started/
--rw-r--r--   0 john      (1000) john      (1000)    41413 2023-05-01 01:03:42.000000 gumbi-0.2.0/docs/source/notebooks/getting_started/introduction.ipynb
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.969108 gumbi-0.2.0/gumbi/
--rw-r--r--   0 john      (1000) john      (1000)      402 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    33679 2023-04-30 03:43:08.000000 gumbi-0.2.0/gumbi/aggregation.py
--rw-r--r--   0 john      (1000) john      (1000)    57752 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/arrays.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.969108 gumbi-0.2.0/gumbi/data/
--rw-r--r--   0 john      (1000) john      (1000)   552642 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/data/Example_DataSet.pkl
--rw-r--r--   0 john      (1000) john      (1000)      136 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/data/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    16993 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/plotting.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.969108 gumbi-0.2.0/gumbi/regression/
--rw-r--r--   0 john      (1000) john      (1000)      124 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/regression/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    52481 2023-04-10 19:27:45.000000 gumbi-0.2.0/gumbi/regression/base.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.969108 gumbi-0.2.0/gumbi/regression/pymc/
--rw-r--r--   0 john      (1000) john      (1000)    37240 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/regression/pymc/GP.py
--rw-r--r--   0 john      (1000) john      (1000)        0 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/regression/pymc/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     1858 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/regression/pymc/extras.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.969108 gumbi-0.2.0/gumbi/style/
--rw-r--r--   0 john      (1000) john      (1000)      236 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/style/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    33984 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/style/breve_presentation.mplstyle
--rw-r--r--   0 john      (1000) john      (1000)    33956 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/style/futura_presentation.mplstyle
--rw-r--r--   0 john      (1000) john      (1000)    33945 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/style/presentation.mplstyle
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.979941 gumbi-0.2.0/gumbi/utils/
--rw-r--r--   0 john      (1000) john      (1000)       76 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/utils/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     2031 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/utils/generic_utils.py
--rw-r--r--   0 john      (1000) john      (1000)      385 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/utils/gp_utils.py
--rw-r--r--   0 john      (1000) john      (1000)     3214 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/utils/misc.py
--rw-r--r--   0 john      (1000) john      (1000)     1414 2023-05-01 01:03:42.000000 gumbi-0.2.0/gumbi/utils/pymc_utils.py
--rw-r--r--   0 john      (1000) john      (1000)      222 2022-10-14 20:45:47.000000 gumbi-0.2.0/gumbi/versions.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.969108 gumbi-0.2.0/gumbi.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3045 2023-05-01 01:04:32.000000 gumbi-0.2.0/gumbi.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1248 2023-05-01 01:04:32.000000 gumbi-0.2.0/gumbi.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-01 01:04:32.000000 gumbi-0.2.0/gumbi.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       77 2023-05-01 01:04:32.000000 gumbi-0.2.0/gumbi.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       12 2023-05-01 01:04:32.000000 gumbi-0.2.0/gumbi.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) john      (1000)      213 2022-10-14 20:45:47.000000 gumbi-0.2.0/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)      104 2023-05-01 01:03:42.000000 gumbi-0.2.0/requirements.txt
--rw-r--r--   0 john      (1000) john      (1000)      199 2023-05-01 01:04:32.979941 gumbi-0.2.0/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     1679 2023-05-01 01:03:42.000000 gumbi-0.2.0/setup.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:04:32.979941 gumbi-0.2.0/tests/
--rw-r--r--   0 john      (1000) john      (1000)        0 2022-10-14 20:45:47.000000 gumbi-0.2.0/tests/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)      615 2022-10-14 20:45:47.000000 gumbi-0.2.0/tests/conftest.py
--rw-r--r--   0 john      (1000) john      (1000)     3983 2022-10-14 20:45:47.000000 gumbi-0.2.0/tests/test_aggregation.py
--rw-r--r--   0 john      (1000) john      (1000)     6873 2023-05-01 01:03:42.000000 gumbi-0.2.0/tests/test_arrays.py
--rw-r--r--   0 john      (1000) john      (1000)     4031 2023-05-01 01:03:42.000000 gumbi-0.2.0/tests/test_plots.py
--rw-r--r--   0 john      (1000) john      (1000)     6391 2023-05-01 01:03:42.000000 gumbi-0.2.0/tests/test_regression.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/
+-rw-r--r--   0 john      (1000) john      (1000)    11357 2022-10-14 20:45:47.000000 gumbi-0.2.1/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)      235 2022-10-14 20:45:47.000000 gumbi-0.2.1/MANIFEST.in
+-rw-r--r--   0 john      (1000) john      (1000)     3045 2023-05-01 01:21:06.287999 gumbi-0.2.1/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     2225 2023-05-01 01:03:42.000000 gumbi-0.2.1/README.md
+-rw-r--r--   0 john      (1000) john      (1000)        5 2023-05-01 01:20:41.000000 gumbi-0.2.1/VERSION
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.222998 gumbi-0.2.1/docs/
+-rw-r--r--   0 john      (1000) john      (1000)      122 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.222998 gumbi-0.2.1/docs/source/
+-rw-r--r--   0 john      (1000) john      (1000)     2829 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/conf.py
+-rw-r--r--   0 john      (1000) john      (1000)      620 2022-10-14 20:45:47.000000 gumbi-0.2.1/docs/source/index.rst
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.212165 gumbi-0.2.1/docs/source/notebooks/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.266332 gumbi-0.2.1/docs/source/notebooks/examples/
+-rw-r--r--   0 john      (1000) john      (1000)  1505160 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Cars_Dataset.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)  2084410 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Latent_GP.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)   423694 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Multioutput_Regression.ipynb
+-rw-r--r--   0 john      (1000) john      (1000)   440843 2023-05-01 01:03:42.000000 gumbi-0.2.1/docs/source/notebooks/examples/Simple_Regression.ipynb
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.277165 gumbi-0.2.1/docs/source/notebooks/getting_started/
+-rw-r--r--   0 john      (1000) john      (1000)    41212 2023-05-01 01:20:41.000000 gumbi-0.2.1/docs/source/notebooks/getting_started/introduction.ipynb
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.277165 gumbi-0.2.1/gumbi/
+-rw-r--r--   0 john      (1000) john      (1000)      402 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    33679 2023-04-30 03:43:08.000000 gumbi-0.2.1/gumbi/aggregation.py
+-rw-r--r--   0 john      (1000) john      (1000)    57752 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/arrays.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/data/
+-rw-r--r--   0 john      (1000) john      (1000)   552642 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/data/Example_DataSet.pkl
+-rw-r--r--   0 john      (1000) john      (1000)      136 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/data/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    16993 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/plotting.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/regression/
+-rw-r--r--   0 john      (1000) john      (1000)      124 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/regression/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    52481 2023-04-10 19:27:45.000000 gumbi-0.2.1/gumbi/regression/base.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/regression/pymc/
+-rw-r--r--   0 john      (1000) john      (1000)    37223 2023-05-01 01:20:41.000000 gumbi-0.2.1/gumbi/regression/pymc/GP.py
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/regression/pymc/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     1858 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/regression/pymc/extras.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/style/
+-rw-r--r--   0 john      (1000) john      (1000)      236 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    33984 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/breve_presentation.mplstyle
+-rw-r--r--   0 john      (1000) john      (1000)    33956 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/futura_presentation.mplstyle
+-rw-r--r--   0 john      (1000) john      (1000)    33945 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/style/presentation.mplstyle
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/gumbi/utils/
+-rw-r--r--   0 john      (1000) john      (1000)       76 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     2031 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/generic_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)      385 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/gp_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)     3214 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/utils/misc.py
+-rw-r--r--   0 john      (1000) john      (1000)     1414 2023-05-01 01:03:42.000000 gumbi-0.2.1/gumbi/utils/pymc_utils.py
+-rw-r--r--   0 john      (1000) john      (1000)      222 2022-10-14 20:45:47.000000 gumbi-0.2.1/gumbi/versions.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.277165 gumbi-0.2.1/gumbi.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3045 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1248 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       77 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       12 2023-05-01 01:21:06.000000 gumbi-0.2.1/gumbi.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) john      (1000)      213 2022-10-14 20:45:47.000000 gumbi-0.2.1/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)      104 2023-05-01 01:03:42.000000 gumbi-0.2.1/requirements.txt
+-rw-r--r--   0 john      (1000) john      (1000)      199 2023-05-01 01:21:06.287999 gumbi-0.2.1/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     1679 2023-05-01 01:03:42.000000 gumbi-0.2.1/setup.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-01 01:21:06.287999 gumbi-0.2.1/tests/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2022-10-14 20:45:47.000000 gumbi-0.2.1/tests/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)      615 2022-10-14 20:45:47.000000 gumbi-0.2.1/tests/conftest.py
+-rw-r--r--   0 john      (1000) john      (1000)     3983 2022-10-14 20:45:47.000000 gumbi-0.2.1/tests/test_aggregation.py
+-rw-r--r--   0 john      (1000) john      (1000)     6873 2023-05-01 01:03:42.000000 gumbi-0.2.1/tests/test_arrays.py
+-rw-r--r--   0 john      (1000) john      (1000)     4031 2023-05-01 01:03:42.000000 gumbi-0.2.1/tests/test_plots.py
+-rw-r--r--   0 john      (1000) john      (1000)     6391 2023-05-01 01:03:42.000000 gumbi-0.2.1/tests/test_regression.py
```

### Comparing `gumbi-0.2.0/LICENSE` & `gumbi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/PKG-INFO` & `gumbi-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `gumbi-0.2.0/README.md` & `gumbi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/docs/source/conf.py` & `gumbi-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/docs/source/index.rst` & `gumbi-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/docs/source/notebooks/examples/Cars_Dataset.ipynb` & `gumbi-0.2.1/docs/source/notebooks/examples/Cars_Dataset.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/docs/source/notebooks/examples/Latent_GP.ipynb` & `gumbi-0.2.1/docs/source/notebooks/examples/Latent_GP.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/docs/source/notebooks/examples/Multioutput_Regression.ipynb` & `gumbi-0.2.1/docs/source/notebooks/examples/Multioutput_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/docs/source/notebooks/examples/Simple_Regression.ipynb` & `gumbi-0.2.1/docs/source/notebooks/examples/Simple_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/docs/source/notebooks/getting_started/introduction.ipynb` & `gumbi-0.2.1/docs/source/notebooks/getting_started/introduction.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886363636363636%*

 * *Differences: {"'cells'": '{delete: [0]}'}*

```diff
@@ -1,18 +1,10 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "c675e224",
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
             "cell_type": "markdown",
             "id": "e8603106",
             "metadata": {},
             "source": [
                 "# Introduction\n",
                 "\n",
                 "Gumbi simplifies the steps needed to build a Gaussian Process model from tabular data. It takes care of shaping,\n",
```

### Comparing `gumbi-0.2.0/gumbi/aggregation.py` & `gumbi-0.2.1/gumbi/aggregation.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/arrays.py` & `gumbi-0.2.1/gumbi/arrays.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/data/Example_DataSet.pkl` & `gumbi-0.2.1/gumbi/data/Example_DataSet.pkl`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/plotting.py` & `gumbi-0.2.1/gumbi/plotting.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/regression/base.py` & `gumbi-0.2.1/gumbi/regression/base.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/regression/pymc/GP.py` & `gumbi-0.2.1/gumbi/regression/pymc/GP.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
         ℓ_μ,
         ℓ_σ,
         period,
         ARD=True,
         **kernel_kwargs,
     ):
         continuous_kernel_factory = self._make_continuous_cov(
-            continuous_cov_func, 2, None, n_s, ℓ_μ, ℓ_σ, ARD=ARD, stabilize=False, **kernel_kwargs
+            continuous_cov_func, 2, None, n_s, ℓ_μ, ℓ_σ, ARD=ARD, **kernel_kwargs
         )
 
         zperiods = [period.z[dim + "_z"].values() for dim in self.continuous_dims]
         zperiods = np.array(zperiods).squeeze() if len(zperiods) > 1 else zperiods[0]
 
         def mapping(x, zperiods):
             c = 2.0 * np.pi * (1.0 / zperiods)
```

### Comparing `gumbi-0.2.0/gumbi/regression/pymc/extras.py` & `gumbi-0.2.1/gumbi/regression/pymc/extras.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/style/breve_presentation.mplstyle` & `gumbi-0.2.1/gumbi/style/breve_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/style/futura_presentation.mplstyle` & `gumbi-0.2.1/gumbi/style/futura_presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/style/presentation.mplstyle` & `gumbi-0.2.1/gumbi/style/presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/utils/generic_utils.py` & `gumbi-0.2.1/gumbi/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/utils/misc.py` & `gumbi-0.2.1/gumbi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi/utils/pymc_utils.py` & `gumbi-0.2.1/gumbi/utils/pymc_utils.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/gumbi.egg-info/PKG-INFO` & `gumbi-0.2.1/gumbi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gumbi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gaussian Process Model Building Interface
 Home-page: https://github.com/JohnGoertz/Gumbi
 Author: John Goertz
 Author-email: 
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `gumbi-0.2.0/gumbi.egg-info/SOURCES.txt` & `gumbi-0.2.1/gumbi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/setup.py` & `gumbi-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/tests/conftest.py` & `gumbi-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/tests/test_aggregation.py` & `gumbi-0.2.1/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/tests/test_arrays.py` & `gumbi-0.2.1/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/tests/test_plots.py` & `gumbi-0.2.1/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `gumbi-0.2.0/tests/test_regression.py` & `gumbi-0.2.1/tests/test_regression.py`

 * *Files identical despite different names*

