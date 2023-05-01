# Comparing `tmp/asterism-1.0.0.tar.gz` & `tmp/asterism-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asterism-1.0.0.tar", last modified: Mon Apr  3 20:27:07 2023, max compression
+gzip compressed data, was "asterism-1.1.0.tar", last modified: Mon May  1 18:10:08 2023, max compression
```

## Comparing `asterism-1.0.0.tar` & `asterism-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:27:07.356857 asterism-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-03 20:26:49.000000 asterism-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-03 20:27:07.356857 asterism-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-03 20:26:49.000000 asterism-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:27:07.356857 asterism-1.0.0/asterism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/bagit_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:27:07.356857 asterism-1.0.0/asterism/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/tests/test_bagit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/tests/test_file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/view_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-04-03 20:26:49.000000 asterism-1.0.0/asterism/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:27:07.356857 asterism-1.0.0/asterism.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-03 20:27:07.000000 asterism-1.0.0/asterism.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-03 20:27:07.000000 asterism-1.0.0/asterism.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:27:07.000000 asterism-1.0.0/asterism.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:27:07.000000 asterism-1.0.0/asterism.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-03 20:27:07.000000 asterism-1.0.0/asterism.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 20:27:07.000000 asterism-1.0.0/asterism.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 20:27:07.356857 asterism-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-03 20:26:49.000000 asterism-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:10:08.035862 asterism-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-01 18:09:49.000000 asterism-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 18:10:08.035862 asterism-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-01 18:09:49.000000 asterism-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:10:08.035862 asterism-1.1.0/asterism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/bagit_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:10:08.035862 asterism-1.1.0/asterism/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/tests/test_bagit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/tests/test_file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/view_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-05-01 18:09:49.000000 asterism-1.1.0/asterism/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:10:08.035862 asterism-1.1.0/asterism.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 18:10:07.000000 asterism-1.1.0/asterism.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 18:10:08.000000 asterism-1.1.0/asterism.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:10:07.000000 asterism-1.1.0/asterism.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:10:07.000000 asterism-1.1.0/asterism.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 18:10:07.000000 asterism-1.1.0/asterism.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 18:10:07.000000 asterism-1.1.0/asterism.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:10:08.035862 asterism-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-01 18:09:49.000000 asterism-1.1.0/setup.py
```

### Comparing `asterism-1.0.0/LICENSE` & `asterism-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/PKG-INFO` & `asterism-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asterism
-Version: 1.0.0
+Version: 1.1.0
 Summary: Helpers for Project Electron infrastructure
 Home-page: http://github.com/RockefellerArchiveCenter/asterism
 Author: Rockefeller Archive Center
 Author-email: archive@rockarch.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `asterism-1.0.0/README.md` & `asterism-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/bagit_helpers.py` & `asterism-1.1.0/asterism/bagit_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Validates a bag against the BagIt specification"""
     bag = bagit.Bag(bag_path)
     return bag.validate()
 
 
 def update_bag_info(bag_path, data):
     """Adds metadata from a dictionary to `bag-info.txt`"""
-    assert(isinstance(data, dict))
+    assert isinstance(data, dict)
     bag = bagit.Bag(bag_path)
     for k, v in data.items():
         bag.info[k] = v
     bag.save()
 
 
 def update_manifests(bag_path):
```

### Comparing `asterism-1.0.0/asterism/file_helpers.py` & `asterism-1.1.0/asterism/file_helpers.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/models.py` & `asterism-1.1.0/asterism/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         max_length=50,
         choices=TYPE_CHOICES,
         null=True,
         blank=True)
     ORIGIN_CHOICES = (
         ('aurora', 'Aurora'),
         ('legacy_digital', 'Legacy Digital Processing'),
-        ('digitization', 'Digitization')
+        ('digitization', 'Digitization'),
+        ('av_digitization', 'Audiovisual Digitization')
     )
     origin = models.CharField(
         max_length=20,
         choices=ORIGIN_CHOICES,
         default='aurora')
     PROCESS_STATUS_CHOICES = (None)
     process_status = models.IntegerField(choices=PROCESS_STATUS_CHOICES)
```

### Comparing `asterism-1.0.0/asterism/tests/helpers.py` & `asterism-1.1.0/asterism/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/tests/test_bagit.py` & `asterism-1.1.0/asterism/tests/test_bagit.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/tests/test_file_helpers.py` & `asterism-1.1.0/asterism/tests/test_file_helpers.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/tests/test_models.py` & `asterism-1.1.0/asterism/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/tests/test_views.py` & `asterism-1.1.0/asterism/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/view_mixins.py` & `asterism-1.1.0/asterism/view_mixins.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism/views.py` & `asterism-1.1.0/asterism/views.py`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/asterism.egg-info/PKG-INFO` & `asterism-1.1.0/asterism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asterism
-Version: 1.0.0
+Version: 1.1.0
 Summary: Helpers for Project Electron infrastructure
 Home-page: http://github.com/RockefellerArchiveCenter/asterism
 Author: Rockefeller Archive Center
 Author-email: archive@rockarch.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `asterism-1.0.0/asterism.egg-info/SOURCES.txt` & `asterism-1.1.0/asterism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asterism-1.0.0/setup.py` & `asterism-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='asterism',
-      version='1.0.0',
+      version='1.1.0',
       description='Helpers for Project Electron infrastructure',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='http://github.com/RockefellerArchiveCenter/asterism',
       author='Rockefeller Archive Center',
       author_email='archive@rockarch.org',
       install_requires=[
```

