# Comparing `tmp/toxicjasmine-0.2.tar.gz` & `tmp/toxicjasmine-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toxicjasmine-0.2.tar", last modified: Tue Apr  7 19:15:12 2020, max compression
+gzip compressed data, was "toxicjasmine-0.2.1.tar", last modified: Mon May  1 03:10:09 2023, max compression
```

## Comparing `toxicjasmine-0.2.tar` & `toxicjasmine-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2020-04-07 19:15:12.000000 toxicjasmine-0.2/
--rw-r--r--   0 juca      (1000) juca      (1000)       70 2018-08-11 02:44:49.000000 toxicjasmine-0.2/MANIFEST.in
--rw-r--r--   0 juca      (1000) juca      (1000)      629 2020-04-07 19:15:12.000000 toxicjasmine-0.2/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)       38 2020-04-07 19:15:12.000000 toxicjasmine-0.2/setup.cfg
--rw-r--r--   0 juca      (1000) juca      (1000)     1073 2020-04-07 19:13:58.000000 toxicjasmine-0.2/setup.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine/
--rw-r--r--   0 juca      (1000) juca      (1000)       26 2018-08-11 03:30:01.000000 toxicjasmine-0.2/toxicjasmine/README
--rw-r--r--   0 juca      (1000) juca      (1000)     7824 2020-02-09 21:08:29.000000 toxicjasmine-0.2/toxicjasmine/__init__.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine/__pycache__/
--rw-r--r--   0 juca      (1000) juca      (1000)     8044 2020-04-07 19:09:17.000000 toxicjasmine-0.2/toxicjasmine/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 juca      (1000) juca      (1000)     6227 2020-04-07 19:05:23.000000 toxicjasmine-0.2/toxicjasmine/boot.js
--rw-r--r--   0 juca      (1000) juca      (1000)    20494 2018-08-11 02:42:53.000000 toxicjasmine-0.2/toxicjasmine/jasmine-clear.css
--rw-r--r--   0 juca      (1000) juca      (1000)    20591 2018-08-11 02:42:53.000000 toxicjasmine-0.2/toxicjasmine/jasmine-dark.css
--rw-r--r--   0 juca      (1000) juca      (1000)    23571 2020-04-07 19:05:23.000000 toxicjasmine-0.2/toxicjasmine/jasmine-html.js
--rw-r--r--   0 juca      (1000) juca      (1000)    21115 2020-04-07 19:06:11.000000 toxicjasmine-0.2/toxicjasmine/jasmine.css
--rw-r--r--   0 juca      (1000) juca      (1000)   232520 2020-04-07 19:05:23.000000 toxicjasmine-0.2/toxicjasmine/jasmine.js
--rw-r--r--   0 juca      (1000) juca      (1000)    17569 2020-04-07 19:05:23.000000 toxicjasmine-0.2/toxicjasmine/json2.js
--rw-r--r--   0 juca      (1000) juca      (1000)     1491 2020-04-07 19:05:23.000000 toxicjasmine-0.2/toxicjasmine/node_boot.js
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine.egg-info/
--rw-r--r--   0 juca      (1000) juca      (1000)      629 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine.egg-info/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)      540 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine.egg-info/SOURCES.txt
--rw-r--r--   0 juca      (1000) juca      (1000)        1 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine.egg-info/dependency_links.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       53 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine.egg-info/entry_points.txt
--rw-r--r--   0 juca      (1000) juca      (1000)        8 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine.egg-info/requires.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       13 2020-04-07 19:15:12.000000 toxicjasmine-0.2/toxicjasmine.egg-info/top_level.txt
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/
+-rw-rw-r--   0 juca      (1001) juca      (1001)       70 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/MANIFEST.in
+-rw-rw-r--   0 juca      (1001) juca      (1001)      594 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/setup.cfg
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1168 2023-05-01 03:09:29.000000 toxicjasmine-0.2.1/setup.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/toxicjasmine/
+-rw-rw-r--   0 juca      (1001) juca      (1001)       26 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/README
+-rw-rw-r--   0 juca      (1001) juca      (1001)     7914 2023-05-01 03:08:27.000000 toxicjasmine-0.2.1/toxicjasmine/__init__.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)     6227 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/boot.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)    20494 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine-clear.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    20591 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine-dark.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    23571 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine-html.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)    21115 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)   232520 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)    17569 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/json2.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)     2198 2023-05-01 03:07:50.000000 toxicjasmine-0.2.1/toxicjasmine/monkey.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1491 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/node_boot.js
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/toxicjasmine.egg-info/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      594 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      514 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/SOURCES.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)        1 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/dependency_links.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       52 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/entry_points.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       68 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/requires.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       13 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toxicjasmine-0.2/PKG-INFO` & `toxicjasmine-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: toxicjasmine
-Version: 0.2
+Version: 0.2.1
 Summary: Toxicjasmine: Nothing interresting here.
