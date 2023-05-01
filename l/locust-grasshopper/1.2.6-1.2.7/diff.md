# Comparing `tmp/locust-grasshopper-1.2.6.tar.gz` & `tmp/locust-grasshopper-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-grasshopper-1.2.6.tar", last modified: Wed Apr 26 18:19:36 2023, max compression
+gzip compressed data, was "locust-grasshopper-1.2.7.tar", last modified: Mon May  1 14:54:02 2023, max compression
```

## Comparing `locust-grasshopper-1.2.6.tar` & `locust-grasshopper-1.2.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.127393 locust-grasshopper-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-04-26 18:19:36.127393 locust-grasshopper-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20359 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-04-26 18:19:22.000000 locust-grasshopper-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 18:19:36.127393 locust-grasshopper-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.119393 locust-grasshopper-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/grasshopper/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/grasshopper/lib/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/grasshopper/lib/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/configuration/gh_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/grasshopper/lib/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)    17214 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/fixtures/grasshopper_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/grasshopper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/grasshopper/lib/journeys/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/journeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/journeys/base_journey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/er_basic_console_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/iextendedreporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/reporter_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/shared_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/grasshopper/lib/util/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      330 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/check_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/launch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/listeners.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/shapes.py
--rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-04-26 18:19:15.000000 locust-grasshopper-1.2.6/src/grasshopper/lib/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 18:19:36.123393 locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-04-26 18:19:36.000000 locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-04-26 18:19:36.000000 locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 18:19:36.000000 locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-26 18:19:36.000000 locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-26 18:19:36.000000 locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-26 18:19:36.000000 locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20359 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-01 14:53:46.000000 locust-grasshopper-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.492007 locust-grasshopper-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.492007 locust-grasshopper-1.2.7/src/grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/src/grasshopper/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/src/grasshopper/lib/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/configuration/gh_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/src/grasshopper/lib/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)    17214 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/fixtures/grasshopper_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/grasshopper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/src/grasshopper/lib/journeys/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/journeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/journeys/base_journey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/er_basic_console_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/iextendedreporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/reporter_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/shared_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/src/grasshopper/lib/util/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/check_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/launch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-05-01 14:53:34.000000 locust-grasshopper-1.2.7/src/grasshopper/lib/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:54:02.496007 locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 14:54:02.000000 locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-05-01 14:54:02.000000 locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 14:54:02.000000 locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-01 14:54:02.000000 locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-01 14:54:02.000000 locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-01 14:54:02.000000 locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/top_level.txt
```

### Comparing `locust-grasshopper-1.2.6/LICENSE` & `locust-grasshopper-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/PKG-INFO` & `locust-grasshopper-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.2.6
+Version: 1.2.7
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `locust-grasshopper-1.2.6/README.md` & `locust-grasshopper-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/pyproject.toml` & `locust-grasshopper-1.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "cmake>=3.11.0,<4.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "locust-grasshopper"
-version = "1.2.6" # Managed by bump2version
+version = "1.2.7" # Managed by bump2version
 readme = {file = "README.md", content-type = "text/markdown"}
 description = "a load testing tool extended from locust"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
```

### Comparing `locust-grasshopper-1.2.6/setup.py` & `locust-grasshopper-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/configuration/gh_configuration.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/configuration/gh_configuration.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/fixtures/__init__.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/fixtures/grasshopper_constants.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/fixtures/grasshopper_constants.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/grasshopper.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/grasshopper.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/journeys/base_journey.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/journeys/base_journey.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/er_basic_console_reporter.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/er_basic_console_reporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/iextendedreporter.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/iextendedreporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/reporter_extensions.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/reporter_extensions.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/reporting/shared_reporting.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/reporting/shared_reporting.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/util/decorators.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/util/decorators.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/util/launch.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/util/launch.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/util/listeners.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/util/listeners.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/util/metrics.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/util/metrics.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/util/shapes.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/util/shapes.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/grasshopper/lib/util/utils.py` & `locust-grasshopper-1.2.7/src/grasshopper/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/PKG-INFO` & `locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.2.6
+Version: 1.2.7
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `locust-grasshopper-1.2.6/src/locust_grasshopper.egg-info/SOURCES.txt` & `locust-grasshopper-1.2.7/src/locust_grasshopper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

