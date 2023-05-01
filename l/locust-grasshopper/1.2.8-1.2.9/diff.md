# Comparing `tmp/locust-grasshopper-1.2.8.tar.gz` & `tmp/locust-grasshopper-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-grasshopper-1.2.8.tar", last modified: Mon May  1 15:08:05 2023, max compression
+gzip compressed data, was "locust-grasshopper-1.2.9.tar", last modified: Mon May  1 21:35:37 2023, max compression
```

## Comparing `locust-grasshopper-1.2.8.tar` & `locust-grasshopper-1.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.669236 locust-grasshopper-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 15:08:05.669236 locust-grasshopper-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20359 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-01 15:07:51.000000 locust-grasshopper-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 15:08:05.669236 locust-grasshopper-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.657235 locust-grasshopper-1.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.657235 locust-grasshopper-1.2.8/src/grasshopper/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.657235 locust-grasshopper-1.2.8/src/grasshopper/lib/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.661236 locust-grasshopper-1.2.8/src/grasshopper/lib/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/configuration/gh_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.661236 locust-grasshopper-1.2.8/src/grasshopper/lib/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)    17214 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/fixtures/grasshopper_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/grasshopper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.661236 locust-grasshopper-1.2.8/src/grasshopper/lib/journeys/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/journeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/journeys/base_journey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.661236 locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/er_basic_console_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/iextendedreporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/reporter_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/shared_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.665236 locust-grasshopper-1.2.8/src/grasshopper/lib/util/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      330 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/check_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/launch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/listeners.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/shapes.py
--rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-05-01 15:07:48.000000 locust-grasshopper-1.2.8/src/grasshopper/lib/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 15:08:05.669236 locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 15:08:05.000000 locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-05-01 15:08:05.000000 locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 15:08:05.000000 locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-01 15:08:05.000000 locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-01 15:08:05.000000 locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-01 15:08:05.000000 locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20359 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-05-01 21:35:20.000000 locust-grasshopper-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/gh_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)    18919 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/grasshopper_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/grasshopper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/base_journey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/er_basic_console_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/iextendedreporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/reporter_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/shared_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/src/grasshopper/lib/util/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/check_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/launch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/top_level.txt
```

### Comparing `locust-grasshopper-1.2.8/LICENSE` & `locust-grasshopper-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/PKG-INFO` & `locust-grasshopper-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.2.8
+Version: 1.2.9
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `locust-grasshopper-1.2.8/README.md` & `locust-grasshopper-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/pyproject.toml` & `locust-grasshopper-1.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "cmake>=3.11.0,<4.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "locust-grasshopper"
-version = "1.2.8" # Managed by bump2version
+version = "1.2.9" # Managed by bump2version
 readme = {file = "README.md", content-type = "text/markdown"}
 description = "a load testing tool extended from locust"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
@@ -44,15 +44,15 @@
 "repository" = "https://github.com/alteryx/locust-grasshopper"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.isort]
 profile = "black"
-known_first_party = [
+known_local_folder = [
     "grasshopper"
 ]
 multi_line_output = 3
 atomic = "True"
 honor_noqa = "True"
 include_trailing_comma = "True"
 force_grid_wrap = "0"
```

### Comparing `locust-grasshopper-1.2.8/setup.py` & `locust-grasshopper-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/configuration/gh_configuration.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/gh_configuration.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/fixtures/__init__.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,70 +50,91 @@
 def global_defaults():
     defaults = {
         k: v.get("default")
         for k, v in ConfigurationConstants.COMPLETE_ATTRS.items()
         if v.get("default") is not None
     }
     config = GHConfiguration(**defaults)
-    logger.info(f"CONFIG FIXTURE: global_defaults {config}")
+    logger.debug(f"CONFIG FIXTURE: global_defaults {config}")
     return config
 
 
 @pytest.fixture(scope="session")
 def grasshopper_config_file_args(request):
     config = GHConfiguration()
     try:
         # TODO: should move yaml read to it's own method
         path = request.getfixturevalue("grasshopper_config_file_path")
         with open(path, "r") as stream:
             raw = yaml.safe_load(stream)
 
-        # transfer each section to GHConfiguration object
+        # transfer each section to GHConfiguration object, any other sections ignored
+        # TODO: should we load any other sections?
         global_vals = raw.get("grasshopper", {})
         config.update(**global_vals)
         test_run_vals = raw.get("test_run", {})
         config.update(**test_run_vals)
         scenario_vals = raw.get("scenario", {})
         config.update(**scenario_vals)
 
     except pytest.FixtureLookupError:
         logger.warning(
-            "Skipping loading from grasshopper configuration file because fixture "
-            "'grasshopper_config_file_path` not found. You can safely ignore this "
-            "warning if you were not intending to use a grasshopper configuration file."
+            "CONFIG FIXTURE: Skipping loading from grasshopper configuration file "
+            "because fixture 'grasshopper_config_file_path` not found. You can safely "
+            "ignore this warning if you were not intending to use a grasshopper "
+            "configuration file."
         )
     except FileNotFoundError:
         logger.warning(
-            f"Skipping loading from grasshopper configuration file because {path} not "
-            f"found."
+            f"CONFIG FIXTURE: Skipping loading from grasshopper configuration file "
+            f"because {path} not found."
         )
     except (yaml.YAMLError, AttributeError) as e:
