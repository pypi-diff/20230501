# Comparing `tmp/yaw_sweep_sg_cali-1.2.tar.gz` & `tmp/yaw_sweep_sg_cali-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaw_sweep_sg_cali-1.2.tar", last modified: Mon May  1 12:15:17 2023, max compression
+gzip compressed data, was "yaw_sweep_sg_cali-2.0.tar", last modified: Mon May  1 12:55:56 2023, max compression
```

## Comparing `yaw_sweep_sg_cali-1.2.tar` & `yaw_sweep_sg_cali-2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:15:17.902012 yaw_sweep_sg_cali-1.2/
--rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-1.2/LICENSE
--rw-rw-rw-   0        0        0    11904 2023-05-01 12:15:17.902012 yaw_sweep_sg_cali-1.2/PKG-INFO
--rw-rw-rw-   0        0        0    11592 2023-05-01 07:45:49.000000 yaw_sweep_sg_cali-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 12:15:17.902012 yaw_sweep_sg_cali-1.2/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-05-01 12:12:15.000000 yaw_sweep_sg_cali-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:15:17.864253 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/
--rw-rw-rw-   0        0        0     5110 2023-04-29 10:45:54.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Calibration_factors.py
--rw-rw-rw-   0        0        0     9605 2023-04-29 10:58:20.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Curve_fitting.py
--rw-rw-rw-   0        0        0    12401 2023-05-01 11:33:22.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Load_data.py
--rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/SQL_utilities.py
--rw-rw-rw-   0        0        0    10567 2023-04-29 14:15:36.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py
--rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:15:17.886392 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali.egg-info/
--rw-rw-rw-   0        0        0    11904 2023-05-01 12:15:17.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-01 12:15:17.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:15:17.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-01 12:15:17.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 12:15:17.000000 yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 12:55:55.998424 yaw_sweep_sg_cali-2.0/
+-rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-2.0/LICENSE
+-rw-rw-rw-   0        0        0    11956 2023-05-01 12:55:55.997424 yaw_sweep_sg_cali-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11631 2023-05-01 12:43:48.000000 yaw_sweep_sg_cali-2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 12:55:55.998424 yaw_sweep_sg_cali-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-05-01 12:49:54.000000 yaw_sweep_sg_cali-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:55:55.970279 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/
+-rw-rw-rw-   0        0        0     5110 2023-04-29 10:45:54.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Calibration_factors.py
+-rw-rw-rw-   0        0        0     9605 2023-04-29 10:58:20.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Curve_fitting.py
+-rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Load_data.py
+-rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/SQL_utilities.py
+-rw-rw-rw-   0        0        0    10567 2023-04-29 14:15:36.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py
+-rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:55:55.994215 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali.egg-info/
+-rw-rw-rw-   0        0        0    11956 2023-05-01 12:55:55.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-01 12:55:55.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 12:55:55.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-01 12:55:55.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-01 12:55:55.000000 yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali.egg-info/top_level.txt
```

### Comparing `yaw_sweep_sg_cali-1.2/LICENSE` & `yaw_sweep_sg_cali-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.2/PKG-INFO` & `yaw_sweep_sg_cali-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: yaw_sweep_sg_cali
-Version: 1.2
-Summary: Package to perform strain gauge of wind turbine towers calibration based on idling opeartions, so called, yaw sweeps
+Version: 2.0
+Summary: Package to perform the strain gauge calibration placed on wind turbine towers based on idling opeartions, so called, yaw sweeps
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # V52 Tower Strain Gauges Calibration
 
 ## Dear dear user, this tool requires the installation of the toolbox Mysqlclient 2.1.1.
 
 Installation:
 ```
 pip install mysqlclient
-```  
+```
+![image1](Images/PseudoCode_Chart.PNG)
+  
 ## Project Overview:
 
 Tower strain gauges are commonly used in wind turbine applications to measure the strain on the tower or structure. To ensure accurate readings for a V52 wind turbine, it is important to regularly calibrate these gauges.This project aims to develop an automatic routine to generate strain gauge calibration factors for around 5 years (2018 to 2023), considering zero drift. The validation of the recordings will be pursued through specific idling operations, so called **Yaw Sweeps**.
 - The research wind turbine V52:
 
 The research wind turbine V52 from Vestas is situated at DTU RisÃ¸ Campus as a part of the row of wind turbines at the fjord. The 850 kW wind turbine arrived at DTU in 2015.- [DTU Wind and Energy Systems](https://wind.dtu.dk/Facilities/The-research-wind-turbine-V52) 
 - Database:
@@ -26,19 +28,14 @@
 To perform the project the databases used to test (SQL):
 
 	- SCADA data from V52 and data from RisÃ¸ met mast.
 	- Strain measures from V52 tower 
 - Package stepwise:
 First, identify yaw sweep operations, in which the aerodynamic contribution to the tower bending moment is negligible (low wind speed). Secondly, using such operations, automatically curve fits the raw bending moment signal and extracts relavant information, as max, min, and mean values. Finally, generate recommended calibration factors (offsets). The number of yaw sweeps operation throughout a year is unknown. 
 
-## Improvements performed from first submission to final submission
-
-- The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
-- The code was check with pycodestyle, to ensure was properly with the recommended standards. 
-- PEP 257 information added to each function
 
 ## Getting Started - How it works
 This is a Python package for identifying and calibrating yaw sweeps in wind turbines. The package includes four main modules:
 
 - Load_data: for loading the 1-minute and 50Hz data from SQL or local source.
 - Yaw_sweep_identification: for identifying the yaw sweep instants based on name and scan_id.
 - Curve_fitting: for fitting sinusoidal curves to the yaw sweep data to extract max, min, mean, and error values.
@@ -132,15 +129,15 @@
 
 ```
 git clone  https://github.com/username/yaw-sweep-sg-cali.git
 cd yaw-sweep-sg-cali
 pip install -r requirements.txt
 ```
 The package can be installed using pip:
-	- [ ] $ git clone https://github.com/username/yaw-sweep-sg-cali.git
+	- [ ]  git clone https://github.com/username/yaw-sweep-sg-cali.git
 	- [ ]  cd yaw-sweep-sg-cali
 	- [ ]  pip install -r requirements.txt
 
 
 
 ## Add your files
 
@@ -183,7 +180,12 @@
 
 ## Authors and acknowledgment
 Show your appreciation to those who have contributed to the project.
 
 ## License
 This code is licensed under the MIT License.
 
+## Improvements performed from first submission to final submission
+
+- The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
+- The code was check with pycodestyle, to ensure was properly with the recommended standards. 
+- PEP 257 information added to each function
```

