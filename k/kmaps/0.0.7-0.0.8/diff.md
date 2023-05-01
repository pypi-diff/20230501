# Comparing `tmp/kmaps-0.0.7.tar.gz` & `tmp/kmaps-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmaps-0.0.7.tar", last modified: Mon May  1 00:04:41 2023, max compression
+gzip compressed data, was "kmaps-0.0.8.tar", last modified: Mon May  1 00:14:45 2023, max compression
```

## Comparing `kmaps-0.0.7.tar` & `kmaps-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:04:41.520397 kmaps-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 00:04:24.000000 kmaps-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 00:04:24.000000 kmaps-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:04:41.520397 kmaps-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 00:04:24.000000 kmaps-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:04:41.516397 kmaps-0.0.7/kmaps/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 00:04:24.000000 kmaps-0.0.7/kmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-01 00:04:24.000000 kmaps-0.0.7/kmaps/folmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-05-01 00:04:24.000000 kmaps-0.0.7/kmaps/kmaps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:04:41.516397 kmaps-0.0.7/kmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:04:41.000000 kmaps-0.0.7/kmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 00:04:41.000000 kmaps-0.0.7/kmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:04:41.000000 kmaps-0.0.7/kmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:04:41.000000 kmaps-0.0.7/kmaps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:04:41.000000 kmaps-0.0.7/kmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 00:04:41.000000 kmaps-0.0.7/kmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 00:04:24.000000 kmaps-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 00:04:41.520397 kmaps-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 00:04:24.000000 kmaps-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:14:45.091000 kmaps-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 00:14:29.000000 kmaps-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 00:14:29.000000 kmaps-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:14:45.091000 kmaps-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 00:14:29.000000 kmaps-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:14:45.091000 kmaps-0.0.8/kmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 00:14:29.000000 kmaps-0.0.8/kmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-01 00:14:29.000000 kmaps-0.0.8/kmaps/folmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-05-01 00:14:29.000000 kmaps-0.0.8/kmaps/kmaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:14:45.091000 kmaps-0.0.8/kmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 00:14:29.000000 kmaps-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 00:14:45.091000 kmaps-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 00:14:29.000000 kmaps-0.0.8/setup.py
```

### Comparing `kmaps-0.0.7/LICENSE` & `kmaps-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.7/PKG-INFO` & `kmaps-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmaps
-Version: 0.0.7
+Version: 0.0.8
 Summary: TBA
 Home-page: https://github.com/ChangwhaOh/kmaps
 Author: Changwha Oh
 Author-email: coh4@vols.utk.edu
 License: MIT license
 Keywords: kmaps
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kmaps-0.0.7/README.md` & `kmaps-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.7/kmaps/folmaps.py` & `kmaps-0.0.8/kmaps/folmaps.py`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.7/kmaps/kmaps.py` & `kmaps-0.0.8/kmaps/kmaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,16 +306,17 @@
         import ipywidgets as widgets
 
         widget = widgets.HTML(value = f'<img src="{url}" width = "{width}" height = "{height}">')
         control = WidgetControl(widget = widget, position = position)
         self.add(control)
 
 
-####### just copied from leafmap
+
     def to_streamlit(self, width=None, height=600, scrolling=False, **kwargs):
+        ####### just copied from leafmap
         """Renders map figure in a Streamlit app.
         Args:
             width (int, optional): Width of the map. Defaults to None.
             height (int, optional): Height of the map. Defaults to 600.
             responsive (bool, optional): Whether to make the map responsive. Defaults to True.
             scrolling (bool, optional): If True, show a scrollbar when the content is larger than the iframe. Otherwise, do not show a scrollbar. Defaults to False.
         Returns:
@@ -334,15 +335,15 @@
             #     st.markdown(make_map_responsive, unsafe_allow_html=True)
             return components.html(
                 self.to_html(), width=width, height=height, scrolling=scrolling
             )
 
         except Exception as e:
             raise Exception(e)
-#######     
+    
 
 
 def generate_random_string(length, upper = False, digit = False, punc = False):
     """Generates a random string of a given length.
 
     Args:
         length (int): A length of the string.
```

### Comparing `kmaps-0.0.7/kmaps.egg-info/PKG-INFO` & `kmaps-0.0.8/kmaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmaps
-Version: 0.0.7
+Version: 0.0.8
 Summary: TBA
 Home-page: https://github.com/ChangwhaOh/kmaps
 Author: Changwha Oh
 Author-email: coh4@vols.utk.edu
 License: MIT license
 Keywords: kmaps
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kmaps-0.0.7/setup.py` & `kmaps-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='kmaps',
     name='kmaps',
     packages=find_packages(include=['kmaps', 'kmaps.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChangwhaOh/kmaps',
-    version='0.0.7',
+    version='0.0.8',
     zip_safe=False,
 )
```

