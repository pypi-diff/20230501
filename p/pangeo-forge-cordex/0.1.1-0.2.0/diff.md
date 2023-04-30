# Comparing `tmp/pangeo-forge-cordex-0.1.1.tar.gz` & `tmp/pangeo-forge-cordex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.1.1.tar", last modified: Sun Apr 30 18:15:06 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.2.0.tar", last modified: Sun Apr 30 22:32:02 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.1.1.tar` & `pangeo-forge-cordex-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:06.056737 pangeo-forge-cordex-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:06.052737 pangeo-forge-cordex-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:06.052737 pangeo-forge-cordex-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-30 18:15:06.056737 pangeo-forge-cordex-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:06.052737 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 18:15:05.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:06.056737 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-30 18:15:06.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-30 18:15:06.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:15:06.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:15:06.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 18:15:06.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 18:15:06.000000 pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-30 18:15:06.056737 pangeo-forge-cordex-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:14:50.000000 pangeo-forge-cordex-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.390650 pangeo-forge-cordex-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.390650 pangeo-forge-cordex-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.390650 pangeo-forge-cordex-0.2.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.1.1/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.1.1/.gitignore` & `pangeo-forge-cordex-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.1.1/LICENSE` & `pangeo-forge-cordex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/recipe.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,73 @@
-import os
-import ssl
+import fsspec
+import pandas as pd
+import xarray as xr
+
+from .esgf_access import esgf_search
+from .parsing import facets_from_iid
+from .utils import freq_map
+
+
+def number_of_timesteps(dset):
+    start = dset["datetime_start"]
+    stop = dset["datetime_stop"]
+    cf_freq = dset["time_frequency"][0]
+    ntime = pd.date_range(start, stop, freq=freq_map[cf_freq]).size
+    print(f"Found {ntime} timesteps!")
+    return ntime
+
+
+def time_chunksize(ntime, size):
+    chunksize_optimal = 100e6
+    return max(int(ntime * chunksize_optimal / size), 1)
+
+
+def target_chunks(dset, url=None, ssl=None):
+    """Estimate chunksize for time
+
+    Estimate time chunksize from the size of the
+    first timestep in the dataset and the total number
+    of timesteps defined by the frequency, datetime_start
+    and datetime_stop.
+
+    """
+    ntime = number_of_timesteps(dset)
+    var = dset["variable"][0]
+    print(url)
+    if url:
+        fs = fsspec.filesystem("https")
+        with xr.open_dataset(fs.open(url, ssl=ssl)) as ds:
+            size = ds[var].isel(time=0).nbytes * ntime
+            # size = ds.nbytes / ds.time.size * ntime
+            print(f"Estimated size: {size/1.e6} MB")
+    else:
+        size = dset["size"]
+    # print(f"Estimated size: {size/1.e6} MB")
+    return {"time": time_chunksize(ntime, size)}
 
-import requests
-from pangeo_forge_recipes.patterns import pattern_from_file_sequence
-from pangeo_forge_recipes.recipes import XarrayZarrRecipe
-from pyesgf.logon import LogonManager
-
-from .utils import (
-    combine_response,
-    parse_dataset_response,
-    sort_files_by_dataset_id,
-    target_chunks,
-)
-
-freq_map = {"mon": "M", "day": "D", "6hr": "6H", "3hr": "3H", "1hr": "1H"}
-
-
-def logon():
-    lm = LogonManager(verify=True)
-    if not lm.is_logged_on():
-        myproxy_host = "esgf-data.dkrz.de"
-        # if we find those in environment, use them.
-        if "ESGF_USER" in os.environ and "ESGF_PASSWORD" in os.environ:
-            lm.logon(
-                hostname=myproxy_host,
-                username=os.environ["ESGF_USER"],
-                password=os.environ["ESGF_PASSWORD"],
-                interactive=False,
-                bootstrap=True,
-            )
-        else:
-            lm.logon(
-                hostname=myproxy_host,
-                interactive=True,
-                bootstrap=True,
-            )
-
-    print(f"logged on: {lm.is_logged_on()}")
-
-    # create SSL context
-    sslcontext = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH)
-    sslcontext.load_verify_locations(capath=lm.esgf_certs_dir)
-    sslcontext.load_cert_chain(lm.esgf_credentials)
-    return sslcontext
 
-
-def create_recipe(urls, recipe_kwargs=None, pattern_kwargs=None):
-    if recipe_kwargs is None:
-        recipe_kwargs = {}
-    if pattern_kwargs is None:
-        pattern_kwargs = {}
-    pattern = pattern_from_file_sequence(urls, "time", **pattern_kwargs)
-    if urls is not None:
-        return XarrayZarrRecipe(
-            pattern, xarray_concat_kwargs={"join": "exact"}, **recipe_kwargs
-        )
-
-
-def request(
-    url="https://esgf-node.llnl.gov/esg-search/search",
-    project="CORDEX",
-    type="File",
-    **search,
-):
-    params = dict(project=project, type=type, format="application/solr+json", limit=500)
-    params.update(search)
-    return requests.get(url, params)
-
-
-def esgf_search(
-    url="https://esgf-node.llnl.gov/esg-search/search",
-    files_type="OPENDAP",
-    project="CORDEX",
-    **search,
-):
-    response = request(url, project, "Dataset", **search)
-    # return response.json()["response"]
-    dset_info = parse_dataset_response(response)
-    response = request(url, project, "File", **search)
-    files_by_id = sort_files_by_dataset_id(response)
-    responses = combine_response(dset_info, files_by_id)
-    return responses
-
-
-def create_recipe_inputs(response, ssl=None):
+def create_recipe_inputs(responses, ssl=None):
     pattern_kwargs = {}
     if ssl:
         pattern_kwargs["fsspec_open_kwargs"] = {"ssl": ssl}
     inputs = {}