### Comparing `yaw_sweep_sg_cali-1.2/README.md` & `yaw_sweep_sg_cali-2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # V52 Tower Strain Gauges Calibration
 
 ## Dear dear user, this tool requires the installation of the toolbox Mysqlclient 2.1.1.
 
 Installation:
 ```
 pip install mysqlclient
-```  
+```
+![image1](Images/PseudoCode_Chart.PNG)
+  
 ## Project Overview:
 
 Tower strain gauges are commonly used in wind turbine applications to measure the strain on the tower or structure. To ensure accurate readings for a V52 wind turbine, it is important to regularly calibrate these gauges.This project aims to develop an automatic routine to generate strain gauge calibration factors for around 5 years (2018 to 2023), considering zero drift. The validation of the recordings will be pursued through specific idling operations, so called **Yaw Sweeps**.
 - The research wind turbine V52:
 
 The research wind turbine V52 from Vestas is situated at DTU Risø Campus as a part of the row of wind turbines at the fjord. The 850 kW wind turbine arrived at DTU in 2015.- [DTU Wind and Energy Systems](https://wind.dtu.dk/Facilities/The-research-wind-turbine-V52) 
 - Database:
@@ -17,19 +19,14 @@
 To perform the project the databases used to test (SQL):
 
 	- SCADA data from V52 and data from Risø met mast.
 	- Strain measures from V52 tower 
 - Package stepwise:
 First, identify yaw sweep operations, in which the aerodynamic contribution to the tower bending moment is negligible (low wind speed). Secondly, using such operations, automatically curve fits the raw bending moment signal and extracts relavant information, as max, min, and mean values. Finally, generate recommended calibration factors (offsets). The number of yaw sweeps operation throughout a year is unknown. 
 
-## Improvements performed from first submission to final submission
-
-- The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
-- The code was check with pycodestyle, to ensure was properly with the recommended standards. 
-- PEP 257 information added to each function
 
 ## Getting Started - How it works
 This is a Python package for identifying and calibrating yaw sweeps in wind turbines. The package includes four main modules:
 
 - Load_data: for loading the 1-minute and 50Hz data from SQL or local source.
 - Yaw_sweep_identification: for identifying the yaw sweep instants based on name and scan_id.
 - Curve_fitting: for fitting sinusoidal curves to the yaw sweep data to extract max, min, mean, and error values.
@@ -123,15 +120,15 @@
 
 ```
 git clone  https://github.com/username/yaw-sweep-sg-cali.git
 cd yaw-sweep-sg-cali
 pip install -r requirements.txt
 ```
 The package can be installed using pip:
-	- [ ] $ git clone https://github.com/username/yaw-sweep-sg-cali.git
+	- [ ]  git clone https://github.com/username/yaw-sweep-sg-cali.git
 	- [ ]  cd yaw-sweep-sg-cali
 	- [ ]  pip install -r requirements.txt
 
 
 
 ## Add your files
 
@@ -174,7 +171,12 @@
 
 ## Authors and acknowledgment
 Show your appreciation to those who have contributed to the project.
 
 ## License
 This code is licensed under the MIT License.
 
+## Improvements performed from first submission to final submission
+
+- The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
+- The code was check with pycodestyle, to ensure was properly with the recommended standards. 
+- PEP 257 information added to each function
```

