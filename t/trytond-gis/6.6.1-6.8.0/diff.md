# Comparing `tmp/trytond_gis-6.6.1.tar.gz` & `tmp/trytond_gis-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_gis-6.6.1.tar", last modified: Sat Mar  4 11:06:59 2023, max compression
+gzip compressed data, was "trytond_gis-6.8.0.tar", last modified: Mon May  1 12:07:11 2023, max compression
```

## Comparing `trytond_gis-6.6.1.tar` & `trytond_gis-6.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:06:59.267460 trytond_gis-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1367 2023-03-04 11:06:55.000000 trytond_gis-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      718 2023-03-04 11:06:55.000000 trytond_gis-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-03-04 11:06:59.267460 trytond_gis-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:06:59.264127 trytond_gis-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1597 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:06:59.267460 trytond_gis-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2742 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:06:59.264127 trytond_gis-6.6.1/trytond_gis/
--rw-r--r--   0 ced       (1000) ced       (1000)      557 2022-12-19 12:03:07.000000 trytond_gis-6.6.1/trytond_gis/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/const.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2323 2023-02-23 20:41:08.000000 trytond_gis-6.6.1/trytond_gis/fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:06:59.267460 trytond_gis-6.6.1/trytond_gis/postgis/
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/postgis/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2187 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/postgis/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2924 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/postgis/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/sql.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:06:59.267460 trytond_gis-6.6.1/trytond_gis/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/tests/gis.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2866 2022-12-19 12:02:59.000000 trytond_gis-6.6.1/trytond_gis/tests/test_fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:06:59.267460 trytond_gis-6.6.1/trytond_gis.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-03-04 11:06:58.000000 trytond_gis-6.6.1/trytond_gis.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-03-04 11:06:59.000000 trytond_gis-6.6.1/trytond_gis.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:06:58.000000 trytond_gis-6.6.1/trytond_gis.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-03-04 11:06:58.000000 trytond_gis-6.6.1/trytond_gis.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:06:58.000000 trytond_gis-6.6.1/trytond_gis.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       42 2023-03-04 11:06:58.000000 trytond_gis-6.6.1/trytond_gis.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       12 2023-03-04 11:06:58.000000 trytond_gis-6.6.1/trytond_gis.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:11.498133 trytond_gis-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1429 2023-05-01 11:18:58.000000 trytond_gis-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      723 2023-05-01 11:18:58.000000 trytond_gis-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_gis-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-04-15 07:12:15.000000 trytond_gis-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     1231 2023-05-01 12:07:11.498133 trytond_gis-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-04-15 07:12:16.000000 trytond_gis-6.8.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:11.491466 trytond_gis-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:16.000000 trytond_gis-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-04-15 07:12:16.000000 trytond_gis-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_gis-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:07:11.498133 trytond_gis-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2738 2023-04-15 07:12:15.000000 trytond_gis-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-04-15 07:12:16.000000 trytond_gis-6.8.0/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:11.491466 trytond_gis-6.8.0/trytond_gis/
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2023-05-01 11:18:52.000000 trytond_gis-6.8.0/trytond_gis/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-01-16 14:00:21.000000 trytond_gis-6.8.0/trytond_gis/const.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2323 2023-04-15 07:12:15.000000 trytond_gis-6.8.0/trytond_gis/fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:11.494799 trytond_gis-6.8.0/trytond_gis/postgis/
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:16.000000 trytond_gis-6.8.0/trytond_gis/postgis/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2187 2023-04-15 07:12:16.000000 trytond_gis-6.8.0/trytond_gis/postgis/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2924 2023-04-15 07:12:16.000000 trytond_gis-6.8.0/trytond_gis/postgis/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-01-16 14:00:21.000000 trytond_gis-6.8.0/trytond_gis/sql.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:11.498133 trytond_gis-6.8.0/trytond_gis/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:15.000000 trytond_gis-6.8.0/trytond_gis/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:21.000000 trytond_gis-6.8.0/trytond_gis/tests/gis.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3166 2023-04-15 07:12:15.000000 trytond_gis-6.8.0/trytond_gis/tests/test_fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:11.494799 trytond_gis-6.8.0/trytond_gis.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1231 2023-05-01 12:07:10.000000 trytond_gis-6.8.0/trytond_gis.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-05-01 12:07:11.000000 trytond_gis-6.8.0/trytond_gis.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:07:10.000000 trytond_gis-6.8.0/trytond_gis.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-05-01 12:07:10.000000 trytond_gis-6.8.0/trytond_gis.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_gis-6.8.0/trytond_gis.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       42 2023-05-01 12:07:10.000000 trytond_gis-6.8.0/trytond_gis.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       12 2023-05-01 12:07:10.000000 trytond_gis-6.8.0/trytond_gis.egg-info/top_level.txt
```

### Comparing `trytond_gis-6.6.1/CHANGELOG` & `trytond_gis-6.8.0/CHANGELOG`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 --------------------------
```

