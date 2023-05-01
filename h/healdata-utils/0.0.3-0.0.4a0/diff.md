# Comparing `tmp/healdata_utils-0.0.3.tar.gz` & `tmp/healdata_utils-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.0.3.tar", last modified: Fri Apr 21 16:17:10 2023, max compression
+gzip compressed data, was "healdata_utils-0.0.4a0.tar", last modified: Mon May  1 21:24:53 2023, max compression
```

## Comparing `healdata_utils-0.0.3.tar` & `healdata_utils-0.0.4a0.tar`

### file list

```diff
@@ -1,40 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.246121 healdata_utils-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.246121 healdata_utils-0.0.3/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-21 16:16:59.000000 healdata_utils-0.0.3/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:17:10.250121 healdata_utils-0.0.3/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-21 16:17:10.000000 healdata_utils-0.0.3/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-21 16:17:10.000000 healdata_utils-0.0.3/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:17:10.000000 healdata_utils-0.0.3/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 16:17:10.000000 healdata_utils-0.0.3/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-21 16:17:10.000000 healdata_utils-0.0.3/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 16:17:10.000000 healdata_utils-0.0.3/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/tests/test_schemas.py
```

### Comparing `healdata_utils-0.0.3/PKG-INFO` & `healdata_utils-0.0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata_utils
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 # HEAL Data Utilities
```

### Comparing `healdata_utils-0.0.3/README.md` & `healdata_utils-0.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/setup.py` & `healdata_utils-0.0.4a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def generate_long_description():
     return Path("README.md").read_text()
 
 
 setup(
     name='healdata_utils',
-    version='0.0.3',
+    version='0.0.4-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
```

### Comparing `healdata_utils-0.0.3/src/healdata_utils/cli.py` & `healdata_utils-0.0.4a0/src/healdata_utils/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 import click 
 from healdata_utils.transforms.csvtemplate.conversion import convert_templatecsv
 from healdata_utils.transforms.jsontemplate.conversion import convert_templatejson
 from healdata_utils.transforms.readstat.conversion import convert_readstat
 from healdata_utils.transforms.redcapcsv.conversion import convert_redcapcsv
 from healdata_utils.transforms.csvdata.conversion import convert_datacsv
+from healdata_utils.validators.validate import validate_vlmd_json,validate_vlmd_csv
 import json
 from pathlib import Path
-from healdata_utils.schemas import validate_json,validate_csv
 import pandas as pd
 import petl as etl
 from collections import deque
 
 from healdata_utils.utils import find_docstring_desc
 
 choice_fxn = {
@@ -93,21 +93,19 @@
     ## add dd title
     if not data_dictionary_props.get('title'):
         data_dictionary_props['title'] = filepath.stem
 
     # get data dictionary package based on the input type
     data_dictionary_package = choice_fxn[inputtype](filepath,data_dictionary_props)
 
-    fields_csv,report_csv = validate_csv(
-        data_dictionary_package['templatecsv']['data_dictionary']
-    )
-    fields_json,report_json = validate_json(
-        data_dictionary_package['templatejson']
-    )
-    templatejson = {**data_dictionary_props,'data_dictionary':fields_json}
+    templatecsv = data_dictionary_package['templatecsv']['data_dictionary'] #TODO: currently only validates tabular but no reason this needs to be case
+    templatejson = data_dictionary_package['templatejson']
+
+    report_csv = validate_vlmd_csv(templatecsv)
+    report_json = validate_vlmd_json(templatejson)
     # write to file
     if outputdir!=None:
         outputdir = Path(outputdir)
         if outputdir.is_dir():
             jsontemplate_path = outputdir/"heal-jsontemplate-data-dictionary.json"
             csvtemplate_path = outputdir/"heal-csvtemplate-data-dictionary.csv"
         elif outputdir.parent.is_dir():
@@ -116,45 +114,38 @@
             outputdir = outputdir.parent
         else:
             raise Exception("outputdir must be an existing directory where files can be saved")
         
         # print data dictionaries
         jsontemplate_path.write_text(json.dumps(templatejson,indent=4))
 
-        etl.fromdicts(fields_csv).tocsv(csvtemplate_path)
+        etl.fromdicts(templatecsv).tocsv(csvtemplate_path)
 
         # print errors
-        items = [list(item) if type(item)==deque else item for item in report_json.values()]
-        keys = list(report_json.keys())
-        jsonerrors = dict(zip(keys,items))
 
-        if jsonerrors.get("_type_checker"):
-            del jsonerrors["_type_checker"] #Not json serializable and internal object anyways
-        
-        if not jsonerrors['valid']:
+        if not report_json['valid']:
             print("JSON data dictionary not valid, see heal-json-errors.json")
  
         if not report_csv['valid']:
             print("CSV data dictionary not valid, see heal-csv-errors.json and")
             print("heal-csv-errors-summary.txt (which is a more human-readable error report)")
         
         
         # write error reports to file
         errordir = Path(outputdir).joinpath('errors')
         errordir.mkdir(exist_ok=True)
         errordir.joinpath('heal-json-errors.json').write_text(
-            json.dumps(jsonerrors,indent=4)
+            json.dumps(report_json,indent=4)
         )
-        report_csv.to_json(errordir/"heal-csv-errors.json")
-        errordir.joinpath("heal-csv-errors-summary.txt").write_text(
-            report_csv.to_summary()
+        errordir.joinpath('heal-csv-errors.json').write_text(
+            json.dumps(report_csv,indent=4)
         )
     
     return {
-        "csvtemplate":fields_csv,
+        "csvtemplate":templatecsv,
         "jsontemplate":templatejson,
         "errors":{
             "csvtemplate":report_csv,
             "jsontemplate":report_json}
         }
 
 @click.command()
```

### Comparing `healdata_utils-0.0.3/src/healdata_utils/io.py` & `healdata_utils-0.0.4a0/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/schemas.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,112 @@
-from pathlib import Path
-import jsonschema
-from frictionless import Resource,Schema
-from frictionless import transform
-import requests
-import petl as etl
-# currently using fields.json and hardcoding 
-jsonschema_url = (
-"https://raw.githubusercontent.com/norc-heal/"
-"heal-metadata-schemas/mbkranz/variable-lvl-csvs/"
-"variable-level-metadata-schema/schemas/jsonschema/fields.json"
-)
-healjsonschema = requests.get(jsonschema_url).json()
-
-healfrictionless = Schema(
-        "https://raw.githubusercontent.com/norc-heal/heal-metadata-schemas/"
-        "mbkranz/variable-lvl-csvs/"
-        "variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json"
-    )
-
-schema = {
-    'type':'object',
-    'required':[
-        'title',
-        'data_dictionary'
-    ],
-    'properties':{
-        'title':{'type':'string'},
-        'description':{'type':'string'},
-        'data_dictionary':{'type':'array','items':healjsonschema}
-    }
-}
+import pandas as pd
+from healdata_utils.utils import to_int_if_base10
+from healdata_utils.io import read_pyreadstat
+from ..jsontemplate.conversion import convert_templatejson
 
-def validate_json(data_dictionary,raise_valid_error=False,schema=schema):
-    """
-    Validates the `data_dictionary` fields property against the specified JSON schema.
-
-    Parameters
-    ----------
-    data_dictionary : list[dict]
-        The list of fields to validate.
-    raise_valid_error : bool, optional
-        If `True`, raises an exception if the validation fails.
-        Default is `False`.
-    schema : dict, optional
-        The JSON schema to be validated against.
-        Default is `schema`.
+from datetime import datetime
 
-    Returns
-    -------
-    tuple
-        A tuple containing the validated `data_dictionary` and the JSON schema
-        validation error report in the form of a dictionary.
-
-    Raises
-    ------
-    Exception
-        If `raise_valid_error` is `True` and the validation fails.
 
-    Notes
-    -----
-    This function uses the `jsonschema` package for validation.
+def convert_readstat(file_path,
+    data_dictionary_props={}):
     """
-    try:
-        print(f'Validating heal-specified json fields.....')
-        jsonschema.validate(data_dictionary,schema=schema)
-        report = {"valid":True}
-        print(f"JSON array of data dictionary fields is VALID")
-    except jsonschema.exceptions.ValidationError as e:
-        report = e.__dict__
-        report['valid'] = False
-        if raise_valid_error:
-            raise Exception(f"Data dictionary not valid: {e.message}")
-            
-        
-    return data_dictionary,report
+    Converts a "metadata-rich" (ie statistical software file) 
+    into a HEAL-specified data dictionary in both csv format and json format.
 
+    This function relies on [readstat](https://github.com/Roche/pyreadstat) which supports SPSS (sav and por), 
+    SAS (sas7bdat), and Stata (dta). 
 
-def validate_csv(data_or_path,schema=healfrictionless):
-    """
-    Validates tabular data by ordering columns according to a schema
-    with frictionless Table Schema standards profile and adds missing
-    columns before validating.
+    > Currently, this function uses both data and metadata to generate 
+    a HEAL specified data dictionary. That is, types are inferred from the 
+    data (so at least test or synthetic data needed) while everything else is taken 
+    from the metadata (eg missing values, variable labels, variable value labels etc)
 
     Parameters
     ----------
-    data_dict_or_path : str or Path or anything excepted by frictionless Resource data
-        data parameter (eg array of fields in the correct specification for csv)
-        Path to data with the data being a tabular HEAL-specified data dictionary
-    schema : dict, optional
-        The schema to compare data_or_path to (default: HEAL frictionless template)
+    csvtemplate : str or path-like or any object
+        Data or path to data with the data being a tabular HEAL-specified data dictionary.
+        This input can be any data object or path-like string excepted by a frictionless Resource object.
+    data_dictionary_props : dict
+        The HEAL-specified data dictionary properties.
+    mappings : dict, optional
+        Mappings (which can be a dictionary of either lambda functions or other to-be-mapped objects).
+        Default: specified fieldmap.
 
     Returns
     -------
-    List[dict]
-        Tabular data in the form of an array of dictionaries for each field (ie keyed) and the validation report
-    Report
-        frictionless report object
+    dict
+        A dictionary with two keys:
+            - 'templatejson': the HEAL-specified JSON object.
+            - 'templatecsv': the HEAL-specified tabular template.
+
     Notes
     -----
-    Currently, in contrast to the `validate_json` function, this validates only
-    at the field level.
+    ## Missing values (from pyreadstat docs)
+
+    SPSS only supports 3 discrete missing in addition to ranges.
+    For POC, only using discrete. TODO: use range(lo,hi+1) to do ranges; JCOIN Core Measures, for example, will need this
+    
+    From module documentation on missing values:
+
+    - SPSS
+        missing_ranges: a dict with keys being variable names. 
+        Values are a list of dicts. 
+        Each dict contains two keys, 'lo' and 'hi' being the lower boundary and higher boundary for the missing range. 
+        Even if the value in both lo and hi are the same, the two elements will always be present. 
+        This appears for SPSS (sav) files when using the option user_missing=True: user defined missing values appear not as nan but as their true value and this dictionary stores the information about which values are to be considered missing.
+    
+    - Stata/SAS
+        missing_user_values: a dict with keys being variable names. 
+        Values are a list of character values (A to Z and _ for SAS, a to z for SATA) 
+        representing user defined missing values in SAS and STATA. 
+        This appears when using user_missing=True in read_sas7bdat or read_dta 
+        if user defined missing values are present.
+
     """
-    schema = Schema(schema)
-    if isinstance(data_or_path,(str,Path)):
-        data_tbl = (
-            pd.read_csv(data_or_path,dtypes="string")
-            .fillna("")
-            .to_dict(orient="records")
-        )
-    elif isinstance(data_or_path, list):
-        if all(isinstance(item, dict) for item in data_or_path):
-            #NOTE: need to add missing field-wise values. 
-            # could also use potential dialect object. Might be worth looking
-            # into if switching to fricitonless v5
-            data_tbl = [
-                {name:field.get(name,"") 
-                for name in schema.field_names} 
-                for field in data_or_path
-            ]
-   
-    print("Validating csv data dictionary...")
-    source = Resource(data=data_tbl,schema=schema)
-    source.format = "inline"
-    source.scheme = "buffer"
-    report = source.validate()
-    if report['valid']:
-        print("Csv is VALID")
-    else:
-        print("Csv is invalid. Check the report")
     
-    return data_tbl,report
+    df,meta = read_pyreadstat(file_path,user_missing=True)
+    df = df.convert_dtypes() #TODO: use visions package for inference (from pandas profile project)
+    fields = pd.io.json.build_table_schema(df,index=False)['fields'] #converts to frictionless Table Schema
+
+
+    for field in fields:
+        field.pop('extDtype',None)
+        fieldname = field['name']
+
+        value_labels = meta.variable_value_labels.get(fieldname)
+        missing_values = meta.missing_user_values.get(fieldname,[])
+        missing_ranges = meta.missing_ranges.get(fieldname,[])
+
+        #see NOTE in docstring (on missing values): 
+        # below maps SPSS missing values
+        for items in missing_ranges:
+            values = list(set(items.values()))
+            if len(values)==1:
+                if isinstance(values[0],datetime):
+                    missing_values.append(str(values[0]))
+                else:
+                    missing_values.append(values[0])
+            else:
+                raise Exception("Currently, only discrete values are supported")
+
+        if value_labels:
+            field['encodings'] = value_labels
+            #NOTE: enums are assumed if labels represent entire set of values
+            # this avoids value labels that are, for example, partials such as top/bottom encodings
+            enums = set(value_labels.keys()).difference(set(missing_values))
+            constraints_enums = {'constraints':{'enum':[str(v) for v in enums]}}
+            field.update(constraints_enums)
+
+        #NOTE/TODO: for SPSS no functionality for incorporating missing ranges
+        
+        if missing_values:
+            field['missingValues'] = missing_values
+
+        variable_label = meta.column_names_to_labels.get(fieldname)
+        if variable_label:
+            field['description'] = variable_label
+
+    data_dictionary = data_dictionary_props.copy()
+    data_dictionary['data_dictionary'] = fields 
+
+    package = convert_templatejson(data_dictionary)
+    return package
```

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/csvtemplate/conversion.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 see convert_templatecsv_to_json and convert_json_to_templatecsv
 ''' 
 import petl as etl
 from pathlib import Path
 from frictionless import Resource,Package
 from healdata_utils.utils import convert_rec_to_json
+from healdata_utils.io import read_table
 from .mappings import fieldmap
 from os import PathLike
 
 def convert_templatecsv(
     csvtemplate: str,
     data_dictionary_props: dict,
     mappings: dict = fieldmap,
@@ -46,27 +47,26 @@
         A dictionary with two keys:
             - 'templatejson': the HEAL-specified JSON object.
             - 'templatecsv': the HEAL-specified tabular template.
 
     """
 
     if isinstance(csvtemplate,(str,PathLike)):
-        resourceinput = {'path':str(Path(csvtemplate))}
+        template_tbl = etl.fromdataframe(read_table(str(Path(csvtemplate))))
     else:
-        resourceinput = {'data':csvtemplate}
+        template_tbl = etl.fromdataframe(pd.DataFrame(csvtemplate))
 
     # apply convert functions for fields that exist in input
     convertfields = {
         propname:fxn 
         for propname,fxn in mappings.items() 
         if propname in etl.fieldnames(template_tbl)
     }
     fields_csv = (
-        Resource(**resourceinput)
-        .to_petl()
+        template_tbl
         .convert(convertfields)
         .convertnumbers() #TODO: make the number conversions explicit
         .dicts()
     )
 
     fields_json = [convert_rec_to_json(rec) for rec in etl.dicts(template_tbl)]
```

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,17 @@
                 fieldtype = "number"
         else:
             fieldtype = "string"
     
     return {
         "type":fieldtype,
         "encodings":{key.strip():val.strip() for key,val in fieldencodings.items()},
-        "constraints.enum":[val.strip() for val in fieldenums]
+        "constraints":{
+            "enum":[val.strip() for val in fieldenums]
+        }
     }
 
 def maptext(field):
     """ 
     TEXT - single-line text box (for text and numbers)
 
     looks at text validation field
@@ -108,20 +110,27 @@
         fieldpattern = "^[0-9]{10}$"
     elif text_validation=="zipcode":
         fieldtype = "string"
         fieldpattern = "^[0-9]{5}$"
     else:
         fieldtype = "string"
     
-    props = zip(
-        ["type","format","constraints.pattern"],
-        [fieldtype,fieldformat,fieldpattern]
-    )
-    return {name:prop for name,prop in props if prop}
+    props = dict(zip(
+        ["type","format","constraints"],
+        [fieldtype,fieldformat,{"pattern":fieldpattern}]
+    ))
+
+    # delete props without values (ie None)
+    for propname in ["type","format"]:
+        if props[propname]==None:
+            del props[propname]
+    if props["constraints"]["pattern"]==None:
+        del props["constraints"]
 
+    return props
 def mapnotes(field):
     """ NOTES	
     large text box for lots of text
     """
     return {"type":"string"}
 
 def mapdropdown(field):
@@ -190,15 +199,15 @@
 
     fieldsnew = [
         {
             "description":f"[choice={choice}]",
             "title": checkboxname.title()+":"+choice,
             "name":checkboxname+"___"+re.sub("^\-","_",val).strip(), #NOTE: REDCAP changes negative sign to underscore
             "type":fieldtype,
-            "constraints.enum":fieldenums,
+            "constraints":{"enum":fieldenums},
             "encodings":fieldencodings
         }
         for val,choice in choices.items()
     ]
     return fieldsnew
 
 def mapfile(field):
```

### Comparing `healdata_utils-0.0.3/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.3/src/healdata_utils/utils.py` & `healdata_utils-0.0.4a0/src/healdata_utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,16 @@
 def convert_rec_to_json(field):
     ''' 
     converts a flattened dictionary to a nested dictionary
     based on JSON path dot notation indicating nesting
     '''
     field_json = {}
     for prop_path,prop in field.items():
-        if prop:
+        
+        if str(prop) and str(prop)!="<NA>" and str(prop)!="nan":
             # initiate the prop to be added with the entire
             # field 
             prop_json = field_json
             # get the inner most dictionary item of the jsonpath
             nested_names = prop_path.split('.')
             for i,prop_name in enumerate(nested_names):
                 is_last_nested = i+1==len(nested_names)
```

### Comparing `healdata_utils-0.0.3/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.0.4a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata-utils
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 # HEAL Data Utilities
```

### Comparing `healdata_utils-0.0.3/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.0.4a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 README.md
 setup.py
 src/healdata_utils/__init__.py
 src/healdata_utils/cli.py
-src/healdata_utils/config.py
 src/healdata_utils/io.py
 src/healdata_utils/schemas.py
 src/healdata_utils/utils.py
 src/healdata_utils.egg-info/PKG-INFO
 src/healdata_utils.egg-info/SOURCES.txt
 src/healdata_utils.egg-info/dependency_links.txt
 src/healdata_utils.egg-info/entry_points.txt
 src/healdata_utils.egg-info/requires.txt
 src/healdata_utils.egg-info/top_level.txt
 src/healdata_utils/transforms/__init__.py
 src/healdata_utils/transforms/csvdata/conversion.py
 src/healdata_utils/transforms/csvtemplate/__init__.py
 src/healdata_utils/transforms/csvtemplate/conversion.py
 src/healdata_utils/transforms/csvtemplate/mappings.py
+src/healdata_utils/transforms/frictionless/__init__.py
+src/healdata_utils/transforms/frictionless/conversion.py
 src/healdata_utils/transforms/jsontemplate/__init__.py
 src/healdata_utils/transforms/jsontemplate/conversion.py
 src/healdata_utils/transforms/jsontemplate/mappings.py
 src/healdata_utils/transforms/readstat/__init__.py
 src/healdata_utils/transforms/readstat/conversion.py
 src/healdata_utils/transforms/redcapcsv/conversion.py
 src/healdata_utils/transforms/redcapcsv/headers.py
 src/healdata_utils/transforms/redcapcsv/mappings.py
-src/healdata_utils/transforms/redcapcsv/schema.py
+src/healdata_utils/transforms/redcapcsv/schema.py
+src/healdata_utils/validators/__init__.py
+src/healdata_utils/validators/frictionless.py
+src/healdata_utils/validators/jsonschema.py
+src/healdata_utils/validators/validate.py
+tests/test_cli.py
+tests/test_schemas.py
```

