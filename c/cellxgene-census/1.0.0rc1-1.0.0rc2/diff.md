# Comparing `tmp/cellxgene_census-1.0.0rc1.tar.gz` & `tmp/cellxgene_census-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.0.0rc1.tar", last modified: Thu Apr 27 16:40:27 2023, max compression
+gzip compressed data, was "cellxgene_census-1.0.0rc2.tar", last modified: Mon May  1 20:53:08 2023, max compression
```

## Comparing `cellxgene_census-1.0.0rc1.tar` & `cellxgene_census-1.0.0rc2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.310041 cellxgene_census-1.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.640638 cellxgene_census-1.0.0rc2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.640638 cellxgene_census-1.0.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.640638 cellxgene_census-1.0.0rc2/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_util.py
```

### Comparing `cellxgene_census-1.0.0rc1/LICENSE` & `cellxgene_census-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/PKG-INFO` & `cellxgene_census-1.0.0rc2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
 
-**Status**: Pre-release, under rapid development. Expect API changes.
-
 
 ## For More Help
 For more help, please file a issue on the repo, or contact us at <soma@chanzuckerberg.com>.
 
 If you believe you have found a security issue, we would appreciate notification. Please send email to <security@chanzuckerberg.com>.
```

### Comparing `cellxgene_census-1.0.0rc1/README.md` & `cellxgene_census-1.0.0rc2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
 
-**Status**: Pre-release, under rapid development. Expect API changes.
-
 
 ## For More Help
 For more help, please file a issue on the repo, or contact us at <soma@chanzuckerberg.com>.
 
 If you believe you have found a security issue, we would appreciate notification. Please send email to <security@chanzuckerberg.com>.
```

### Comparing `cellxgene_census-1.0.0rc1/pyproject.toml` & `cellxgene_census-1.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/release_process.md` & `cellxgene_census-1.0.0rc2/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census/__init__.py` & `cellxgene_census-1.0.0rc2/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.0.0rc2/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.0.0rc2/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census/_open.py` & `cellxgene_census-1.0.0rc2/src/cellxgene_census/_open.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the MIT License.
 
 """Open census and related datasets
 
 Contains methods to open publicly hosted versions of Census object and access its source datasets.
 """
-
+import logging
 import os.path
 import urllib.parse
 from typing import Any, Dict, Optional
 
 import certifi
 import s3fs
 import tiledbsoma as soma
@@ -22,14 +22,18 @@
     # https://docs.tiledb.com/main/how-to/configuration#configuration-parameters
     "py.init_buffer_bytes": 1 * 1024**3,
     "soma.init_buffer_bytes": 1 * 1024**3,
     # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
     "vfs.s3.ca_file": certifi.where(),
 }
 
+api_logger = logging.getLogger("cellxgene_census")
+api_logger.setLevel(logging.INFO)
+api_logger.addHandler(logging.StreamHandler())
+
 
 def _open_soma(locator: CensusLocator, context: Optional[soma.options.SOMATileDBContext] = None) -> soma.Collection:
     """Private. Merge config defaults and return open census as a soma Collection/context."""
     s3_region = locator.get("s3_region")
 
     if not context:
         # if no user-defined context, cellxgene_census defaults take precedence over SOMA defaults
@@ -46,15 +50,15 @@
             context = context.replace(tiledb_config=tiledb_config)
 
     return soma.open(locator["uri"], mode="r", soma_type=soma.Collection, context=context)
 
 
 def open_soma(
     *,
-    census_version: Optional[str] = "latest",
+    census_version: Optional[str] = "stable",
     uri: Optional[str] = None,
     context: Optional[soma.options.SOMATileDBContext] = None,
 ) -> soma.Collection:
     """Open the Census by version or URI.
 
     Args:
         census_version:
@@ -107,15 +111,37 @@
 
     if uri is not None:
         return _open_soma({"uri": uri, "s3_region": None}, context)
 
     if census_version is None:
         raise ValueError("Must specify either a census version or an explicit URI.")
 
-    description = get_census_version_description(census_version)  # raises
+    try:
+        description = get_census_version_description(census_version)  # raises
+    except KeyError:
+        # TODO: After the first "stable" is available, this conditional can be removed (keep the 'else' logic)
+        if census_version == "stable":
+            description = get_census_version_description("latest")
+            api_logger.warning(
+                f'The "{census_version}" Census version is not yet available. Using "latest" Census version '
+                f"instead."
+            )
+        else:
+            raise ValueError(
+                f'The "{census_version}" Census version is not valid. Use get_census_version_directory() to retrieve '
+                f"available versions."
+            ) from None
+
+    if description["alias"]:
+        api_logger.info(
+            f"The \"{description['alias']}\" release is currently {description['release_build']}. Specify "
+            f"'census_version=\"{description['release_build']}\"' in future calls to open_soma() to ensure data "
+            "consistency."
+        )
+
     return _open_soma(description["soma"], context)
 
 
 def get_source_h5ad_uri(dataset_id: str, *, census_version: str = "latest") -> CensusLocator:
     """Open the named version of the census, and return the URI for the ``dataset_id``. This
     does not guarantee that the H5AD exists or is accessible to the user.