### Comparing `yaw_sweep_sg_cali-1.2/setup.py` & `yaw_sweep_sg_cali-2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='yaw_sweep_sg_cali',
-version='1.2',
-description='Package to perform strain gauge of wind turbine towers calibration based on idling opeartions, so called, yaw sweeps', 
+version='2.0',
+description='Package to perform the strain gauge calibration placed on wind turbine towers based on idling opeartions, so called, yaw sweeps', 
 long_description = long_description,
 long_description_content_type='text/markdown',
 author='Bruno and Zahra',
 author_email='brofa@dtu.dk',
 packages=['yaw_sweep_sg_cali'],
 # packages_data={'yaw_sweep_sg_cali':['Data/V52_1min_data/*.txt', 'Data/V52_50Hz_data/*.txt','Data/V52_inputs.txt']}
 install_requires = [
```

### Comparing `yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Calibration_factors.py` & `yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Calibration_factors.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Curve_fitting.py` & `yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Curve_fitting.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Load_data.py` & `yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
                              skiprows=1, unpack=True)
         else:
             if count == 0:
                 I = inputs_SQL()
                 count += 1
                 # cnx = SQLconnect(I)
             downsampling = str(50*60)  # from 50Hz to 1min
-            breakpoint()
             df = get_data_from_SQL(I['user'], I['password'],
                                    '*', I['database'],
                                    ['yaw', 'Wdir_41m', 'WS',
                                     'ROT', 'pitch', 'MxTB', 'name', 'scan_id'],
                                    tablename, I['host'],
                                    ['`scan_id`%'+downsampling+'=0'])
             MxTB_m = df['MxTB'].to_numpy()