### Comparing `trytond_gis-6.6.1/COPYRIGHT` & `trytond_gis-6.8.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (c) 2017-2023 B2CK.
 Copyright (c) 2017-2023 Cédric Krier.
-Copyright (c) 2017 Nicolas Évrard.
+Copyright (c) 2017-2023 Nicolas Évrard.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_gis-6.6.1/LICENSE` & `trytond_gis-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_gis-6.6.1/PKG-INFO` & `trytond_gis-6.8.0/trytond_gis.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
-Name: trytond_gis
-Version: 6.6.1
+Name: trytond-gis
+Version: 6.8.0
 Summary: Adds Geographic Information System support to trytond
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/
+Project-URL: Documentation, https://docs.tryton.org/projects/backend-gis
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/trytond-gis
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton GIS
 Platform: any
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 Tryton GIS backend
 ==================
 
 It adds GIS__ support to Tryton.
```

### Comparing `trytond_gis-6.6.1/doc/conf.py` & `trytond_gis-6.8.0/doc/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     return info
```

### Comparing `trytond_gis-6.6.1/setup.py` & `trytond_gis-6.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,15 @@
     content = read('README.rst')
     content = re.sub(
         r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
     return content
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 def get_version():
     init = read(os.path.join('trytond_gis', '__init__.py'))
@@ -38,50 +35,53 @@
 
 version = get_version()
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_gis'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['geomet', get_require_version('trytond'), 'psycopg2 >= 2.0.14']
 
 setup(name=name,
     version=version,
     description='Adds Geographic Information System support to trytond',
     long_description=readme(),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": 'https://docs.tryton.org/projects/backend-gis',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/trytond-gis',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton GIS',
     packages=find_packages(),
     classifiers=[
         'Framework :: Tryton',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules'
         ],
     platforms='any',
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     entry_points={
         'trytond.backend': [
             'postgis = trytond_gis.postgis',
             ],
         'trytond.tests': [
             'test_geographic_fields = trytond_gis.tests',
```

### Comparing `trytond_gis-6.6.1/trytond_gis/__init__.py` & `trytond_gis-6.8.0/trytond_gis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of trytond_gis.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.config import config
 
 from .const import WGS_84
 
-__version__ = "6.6.1"
+__version__ = "6.8.0"
 
 
 class _GeoJSON(dict):
 
     def __init__(self, *args, **kwargs):
         super(_GeoJSON, self).__init__(*args, **kwargs)
         if 'meta' not in self:
```

### Comparing `trytond_gis-6.6.1/trytond_gis/fields.py` & `trytond_gis-6.8.0/trytond_gis/fields.py`

 * *Files identical despite different names*

### Comparing `trytond_gis-6.6.1/trytond_gis/postgis/database.py` & `trytond_gis-6.8.0/trytond_gis/postgis/database.py`

 * *Files identical despite different names*

### Comparing `trytond_gis-6.6.1/trytond_gis/postgis/table.py` & `trytond_gis-6.8.0/trytond_gis/postgis/table.py`

 * *Files identical despite different names*

### Comparing `trytond_gis-6.6.1/trytond_gis/tests/test_fields.py` & `trytond_gis-6.8.0/trytond_gis/tests/test_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 class TestGeographicFields(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
 
     @with_transaction()
+    def test_fields_get(self):
+        "Test fields_get"
+        pool = Pool()
+
+        GISPoint = pool.get('test.gis.point')
+
+        self.assertDictContainsSubset(
+            {'dimension': 2, 'geometry_type': 'POINT'},
+            GISPoint.fields_get(['point'])['point'])
+
+    @with_transaction()
     def test_create_save(self):
         "Testing create/write with GIS types"
         pool = Pool()
 
         GISPoint = pool.get('test.gis.point')
         point_a = {
             'meta': {'srid': 4326},
```

### Comparing `trytond_gis-6.6.1/trytond_gis.egg-info/PKG-INFO` & `trytond_gis-6.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
-Name: trytond-gis
-Version: 6.6.1
+Name: trytond_gis
+Version: 6.8.0
 Summary: Adds Geographic Information System support to trytond
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/
+Project-URL: Documentation, https://docs.tryton.org/projects/backend-gis
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/trytond-gis
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton GIS
 Platform: any
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 Tryton GIS backend
 ==================
 
 It adds GIS__ support to Tryton.
```

### Comparing `trytond_gis-6.6.1/trytond_gis.egg-info/SOURCES.txt` & `trytond_gis-6.8.0/trytond_gis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