-Home-page: UNKNOWN
+Home-page: 
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: GPL
-Description: Toxicjasmine: Nothing interresting here.
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Provides: toxicjasmine
+
+Toxicjasmine: Nothing interresting here.
```

### Comparing `toxicjasmine-0.2/setup.py` & `toxicjasmine-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
-VERSION = '0.2'
+VERSION = '0.2.1'
 
 DESCRIPTION = """
 Toxicjasmine: Nothing interresting here.
 """.strip()
 
 
 setup(name='toxicjasmine',
@@ -15,15 +15,16 @@
       author_email='juca@poraodojuca.net',
       url='',
       description=DESCRIPTION,
       long_description=DESCRIPTION,
       packages=find_packages(exclude=['tests', 'tests.*']),
       license='GPL',
       include_package_data=True,
-      install_requires=['jasmine'],
+      install_requires=['jasmine==3.5.0', 'jasmine-core==3.5.0',
+                        'Jinja2==2.10.3', 'markupsafe==2.0.1'],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Environment :: No Input/Output (Daemon)',
           'Environment :: Web Environment',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: GNU General Public License (GPL)',
           'Natural Language :: English',
```

### Comparing `toxicjasmine-0.2/toxicjasmine/__init__.py` & `toxicjasmine-0.2.1/toxicjasmine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,8 +226,11 @@
     else:
         args = sys.argv[1:]
 
     cmd.run(args)
 
 
 if __name__ == '__main__':
+    from .monkey import MonkeyPatcher
+    monkey = MonkeyPatcher()
+    monkey.patch_all()
     begin()
```

### Comparing `toxicjasmine-0.2/toxicjasmine/boot.js` & `toxicjasmine-0.2.1/toxicjasmine/boot.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine/jasmine-clear.css` & `toxicjasmine-0.2.1/toxicjasmine/jasmine-clear.css`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine/jasmine-dark.css` & `toxicjasmine-0.2.1/toxicjasmine/jasmine-dark.css`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine/jasmine-html.js` & `toxicjasmine-0.2.1/toxicjasmine/jasmine-html.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine/jasmine.css` & `toxicjasmine-0.2.1/toxicjasmine/jasmine.css`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine/jasmine.js` & `toxicjasmine-0.2.1/toxicjasmine/jasmine.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine/json2.js` & `toxicjasmine-0.2.1/toxicjasmine/json2.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine/node_boot.js` & `toxicjasmine-0.2.1/toxicjasmine/node_boot.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2/toxicjasmine.egg-info/PKG-INFO` & `toxicjasmine-0.2.1/toxicjasmine.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: toxicjasmine
-Version: 0.2
+Version: 0.2.1
 Summary: Toxicjasmine: Nothing interresting here.
-Home-page: UNKNOWN
+Home-page: 
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: GPL
-Description: Toxicjasmine: Nothing interresting here.
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Provides: toxicjasmine
+
+Toxicjasmine: Nothing interresting here.
```

### Comparing `toxicjasmine-0.2/toxicjasmine.egg-info/SOURCES.txt` & `toxicjasmine-0.2.1/toxicjasmine.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 toxicjasmine/boot.js
 toxicjasmine/jasmine-clear.css
 toxicjasmine/jasmine-dark.css
 toxicjasmine/jasmine-html.js
 toxicjasmine/jasmine.css
 toxicjasmine/jasmine.js
 toxicjasmine/json2.js
+toxicjasmine/monkey.py
 toxicjasmine/node_boot.js
 toxicjasmine.egg-info/PKG-INFO
 toxicjasmine.egg-info/SOURCES.txt
 toxicjasmine.egg-info/dependency_links.txt
 toxicjasmine.egg-info/entry_points.txt
 toxicjasmine.egg-info/requires.txt
-toxicjasmine.egg-info/top_level.txt
-toxicjasmine/__pycache__/__init__.cpython-37.pyc
+toxicjasmine.egg-info/top_level.txt
```