-        logger.warning(f"Unable to parse yaml file {path} with error {e}.")
+        logger.warning(
+            f"CONFIG FIXTURE: Unable to parse yaml file {path} with error " f"{e}."
+        )
 
+    logger.debug(f"CONFIG FIXTURE: grasshopper_config_file {config}")
     return config
 
 
 @pytest.fixture(scope="session")
 def env_var_prefix_key(request):
     prefix = "GH_"
     try:
         prefix = request.getfixturevalue("configuration_prefix_key")
+        if type(prefix) != str or (type(prefix) == str and len(prefix) == 0):
+            logger.warning(
+                f"CONFIG FIXTURE: Fixture configuration_prefix_key may only be a non "
+                f"zero length str, returned value {prefix}, ignoring value."
+            )
+            prefix = "GH_"
     except pytest.FixtureLookupError:
-        logger.info(f"Using default environment variable prefix of {prefix}")
         pass
+
+    logger.debug(f"CONFIG FIXTURE: env_var_prefix_key {prefix}")
     return prefix
 
 
 @pytest.fixture(scope="session")
 def extra_env_var_keys(request):
     keys = []
     try:
         keys = request.getfixturevalue("configuration_extra_env_var_keys")
+        # only allow a list of strings for env_var_keys
+        if not type_check_list_of_strs(keys):
+            logger.warning(
+                f"CONFIG FIXTURE: Fixture configuration_extra_env_var_keys may only "
+                f"return a list of strings, returned value {keys}, ignoring value."
+            )
+            keys = []
     except pytest.FixtureLookupError:
         pass
+
+    logger.debug(f"CONFIG FIXTURE: extra_env_var_keys {keys}")
     return keys
 
 
 @pytest.fixture(scope="session")
 def env_var_args(env_var_prefix_key, extra_env_var_keys):
     config = GHConfiguration()
 
@@ -125,14 +146,16 @@
         ):
             if env_var_name.startswith(env_var_prefix_key):
                 env_var_name = env_var_name.lstrip(env_var_prefix_key)
 
             if len(env_var_name) > 0:
                 config.update_single_key(env_var_name.lower(), env_var_value)
 
