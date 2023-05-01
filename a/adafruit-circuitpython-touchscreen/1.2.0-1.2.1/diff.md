# Comparing `tmp/adafruit-circuitpython-touchscreen-1.2.0.tar.gz` & `tmp/adafruit-circuitpython-touchscreen-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-touchscreen-1.2.0.tar", last modified: Mon Feb 27 22:09:22 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-touchscreen-1.2.1.tar", last modified: Mon May  1 15:02:35 2023, max compression
```

## Comparing `adafruit-circuitpython-touchscreen-1.2.0.tar` & `adafruit-circuitpython-touchscreen-1.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.848678 adafruit-circuitpython-touchscreen-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-27 22:09:22.000000 adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-27 22:09:22.000000 adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 22:09:22.000000 adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 22:09:22.000000 adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-27 22:09:22.000000 adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-02-27 22:09:15.000000 adafruit-circuitpython-touchscreen-1.2.0/adafruit_touchscreen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:09:22.852678 adafruit-circuitpython-touchscreen-1.2.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6145 2023-02-27 22:09:15.000000 adafruit-circuitpython-touchscreen-1.2.0/examples/touchscreen_calibrator_built_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-27 22:09:15.000000 adafruit-circuitpython-touchscreen-1.2.0/examples/touchscreen_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-27 22:09:15.000000 adafruit-circuitpython-touchscreen-1.2.0/examples/touchscreen_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-27 22:09:15.000000 adafruit-circuitpython-touchscreen-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-27 22:09:07.000000 adafruit-circuitpython-touchscreen-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 22:09:22.856678 adafruit-circuitpython-touchscreen-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.582328 adafruit-circuitpython-touchscreen-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.582328 adafruit-circuitpython-touchscreen-1.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.582328 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_touchscreen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6145 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_calibrator_built_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/setup.cfg
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-touchscreen-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/.gitignore` & `adafruit-circuitpython-touchscreen-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/.pre-commit-config.yaml` & `adafruit-circuitpython-touchscreen-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/.pylintrc` & `adafruit-circuitpython-touchscreen-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-touchscreen-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/LICENSE` & `adafruit-circuitpython-touchscreen-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-touchscreen-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/LICENSES/MIT.txt` & `adafruit-circuitpython-touchscreen-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-touchscreen-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/PKG-INFO` & `adafruit-circuitpython-touchscreen-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-touchscreen
-Version: 1.2.0
+Version: 1.2.1
 Summary: CircuitPython library for 4-wire resistive touchscreens
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen
 Keywords: adafruit,blinka,circuitpython,micropython,touchscreen,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/README.rst` & `adafruit-circuitpython-touchscreen-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO` & `adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-touchscreen
-Version: 1.2.0
+Version: 1.2.1
 Summary: CircuitPython library for 4-wire resistive touchscreens
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen
 Keywords: adafruit,blinka,circuitpython,micropython,touchscreen,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt` & `adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/adafruit_touchscreen.py` & `adafruit-circuitpython-touchscreen-1.2.1/adafruit_touchscreen.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen.git"
 
 from digitalio import DigitalInOut
 from analogio import AnalogIn
 
 try:
     from typing import Optional, Tuple
@@ -154,26 +154,26 @@
                             len(self._xsamples)
                         ):
                             self._xsamples[i] = x_p.value
             x = sum(self._xsamples) / len(self._xsamples)
             x_size = 65535
             if self._size:
                 x_size = self._size[0]
-            x = int(map_range(x, self._calib[0][0], self._calib[0][1], 0, x_size))
+            x = int(map_range(x, self._calib[0][0], self._calib[0][1], 0, x_size - 1))
 
             with DigitalInOut(self._xp_pin) as x_p:
                 with DigitalInOut(self._xm_pin) as x_m:
                     with AnalogIn(self._yp_pin) as y_p:
                         x_p.switch_to_output(True)
                         x_m.switch_to_output(False)
                         for i in range(  # pylint: disable=consider-using-enumerate
                             len(self._ysamples)
                         ):
                             self._ysamples[i] = y_p.value
             y = sum(self._ysamples) / len(self._ysamples)
             y_size = 65535
             if self._size:
                 y_size = self._size[1]
-            y = int(map_range(y, self._calib[1][0], self._calib[1][1], 0, y_size))
+            y = int(map_range(y, self._calib[1][0], self._calib[1][1], 0, y_size - 1))
 
             return (x, y, z)
         return None
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/docs/_static/favicon.ico` & `adafruit-circuitpython-touchscreen-1.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/docs/conf.py` & `adafruit-circuitpython-touchscreen-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/docs/index.rst` & `adafruit-circuitpython-touchscreen-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/examples/touchscreen_calibrator_built_in.py` & `adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_calibrator_built_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/examples/touchscreen_orientation.py` & `adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_orientation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/examples/touchscreen_simpletest.py` & `adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.0/pyproject.toml` & `adafruit-circuitpython-touchscreen-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-touchscreen"
 description = "CircuitPython library for 4-wire resistive touchscreens"
-version = "1.2.0"
+version = "1.2.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen"}
 keywords = [
     "adafruit",
```

