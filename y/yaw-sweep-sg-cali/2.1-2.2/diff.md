# Comparing `tmp/yaw_sweep_sg_cali-2.1.tar.gz` & `tmp/yaw_sweep_sg_cali-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaw_sweep_sg_cali-2.1.tar", last modified: Mon May  1 13:14:01 2023, max compression
+gzip compressed data, was "yaw_sweep_sg_cali-2.2.tar", last modified: Mon May  1 13:29:05 2023, max compression
```

## Comparing `yaw_sweep_sg_cali-2.1.tar` & `yaw_sweep_sg_cali-2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:14:01.805669 yaw_sweep_sg_cali-2.1/
--rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-2.1/LICENSE
--rw-rw-rw-   0        0        0    11982 2023-05-01 13:14:01.803645 yaw_sweep_sg_cali-2.1/PKG-INFO
--rw-rw-rw-   0        0        0    11631 2023-05-01 12:43:48.000000 yaw_sweep_sg_cali-2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 13:14:01.806101 yaw_sweep_sg_cali-2.1/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-05-01 13:12:42.000000 yaw_sweep_sg_cali-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:14:01.740388 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/
--rw-rw-rw-   0        0        0     5110 2023-04-29 10:45:54.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Calibration_factors.py
--rw-rw-rw-   0        0        0     9605 2023-04-29 10:58:20.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Curve_fitting.py
--rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Load_data.py
--rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/SQL_utilities.py
--rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py
--rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:14:01.790519 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali.egg-info/
--rw-rw-rw-   0        0        0    11982 2023-05-01 13:14:00.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-01 13:14:01.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:14:00.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-01 13:14:00.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 13:14:00.000000 yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 13:29:05.902397 yaw_sweep_sg_cali-2.2/
+-rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-2.2/LICENSE
+-rw-rw-rw-   0        0        0    11982 2023-05-01 13:29:05.900348 yaw_sweep_sg_cali-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11631 2023-05-01 12:43:48.000000 yaw_sweep_sg_cali-2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 13:29:05.904392 yaw_sweep_sg_cali-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      891 2023-05-01 13:27:46.000000 yaw_sweep_sg_cali-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:29:05.829843 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/
+-rw-rw-rw-   0        0        0     5082 2023-05-01 13:24:28.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Calibration_factors.py
+-rw-rw-rw-   0        0        0     9533 2023-05-01 13:25:44.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Curve_fitting.py
+-rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Load_data.py
+-rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/SQL_utilities.py
+-rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py
+-rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:29:05.888928 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/
+-rw-rw-rw-   0        0        0    11982 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-01 13:29:05.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/top_level.txt
```

### Comparing `yaw_sweep_sg_cali-2.1/LICENSE` & `yaw_sweep_sg_cali-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.1/PKG-INFO` & `yaw_sweep_sg_cali-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw_sweep_sg_cali
-Version: 2.1
+Version: 2.2
 Summary: Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # V52 Tower Strain Gauges Calibration
```

### Comparing `yaw_sweep_sg_cali-2.1/README.md` & `yaw_sweep_sg_cali-2.2/README.md`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.1/setup.py` & `yaw_sweep_sg_cali-2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='yaw_sweep_sg_cali',
-version='2.1',
+version='2.2',
 description='Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.', 
 long_description = long_description,
 long_description_content_type='text/markdown',
 author='Bruno and Zahra',
 author_email='brofa@dtu.dk',
 packages=['yaw_sweep_sg_cali'],
 # packages_data={'yaw_sweep_sg_cali':['Data/V52_1min_data/*.txt', 'Data/V52_50Hz_data/*.txt','Data/V52_inputs.txt']}
```

### Comparing `yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Calibration_factors.py` & `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Calibration_factors.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     folder_package = Path.cwd().joinpath(folder_data)
     file = folder_package.joinpath(file_name)
     # analytical
     if file.exists():
         gain_ana = np.genfromtxt(file, dtype=float, skip_header=28)[0]
     else:
         print('\nThere is no .txt providing the analytical gains for the\
-              get_cali_factors.py to properly convert measured [mV/V] into\
-              [kNm]\n')
+get_cali_factors.py to properly convert measured [mV/V] into\
+[kNm]\n')
         return
     for n in range(len(data_all)):
         data = data_all['Yaw Sweep ' + str(n + 1)]
         data['offset_kNm'] = gain_ana*data['offset']
         data['max_kNm'] = gain_ana*abs(data['amp'])
         data['offset_kNm_unc'] = gain_ana*data['perr'][3]
         dic['Yaw Sweep '+str(n+1)] = data
```

### Comparing `yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Curve_fitting.py` & `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Curve_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,18 +180,18 @@
         dic_one_ys['name'] = [name_ys[0][n], name_ys[1][n]]
         dic_ys['Yaw Sweep ' + str(n + 1)] = dic_one_ys
         if partial_plot and numb_ys <= 20:
             plotting_curve_fitting(MxTB_noisy, time_noisy,
                                    time_cutted, dic_one_ys, idx)
         elif partial_plot and numb_ys > 20 and count:
             print("\nSorry my friend, the curve_fitting_ys\n\
-                  function would generate too many\n\
-                  yaw sweeps plots,try only one\n\
-                  month at a time for the sake\n\
-                  of plotting! :( \n")
+function would generate too many\n\
+yaw sweeps plots,try only one\n\
+month at a time for the sake\n\
+of plotting! :( \n")
             count = False
         if len(warnings_ys) != 0:
             warnings.append(warnings_ys)
     return dic_ys, warnings
 
 
 def plotting_curve_fitting(signal_noisy, time_noisy,
@@ -218,15 +218,15 @@
 
     '''
     time_array_noisy = np.arange(0, int(signal_noisy.size)/50, 0.02)
     amp = dic_one_ys['amp']
     omega = dic_one_ys['omega']
     phase = dic_one_ys['phase']
     offset = dic_one_ys['offset']
-    signal_fitted = amp * np.sin(omega * time_fitted + phase) + offset
+    signal_fitted = amp * np.sin(omega * time_fitted + phase) - offset
     title_from = str(dic_one_ys['name'][0])
     title_to = str(dic_one_ys['name'][1])
     title_aux = 'Fitting noisy signals with sinusoidal\
                  shape \n From file '\
         + title_from + ' to ' + title_to
     fig, ax = plt.subplots(1, clear=True, figsize=(15, 8))
     fig.suptitle(title_aux, fontsize=18)
```

### Comparing `yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Load_data.py` & `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Load_data.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/SQL_utilities.py` & `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/SQL_utilities.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py` & `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.1/yaw_sweep_sg_cali.egg-info/PKG-INFO` & `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw-sweep-sg-cali
-Version: 2.1
+Version: 2.2
 Summary: Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # V52 Tower Strain Gauges Calibration
```

