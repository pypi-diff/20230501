# Comparing `tmp/linuxp-plugin-1.0.2.tar.gz` & `tmp/linuxp-plugin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxp-plugin-1.0.2.tar", last modified: Fri Apr  7 03:09:08 2023, max compression
+gzip compressed data, was "linuxp-plugin-1.0.3.tar", last modified: Mon May  1 20:19:58 2023, max compression
```

## Comparing `linuxp-plugin-1.0.2.tar` & `linuxp-plugin-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:09:08.158911 linuxp-plugin-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 03:08:47.000000 linuxp-plugin-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-07 03:09:08.158911 linuxp-plugin-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-07 03:08:47.000000 linuxp-plugin-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:09:08.158911 linuxp-plugin-1.0.2/linux_profile_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-07 03:08:47.000000 linuxp-plugin-1.0.2/linux_profile_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-07 03:08:47.000000 linuxp-plugin-1.0.2/linux_profile_plugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-07 03:08:47.000000 linuxp-plugin-1.0.2/linux_profile_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:09:08.158911 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-07 03:09:08.000000 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-07 03:09:08.000000 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 03:09:08.000000 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 03:09:08.000000 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-07 03:09:08.000000 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-07 03:09:08.000000 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 03:09:07.000000 linuxp-plugin-1.0.2/linuxp_plugin.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 03:09:08.158911 linuxp-plugin-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-07 03:08:47.000000 linuxp-plugin-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:58.796107 linuxp-plugin-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 20:19:32.000000 linuxp-plugin-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-01 20:19:58.796107 linuxp-plugin-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-01 20:19:32.000000 linuxp-plugin-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:58.792107 linuxp-plugin-1.0.3/linux_profile_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-01 20:19:32.000000 linuxp-plugin-1.0.3/linux_profile_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-01 20:19:32.000000 linuxp-plugin-1.0.3/linux_profile_plugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-01 20:19:32.000000 linuxp-plugin-1.0.3/linux_profile_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:58.796107 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-01 20:19:58.000000 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-01 20:19:58.000000 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:19:58.000000 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-01 20:19:58.000000 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 20:19:58.000000 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 20:19:58.000000 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:19:58.000000 linuxp-plugin-1.0.3/linuxp_plugin.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:19:58.796107 linuxp-plugin-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-01 20:19:32.000000 linuxp-plugin-1.0.3/setup.py
```

### Comparing `linuxp-plugin-1.0.2/LICENSE` & `linuxp-plugin-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxp-plugin-1.0.2/PKG-INFO` & `linuxp-plugin-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: linuxp-plugin
-Version: 1.0.2
+Version: 1.0.3
 Summary: 🐧 Plugin Linux Profile
 Home-page: https://github.com/linux-profile/linux-profile-plugin
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/linux-profile/linux-profile-plugin/blob/master/docs/linuxp.png?raw=true">
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/linux-profile?label=LinuxProfile&style=flat-square)
```

### Comparing `linuxp-plugin-1.0.2/README.md` & `linuxp-plugin-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `linuxp-plugin-1.0.2/linux_profile_plugin/__init__.py` & `linuxp-plugin-1.0.3/linux_profile_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 __author__ = 'Fernando Celmer <email@fernandocelmer.com>'
 __copyright__ = """MIT License
 
 Copyright (c) 2023 Linux Profile
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `linuxp-plugin-1.0.2/linux_profile_plugin/commands.py` & `linuxp-plugin-1.0.3/linux_profile_plugin/commands.py`

 * *Files identical despite different names*

### Comparing `linuxp-plugin-1.0.2/linux_profile_plugin/main.py` & `linuxp-plugin-1.0.3/linux_profile_plugin/main.py`

 * *Files identical despite different names*

### Comparing `linuxp-plugin-1.0.2/linuxp_plugin.egg-info/PKG-INFO` & `linuxp-plugin-1.0.3/linuxp_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: linuxp-plugin
-Version: 1.0.2
+Version: 1.0.3
 Summary: 🐧 Plugin Linux Profile
 Home-page: https://github.com/linux-profile/linux-profile-plugin
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/linux-profile/linux-profile-plugin/blob/master/docs/linuxp.png?raw=true">
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/linux-profile?label=LinuxProfile&style=flat-square)
```

### Comparing `linuxp-plugin-1.0.2/setup.py` & `linuxp-plugin-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,27 +24,28 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/linux-profile/linux-profile-plugin",
     cmdclass={
         'install': CustomInstallCommand,
     },
     install_requires=[
-        'linuxp>=1.0.16'
+        'linuxp>=1.0.18'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Developers',
         'Natural Language :: English',
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     include_package_data=True,
     python_requires=">=3.6",
     zip_safe=True,
     fullname='linuxp-plugin',
     entry_points={
         'console_scripts': ['linuxp_plugin=linux_profile_plugin.main:main'],
```

