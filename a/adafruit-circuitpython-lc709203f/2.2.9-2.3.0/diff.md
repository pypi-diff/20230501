# Comparing `tmp/adafruit-circuitpython-lc709203f-2.2.9.tar.gz` & `tmp/adafruit-circuitpython-lc709203f-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lc709203f-2.2.9.tar", last modified: Mon Nov 28 18:11:44 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-lc709203f-2.3.0.tar", last modified: Mon May  1 13:48:40 2023, max compression
```

## Comparing `adafruit-circuitpython-lc709203f-2.2.9.tar` & `adafruit-circuitpython-lc709203f-2.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.541233 adafruit-circuitpython-lc709203f-2.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.533233 adafruit-circuitpython-lc709203f-2.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.537233 adafruit-circuitpython-lc709203f-2.2.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.537233 adafruit-circuitpython-lc709203f-2.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6192 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.537233 adafruit-circuitpython-lc709203f-2.2.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3598 2022-11-28 18:11:44.541233 adafruit-circuitpython-lc709203f-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2813 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.537233 adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3598 2022-11-28 18:11:44.000000 adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2022-11-28 18:11:44.000000 adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:11:44.000000 adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      146 2022-11-28 18:11:44.000000 adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-28 18:11:44.000000 adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8284 2022-11-28 18:11:34.000000 adafruit-circuitpython-lc709203f-2.2.9/adafruit_lc709203f.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.541233 adafruit-circuitpython-lc709203f-2.2.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.541233 adafruit-circuitpython-lc709203f-2.2.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      292 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5897 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:44.541233 adafruit-circuitpython-lc709203f-2.2.9/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      628 2022-11-28 18:11:34.000000 adafruit-circuitpython-lc709203f-2.2.9/examples/lc709203f_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      691 2022-11-28 18:11:34.000000 adafruit-circuitpython-lc709203f-2.2.9/examples/lc709203f_thermistortest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2022-11-28 18:11:34.000000 adafruit-circuitpython-lc709203f-2.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      243 2022-11-28 18:11:26.000000 adafruit-circuitpython-lc709203f-2.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:11:44.541233 adafruit-circuitpython-lc709203f-2.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_lc709203f.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/examples/lc709203f_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/examples/lc709203f_thermistortest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/setup.cfg
```

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lc709203f-2.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/.gitignore` & `adafruit-circuitpython-lc709203f-2.3.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/.pre-commit-config.yaml` & `adafruit-circuitpython-lc709203f-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/.pylintrc` & `adafruit-circuitpython-lc709203f-2.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lc709203f-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/LICENSE` & `adafruit-circuitpython-lc709203f-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lc709203f-2.3.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/LICENSES/MIT.txt` & `adafruit-circuitpython-lc709203f-2.3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lc709203f-2.3.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/PKG-INFO` & `adafruit-circuitpython-lc709203f-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lc709203f
-Version: 2.2.9
+Version: 2.3.0
 Summary: Library for I2C LC709203F battery status and fuel gauge
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LC709203F
 Keywords: adafruit,blinka,circuitpython,micropython,lc709203f,battery,lipoly,status,fuel,gauge,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/README.rst` & `adafruit-circuitpython-lc709203f-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO` & `adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lc709203f
-Version: 2.2.9
+Version: 2.3.0
 Summary: Library for I2C LC709203F battery status and fuel gauge
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LC709203F
 Keywords: adafruit,blinka,circuitpython,micropython,lc709203f,battery,lipoly,status,fuel,gauge,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt` & `adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/adafruit_lc709203f.py` & `adafruit-circuitpython-lc709203f-2.3.0/adafruit_lc709203f.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,39 +28,43 @@
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
+import time
+
 from micropython import const
 from adafruit_bus_device import i2c_device
 
 try:
     from typing import Iterable, Optional, Tuple
     from typing_extensions import Literal
     from circuitpython_typing import ReadableBuffer
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.2.9"
+__version__ = "2.3.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LC709203F.git"
 
 LC709203F_I2CADDR_DEFAULT = const(0x0B)
 LC709203F_CMD_ICVERSION = const(0x11)
 LC709203F_CMD_BATTPROF = const(0x12)
 LC709203F_CMD_POWERMODE = const(0x15)
 LC709203F_CMD_APA = const(0x0B)
 LC709203F_CMD_INITRSOC = const(0x07)
 LC709203F_CMD_CELLVOLTAGE = const(0x09)
 LC709203F_CMD_CELLITE = const(0x0F)
 LC709203F_CMD_CELLTEMPERATURE = const(0x08)
 LC709203F_CMD_THERMISTORB = const(0x06)
 LC709203F_CMD_STATUSBIT = const(0x16)
+LC709203F_CMD_ALARMPERCENT = const(0x13)
+LC709203F_CMD_ALARMVOLTAGE = const(0x14)
 
 
 class CV:
     """struct helper"""
 
     @classmethod
     def add_values(
@@ -106,34 +110,48 @@
     (
         ("MAH100", 0x08, "100 mAh", 100),
         ("MAH200", 0x0B, "200 mAh", 200),
         ("MAH400", 0x0E, "400 mAh", 400),
         ("MAH500", 0x10, "500 mAh", 500),
         ("MAH1000", 0x19, "1000 mAh", 1000),
         ("MAH2000", 0x2D, "2000 mAh", 2000),
+        ("MAH2200", 0x30, "2200 mAh", 2200),
         ("MAH3000", 0x36, "3000 mAh", 3000),
     )
 )
 
 
 class LC709203F:
     """Interface library for LC709203F battery monitoring and fuel gauge sensors
 
     :param ~busio.I2C i2c_bus: The I2C bus the device is connected to
     :param int address: The I2C device address. Defaults to :const:`0x0B`
 
     """
 
     def __init__(self, i2c_bus: I2C, address: int = LC709203F_I2CADDR_DEFAULT) -> None:
-        self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
+        value_exc = None
+        for _ in range(3):
+            try:
+                self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
+                break
+            except ValueError as exc:
+                value_exc = exc
+                # Wait a bit for the sensor to wake up.
+                time.sleep(0.1)
+        else:
+            raise value_exc
+
         self._buf = bytearray(10)
         self.power_mode = PowerMode.OPERATE  # pylint: disable=no-member
         self.pack_size = PackSize.MAH500  # pylint: disable=no-member
-        self.battery_profile = 1
+        self.battery_profile = 1  # 4.2V profile
+        time.sleep(0.1)
         self.init_RSOC()
+        time.sleep(0.1)
 
     def init_RSOC(self) -> None:  # pylint: disable=invalid-name
         """Initialize the state of charge calculator"""
         self._write_word(LC709203F_CMD_INITRSOC, 0xAA55)
 
     @property
     def cell_voltage(self) -> float:
@@ -150,15 +168,15 @@
         """Returns the temperature of the cell"""
         return self._read_word(LC709203F_CMD_CELLTEMPERATURE) / 10 - 273.15
 
     @cell_temperature.setter
     def cell_temperature(self, value: float) -> None:
         """Sets the temperature in the LC709203F"""
         if self.thermistor_enable:
-            raise AttributeError("temperature can only be set in i2c mode")
+            raise ValueError("temperature can only be set in i2c mode")
         self._write_word(LC709203F_CMD_CELLTEMPERATURE, int(value + 273.15) * 10)
 
     @property
     def ic_version(self) -> int:
         """Returns read-only chip version"""
         return self._read_word(LC709203F_CMD_ICVERSION)
 
@@ -166,37 +184,37 @@
     def power_mode(self) -> Literal[1, 2]:
         """Returns current power mode (operating or sleeping)"""
         return self._read_word(LC709203F_CMD_POWERMODE)
 
     @power_mode.setter
     def power_mode(self, mode: Literal[1, 2]) -> None:
         if not PowerMode.is_valid(mode):
-            raise AttributeError("power_mode must be a PowerMode")
+            raise ValueError("power_mode must be a PowerMode")
         self._write_word(LC709203F_CMD_POWERMODE, mode)
 
     @property
     def battery_profile(self) -> Literal[0, 1]:
         """Returns current battery profile (0 or 1)"""
         return self._read_word(LC709203F_CMD_BATTPROF)
 
     @battery_profile.setter
     def battery_profile(self, mode: Literal[0, 1]) -> None:
         if not mode in (0, 1):
-            raise AttributeError("battery_profile must be 0 or 1")
+            raise ValueError("battery_profile must be 0 or 1")
         self._write_word(LC709203F_CMD_BATTPROF, mode)
 
     @property
     def pack_size(self) -> int:
         """Returns current battery pack size"""
         return self._read_word(LC709203F_CMD_APA)
 
     @pack_size.setter
     def pack_size(self, size: int) -> None:
         if not PackSize.is_valid(size):
-            raise AttributeError("pack_size must be a PackSize")
+            raise ValueError("pack_size must be a PackSize")
         self._write_word(LC709203F_CMD_APA, size)
 
     @property
     def thermistor_bconstant(self) -> int:
         """Returns the thermistor B-constant"""
         return self._read_word(LC709203F_CMD_THERMISTORB)
 
@@ -210,17 +228,43 @@
         """Returns the current temperature source"""
         return self._read_word(LC709203F_CMD_STATUSBIT)
 
     @thermistor_enable.setter
     def thermistor_enable(self, status: bool) -> None:
         """Sets the temperature source to Tsense"""
         if not isinstance(status, bool):
-            raise AttributeError("thermistor_enable must be True or False")
+            raise ValueError("thermistor_enable must be True or False")
         self._write_word(LC709203F_CMD_STATUSBIT, status)
 
+    @property
+    def low_voltage_alarm_percent(self) -> int:
+        """Return the current low voltage alarm percentage.
+        0 indicates disabled."""
+        return self._read_word(LC709203F_CMD_ALARMPERCENT)
+
+    @low_voltage_alarm_percent.setter
+    def low_voltage_alarm_percent(self, percent: int) -> None:
+        """Set the low voltage alarm percentage.
+        Value of 0 disables the alarm"""
+        if not 0 <= percent <= 100:
+            raise ValueError("alarm voltage percent must be 0-100")
+        self._write_word(LC709203F_CMD_ALARMPERCENT, percent)
+
+    @property
+    def low_voltage_alarm(self) -> int:
+        """Return the current low voltage alarm value in mV
+        0 indicates disabled"""
+        return self._read_word(LC709203F_CMD_ALARMVOLTAGE)
+
+    @low_voltage_alarm.setter
+    def low_voltage_alarm(self, voltage: int) -> None:
+        """Set the low voltage alarm value in mV.
+        Value of 0 disables the alarm."""
+        self._write_word(LC709203F_CMD_ALARMVOLTAGE, voltage)
+
     # pylint: disable=no-self-use
     def _generate_crc(self, data: ReadableBuffer) -> int:
         """8-bit CRC algorithm for checking data"""
         crc = 0x00
         # calculates 8-Bit checksum with given polynomial
         for byte in data:
             crc ^= byte
@@ -239,15 +283,15 @@
 
         with self.i2c_device as i2c:
             i2c.write_then_readinto(
                 self._buf, self._buf, out_start=1, out_end=2, in_start=3, in_end=7
             )
         crc8 = self._generate_crc(self._buf[0:5])
         if crc8 != self._buf[5]:
-            raise RuntimeError("CRC failure on reading word")
+            raise OSError("CRC failure on reading word")
         return (self._buf[4] << 8) | self._buf[3]
 
     def _write_word(self, command: int, data: int) -> None:
         self._buf[0] = LC709203F_I2CADDR_DEFAULT * 2  # write byte
         self._buf[1] = command  # command / register
         self._buf[2] = data & 0xFF
         self._buf[3] = (data >> 8) & 0xFF
```

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/docs/_static/favicon.ico` & `adafruit-circuitpython-lc709203f-2.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/docs/conf.py` & `adafruit-circuitpython-lc709203f-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/docs/index.rst` & `adafruit-circuitpython-lc709203f-2.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/examples/lc709203f_thermistortest.py` & `adafruit-circuitpython-lc709203f-2.3.0/examples/lc709203f_thermistortest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.2.9/pyproject.toml` & `adafruit-circuitpython-lc709203f-2.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-lc709203f"
 description = "Library for I2C LC709203F battery status and fuel gauge"
-version = "2.2.9"
+version = "2.3.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LC709203F"}
 keywords = [
     "adafruit",
```