-    for k, v in response.items():
+    for k, v in responses.items():
         inputs[k] = {}
         urls = v["urls"]["netcdf"]
         recipe_kwargs = {}
 
         recipe_kwargs["target_chunks"] = target_chunks(v, urls[0], ssl)
         inputs[k]["urls"] = urls
         inputs[k]["recipe_kwargs"] = recipe_kwargs
         inputs[k]["pattern_kwargs"] = pattern_kwargs
     return inputs
+
+
+def recipe_inputs_from_iids(iids, ssl=None):
+    if not isinstance(iids, list):
+        iids = [iids]
+    dset_responses = {}
+    for iid in iids:
+        facets = facets_from_iid(iid)
+        dset_responses.update(esgf_search(**facets))
+
+    return create_recipe_inputs(dset_responses, ssl)
```

### Comparing `pangeo-forge-cordex-0.1.1/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import re
 
 import requests
 
 # 'cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas'
 known_projects = [
-    "CMIP6",
-    "CMIP5",
-    "obs4MIPs",
-    "input4MIPs",
     "CORDEX",  # Usual Cordex datasets from CMIP5 downscaling
     "CORDEX-Reklies",  # This is Downscaling from Reklies project
     "CORDEX-Adjust",  # Bias adjusted output
     "CORDEX-ESD",  # Statistical downscaling
 ]
 
 
 cordex_template = "project.product.domain.institute.driving_model.experiment.ensemble.rcm_name.rcm_version.time_frequency.variable.version"
 cordex_adjust_template = "project.product.domain.institute.driving_model.experiment.ensemble.rcm_name.bias_adjustment.time_frequency.variable.version"
 
 base_params = {
     # "type": "File",
     "format": "application/solr+json",
     # "fields": "instance_id",
-    "fields": "url,size,table_id,title,instance_id,replica,data_node,frequency,time_frequency",
+    "fields": "url,size,table_id,title,instance_id,replica,data_node,frequency,time_frequency,version",
     "latest": True,
     "distrib": True,
     "limit": 500,
 }
 
 cordex_params = base_params
 
@@ -61,26 +57,27 @@
 
 def project_from_iid(iid):
     """Get project information from first iid entry"""
     return ensure_project_str(iid.split(".")[0])
 
 
 def facets_from_iid(iid, project=None):
-    """Translates iid string to facet dict according to CMIP6 naming scheme"""
+    """Translates iid string to facet dict according to project naming scheme"""
     if project is None:
         # take project id from first iid entry by default
         project = project_from_iid(iid)
     iid = f"{project}." + ".".join(iid.split(".")[1:])
     iid_name_template = id_templates[project]
     # this does not work yet with CORDEX project
     # template = get_dataset_id_template(project)
     # facet_names = facets_from_template(template)
     facets = {}
     for name, value in zip(iid_name_template.split("."), iid.split(".")):
-        facets[name] = value
+        if value != "*":
+            facets[name] = value
     if project == "CORDEX-Reklies":
         # There is another problem with CORDEX-Reklies, e.g.
         # "cordex-reklies.output.EUR-11.GERICS.MIROC-MIROC5.historical.r1i1p1.REMO2015.v1.mon.tas"
         # The product="output" facet will give no result although the dataset_id clearly says it's "output".
         # However the API result is empty list, so the output facet has to be removed when CORDEX-Reklies is searched, hmmm...
         del facets["product"]
     return facets
@@ -153,16 +150,15 @@
                 .replace("'", "")
                 .replace(" ", "")
                 .split(",")
             )
         facets[k] = v
     facets_filtered = {k: v for k, v in facets.items() if v != "*" and k != "project"}
     params = facets_filtered | params
-    # print(facets_filtered)
-    # TODO: how do I iterate over this more efficiently? Maybe we do not want to allow more than x files parsed?
+
     resp = request_from_facets(url, project, **params)
     if resp.status_code != 200:
         print(f"Request [{resp.url}] failed with {resp.status_code}")
         return resp
     else:
         json_dict = resp.json()
         return instance_ids_from_request(json_dict)
```

### Comparing `pangeo-forge-cordex-0.1.1/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 LICENSE
 README.md
 environment.yaml
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
+.github/workflows/ci.yaml
 .github/workflows/release.yaml
+ci/environment.yml
 pangeo_forge_cordex/__init__.py
 pangeo_forge_cordex/_version.py
 pangeo_forge_cordex/esgf_access.py
 pangeo_forge_cordex/parsing.py
 pangeo_forge_cordex/recipe.py
 pangeo_forge_cordex/utils.py
 pangeo_forge_cordex.egg-info/PKG-INFO
 pangeo_forge_cordex.egg-info/SOURCES.txt
 pangeo_forge_cordex.egg-info/dependency_links.txt
 pangeo_forge_cordex.egg-info/not-zip-safe
 pangeo_forge_cordex.egg-info/requires.txt
-pangeo_forge_cordex.egg-info/top_level.txt
+pangeo_forge_cordex.egg-info/top_level.txt
+tests/__init__.py
+tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.1.1/setup.cfg` & `pangeo-forge-cordex-0.2.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 python_requires = >=3.9
 packages = find:
 include_package_data = True
 install_requires = 
 	aiohttp
 	requests
 
+[tool:pytest]
+python_files = test_*.py
+testpaths = tests
+filterwarnings = 
+	ignore:numpy.ufunc size changed, may indicate binary incompatibility.:RuntimeWarning
+
 [flake8]
 ignore = 
 	E203
 	E402
 	E501
 	E731
 	W503
```