```

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.0.0rc2/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.0.0rc2/src/cellxgene_census/_release_directory.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # Licensed under the MIT License.
 
 """Versioning of Census builds
 
 Methods to retrieve information about versions of the publicly hosted Census object.
 """
-
 from typing import Dict, Optional, Union, cast
 
 import requests
 from typing_extensions import TypedDict
 
 """
 The following types describe the expected directory of Census builds, used
@@ -27,21 +26,22 @@
 CensusVersionDescription = TypedDict(
     "CensusVersionDescription",
     {
         "release_date": Optional[str],  # date of release, optional
         "release_build": str,  # date of build
         "soma": CensusLocator,  # SOMA objects locator
         "h5ads": CensusLocator,  # source H5ADs locator
+        "alias": Optional[str],  # the alias of this entry
     },
 )
 CensusDirectory = Dict[CensusVersionName, Union[CensusVersionName, CensusVersionDescription]]
 
 
 # URL for the default top-level directory of all public data
-CELL_CENSUS_RELEASE_DIRECTORY_URL = "https://census.cellxgene.cziscience.com/cell-census/release.json"
+CELL_CENSUS_RELEASE_DIRECTORY_URL = "https://census.cellxgene.cziscience.com/cellxgene-census/release.json"
 
 
 def get_census_version_description(census_version: str) -> CensusVersionDescription:
     """Get release description for given Census version, from the Census release directory.
 
     Args:
         census_version:
@@ -113,21 +113,23 @@
     response.raise_for_status()
     directory: CensusDirectory = cast(CensusDirectory, response.json())
 
     # Resolve all aliases for easier use
     for census_version in list(directory.keys()):
         # Strings are aliases for other census_version
         points_at = directory[census_version]
+        alias = census_version if isinstance(points_at, str) else None
         while isinstance(points_at, str):
             # resolve aliases
             if points_at not in directory:
                 # oops, dangling pointer -- drop original census_version
                 directory.pop(census_version)
                 break
 
             points_at = directory[points_at]
 
         if isinstance(points_at, dict):
-            directory[census_version] = points_at
+            directory[census_version] = points_at.copy()
+            cast(CensusVersionDescription, directory[census_version])["alias"] = alias
 
     # Cast is safe, as we have removed all aliases
     return cast(Dict[CensusVersionName, CensusVersionDescription], directory)
```

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
 
-**Status**: Pre-release, under rapid development. Expect API changes.
-
 
 ## For More Help
 For more help, please file a issue on the repo, or contact us at <soma@chanzuckerberg.com>.
 
 If you believe you have found a security issue, we would appreciate notification. Please send email to <security@chanzuckerberg.com>.
```

### Comparing `cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/tests/README.md` & `cellxgene_census-1.0.0rc2/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/tests/test_acceptance.py` & `cellxgene_census-1.0.0rc2/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/tests/test_directory.py` & `cellxgene_census-1.0.0rc2/tests/test_directory.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import requests_mock as rm
 import s3fs
 
 import cellxgene_census
 from cellxgene_census._release_directory import CELL_CENSUS_RELEASE_DIRECTORY_URL
 
 DIRECTORY_JSON = {
+    "stable": "2022-10-01",
     "latest": "2022-11-01",
     "2022-11-01": {
         "release_date": "2022-11-30",
         "release_build": "2022-11-01",
         "soma": {
             "uri": "s3://cellxgene-data-public/cell-census/2022-11-01/soma/",
             "s3_region": "us-west-2",
@@ -48,20 +49,21 @@
     directory = cellxgene_census.get_census_version_directory()
 
     assert isinstance(directory, dict)
     assert len(directory) > 0
     assert all((type(k) == str for k in directory.keys()))
     assert all((type(v) == dict for v in directory.values()))
 
-    for tag in DIRECTORY_JSON:
-        assert tag[0] == "_" or tag in directory
-        if isinstance(DIRECTORY_JSON[tag], dict):
-            assert directory[tag] == DIRECTORY_JSON[tag]
+    assert "_dangling" not in directory
 
-    assert directory["latest"] == directory["2022-11-01"]
+    assert directory["2022-11-01"] == {**DIRECTORY_JSON["2022-11-01"], "alias": None}  # type: ignore
+    assert directory["2022-10-01"] == {**DIRECTORY_JSON["2022-10-01"], "alias": None}  # type: ignore
+
+    assert directory["latest"] == {**DIRECTORY_JSON["2022-11-01"], "alias": "latest"}  # type: ignore
+    assert directory["stable"] == {**DIRECTORY_JSON["2022-10-01"], "alias": "stable"}  # type: ignore
 
     for tag in directory:
         assert directory[tag] == cellxgene_census.get_census_version_description(tag)
 
 
 def test_get_census_version_description_errors() -> None:
     with pytest.raises(KeyError):
```

### Comparing `cellxgene_census-1.0.0rc1/tests/test_get_anndata.py` & `cellxgene_census-1.0.0rc2/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/tests/test_get_helpers.py` & `cellxgene_census-1.0.0rc2/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc1/tests/test_util.py` & `cellxgene_census-1.0.0rc2/tests/test_util.py`

 * *Files identical despite different names*