+    logger.debug(f"CONFIG FIXTURE: env_var_args {config}")
+
     return config
 
 
 @pytest.fixture(scope="session")
 def request_config(request):
     """Separate config so that we have something to patch during unit testing.
 
@@ -150,14 +173,16 @@
 @pytest.fixture(scope="session")
 def cmdln_args(request_config):
     config = GHConfiguration()
 
     for attr_name, attr_definition in ConfigurationConstants.COMPLETE_ATTRS.items():
         config.update_single_key(attr_name, request_config.getoption(f"--{attr_name}"))
 
+    logger.debug(f"CONFIG FIXTURE: cmdln_args {config}")
+
     return config
 
 
 @pytest.fixture(scope="session")
 def pre_processed_args(
     global_defaults, grasshopper_config_file_args, env_var_args, cmdln_args
 ):
@@ -169,30 +194,29 @@
         # from scenario file. the collection code for when a yaml is specified will
         # perform collection and call pytest.main again with the scenario file &
         # scenario name
         scenario_file = fetch_value_from_multiple_sources(
             [cmdln_args, env_var_args, grasshopper_config_file_args, global_defaults],
             "scenario_file",
         )
-        logger.info(f"scenario file value = {scenario_file}")
         pre_config.update_single_key("scenario_file", scenario_file)
-        logger.info(f"pre_config = {pre_config}")
 
         scenario_name = fetch_value_from_multiple_sources(
             [cmdln_args, env_var_args, grasshopper_config_file_args, global_defaults],
             "scenario_name",
         )
         pre_config.update_single_key("scenario_name", scenario_name)
 
     except Exception as e:
         logger.error(
-            f"Uncaught exception in pre_processed_args fixture: "
+            f"CONFIG_FIXTURE: Uncaught exception in pre_processed_args fixture: "
             f"{type(e).__name__} | {e}"
         )
 
+    logger.debug(f"CONFIG FIXTURE: pre_processed_args {pre_config}")
     return pre_config
 
 
 @pytest.fixture(scope="session")
 def scenario_file_args(pre_processed_args):
     config = GHConfiguration()
 
@@ -212,43 +236,50 @@
             config.update(scenario.get("grasshopper_scenario_args", {}))
             config.update_single_key(
                 "scenario_test_file_name", scenario.get("test_file_name")
             )
             config.update_single_key("scenario_tags", scenario.get("tags"))
         except Exception as e:
             logger.warning(
-                f"Unexpected error loading scenario {scenario_name} from "
-                f"{scenario_file}: {type(e).__name__} | {e}"
+                f"CONFIG FIXTURE: Unexpected error loading scenario {scenario_name} "
+                f"from {scenario_file}: {type(e).__name__} | {e}"
             )
 
+    logger.debug(f"CONFIG FIXTURE: scenario_file_args {config}")
+
     return config
 
 
 @pytest.fixture(scope="session")
 def merge_sources(
     global_defaults,
     grasshopper_config_file_args,
     scenario_file_args,
     env_var_args,
     cmdln_args,
 ):
-    complete_config = GHConfiguration()
+    config = GHConfiguration()
 
     # order matters here, this is determining the variable precedence
     try:
-        complete_config.update(global_defaults)
-        complete_config.update(grasshopper_config_file_args)
-        complete_config.update(scenario_file_args)
-        complete_config.update(env_var_args)
-        complete_config.update(cmdln_args)
+        config.update(global_defaults)
+        config.update(grasshopper_config_file_args)
+        config.update(scenario_file_args)
+        config.update(env_var_args)
+        config.update(cmdln_args)
     except Exception as e:
-        logger.error(f"Unexpected error in merge_sources: {type(e).__name__} | {e}")
+        logger.error(
+            f"CONFIG FIXTURE: Unexpected error in merge_sources: "
+            f"{type(e).__name__} | {e}"
+        )
         pass
 
-    return complete_config
+    logger.debug(f"CONFIG FIXTURE: env_var_args {config}")
+
+    return config
 
 
 @pytest.fixture(scope="session")
 def typecast(merge_sources):
     config = GHConfiguration(merge_sources)
 
     # get the collection of attrs that have a typecast func listed
@@ -259,14 +290,16 @@
     }
 
     # apply the typecast lambda to the value
     for k, v in attrs.items():
         if config.get(k) is not None:
             config[k] = v["typecast"](config[k])
 
+    logger.debug(f"CONFIG FIXTURE: typecast {config}")
+
     return config
 
 
 @pytest.fixture(scope="session")
 def process_shape(typecast):
     config = GHConfiguration(typecast)
     shape = config.get("shape")
@@ -292,28 +325,31 @@
             for k, v in overrides.items()
             if k in ConfigurationConstants.SHAPE_OVERRIDE_ATTR_NAMES
         }
 
         # add the overrides
         config.update(overrides)
     else:
-        logger.error(f"Shape is missing from configuration {config}")
+        logger.error(f"CONFIG FIXTURE: Shape is missing from configuration {config}")
+
+    logger.debug(f"CONFIG FIXTURE: process_shape {config}")
 
     return config
 
 
 @pytest.fixture(scope="session")
 def complete_configuration(process_shape):
     config = GHConfiguration(process_shape)
-    # TODO-DEPRECATED
-    # Transfer the value from the deprecated arg to the new arg, so that we can
-    # gracefully transfer use to the new arg
+    # TODO-DEPRECATED: Transfer the value from the deprecated arg to the new arg,
+    # TODO: so that we can gracefully transfer use to the new arg
     # influxdb --> influx_host
     config.update_single_key("influx_host", config.get("influxdb"))
 
+    logger.debug(f"CONFIG FIXTURE: complete_configuration {config}")
+
     return config
 
 
 # -------------------------------- OTHER FIXTURES ------------------------------
 @pytest.fixture(scope="function", autouse=True)
 def do_scenario_delay(grasshopper_args):
     """Functionality to delay between each scenario run."""
@@ -472,7 +508,18 @@
     the entire merge of values.
 
     """
     value = None
     for source in sources:
         value = value or source.get(key)
     return value
+
+
+def type_check_list_of_strs(list_of_strs):
+    """Return True if list of strings or [], false if anything else."""
+    check_passed = False
+    if type(list_of_strs) == list:
+        all_strs = True
+        for s in list_of_strs:
+            all_strs = all_strs and type(s) == str
+        check_passed = all_strs
+    return check_passed
```

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/fixtures/grasshopper_constants.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/grasshopper_constants.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/grasshopper.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/grasshopper.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/journeys/base_journey.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/base_journey.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/er_basic_console_reporter.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/er_basic_console_reporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/iextendedreporter.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/iextendedreporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/reporter_extensions.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/reporter_extensions.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/reporting/shared_reporting.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/shared_reporting.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/util/decorators.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/util/decorators.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/util/launch.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/util/launch.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/util/listeners.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/util/listeners.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/util/metrics.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/util/metrics.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/util/shapes.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/util/shapes.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/grasshopper/lib/util/utils.py` & `locust-grasshopper-1.2.9/src/grasshopper/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/PKG-INFO` & `locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.2.8
+Version: 1.2.9
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `locust-grasshopper-1.2.8/src/locust_grasshopper.egg-info/SOURCES.txt` & `locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

