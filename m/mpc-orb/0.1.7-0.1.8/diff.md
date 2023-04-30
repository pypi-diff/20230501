# Comparing `tmp/mpc_orb-0.1.7.tar.gz` & `tmp/mpc_orb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_orb-0.1.7.tar", last modified: Tue Apr 25 02:15:20 2023, max compression
+gzip compressed data, was "mpc_orb-0.1.8.tar", last modified: Sun Apr 30 23:20:13 2023, max compression
```

## Comparing `mpc_orb-0.1.7.tar` & `mpc_orb-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb/demo_json/
--rw-r--r--   0 runner    (1001) docker     (122)     8036 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb/schema_json/
--rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_latest.json
--rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.1.json
--rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.2.json
--rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.3.json
--rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.4.json
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/validate_mpcorb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/filepaths_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb/demo_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     8036 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8429 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb/schema_json/
+-rw-r--r--   0 runner    (1001) docker     (122)    36424 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_latest.json
+-rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.3.json
+-rw-r--r--   0 runner    (1001) docker     (122)    36424 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.4.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/validate_mpcorb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/filepaths_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2117 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_validation.py
```

### Comparing `mpc_orb-0.1.7/LICENSE` & `mpc_orb-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/PKG-INFO` & `mpc_orb-0.1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,73 @@
-Metadata-Version: 2.1
-Name: mpc_orb
-Version: 0.1.7
-Home-page: https://github.com/Smithsonian/mpc-public
-Author: MJP:MPC
-Author-email: mpayne@cfa.harvard.edu
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # mpc-public/mpc_orb
 
+Documentation and code related to a standardized format for the exchange of data on the *best-fit orbit* for solar-system bodies, including minor-planets, comets, irregular satellites, and interstellar interlopers. 
 
-Code related to the "mpc_orb.json" format.
-
-This format is intended to be used to describe the orbits of solar-system minor-planets, comets, irregular satellites, and interstellar interlopers.
+The format uses JSON files for the exchange of data, and is refered to as the *mpc_orb.json* format.
 
 The MPC currently populates mpc_orb.json files using data from the orbfit package, but we emphasize that the mpc_orb.json format is intended for the generic exchange of orbit data from any source.  
 
 As of April 2023, the latest version of the defining schema is version 0.4
  - While the schema versions are numbered < 1, the format should be considered experimental/developmental/beta/WIP.
 
-The repo currently contains code and documentation related to: 
- - A description of the "mpc_orb.json" format, and an associated defining JSON schema.
- - Python code to demonstrate the validation of files in the "mpc_orb.json" format. 
- - Python code to facilitate the parsing of files in the "mpc_orb.json" format. 
+This repository currently contains code and documentation related to: 
+ - A description of the *mpc_orb.json* format, and an associated defining JSON schema.
+ - Examples of the *mpc_orb.json* format for some specific objects
+ - Python code to demonstrate the validation of files in the *mpc_orb.json* format. 
+ - Python code to facilitate the parsing of files in the *mpc_orb.json* format. 
 
 ## Repo Contents 
 
-(a) demos            
-
- - Demonstrations of python code usage, including *python-scripts* and *jupyter notebooks*.
 
+### Sample JSON Files 
 
-(b) mpc_orb            
-
- - The main python code directory.
-
- - Contains code to both validate & parse mpc-orb-json files 
+Examples of the *mpc_orb.json* format for some specific objects can be found in */mpc_orb/demo_json*
  
