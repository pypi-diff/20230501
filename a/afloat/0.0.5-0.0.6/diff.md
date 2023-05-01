# Comparing `tmp/afloat-0.0.5.tar.gz` & `tmp/afloat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afloat-0.0.5.tar", last modified: Mon May  1 13:43:04 2023, max compression
+gzip compressed data, was "afloat-0.0.6.tar", last modified: Mon May  1 13:50:48 2023, max compression
```

## Comparing `afloat-0.0.5.tar` & `afloat-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:43:04.882614 afloat-0.0.5/
--rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      239 2023-05-01 13:43:04.880611 afloat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2022-08-09 15:09:43.000000 afloat-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 13:43:04.857609 afloat-0.0.5/afloat/
--rw-rw-rw-   0        0        0      138 2023-05-01 13:42:21.000000 afloat-0.0.5/afloat/__init__.py
--rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.0.5/afloat/bottom_lander.py
--rw-rw-rw-   0        0        0    13218 2022-12-07 02:43:21.000000 afloat-0.0.5/afloat/clean.py
--rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.0.5/afloat/currents.py
--rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.0.5/afloat/netcdf.py
--rw-rw-rw-   0        0        0     7419 2023-04-27 06:11:19.000000 afloat-0.0.5/afloat/operational.py
--rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.0.5/afloat/pca.py
--rw-rw-rw-   0        0        0     1520 2023-04-27 13:53:14.000000 afloat-0.0.5/afloat/sentinel.py
--rw-rw-rw-   0        0        0     1821 2022-01-21 01:42:50.000000 afloat-0.0.5/afloat/shape.py
--rw-rw-rw-   0        0        0    11409 2022-12-06 08:25:41.000000 afloat-0.0.5/afloat/time.py
--rw-rw-rw-   0        0        0    26775 2022-12-07 02:44:11.000000 afloat-0.0.5/afloat/timeseries.py
--rw-rw-rw-   0        0        0     2755 2021-09-22 07:39:10.000000 afloat-0.0.5/afloat/xr.py
--rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.0.5/afloat/xrwrap.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:43:04.877611 afloat-0.0.5/afloat.egg-info/
--rw-rw-rw-   0        0        0      239 2023-05-01 13:43:04.000000 afloat-0.0.5/afloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-05-01 13:43:04.000000 afloat-0.0.5/afloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:43:04.000000 afloat-0.0.5/afloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-01 13:43:04.000000 afloat-0.0.5/afloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 13:43:04.000000 afloat-0.0.5/afloat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 13:43:04.882614 afloat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-05-01 13:42:26.000000 afloat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:50:48.908231 afloat-0.0.6/
+-rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      239 2023-05-01 13:50:48.908231 afloat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1751 2022-08-09 15:09:43.000000 afloat-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 13:50:48.892601 afloat-0.0.6/afloat/
+-rw-rw-rw-   0        0        0      165 2023-05-01 13:45:56.000000 afloat-0.0.6/afloat/__init__.py
+-rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.0.6/afloat/bottom_lander.py
+-rw-rw-rw-   0        0        0    13218 2022-12-07 02:43:21.000000 afloat-0.0.6/afloat/clean.py
+-rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.0.6/afloat/currents.py
+-rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.0.6/afloat/netcdf.py
+-rw-rw-rw-   0        0        0     7419 2023-04-27 06:11:19.000000 afloat-0.0.6/afloat/operational.py
+-rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.0.6/afloat/pca.py
+-rw-rw-rw-   0        0        0     1520 2023-04-27 13:53:14.000000 afloat-0.0.6/afloat/sentinel.py
+-rw-rw-rw-   0        0        0     1821 2022-01-21 01:42:50.000000 afloat-0.0.6/afloat/shape.py
+-rw-rw-rw-   0        0        0    11409 2022-12-06 08:25:41.000000 afloat-0.0.6/afloat/time.py
+-rw-rw-rw-   0        0        0    26775 2022-12-07 02:44:11.000000 afloat-0.0.6/afloat/timeseries.py
+-rw-rw-rw-   0        0        0     2755 2021-09-22 07:39:10.000000 afloat-0.0.6/afloat/xr.py
+-rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.0.6/afloat/xrwrap.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:50:48.908231 afloat-0.0.6/afloat.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-05-01 13:50:48.000000 afloat-0.0.6/afloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-05-01 13:50:48.000000 afloat-0.0.6/afloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:50:48.000000 afloat-0.0.6/afloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-01 13:50:48.000000 afloat-0.0.6/afloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 13:50:48.000000 afloat-0.0.6/afloat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 13:50:48.908231 afloat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-05-01 13:47:53.000000 afloat-0.0.6/setup.py
```

### Comparing `afloat-0.0.5/LICENSE` & `afloat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/README.md` & `afloat-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/bottom_lander.py` & `afloat-0.0.6/afloat/bottom_lander.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/clean.py` & `afloat-0.0.6/afloat/clean.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/currents.py` & `afloat-0.0.6/afloat/currents.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/netcdf.py` & `afloat-0.0.6/afloat/netcdf.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/operational.py` & `afloat-0.0.6/afloat/operational.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/pca.py` & `afloat-0.0.6/afloat/pca.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/sentinel.py` & `afloat-0.0.6/afloat/sentinel.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/shape.py` & `afloat-0.0.6/afloat/shape.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/time.py` & `afloat-0.0.6/afloat/time.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/timeseries.py` & `afloat-0.0.6/afloat/timeseries.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/xr.py` & `afloat-0.0.6/afloat/xr.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/afloat/xrwrap.py` & `afloat-0.0.6/afloat/xrwrap.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.5/setup.py` & `afloat-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class BinaryDistribution(Distribution):
     def is_pure(self):
         return False
 
 		
 setup(name='afloat',
-      version='0.0.5',
+      version='0.0.6',
       description='A Fairly useful Library of Ocean Analysis Tools',
       author='Andrew Zulberti',
       author_email='andrew.zulberti@gmail.com',
       packages=find_packages(),
       install_requires=['numpy',
                         'matplotlib', 
                         'netcdf4',
```

