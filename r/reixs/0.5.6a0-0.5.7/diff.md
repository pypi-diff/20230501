# Comparing `tmp/reixs-0.5.6a0.tar.gz` & `tmp/reixs-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.5.6a0.tar", last modified: Fri Apr 21 21:40:12 2023, max compression
+gzip compressed data, was "reixs-0.5.7.tar", last modified: Mon May  1 20:54:07 2023, max compression
```

## Comparing `reixs-0.5.6a0.tar` & `reixs-0.5.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:40:12.292426 reixs-0.5.6a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-21 21:39:58.000000 reixs-0.5.6a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-04-21 21:40:12.292426 reixs-0.5.6a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-21 21:39:58.000000 reixs-0.5.6a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 21:39:58.000000 reixs-0.5.6a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-21 21:40:12.292426 reixs-0.5.6a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:40:12.284426 reixs-0.5.6a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:40:12.288426 reixs-0.5.6a0/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    59076 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/beamline_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-21 21:39:58.000000 reixs-0.5.6a0/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:40:12.292426 reixs-0.5.6a0/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-04-21 21:40:12.000000 reixs-0.5.6a0/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 21:40:12.000000 reixs-0.5.6a0/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:40:12.000000 reixs-0.5.6a0/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-21 21:40:12.000000 reixs-0.5.6a0/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 21:40:12.000000 reixs-0.5.6a0/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:07.507561 reixs-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 20:53:49.000000 reixs-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-05-01 20:54:07.507561 reixs-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-01 20:53:49.000000 reixs-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 20:53:49.000000 reixs-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-01 20:54:07.507561 reixs-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:07.495561 reixs-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:07.503561 reixs-0.5.7/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    59076 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33022 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-01 20:53:49.000000 reixs-0.5.7/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:07.507561 reixs-0.5.7/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-05-01 20:54:07.000000 reixs-0.5.7/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-01 20:54:07.000000 reixs-0.5.7/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:54:07.000000 reixs-0.5.7/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 20:54:07.000000 reixs-0.5.7/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 20:54:07.000000 reixs-0.5.7/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.5.6a0/LICENSE` & `reixs-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/PKG-INFO` & `reixs-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.6a0
+Version: 0.5.7
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.6a0/README.md` & `reixs-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/setup.cfg` & `reixs-0.5.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.5.6a
+version = 0.5.7
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls =
```

### Comparing `reixs-0.5.6a0/src/reixs/LoadData.py` & `reixs-0.5.7/src/reixs/LoadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/ReadData.py` & `reixs-0.5.7/src/reixs/ReadData.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,16 +345,19 @@
                     info_dict[key] = dict()
                     for k in f.keys():
                         if k.startswith("SCAN_"):  # Groups must start with the SCAN prefix
                             try:
                                 info_dict[key][int(
                                     k.split("_")[1])] = f[f'{k}/{key}'][()].decode("utf-8")
                             except AttributeError:
+                                entry = f[f'{k}/{key}'][()]
+                                if isinstance(entry, np.ndarray) and len(entry)==1:
+                                    entry = entry[0]
                                 info_dict[key][int(
-                                    k.split("_")[1])] = f[f'{k}/{key}'][()]
+                                    k.split("_")[1])] = entry
 
         except:
             raise KeyError("Error opening and processing file.")
 
         return info_dict
```

### Comparing `reixs-0.5.6a0/src/reixs/add_subtract.py` & `reixs-0.5.7/src/reixs/add_subtract.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/beamline_info.py` & `reixs-0.5.7/src/reixs/beamline_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,17 +56,20 @@
 
 def get_spreadsheet(basedir, file, columns=None):
     if columns == None:
         columns = dict()
 
         #columns['Sample'] = 'command'
         columns['Command'] = 'command'
-        #columns['Dwell'] = 'command'
-        columns['Spectrometer'] = 'Endstation/Motors/detz'
-        columns['Flux'] = 'Beamline/Apertures/4-Jaw_2/horz_gap'
+        columns['Sample Stage (ssh)'] = 'Endstation/Motors/ssh'
+        columns['Sample Stage (ssv)'] = 'Endstation/Motors/ssv'
+        columns['Sample Stage (ssd)'] = 'Endstation/Motors/ssd'
+        columns['Spectrometer (XES dist)'] = 'Endstation/Motors/spd'
+        columns['Spectrometer (XES angl)'] = 'Endstation/Motors/spa'
+        columns['Flux 4-Jaw (mm)'] = 'Beamline/Apertures/4-Jaw_2/horz_gap'
         columns['Mono Grating'] = '/Beamline/Monochromator/grating'
         columns['Mono Mirror'] = '/Beamline/Monochromator/mirror'
         columns['Polarization'] = 'Beamline/Source/EPU/Polarization'
         #columns['Comment'] = 'command'
         columns['Status'] = 'status'
 
     info = REIXS(basedir, file).Info(list(columns.values()))
```

### Comparing `reixs-0.5.6a0/src/reixs/mca.py` & `reixs-0.5.7/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/mesh.py` & `reixs-0.5.7/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/parser.py` & `reixs-0.5.7/src/reixs/parser.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/rixs_readutil.py` & `reixs-0.5.7/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/rsxs_mcp.py` & `reixs-0.5.7/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/rsxs_readutil.py` & `reixs-0.5.7/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/sca.py` & `reixs-0.5.7/src/reixs/sca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/simplemath.py` & `reixs-0.5.7/src/reixs/simplemath.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/spec_config.py` & `reixs-0.5.7/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/util.py` & `reixs-0.5.7/src/reixs/util.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs/xeol.py` & `reixs-0.5.7/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.6a0/src/reixs.egg-info/PKG-INFO` & `reixs-0.5.7/src/reixs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.6a0
+Version: 0.5.7
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.6a0/src/reixs.egg-info/SOURCES.txt` & `reixs-0.5.7/src/reixs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