@@ -237,15 +236,14 @@
         rotor speed, pitch, wind speed, and
         bending moment. n is equal to the number
         of months loaded.
     Returns
     -------
     None
     """
-    breakpoint()
     name, scan_id, yaw, yaw_err, pitch, rot, ws, MxTB = sensors_to_be_saved
     num_col = len(sensors_to_be_saved)
     final_output = np.empty((name.size, num_col))
     # Add values to the empty array
     final_output[:, 0] = name
     final_output[:, 1] = scan_id
     final_output[:, 2] = yaw
@@ -257,14 +255,15 @@
     year_i = str(name[0])[0:4]
     month_i = calendar.month_name[int(str(name[0])[4:6])]
     # Creating a directory only for the first
     output_file = year_i + '_' + month_i + '_V52_data_1min.txt'
     output_path1 = 'Data'
     output_path2 = 'V52_1min_data'
     folder_package = Path.cwd().joinpath(output_path1)
+    folder_package.mkdir(exist_ok=True)
     output_path = folder_package.joinpath(output_path2)
     output_path.mkdir(exist_ok=True)
     output = output_path.joinpath(output_file)
     # Setting the header of the output
     header = 'Name(-)\tscan_id(-)\tyaw(deg)\tyaw_err(deg)\
     \tpitch(deg)\tROT(rpm)\tWS(m/s)\tMxTB(mV/V)'
     np.savetxt(output, final_output,
@@ -307,14 +306,15 @@
     final_output[:, 1] = scan_id
     final_output[:, 2] = MxTB
     final_output[:, 3] = ws
     output_file = '{}_to_{}_V52_data_50Hz.txt'.format(name_from, name_to)
     output_path1 = 'Data'
     output_path2 = 'V52_50Hz_data'
     folder_package = Path.cwd().joinpath(output_path1)
+    folder_package.mkdir(exist_ok=True)
     output_path = folder_package.joinpath(output_path2)
     output_path.mkdir(parents=True, exist_ok=True)
     output = output_path.joinpath(output_file)
     # Setting the header of the output
     header = 'Name(-)\tscan_id(-)\tMxTB(mV/V)\tws(m/s)'
     np.savetxt(output, final_output, fmt=("%d", "%d",
                                           "%.8f", "%.2f"), header=header,
```

### Comparing `yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/SQL_utilities.py` & `yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/SQL_utilities.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py` & `yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-1.2/yaw_sweep_sg_cali.egg-info/PKG-INFO` & `yaw_sweep_sg_cali-2.0/yaw_sweep_sg_cali.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: yaw-sweep-sg-cali
-Version: 1.2
-Summary: Package to perform strain gauge of wind turbine towers calibration based on idling opeartions, so called, yaw sweeps
+Version: 2.0
+Summary: Package to perform the strain gauge calibration placed on wind turbine towers based on idling opeartions, so called, yaw sweeps
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # V52 Tower Strain Gauges Calibration
 
 ## Dear dear user, this tool requires the installation of the toolbox Mysqlclient 2.1.1.
 
 Installation:
 ```
 pip install mysqlclient
-```  
+```
+![image1](Images/PseudoCode_Chart.PNG)
+  
 ## Project Overview:
 
 Tower strain gauges are commonly used in wind turbine applications to measure the strain on the tower or structure. To ensure accurate readings for a V52 wind turbine, it is important to regularly calibrate these gauges.This project aims to develop an automatic routine to generate strain gauge calibration factors for around 5 years (2018 to 2023), considering zero drift. The validation of the recordings will be pursued through specific idling operations, so called **Yaw Sweeps**.
 - The research wind turbine V52:
 
 The research wind turbine V52 from Vestas is situated at DTU RisÃ¸ Campus as a part of the row of wind turbines at the fjord. The 850 kW wind turbine arrived at DTU in 2015.- [DTU Wind and Energy Systems](https://wind.dtu.dk/Facilities/The-research-wind-turbine-V52) 
 - Database:
@@ -26,19 +28,14 @@
 To perform the project the databases used to test (SQL):
 
 	- SCADA data from V52 and data from RisÃ¸ met mast.
 	- Strain measures from V52 tower 
 - Package stepwise:
 First, identify yaw sweep operations, in which the aerodynamic contribution to the tower bending moment is negligible (low wind speed). Secondly, using such operations, automatically curve fits the raw bending moment signal and extracts relavant information, as max, min, and mean values. Finally, generate recommended calibration factors (offsets). The number of yaw sweeps operation throughout a year is unknown. 
 
-## Improvements performed from first submission to final submission
-
-- The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
-- The code was check with pycodestyle, to ensure was properly with the recommended standards. 
-- PEP 257 information added to each function
 
 ## Getting Started - How it works
 This is a Python package for identifying and calibrating yaw sweeps in wind turbines. The package includes four main modules:
 
 - Load_data: for loading the 1-minute and 50Hz data from SQL or local source.
 - Yaw_sweep_identification: for identifying the yaw sweep instants based on name and scan_id.
 - Curve_fitting: for fitting sinusoidal curves to the yaw sweep data to extract max, min, mean, and error values.
@@ -132,15 +129,15 @@
 
 ```
 git clone  https://github.com/username/yaw-sweep-sg-cali.git
 cd yaw-sweep-sg-cali
 pip install -r requirements.txt
 ```
 The package can be installed using pip:
-	- [ ] $ git clone https://github.com/username/yaw-sweep-sg-cali.git
+	- [ ]  git clone https://github.com/username/yaw-sweep-sg-cali.git
 	- [ ]  cd yaw-sweep-sg-cali
 	- [ ]  pip install -r requirements.txt
 
 
 
 ## Add your files
 
@@ -183,7 +180,12 @@
 
 ## Authors and acknowledgment
 Show your appreciation to those who have contributed to the project.
 
 ## License
 This code is licensed under the MIT License.
 
+## Improvements performed from first submission to final submission
+
+- The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
+- The code was check with pycodestyle, to ensure was properly with the recommended standards. 
+- PEP 257 information added to each function
```

