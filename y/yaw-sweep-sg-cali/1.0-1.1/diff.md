# Comparing `tmp/yaw_sweep_sg_cali-1.0.tar.gz` & `tmp/yaw_sweep_sg_cali-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yaw_sweep_sg_cali-1.0.tar", last modified: Mon May  1 09:38:00 2023, max compression
+gzip compressed data, was "dist\yaw_sweep_sg_cali-1.1.tar", last modified: Mon May  1 11:55:07 2023, max compression
```

## Comparing `yaw_sweep_sg_cali-1.0.tar` & `yaw_sweep_sg_cali-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 09:38:00.000000 yaw_sweep_sg_cali-1.0/
--rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-1.0/LICENSE
--rw-rw-rw-   0        0        0    11904 2023-05-01 09:38:00.000000 yaw_sweep_sg_cali-1.0/PKG-INFO
--rw-rw-rw-   0        0        0    11592 2023-05-01 07:45:49.000000 yaw_sweep_sg_cali-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 09:38:00.000000 yaw_sweep_sg_cali-1.0/setup.cfg
--rw-rw-rw-   0        0        0      918 2023-05-01 09:32:48.000000 yaw_sweep_sg_cali-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:38:00.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/
--rw-rw-rw-   0        0        0     5110 2023-04-29 10:45:54.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Calibration_factors.py
--rw-rw-rw-   0        0        0     9605 2023-04-29 10:58:20.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Curve_fitting.py
--rw-rw-rw-   0        0        0    12361 2023-05-01 08:52:59.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Load_data.py
--rw-rw-rw-   0        0        0    15705 2023-05-01 07:45:49.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/SQL_utilities.py
--rw-rw-rw-   0        0        0    10567 2023-04-29 14:15:36.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py
--rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:38:00.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali.egg-info/
--rw-rw-rw-   0        0        0    11904 2023-05-01 09:37:59.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-01 09:37:59.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 09:37:59.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-05-01 09:37:59.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 09:37:59.000000 yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/
+-rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-1.1/LICENSE
+-rw-rw-rw-   0        0        0    11904 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11592 2023-05-01 07:45:49.000000 yaw_sweep_sg_cali-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-05-01 11:52:42.000000 yaw_sweep_sg_cali-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/
+-rw-rw-rw-   0        0        0     5110 2023-04-29 10:45:54.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Calibration_factors.py
+-rw-rw-rw-   0        0        0     9605 2023-04-29 10:58:20.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Curve_fitting.py
+-rw-rw-rw-   0        0        0    12401 2023-05-01 11:33:22.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Load_data.py
+-rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/SQL_utilities.py
+-rw-rw-rw-   0        0        0    10567 2023-04-29 14:15:36.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py
+-rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali.egg-info/
+-rw-rw-rw-   0        0        0    11904 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-01 11:55:07.000000 yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali.egg-info/top_level.txt
```

### Comparing `yaw_sweep_sg_cali-1.0/LICENSE` & `yaw_sweep_sg_cali-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.0/PKG-INFO` & `yaw_sweep_sg_cali-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw_sweep_sg_cali
-Version: 1.0
+Version: 1.1
 Summary: Package to perform strain gauge of wind turbine towers calibration based on idling opeartions, so called, yaw sweeps
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # V52 Tower Strain Gauges Calibration
```

### Comparing `yaw_sweep_sg_cali-1.0/README.md` & `yaw_sweep_sg_cali-1.1/README.md`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.0/setup.py` & `yaw_sweep_sg_cali-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='yaw_sweep_sg_cali',
-version='1.0',
+version='1.1',
 description='Package to perform strain gauge of wind turbine towers calibration based on idling opeartions, so called, yaw sweeps', 
 long_description = long_description,
 long_description_content_type='text/markdown',
 author='Bruno and Zahra',
 author_email='brofa@dtu.dk',
 packages=['yaw_sweep_sg_cali'],
 # packages_data={'yaw_sweep_sg_cali':['Data/V52_1min_data/*.txt', 'Data/V52_50Hz_data/*.txt','Data/V52_inputs.txt']}
```

### Comparing `yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Calibration_factors.py` & `yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Calibration_factors.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Curve_fitting.py` & `yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Curve_fitting.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Load_data.py` & `yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,20 +108,21 @@
                              skiprows=1, unpack=True)
         else:
             if count == 0:
                 I = inputs_SQL()
                 count += 1
                 # cnx = SQLconnect(I)
             downsampling = str(50*60)  # from 50Hz to 1min
+            breakpoint()
             df = get_data_from_SQL(I['user'], I['password'],
                                    '*', I['database'],
                                    ['yaw', 'Wdir_41m', 'WS',
                                     'ROT', 'pitch', 'MxTB', 'name', 'scan_id'],
                                    tablename, I['host'],
-                                   ['`scan_id`%'+downsampling+'3000=0'])
+                                   ['`scan_id`%'+downsampling+'=0'])
             MxTB_m = df['MxTB'].to_numpy()
             yaw_m = df['yaw'].to_numpy()
             ws_m = df['WS'].to_numpy()
             pitch_m = df['pitch'].to_numpy()
             rot_m = df['ROT'].to_numpy()
             scan_id_m = df['scan_id'].to_numpy()
             Wdir_41m_m = df['Wdir_41m'].to_numpy()
@@ -236,14 +237,15 @@
         rotor speed, pitch, wind speed, and
         bending moment. n is equal to the number
         of months loaded.
     Returns
     -------
     None
     """
+    breakpoint()
     name, scan_id, yaw, yaw_err, pitch, rot, ws, MxTB = sensors_to_be_saved
     num_col = len(sensors_to_be_saved)
     final_output = np.empty((name.size, num_col))
     # Add values to the empty array
     final_output[:, 0] = name
     final_output[:, 1] = scan_id
     final_output[:, 2] = yaw
```

### Comparing `yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/SQL_utilities.py` & `yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/SQL_utilities.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py` & `yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.0/yaw_sweep_sg_cali.egg-info/PKG-INFO` & `yaw_sweep_sg_cali-1.1/yaw_sweep_sg_cali.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw-sweep-sg-cali
-Version: 1.0
+Version: 1.1
 Summary: Package to perform strain gauge of wind turbine towers calibration based on idling opeartions, so called, yaw sweeps
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # V52 Tower Strain Gauges Calibration
```

