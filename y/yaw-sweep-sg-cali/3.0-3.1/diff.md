# Comparing `tmp/yaw_sweep_sg_cali-3.0.tar.gz` & `tmp/yaw_sweep_sg_cali-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaw_sweep_sg_cali-3.0.tar", last modified: Mon May  1 16:49:40 2023, max compression
+gzip compressed data, was "yaw_sweep_sg_cali-3.1.tar", last modified: Mon May  1 16:53:57 2023, max compression
```

## Comparing `yaw_sweep_sg_cali-3.0.tar` & `yaw_sweep_sg_cali-3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 16:49:40.635230 yaw_sweep_sg_cali-3.0/
--rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-3.0/LICENSE
--rw-rw-rw-   0        0        0      533 2023-05-01 16:49:40.634231 yaw_sweep_sg_cali-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     9922 2023-05-01 16:40:38.000000 yaw_sweep_sg_cali-3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 16:49:40.636226 yaw_sweep_sg_cali-3.0/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-05-01 16:49:32.000000 yaw_sweep_sg_cali-3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 16:49:40.578987 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/
--rw-rw-rw-   0        0        0     5082 2023-05-01 13:24:28.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Calibration_factors.py
--rw-rw-rw-   0        0        0     9533 2023-05-01 13:25:44.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Curve_fitting.py
--rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Load_data.py
--rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/SQL_utilities.py
--rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py
--rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 16:49:40.631262 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/
--rw-rw-rw-   0        0        0      533 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 16:53:57.428768 yaw_sweep_sg_cali-3.1/
+-rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-3.1/LICENSE
+-rw-rw-rw-   0        0        0      533 2023-05-01 16:53:57.427424 yaw_sweep_sg_cali-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9922 2023-05-01 16:40:38.000000 yaw_sweep_sg_cali-3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 16:53:57.428768 yaw_sweep_sg_cali-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-05-01 16:53:46.000000 yaw_sweep_sg_cali-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:53:57.388801 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/
+-rw-rw-rw-   0        0        0     5082 2023-05-01 13:24:28.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Calibration_factors.py
+-rw-rw-rw-   0        0        0     9533 2023-05-01 13:25:44.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Curve_fitting.py
+-rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Load_data.py
+-rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/SQL_utilities.py
+-rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py
+-rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:53:57.424237 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/top_level.txt
```

### Comparing `yaw_sweep_sg_cali-3.0/LICENSE` & `yaw_sweep_sg_cali-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.0/PKG-INFO` & `yaw_sweep_sg_cali-3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw_sweep_sg_cali
-Version: 3.0
+Version: 3.1
 Summary: Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Please Refer To The Gitlab page:
```

### Comparing `yaw_sweep_sg_cali-3.0/README.md` & `yaw_sweep_sg_cali-3.1/README.md`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.0/setup.py` & `yaw_sweep_sg_cali-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory1 = Path(__file__).parent
 this_directory = this_directory1.joinpath('yaw_sweep_sg_cali')
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='yaw_sweep_sg_cali',
-version='3.0',
+version='3.1',
 description='Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.', 
 long_description = long_description,
 long_description_content_type='text/markdown',
 author='Bruno and Zahra',
 author_email='brofa@dtu.dk',
 packages=['yaw_sweep_sg_cali'],
 # packages_data={'yaw_sweep_sg_cali':['Data/V52_1min_data/*.txt', 'Data/V52_50Hz_data/*.txt','Data/V52_inputs.txt']}
```

### Comparing `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Calibration_factors.py` & `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Calibration_factors.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Curve_fitting.py` & `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Curve_fitting.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Load_data.py` & `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Load_data.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/SQL_utilities.py` & `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/SQL_utilities.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py` & `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/PKG-INFO` & `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw-sweep-sg-cali
-Version: 3.0
+Version: 3.1
 Summary: Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Please Refer To The Gitlab page:
```

