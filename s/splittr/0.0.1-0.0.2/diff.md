# Comparing `tmp/splittr-0.0.1.tar.gz` & `tmp/splittr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splittr-0.0.1.tar", last modified: Sun Apr 30 13:34:53 2023, max compression
+gzip compressed data, was "splittr-0.0.2.tar", last modified: Mon May  1 15:42:18 2023, max compression
```

## Comparing `splittr-0.0.1.tar` & `splittr-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:34:53.963757 splittr-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-30 13:34:42.000000 splittr-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-30 13:34:53.963757 splittr-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 13:34:42.000000 splittr-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 13:34:53.963757 splittr-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3408 2023-04-30 13:34:42.000000 splittr-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:34:53.963757 splittr-0.0.1/splittr/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-30 13:34:42.000000 splittr-0.0.1/splittr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:34:53.963757 splittr-0.0.1/splittr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:42:18.838761 splittr-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 15:42:06.000000 splittr-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 15:42:18.838761 splittr-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 15:42:06.000000 splittr-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:42:18.838761 splittr-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-05-01 15:42:06.000000 splittr-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:42:18.838761 splittr-0.0.2/splittr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-01 15:42:06.000000 splittr-0.0.2/splittr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:42:18.838761 splittr-0.0.2/splittr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/top_level.txt
```

### Comparing `splittr-0.0.1/LICENSE` & `splittr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splittr-0.0.1/setup.py` & `splittr-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -125,8 +125,8 @@
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
 )
-# endregion
+# endregion
```