- - Contains directories holding the defining schema (*/mpc_orb/schema_json/*) and sample files (*/mpc_orb/demo_json/*). 
 
-(c) docs 
+### MPC_ORB JSON schema 
 
- - Documentation describing the "mpc_orb.json" format, including *allowed* fields, *required* fields, etc
+The JSON files defining the *mpc_orb.json* format can be found in */mpc_orb/schema_json*
+ 
+### Documentation
 
-(d) tests
+Documentation describing the *mpc_orb.json* format, including *allowed* fields, *required* fields, constraints, etc, can be found in the */docs/* directory.
 
- - Tests of the python code in the *mpc_orb* directory. For details of the test code, including how to execute the tests, please see the file */tests/README.md*.
 
+### Python Functionalities (*/mpc_orb/*)
 
-## MPC_ORB JSON schema 
+The */mpc_orb/* directory contains some python code to both validate & parse mpc-orb-json files 
 
- - The JSON files defining the "mpc_orb.json" format can be found in */mpc_orb/schema_json*
- 
- - Further documentation on the format can be found in */docs/*
+#### Parsing *mpc_orb.json* formatted data
 
+The code in *mpc_orb/parse.py* provides functions & classes to facilitate the parsing of *mpc_orb.json* files in python. 
 
+It is expected that this functionality will be used regularly by both internal MPC staff & external community users.
 
+Some demonstrations of code usage can be found in the */demo/* directory and in the *mpc_orb/demo.py* script.
 
-## Python Functionalities (*mpc_orb*)
 
-(i) Provide "parse" functions for JSON files containing "MPC_ORB.JSON" formatted data
+#### Validating *mpc_orb.json* files
 
- - It is expected that this functionality will be used regularly by both internal MPC staff & external community users.
+The code in *mpc_orb/parse.py* provides functions & classes to validate *mpc_orb.json* files in python. 
 
- - The parsing code is in mpc_orb/parse.py
+It is expected that these validation functionalities will typically be used as part of the "parse" functions described above. 
 
- - Demonstrations of code usage can be found in demo/Example_parse_mpcorb_json.ipynb and demo/demo_parse.py
+I.e. it is *not* expected that the end-user will regularly access the validation functions *directly*, but rather, the validation functions will be called under-the-hood by the *mpc_orb/parse.py* routines. 
 
 
-(ii) Provide validation functions
 
- - It is expected that these validation functionalities will typically be used as part of the "parse" functions described in (i) above. 
- 
- - I.e. it is *not* expected that the end-user will directly access the validation functions themselves, but rather, the validation functions are called under-the-hood by the mpc_orb/parse.py routines. 
+#### Installation and Usage 
 
- - The code that performs the validation can be found in mpc_orb/validate_mpcorb.py
+The python code in *mpc_orb* is available as a pip-installable python package. 
 
+Further details can be found in *mpc_orb/README.md*
 
-## Installation and Usage 
+ 
 
-The python code in *mpc_orb* is available as a pip-installable python package. 
 
-To do so the user can type:
-> pip install mpc_orb
+### Python Tests (*/tests/*)
 
+Tests of the python code in the *mpc_orb* directory are provided in the *tests* directory. 
  
+ For details of the test code, including how to execute the tests, please see the file */tests/README.md*.
+
```

### Comparing `mpc_orb-0.1.7/mpc_orb/demo.py` & `mpc_orb-0.1.8/mpc_orb/demo.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json` & `mpc_orb-0.1.8/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/mpc_orb/interpret.py` & `mpc_orb-0.1.8/mpc_orb/interpret.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/mpc_orb/parse.py` & `mpc_orb-0.1.8/mpc_orb/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,25 @@
         if self.schema_json is None:
             self.schema_json = validate_mpcorb.load_schema()
                     
                     
         # Find the appropriate variable name to use to search for a description ...
         # (i) If variable_name is a top-level property such as 'designation_data', 'COM', etc
         if variable_name in self.schema_json['properties'].keys():
-            return  {variable_name: {'description':self.schema_json['properties'][variable_name]['description'] }}
+            return  {variable_name:
+                        {'description':
+                            self.schema_json['properties'][variable_name]['description'] ,
+                        'allowed properties':
+                            list(self.schema_json['properties'][variable_name]['properties'].keys())
+                        }
+                    }
+            
 
         if variable_name == 'schema_json':
-            return {variable_name: {'filepath':filepaths.mpcorb_schema} }
+            return {variable_name: {'filepath':filepaths.schema_relative_filepath} }
 
         # (ii) If variable_name is one of the defined-schema variables
         if variable_name in self.schema_json['$defs']:
             def_var_name = variable_name
             
         # (iii) If variable_name is an attribute of COM
         elif variable_name in self.COM.__dict__:
@@ -99,17 +106,22 @@
             
         # Extract a description
         return  {variable_name: None } if def_var_name is None else \
                 {variable_name: self._clean(self.schema_json['$defs'][def_var_name])}
             
 
     def _clean(self,d):
-        """ """
-        return { k: self._clean(v) if isinstance(v, dict) else v for k,v in d.items() if k not in ['type']}
-        
+        """
+        Provides an easy-to-read form of the schema-data for a specific $defs component
+        """
+        #return { k: self._clean(v) if isinstance(v, dict) else v for k,v in d.items() if k not in ['type']}
+        return {
+            "description": d["description"],
+            "units": d["properties"]["unit"]["enum"],
+        }
 
     
     def _add_various_attributes(self,json_dict):
         """
         expose various quantities from mpcorb.json as object attributes
         """
```

### Comparing `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_latest.json` & `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_latest.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999492694805195%*

 * *Differences: {"'properties'": "{'categorization': {'properties': {'object_type_str': {'description': 'Object "*

 * *                 'Type (String): E.g. Minor-Planet / Comet / Dual-Status / Binary MP / etc. For a '*

 * *                 'full description of allowed object types, see '*

 * *                 "https://minorplanetcenter.net/mpcops/documentation/object-types/ '}, "*

 * *                 "'object_type_int': {'description': 'Object Type (Integer): E.g.      "*

 * *                 '0            10       20          1. For a full desc […]*

```diff
@@ -661,55 +661,55 @@
                 "covariance"
             ]
         },
         "categorization": {
             "description": "Various different ways to categorize / sub-set orbit / object types",
             "properties": {
                 "object_type_int": {
-                    "description": "#     0            10       20          1",
+                    "description": "Object Type (Integer): E.g.      0            10       20          1. For a full description of allowed object types, see https://minorplanetcenter.net/mpcops/documentation/object-types/ ",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "object_type_str": {
-                    "description": "# Minor-Planet / Comet / Dual-Status / Binary MP / ...",
+                    "description": "Object Type (String): E.g. Minor-Planet / Comet / Dual-Status / Binary MP / etc. For a full description of allowed object types, see https://minorplanetcenter.net/mpcops/documentation/object-types/ ",
                     "type": "string"
                 },
                 "orbit_subtype_int": {
-                    "description": "# ...",
+                    "description": "Orbit Sub-Type (Integer)",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "orbit_subtype_str": {
-                    "description": "# Apollo / Amor / ...",
+                    "description": "Orbit Sub-Type (String): E.g. Apollo / Amor / ...",
                     "type": "string"
                 },
                 "orbit_type_int": {
-                    "description": "# 0 /1/2/3/4",
+                    "description": "Orbit Type (Integer): E.g. 0 /1/2/3/4/etc. For a full description of allowed orbit types, see https://minorplanetcenter.net/mpcops/documentation/orbit-types/ ",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "orbit_type_str": {
-                    "description": "# NEAs / MBAs / TNOs / ...",
+                    "description": "Orbit Type (String): E.g. NEAs / MBAs / TNOs / etc. For a full description of allowed orbit types, see https://minorplanetcenter.net/mpcops/documentation/orbit-types/ ",
                     "type": "string"
                 },
                 "parent_planet_int": {
-                    "description": "# For Nat-Sats",
+                    "description": "Parent Planet (Integer) if Natural Satellite",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "parent_planet_str": {
-                    "description": "# For Nat-Sats",
+                    "description": "Parent Planet (String) if Natural Satellite",
                     "type": "string"
                 }
             },
             "required": [
                 "object_type_str",
                 "object_type_int",
                 "orbit_type_str",
```

### Comparing `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.1.json` & `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.1.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.2.json` & `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.2.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.3.json` & `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.3.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.4.json` & `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.4.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999492694805195%*

 * *Differences: {"'properties'": "{'categorization': {'properties': {'object_type_str': {'description': 'Object "*

 * *                 'Type (String): E.g. Minor-Planet / Comet / Dual-Status / Binary MP / etc. For a '*

 * *                 'full description of allowed object types, see '*

 * *                 "https://minorplanetcenter.net/mpcops/documentation/object-types/ '}, "*

 * *                 "'object_type_int': {'description': 'Object Type (Integer): E.g.      "*

 * *                 '0            10       20          1. For a full desc […]*

```diff
@@ -661,55 +661,55 @@
                 "covariance"
             ]
         },
         "categorization": {
             "description": "Various different ways to categorize / sub-set orbit / object types",
             "properties": {
                 "object_type_int": {
-                    "description": "#     0            10       20          1",
+                    "description": "Object Type (Integer): E.g.      0            10       20          1. For a full description of allowed object types, see https://minorplanetcenter.net/mpcops/documentation/object-types/ ",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "object_type_str": {
-                    "description": "# Minor-Planet / Comet / Dual-Status / Binary MP / ...",
+                    "description": "Object Type (String): E.g. Minor-Planet / Comet / Dual-Status / Binary MP / etc. For a full description of allowed object types, see https://minorplanetcenter.net/mpcops/documentation/object-types/ ",
                     "type": "string"
                 },
                 "orbit_subtype_int": {
-                    "description": "# ...",
+                    "description": "Orbit Sub-Type (Integer)",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "orbit_subtype_str": {
-                    "description": "# Apollo / Amor / ...",
+                    "description": "Orbit Sub-Type (String): E.g. Apollo / Amor / ...",
                     "type": "string"
                 },
                 "orbit_type_int": {
-                    "description": "# 0 /1/2/3/4",
+                    "description": "Orbit Type (Integer): E.g. 0 /1/2/3/4/etc. For a full description of allowed orbit types, see https://minorplanetcenter.net/mpcops/documentation/orbit-types/ ",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "orbit_type_str": {
-                    "description": "# NEAs / MBAs / TNOs / ...",
+                    "description": "Orbit Type (String): E.g. NEAs / MBAs / TNOs / etc. For a full description of allowed orbit types, see https://minorplanetcenter.net/mpcops/documentation/orbit-types/ ",
                     "type": "string"
                 },
                 "parent_planet_int": {
-                    "description": "# For Nat-Sats",
+                    "description": "Parent Planet (Integer) if Natural Satellite",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "parent_planet_str": {
-                    "description": "# For Nat-Sats",
+                    "description": "Parent Planet (String) if Natural Satellite",
                     "type": "string"
                 }
             },
             "required": [
                 "object_type_str",
                 "object_type_int",
                 "orbit_type_str",
```

### Comparing `mpc_orb-0.1.7/mpc_orb/validate_mpcorb.py` & `mpc_orb-0.1.8/mpc_orb/validate_mpcorb.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/mpc_orb.egg-info/PKG-INFO` & `mpc_orb-0.1.8/mpc_orb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,82 @@
 Metadata-Version: 2.1
 Name: mpc-orb
-Version: 0.1.7
+Version: 0.1.8
 Home-page: https://github.com/Smithsonian/mpc-public
 Author: MJP:MPC
 Author-email: mpayne@cfa.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpc-public/mpc_orb
 
+Documentation and code related to a standardized format for the exchange of data on the *best-fit orbit* for solar-system bodies, including minor-planets, comets, irregular satellites, and interstellar interlopers. 
 
-Code related to the "mpc_orb.json" format.
-
-This format is intended to be used to describe the orbits of solar-system minor-planets, comets, irregular satellites, and interstellar interlopers.
+The format uses JSON files for the exchange of data, and is refered to as the *mpc_orb.json* format.
 
 The MPC currently populates mpc_orb.json files using data from the orbfit package, but we emphasize that the mpc_orb.json format is intended for the generic exchange of orbit data from any source.  
 
 As of April 2023, the latest version of the defining schema is version 0.4
  - While the schema versions are numbered < 1, the format should be considered experimental/developmental/beta/WIP.
 
-The repo currently contains code and documentation related to: 
- - A description of the "mpc_orb.json" format, and an associated defining JSON schema.
- - Python code to demonstrate the validation of files in the "mpc_orb.json" format. 
- - Python code to facilitate the parsing of files in the "mpc_orb.json" format. 
+This repository currently contains code and documentation related to: 
+ - A description of the *mpc_orb.json* format, and an associated defining JSON schema.
+ - Examples of the *mpc_orb.json* format for some specific objects
+ - Python code to demonstrate the validation of files in the *mpc_orb.json* format. 
+ - Python code to facilitate the parsing of files in the *mpc_orb.json* format. 
 
 ## Repo Contents 
 
-(a) demos            
-
- - Demonstrations of python code usage, including *python-scripts* and *jupyter notebooks*.
 
+### Sample JSON Files 
 
-(b) mpc_orb            
+Examples of the *mpc_orb.json* format for some specific objects can be found in */mpc_orb/demo_json*
+ 
 
- - The main python code directory.
+### MPC_ORB JSON schema 
 
- - Contains code to both validate & parse mpc-orb-json files 
+The JSON files defining the *mpc_orb.json* format can be found in */mpc_orb/schema_json*
  
- - Contains directories holding the defining schema (*/mpc_orb/schema_json/*) and sample files (*/mpc_orb/demo_json/*). 
+### Documentation
 
-(c) docs 
+Documentation describing the *mpc_orb.json* format, including *allowed* fields, *required* fields, constraints, etc, can be found in the */docs/* directory.
 
- - Documentation describing the "mpc_orb.json" format, including *allowed* fields, *required* fields, etc
 
-(d) tests
+### Python Functionalities (*/mpc_orb/*)
 
- - Tests of the python code in the *mpc_orb* directory. For details of the test code, including how to execute the tests, please see the file */tests/README.md*.
+The */mpc_orb/* directory contains some python code to both validate & parse mpc-orb-json files 
 
+#### Parsing *mpc_orb.json* formatted data
 
-## MPC_ORB JSON schema 
-
- - The JSON files defining the "mpc_orb.json" format can be found in */mpc_orb/schema_json*
- 
- - Further documentation on the format can be found in */docs/*
+The code in *mpc_orb/parse.py* provides functions & classes to facilitate the parsing of *mpc_orb.json* files in python. 
 
+It is expected that this functionality will be used regularly by both internal MPC staff & external community users.
 
+Some demonstrations of code usage can be found in the */demo/* directory and in the *mpc_orb/demo.py* script.
 
 
-## Python Functionalities (*mpc_orb*)
+#### Validating *mpc_orb.json* files
 
-(i) Provide "parse" functions for JSON files containing "MPC_ORB.JSON" formatted data
+The code in *mpc_orb/parse.py* provides functions & classes to validate *mpc_orb.json* files in python. 
 
- - It is expected that this functionality will be used regularly by both internal MPC staff & external community users.
+It is expected that these validation functionalities will typically be used as part of the "parse" functions described above. 
 
- - The parsing code is in mpc_orb/parse.py
+I.e. it is *not* expected that the end-user will regularly access the validation functions *directly*, but rather, the validation functions will be called under-the-hood by the *mpc_orb/parse.py* routines. 
 
- - Demonstrations of code usage can be found in demo/Example_parse_mpcorb_json.ipynb and demo/demo_parse.py
 
 
-(ii) Provide validation functions
+#### Installation and Usage 
 
- - It is expected that these validation functionalities will typically be used as part of the "parse" functions described in (i) above. 
- 
- - I.e. it is *not* expected that the end-user will directly access the validation functions themselves, but rather, the validation functions are called under-the-hood by the mpc_orb/parse.py routines. 
+The python code in *mpc_orb* is available as a pip-installable python package. 
 
- - The code that performs the validation can be found in mpc_orb/validate_mpcorb.py
+Further details can be found in *mpc_orb/README.md*
 
+ 
 
-## Installation and Usage 
 
-The python code in *mpc_orb* is available as a pip-installable python package. 
-
-To do so the user can type:
-> pip install mpc_orb
+### Python Tests (*/tests/*)
 
+Tests of the python code in the *mpc_orb* directory are provided in the *tests* directory. 
  
+ For details of the test code, including how to execute the tests, please see the file */tests/README.md*.
+
```

### Comparing `mpc_orb-0.1.7/mpc_orb.egg-info/SOURCES.txt` & `mpc_orb-0.1.8/mpc_orb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/setup.py` & `mpc_orb-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mpc_orb',
-    version='0.1.7',
+    version='0.1.8',
     long_description=long_description,  
     long_description_content_type="text/markdown",
     author='MJP:MPC',
     author_email='mpayne@cfa.harvard.edu',
     url='https://github.com/Smithsonian/mpc-public',
     install_requires=[
         'jsonschema',
```

### Comparing `mpc_orb-0.1.7/tests/test_interpret.py` & `mpc_orb-0.1.8/tests/test_interpret.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 def test_interpret_A(  ):
     '''
     Test that an input json filepath is correctly read ...
     '''
     
     # use the schema as an example of a valid json file
     working_dir = os.path.dirname(os.path.abspath(__file__))
+    
     # Loop over the mpcorb files that are expect to "pass"
     valid_jsons = [k for k in filepaths_for_testing.__dict__ if "__" not in k and "pass" in k]
     assert valid_jsons
     for k in valid_jsons:
         full_path = os.path.join(working_dir, filepaths_for_testing.__dict__[k])
         # read it using interpret.interpret()
         d,fp = interpret.interpret(full_path)
@@ -62,15 +63,15 @@
     # read it using interpret.interpret()
     d,fp = interpret.interpret(filepath)
     
 
     
 def test_interpret_D(  ):
     '''
-    Test that an input dictionary ...
+    Test that an input dictionary is correctly interpreted ...
     '''
     
     # use the schema as an example of a valid json file
     # read it using validate_mpcorb.load_json
     d_in = validate_mpcorb.load_schema()
     
     # "read" d using interpret.interpret()
```

### Comparing `mpc_orb-0.1.7/tests/test_parse.py` & `mpc_orb-0.1.8/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.7/tests/test_validation.py` & `mpc_orb-0.1.8/tests/test_validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 Test validation schema
 """
 
-
-
 # Standard imports
 # -----------------------
 import pytest
 import os
 import sys
 import pkgutil
 import json
@@ -24,15 +22,15 @@
     raw_bytes = pkgutil.get_data(__package__ , filepath_relative_to_package)
     return json.loads(raw_bytes.decode('utf-8'))
     
 
 # Lower level tests
 # -----------------------
 def test_schema():
-    ''' Test that the supplied schema is a valid (loadable) json'''
+    ''' Test that the *load_schema* function works ... '''
     assert validate_mpcorb.load_schema(), \
         f'could not open schema'
 
 def test_validation_A():
     ''' Test that a single, valid json-file successfully validates'''
     data_dict = load_package_json(filepaths_for_testing.test_pass_yarkovski)
     assert validate_mpcorb.validate_mpcorb( data_dict ), \
@@ -44,15 +42,15 @@
 # -----------------------
 def test_validation_B(  ):
     '''
     Test that all valid JSON-files in the 'test_pass_mpcorb' directory pass validation as expected
     '''
   
     # Get all of the json filenames defined in filepaths_for_testing that have '...pass...' in the name
-    # NB : At the time of writing there was only one filepath ... in which case test_validation_B == test_validation_A
+    # NB : At the time of writing there was only one filepath ... 
     valid_jsons = [k for k in filepaths_for_testing.__dict__ if "__" not in k and "pass" in k]
     assert valid_jsons
     for k in valid_jsons:
         data_dict = load_package_json(filepaths_for_testing.__dict__[k])
         assert validate_mpcorb.validate_mpcorb( data_dict )
```

