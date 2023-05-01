# Comparing `tmp/afloat-0.0.8.tar.gz` & `tmp/afloat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afloat-0.0.8.tar", last modified: Mon May  1 14:21:51 2023, max compression
+gzip compressed data, was "afloat-0.0.9.tar", last modified: Mon May  1 14:29:18 2023, max compression
```

## Comparing `afloat-0.0.8.tar` & `afloat-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:21:51.701277 afloat-0.0.8/
--rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      239 2023-05-01 14:21:51.700275 afloat-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2022-08-09 15:09:43.000000 afloat-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 14:21:51.597254 afloat-0.0.8/afloat/
--rw-rw-rw-   0        0        0      221 2023-05-01 14:20:35.000000 afloat-0.0.8/afloat/__init__.py
--rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.0.8/afloat/bottom_lander.py
--rw-rw-rw-   0        0        0    13218 2022-12-07 02:43:21.000000 afloat-0.0.8/afloat/clean.py
--rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.0.8/afloat/currents.py
--rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.0.8/afloat/netcdf.py
--rw-rw-rw-   0        0        0     7419 2023-04-27 06:11:19.000000 afloat-0.0.8/afloat/operational.py
--rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.0.8/afloat/pca.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:21:51.645262 afloat-0.0.8/afloat/plot/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.8/afloat/plot/__init__.py
--rw-rw-rw-   0        0        0     6711 2023-03-03 13:23:31.000000 afloat-0.0.8/afloat/plot/gif.py
--rw-rw-rw-   0        0        0    15402 2022-08-16 12:11:30.000000 afloat-0.0.8/afloat/plot/plotting.py
--rw-rw-rw-   0        0        0     1520 2023-04-27 13:53:14.000000 afloat-0.0.8/afloat/sentinel.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:21:51.661267 afloat-0.0.8/afloat/sfodautils/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.8/afloat/sfodautils/__init__.py
--rw-rw-rw-   0        0        0     8537 2023-05-01 13:37:05.000000 afloat-0.0.8/afloat/sfodautils/harmonic_analysis.py
--rw-rw-rw-   0        0        0     1821 2022-01-21 01:42:50.000000 afloat-0.0.8/afloat/shape.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:21:51.677271 afloat-0.0.8/afloat/tides/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.8/afloat/tides/__init__.py
--rw-rw-rw-   0        0        0    12795 2022-08-09 16:36:10.000000 afloat-0.0.8/afloat/tides/cons.py
--rw-rw-rw-   0        0        0    11409 2022-12-06 08:25:41.000000 afloat-0.0.8/afloat/time.py
--rw-rw-rw-   0        0        0    26775 2022-12-07 02:44:11.000000 afloat-0.0.8/afloat/timeseries.py
--rw-rw-rw-   0        0        0     2755 2021-09-22 07:39:10.000000 afloat-0.0.8/afloat/xr.py
--rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.0.8/afloat/xrwrap.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:21:51.698274 afloat-0.0.8/afloat/xutils/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.8/afloat/xutils/__init__.py
--rw-rw-rw-   0        0        0    26195 2022-02-28 02:28:59.000000 afloat-0.0.8/afloat/xutils/windrose.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:21:51.615257 afloat-0.0.8/afloat.egg-info/
--rw-rw-rw-   0        0        0      239 2023-05-01 14:21:51.000000 afloat-0.0.8/afloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-05-01 14:21:51.000000 afloat-0.0.8/afloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:21:51.000000 afloat-0.0.8/afloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-01 14:21:51.000000 afloat-0.0.8/afloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 14:21:51.000000 afloat-0.0.8/afloat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 14:21:51.702277 afloat-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-05-01 14:21:05.000000 afloat-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.746236 afloat-0.0.9/
+-rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      239 2023-05-01 14:29:18.744235 afloat-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1751 2022-08-09 15:09:43.000000 afloat-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.696240 afloat-0.0.9/afloat/
+-rw-rw-rw-   0        0        0      240 2023-05-01 14:28:14.000000 afloat-0.0.9/afloat/__init__.py
+-rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.0.9/afloat/bottom_lander.py
+-rw-rw-rw-   0        0        0    13218 2022-12-07 02:43:21.000000 afloat-0.0.9/afloat/clean.py
+-rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.0.9/afloat/currents.py
+-rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.0.9/afloat/netcdf.py
+-rw-rw-rw-   0        0        0     7419 2023-04-27 06:11:19.000000 afloat-0.0.9/afloat/operational.py
+-rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.0.9/afloat/pca.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.719244 afloat-0.0.9/afloat/plot/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/plot/__init__.py
+-rw-rw-rw-   0        0        0     6711 2023-03-03 13:23:31.000000 afloat-0.0.9/afloat/plot/gif.py
+-rw-rw-rw-   0        0        0    15402 2022-08-16 12:11:30.000000 afloat-0.0.9/afloat/plot/plotting.py
+-rw-rw-rw-   0        0        0     1520 2023-04-27 13:53:14.000000 afloat-0.0.9/afloat/sentinel.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.725245 afloat-0.0.9/afloat/sfodautils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/sfodautils/__init__.py
+-rw-rw-rw-   0        0        0     8537 2023-05-01 13:37:05.000000 afloat-0.0.9/afloat/sfodautils/harmonic_analysis.py
+-rw-rw-rw-   0        0        0     1821 2022-01-21 01:42:50.000000 afloat-0.0.9/afloat/shape.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.732248 afloat-0.0.9/afloat/tides/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/tides/__init__.py
+-rw-rw-rw-   0        0        0    12795 2022-08-09 16:36:10.000000 afloat-0.0.9/afloat/tides/cons.py
+-rw-rw-rw-   0        0        0    11409 2022-12-06 08:25:41.000000 afloat-0.0.9/afloat/time.py
+-rw-rw-rw-   0        0        0    26775 2022-12-07 02:44:11.000000 afloat-0.0.9/afloat/timeseries.py
+-rw-rw-rw-   0        0        0     2755 2021-09-22 07:39:10.000000 afloat-0.0.9/afloat/xr.py
+-rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.0.9/afloat/xrwrap.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.739234 afloat-0.0.9/afloat/xutils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/xutils/__init__.py
+-rw-rw-rw-   0        0        0    26195 2022-02-28 02:28:59.000000 afloat-0.0.9/afloat/xutils/windrose.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.712242 afloat-0.0.9/afloat.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 14:29:18.747236 afloat-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-05-01 14:28:46.000000 afloat-0.0.9/setup.py
```

### Comparing `afloat-0.0.8/LICENSE` & `afloat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/README.md` & `afloat-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/bottom_lander.py` & `afloat-0.0.9/afloat/bottom_lander.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/clean.py` & `afloat-0.0.9/afloat/clean.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/currents.py` & `afloat-0.0.9/afloat/currents.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/netcdf.py` & `afloat-0.0.9/afloat/netcdf.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/operational.py` & `afloat-0.0.9/afloat/operational.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/pca.py` & `afloat-0.0.9/afloat/pca.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/plot/gif.py` & `afloat-0.0.9/afloat/plot/gif.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/plot/plotting.py` & `afloat-0.0.9/afloat/plot/plotting.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/sentinel.py` & `afloat-0.0.9/afloat/sentinel.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/sfodautils/harmonic_analysis.py` & `afloat-0.0.9/afloat/sfodautils/harmonic_analysis.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/shape.py` & `afloat-0.0.9/afloat/shape.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/tides/cons.py` & `afloat-0.0.9/afloat/tides/cons.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/time.py` & `afloat-0.0.9/afloat/time.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/timeseries.py` & `afloat-0.0.9/afloat/timeseries.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/xr.py` & `afloat-0.0.9/afloat/xr.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/xrwrap.py` & `afloat-0.0.9/afloat/xrwrap.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat/xutils/windrose.py` & `afloat-0.0.9/afloat/xutils/windrose.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/afloat.egg-info/SOURCES.txt` & `afloat-0.0.9/afloat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `afloat-0.0.8/setup.py` & `afloat-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class BinaryDistribution(Distribution):
     def is_pure(self):
         return False
 
 		
 setup(name='afloat',
-      version='0.0.8',
+      version='0.0.9',
       description='A Fairly useful Library of Ocean Analysis Tools',
       author='Andrew Zulberti',
       author_email='andrew.zulberti@gmail.com',
       packages=find_packages(),
       install_requires=['numpy',
                         'matplotlib', 
                         'netcdf4',
```

