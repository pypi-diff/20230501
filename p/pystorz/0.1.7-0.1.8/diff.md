# Comparing `tmp/pystorz-0.1.7.tar.gz` & `tmp/pystorz-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.1.7.tar", last modified: Sat Apr 29 21:19:16 2023, max compression
+gzip compressed data, was "dist/pystorz-0.1.8.tar", last modified: Mon May  1 01:22:48 2023, max compression
```

## Comparing `pystorz-0.1.7.tar` & `pystorz-0.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.406955 pystorz-0.1.7/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.7/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-29 21:19:16.406710 pystorz-0.1.7/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.1.7/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.399310 pystorz-0.1.7/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.7/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.400393 pystorz-0.1.7/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.7/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      334 2023-04-29 21:02:22.000000 pystorz-0.1.7/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.401892 pystorz-0.1.7/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.7/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.7/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     6231 2023-04-29 19:33:35.000000 pystorz-0.1.7/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.404218 pystorz-0.1.7/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.7/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.7/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.7/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.7/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.7/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.7/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)      846 2023-04-25 04:12:40.000000 pystorz-0.1.7/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.7/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.7/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.7/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.404669 pystorz-0.1.7/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.7/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)    11696 2023-04-29 21:18:32.000000 pystorz-0.1.7/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.406312 pystorz-0.1.7/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.7/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.1.7/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4437 2023-04-27 06:31:29.000000 pystorz-0.1.7/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2997 2023-04-29 20:57:56.000000 pystorz-0.1.7/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2869 2023-04-29 00:20:58.000000 pystorz-0.1.7/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 21:19:16.400103 pystorz-0.1.7/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-29 21:19:16.000000 pystorz-0.1.7/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-29 21:19:16.000000 pystorz-0.1.7/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-29 21:19:16.000000 pystorz-0.1.7/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-29 21:19:16.000000 pystorz-0.1.7/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-29 21:19:16.000000 pystorz-0.1.7/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-29 21:19:16.407008 pystorz-0.1.7/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-29 21:18:57.000000 pystorz-0.1.7/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.425420 pystorz-0.1.8/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.8/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-01 01:22:48.424780 pystorz-0.1.8/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.1.8/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.417418 pystorz-0.1.8/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.8/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.418490 pystorz-0.1.8/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.8/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      334 2023-04-29 21:02:22.000000 pystorz-0.1.8/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.420008 pystorz-0.1.8/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.8/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.8/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     6231 2023-04-29 19:33:35.000000 pystorz-0.1.8/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.422231 pystorz-0.1.8/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.8/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.8/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.8/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.8/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.8/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.8/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.1.8/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.8/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.8/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.8/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.422578 pystorz-0.1.8/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.8/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    11696 2023-05-01 01:22:26.000000 pystorz-0.1.8/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.424274 pystorz-0.1.8/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.8/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.1.8/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4437 2023-04-27 06:31:29.000000 pystorz-0.1.8/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2997 2023-04-29 20:57:56.000000 pystorz-0.1.8/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2869 2023-04-29 00:20:58.000000 pystorz-0.1.8/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 01:22:48.418216 pystorz-0.1.8/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-01 01:22:48.000000 pystorz-0.1.8/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-05-01 01:22:48.000000 pystorz-0.1.8/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-05-01 01:22:48.000000 pystorz-0.1.8/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-05-01 01:22:48.000000 pystorz-0.1.8/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-05-01 01:22:48.000000 pystorz-0.1.8/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-05-01 01:22:48.425496 pystorz-0.1.8/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-05-01 01:20:25.000000 pystorz-0.1.8/setup.py
```

### Comparing `pystorz-0.1.7/LICENSE` & `pystorz-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/PKG-INFO` & `pystorz-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.1.7/README.md` & `pystorz-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/mgen/builder.py` & `pystorz-0.1.8/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/mgen/loader.py` & `pystorz-0.1.8/pystorz/mgen/loader.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/mgen/templates/structure.py` & `pystorz-0.1.8/pystorz/mgen/templates/structure.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 
 	{% for prop in data.properties %}
 	{% if prop.name != "External" %}
 
 	def Set{{ prop.name }}(self, val):
 		{% if prop.type == "datetime" %}
 		self.{{ prop.name }}_ = utils.datetime_string(val)
+		{% elif prop.type == "string" %}
+		self.{{ prop.name }}_ = str(val)
+		{% elif prop.type == "int" %}
+		self.{{ prop.name }}_ = int(val)
+		{% elif prop.type == "float" %}
+		self.{{ prop.name }}_ = float(val)
+		{% elif prop.type == "bool" %}
+		self.{{ prop.name }}_ = bool(val)
 		{% else %}
 		self.{{ prop.name }}_ = val
 		{% endif %}
 
 	def {{ prop.name }}(self):
 		{% if prop.type == "datetime" %}
 		return utils.datetime_parse(self.{{ prop.name }}_)
```

### Comparing `pystorz-0.1.7/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.1.8/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/mgen/test.py` & `pystorz-0.1.8/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/mgen/utils.py` & `pystorz-0.1.8/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/sql/store.py` & `pystorz-0.1.8/pystorz/sql/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/store/meta.py` & `pystorz-0.1.8/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/store/options.py` & `pystorz-0.1.8/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/store/store.py` & `pystorz-0.1.8/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz/store/utils.py` & `pystorz-0.1.8/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/pystorz.egg-info/PKG-INFO` & `pystorz-0.1.8/pystorz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.1.7/pystorz.egg-info/SOURCES.txt` & `pystorz-0.1.8/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.7/setup.py` & `pystorz-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.1.7',
+    version='0.1.8',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

