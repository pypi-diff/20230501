# Comparing `tmp/yaw_sweep_sg_cali-2.2.tar.gz` & `tmp/yaw_sweep_sg_cali-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaw_sweep_sg_cali-2.2.tar", last modified: Mon May  1 13:29:05 2023, max compression
+gzip compressed data, was "yaw_sweep_sg_cali-3.0.tar", last modified: Mon May  1 16:49:40 2023, max compression
```

## Comparing `yaw_sweep_sg_cali-2.2.tar` & `yaw_sweep_sg_cali-3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:29:05.902397 yaw_sweep_sg_cali-2.2/
--rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-2.2/LICENSE
--rw-rw-rw-   0        0        0    11982 2023-05-01 13:29:05.900348 yaw_sweep_sg_cali-2.2/PKG-INFO
--rw-rw-rw-   0        0        0    11631 2023-05-01 12:43:48.000000 yaw_sweep_sg_cali-2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 13:29:05.904392 yaw_sweep_sg_cali-2.2/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-05-01 13:27:46.000000 yaw_sweep_sg_cali-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:29:05.829843 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/
--rw-rw-rw-   0        0        0     5082 2023-05-01 13:24:28.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Calibration_factors.py
--rw-rw-rw-   0        0        0     9533 2023-05-01 13:25:44.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Curve_fitting.py
--rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Load_data.py
--rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/SQL_utilities.py
--rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py
--rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:29:05.888928 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/
--rw-rw-rw-   0        0        0    11982 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-01 13:29:05.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 13:29:04.000000 yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 16:49:40.635230 yaw_sweep_sg_cali-3.0/
+-rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-3.0/LICENSE
+-rw-rw-rw-   0        0        0      533 2023-05-01 16:49:40.634231 yaw_sweep_sg_cali-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9922 2023-05-01 16:40:38.000000 yaw_sweep_sg_cali-3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 16:49:40.636226 yaw_sweep_sg_cali-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-05-01 16:49:32.000000 yaw_sweep_sg_cali-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:49:40.578987 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/
+-rw-rw-rw-   0        0        0     5082 2023-05-01 13:24:28.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Calibration_factors.py
+-rw-rw-rw-   0        0        0     9533 2023-05-01 13:25:44.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Curve_fitting.py
+-rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Load_data.py
+-rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/SQL_utilities.py
+-rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py
+-rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:49:40.631262 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-01 16:49:39.000000 yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali.egg-info/top_level.txt
```

### Comparing `yaw_sweep_sg_cali-2.2/LICENSE` & `yaw_sweep_sg_cali-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.2/PKG-INFO` & `yaw_sweep_sg_cali-3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,191 +1,234 @@
-Metadata-Version: 2.1
-Name: yaw_sweep_sg_cali
-Version: 2.2
-Summary: Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.
-Author: Bruno and Zahra
-Author-email: brofa@dtu.dk
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # V52 Tower Strain Gauges Calibration
 
-## Dear dear user, this tool requires the installation of the toolbox Mysqlclient 2.1.1.
+***Note:*** Let's have a look on the [V52 Tower Strain Gauges Calibration project](https://gitlab.windenergy.dtu.dk/brofa/v52-strain-gauge-calibration/-/tree/main/) if you want to keep track on the commits. 
+
+
+## Installation:
 
-Installation:
 ```
-pip install mysqlclient
+pip install yaw-sweep-sg-cali
+
+Note: Python 3.8 is the minimum requirement version.
+
 ```
-![image1](Images/PseudoCode_Chart.PNG)
-  
+Note: In case there is no Data already available [Data](https://gitlab.windenergy.dtu.dk/brofa/v52-strain-gauge-calibration/-/tree/main/Data) and V52 is the wanted turbine, remember to connect DTU VPN.
+
+
 ## Project Overview:
 
-Tower strain gauges are commonly used in wind turbine applications to measure the strain on the tower or structure. To ensure accurate readings for a V52 wind turbine, it is important to regularly calibrate these gauges.This project aims to develop an automatic routine to generate strain gauge calibration factors for around 5 years (2018 to 2023), considering zero drift. The validation of the recordings will be pursued through specific idling operations, so called **Yaw Sweeps**.
-- The research wind turbine V52:
+Tower strain gauges are commonly used in wind turbine applications to measure the strain on the tower or structure. To ensure accurate readings, it is important to regularly calibrate these gauges. This project aims to develop an automatic routine to generate strain gauge calibration factors (offset and gain) for a given amount of input time-series, considering the zero drift. The validation of the recordings will be pursued through specific idling operations, so called **Yaw Sweeps**. 
+
+bruno- commet yaw sweep
+
+
+## Repo files 
+
+- ***main.py*** is an example applied for DTU V52 using around 4 years of data. The code is built to be generalizable so that it can be used for different time ranges (from 2018 to 2022). 
+- ***yaw_sweep_sg_cali*** contains the modules from the package  could be used to calibrate strain gauges in any wind turbine tower.
+- ***how_to_use.ipynb*** is a Jupyter notebook with an input of only one month. This will facilitate the user to understand the code and  visualize two partial results: the yaw sweep identification and the curve fitting.
+- ***Data*** contains already loaded and saved DTU V52 SQL data(1 min and 50Hz) that will be used (using also Load_data.py). The idea is to save time and help the user to visualize the functioning of the package. This will be further commented below.
+
+
+## The research wind turbine V52
+
+The research wind turbine V52 from Vestas is situated at DTU Risø Campus as a part of the row of wind turbines at the fjord. The 850 kW wind turbine arrived at DTU in 2015.- [DTU Wind and Energy Systems](https://wind.dtu.dk/Facilities/The-research-wind-turbine-V52) 
 
-The research wind turbine V52 from Vestas is situated at DTU RisÃ¸ Campus as a part of the row of wind turbines at the fjord. The 850 kW wind turbine arrived at DTU in 2015.- [DTU Wind and Energy Systems](https://wind.dtu.dk/Facilities/The-research-wind-turbine-V52) 
 - Database:
 
 To perform the project the databases used to test (SQL):
 
-	- SCADA data from V52 and data from RisÃ¸ met mast.
+	- SCADA data from V52 and data from Risø met mast.
 	- Strain measures from V52 tower 
+	
 - Package stepwise:
+
 First, identify yaw sweep operations, in which the aerodynamic contribution to the tower bending moment is negligible (low wind speed). Secondly, using such operations, automatically curve fits the raw bending moment signal and extracts relavant information, as max, min, and mean values. Finally, generate recommended calibration factors (offsets). The number of yaw sweeps operation throughout a year is unknown. 
 
+# Lets start running the code :) 
+
+## main.py: Getting Started - How it works
+
+***Please make sure to have the "Data" folder as in the repo. Since, if not included, the code will ask for V52 DTU SQL login information. And not just that, but each month of data can take around 5min to be loaded. For the sake of testing, we provided the operational data already, for both 1min and 50Hz data. But feel free to remove data and test the SQL routines***
+
+The package includes four main modules:
+
+- ***Load_data.py***: for loading the 1-minute and 50Hz data from SQL or local source.
+- ***Yaw_sweep_identification.py***: for identifying the yaw sweep instants based on the linear behavior of the yaw; and triggers of rotor speed and blade pitch.
+- ***Curve_fitting.py***: for fitting sinusoidal curves to the bending moment (strain gauge) while in a yaw sweep operation to extract max, min, mean, and error values.
+- ***Calibration_factor.py***: for calculating the calibration factors (offset, gain, and wind speed) for the yaw sensors in kNm.
+
+
+In the following section, we will provide a detailed explanation of the main.py file.
 
-## Getting Started - How it works
-This is a Python package for identifying and calibrating yaw sweeps in wind turbines. The package includes four main modules:
+ 
 
-- Load_data: for loading the 1-minute and 50Hz data from SQL or local source.
-- Yaw_sweep_identification: for identifying the yaw sweep instants based on name and scan_id.
-- Curve_fitting: for fitting sinusoidal curves to the yaw sweep data to extract max, min, mean, and error values.
-- Calibration_factors: for calculating the calibration factors (offset, gain, and wind speed) for the yaw sensors.
-
-### Step 1:User Input
-- start (YYYY,MM)
-- stop (YYYY,MM)
+### Step 1: User Input
 
 The following variables are required to be defined by the user:
 
-start: A tuple of the form (year, month) representing the start time period for analysis.
-stop: A tuple of the form (year, month) representing the end time period for analysis.
-turbine_file: The name of the file containing turbine data that will be used for calibration factors.
-### Step 2:First Data loading (SQL or Local)
+- start: A tuple 
+
+of the form (year, month) representing the start time period for analysis.
+
+- stop: A tuple 
+
+of the form (year, month) representing the end time period for analysis.
+
+- turbine_file: 
+
+The name of the file containing turbine data that will be used for calibration factors.
+
+### Step 2: First Data loading (SQL or Local)(get_SQL_1_min)
+
  This code loads data either from a local source or from an SQL database. It uses the function get_SQL_1_min(start, stop) from the module yaw_sweep_sg_cali.Load_data.
+ 
 #### Inputs
-- start: A tuple representing the start date and time for the data to be loaded in the format (year, month).
-- stop: A tuple representing the stop date and time for the data to be loaded in the format (year, month).
+
+- start: A tuple 
+
+representing the start date and time for the data to be loaded in the format (year, month).
+
+- stop: A tuple 
+
+representing the stop date and time for the data to be loaded in the format (year, month).
+
 #### Outputs
-- data_1_min: A pandas DataFrame containing the loaded data.
-Note: The specific source of the data (local or SQL) is determined by the implementation of the get_SQL_1_min() function, and is not directly controlled by the user through these inputs
-### Step 3:Identifying the Yaw Sweep (ys) instants based on name and scan_id
+
+- data_1_min: A pandas DataFrame 
+
+containing the loaded data.
+
+**Note:**
+ The specific source of the data (local or SQL) is determined by the implementation of the get_SQL_1_min() function, and is not directly controlled by the user through these inputs
+
+### Step 3: Identifying the Yaw Sweep (ys) instants based on name and scan_id (identify_yaw_sweep)
+
 This code line identifies the Yaw Sweep (ys) instants based on the input data data_1_min. It returns three variables name_ys, scan_id_ys, and numb_ys.
+
 #### Inputs
-- data_1_min: Input data to be analyzed to identify the yaw sweep.
+
+- sensors : tuble with lists
+
+Each list contains n number of numpy arrays, n equal to the number of months loaded.
+
+The sensors should include: name, scan_id, yaw, rotor speed, pitch, wind speed, bending moment.
+
+- partial_plot : bool, optional
+
+If true, plot the identified yaw sweeps. The default is False.
+
+Obs: we only plot in case one month is analayzed. Otherwise, the
+chart would not be clear.
+
+***Note***
+
+If the input is less than three months, the program will execute successfully. However, if the input exceeds three months, the program will display a message to the user indicating that it cannot visualize the results for such a large timeframe. This is simply to help users understand the limitations of the program 
 
 #### Outputs
-- name_ys: Name of the Yaw Sweep.
-- scan_id_ys: Scan ID of the Yaw Sweep.
-- numb_ys: Number of Yaw Sweeps present in the input data.
-#### Parameters
-- partial_plot: A Boolean parameter. If it's True, the partial plot will be shown during the analysis
-### Step 4:Second Data Loading (SQL or Local) for calibration factors
-get_SQL_50_Hz function loads data at 50Hz from the SQL database for yaw sweep data that was previously identified using identify_yaw_sweep function.
+
+- name_ys : array of int
+
+contains the a 2xn, where 2 is for the initial and end name, and n is for the number of ys.
+
+- scan_id_ys : array of int
+
+contains the a 2xn, where 2 is for the initial and end scan_id, and n is for the number of ys.
+
+- numb_ys : int
+
+number of identified ys
+
+### Step 4: Second Data Loading (SQL or Local) for calibration factors(get_SQL_50_Hz)
+
+Retrieves 1-minute data from an SQL database or local files. This function retrieves 1-minute data from an SQL database or from local files if available. If local files are not available, the function accesses the SQL database and saves the data in the correct format for future use. The data is organized by month, and each month takes approximately 5-10 minutes to load from the SQL database, but less than a second to load from local files.
+   
 #### Inputs
-- name_ys: the name of the data file containing yaw sweep data
-- scan_id_ys: the ID of the scan where yaw sweep data is stored
-- db_connection_string (optional): a connection string for connecting to the SQL database. If not provided, the function will use a default connection string.
+
+- start : tuple of int
+
+containing the year and month to start data retrieval.
+
+- stop : tuple of int
+
+containing the year and month to stop data retrieval (non-inclusive).
 
 #### Outputs
-- data_50_Hz: a pandas DataFrame containing the 50Hz yaw sweep data
-### Step 4: Fitting Sinus to extract max, min, mean, errs of curve fitting
+
+- data_50_Hz: a pandas DataFrame 
+
+containing the 50Hz yaw sweep data.
+
+### Step 5: Fitting Sinus to extract max, min, mean, errs of curve fitting(curve_fitting_ys)
+
 The curve_fitting_ys function in this module fits a sinusoidal curve to the yaw sweep data and returns the maximum, minimum, mean, and error values. The input parameters for this function are:
 
-- numb_ys: the number of yaw sweeps to fit.
-- data_50_Hz: data with 50 Hz sampling frequency.
-- name_ys: a string specifying the name of the yaw sweep.
-- scan_id_ys: a string specifying the scan id of the yaw sweep.
-- partial_plot: boolean specifying whether or not to plot partial results.
-The output of the function is a dictionary containing the fitted curve outputs and warnings.
-#### Usage
-To use the curve_fitting_ys function, first call the get_SQL_1_min and get_SQL_50_Hz functions from the Load_data module to load the required data. Then use the identify_yaw_sweep function from the Yaw_sweep_identification module to identify the yaw sweep instances. Finally, call the curve_fitting_ys function with the required input parameters.
-### Step 5:Calibration Factors (offset,gain,windspeed)
-This script is designed to calculate calibration factors for a wind turbine based on data collected during yaw sweeps. The script requires several input parameters, and the output is a set of calibration factors that can be used to improve the accuracy of wind speed measurements.
-#### Required Libraries
-The following libraries are required for this script:
+#### Inputs
 
-- yaw_sweep_sg_cali.Load_data
-- yaw_sweep_sg_cali.Yaw_sweep_identification
-- yaw_sweep_sg_cali.Curve_fitting
-- yaw_sweep_sg_cali.Calibration_factors
-#### User Input
-
-The script requires the following user input parameters:
-
-- start: a tuple representing the start date of the data collection period (year, month)
-- stop: a tuple representing the end date of the data collection period (year, month)
-turbine_file: a string representing the name of a file containing turbine inputs
-##### Data Loading
-The script first loads data from the SQL database or from local files using the get_SQL_1_min function.
-##### Identifying Yaw Sweeps
-The script then identifies the yaw sweep instants based on name and scan_id using the identify_yaw_sweep function. This function takes in the loaded data and returns three variables:
-- name_ys: a string representing the name of the yaw sweep
-- scan_id_ys: an integer representing the scan ID of the yaw sweep
-- numb_ys: an integer representing the number of yaw sweeps in the data
-##### Second Data Loading
-The script then loads data from the SQL database or from local files using the get_SQL_50_Hz function.
-##### Fitting Sinus
-The script fits a sinus curve to the yaw sweep data using the curve_fitting_ys function. This function takes in the yaw sweep data and other variables returned by identify_yaw_sweep and returns two variables:
-
-- fitted_curve_outputs: a list containing the maximum, minimum, mean, and error of the fitted sinus curve
-- warnings: a string containing any warnings generated during curve fitting
-##### Calculating Calibration Factors
-The script then calculates calibration factors using the get_cali_factors function. This function takes in the fitted curve outputs, the turbine file name, and any warnings generated during curve fitting. It returns a dictionary containing the calibration factors.
-#### User Input
-The output of the script is a set of calibration factors that can be used to improve the accuracy of wind speed measurements. The calibration factors are stored in a dictionary with keys offset, gain, and windspeed. A plot of the fitted curve can also be generated by setting the plot parameter of get_cali_factors to True.
+- data_50_Hz: An array of intdata 
 
-## Installation
-To use this code, clone the repository and install the required dependencies:
+with 50 Hz sampling frequency.
 
-```
-git clone  https://github.com/username/yaw-sweep-sg-cali.git
-cd yaw-sweep-sg-cali
-pip install -r requirements.txt
-```
-The package can be installed using pip:
-	- [ ]  git clone https://github.com/username/yaw-sweep-sg-cali.git
-	- [ ]  cd yaw-sweep-sg-cali
-	- [ ]  pip install -r requirements.txt
+- name_ys: a string 
 
+specifying the name of the yaw sweep.
 
+- scan_id_ys: A string 
 
-## Add your files
+specifying the scan id of the yaw sweep.
 
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+- partial_plot: A boolean
 
-```
-cd existing_repo
-git remote add origin https://gitlab.windenergy.dtu.dk/python-at-risoe/spp-2023/v52-strain-gauge-calibration.git
-git branch -M main
-git push -uf origin main
-```
+ specifying whether or not to plot partial results.
+
+#### Outputs
 
-## Integrate with your tools
+ dic: A dictionary 
+ 
+ containing the fitted curve outputs and warnings.
 
-- [ ] [Set up project integrations](https://gitlab.windenergy.dtu.dk/python-at-risoe/spp-2023/v52-strain-gauge-calibration/-/settings/integrations)
+## Step 5:Calibration Factors (offset,gain,windspeed)(get_cali_factors)
 
-## Collaborate with your team
+This script is designed to calculate calibration factors for a wind turbine based on data collected during yaw sweeps. The script requires several input parameters, and the output is a set of calibration factors that can be used to improve the accuracy of wind speed measurements.
+
+### Inputs
+
+- data_all : A dictionary
+
+ contains the information of the different ys identifies.
+ 
+- file_name : A string 
+
+contains the file name of the turbine to be analyzed.
 
-- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+- warnings : A list 
 
-## Test and Deploy
+Contains the initial and end name of the signals where the fiting function did not suceed to fit at all an sinus shape.
 
-Use the built-in continuous integration in GitLab.
+- plot : A bool
 
-- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+ optional if final plotted is wanted. The default is False.
 
-***
+### Outputs
 
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+dic : A dictionary 
+
+similar to the input dict, but now adding the generated calibration factors.
+
+***Note***: the dictionary contains way more nice information than the plotting functions can handle for now. More in progress.
 
 ## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
+
+- Thanks to [Mikkel Friis-Møller](https://gitlab.windenergy.dtu.dk/V52/V52) that provided some of the functions inside the module [SQL_utilities.py](https://gitlab.windenergy.dtu.dk/python-at-risoe/spp-2023/group_4_shaking_hands/-/blob/main/Final_Project/yaw_sweep_sg_cali/SQL_utilities.py).
+
+- DTU for the V52 SQL data.
 
 ## License
 This code is licensed under the MIT License.
 
 ## Improvements performed from first submission to final submission
 
 - The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
 - The code was check with pycodestyle, to ensure was properly with the recommended standards. 
 - PEP 257 information added to each function
+
+## Peer Review
```

### Comparing `yaw_sweep_sg_cali-2.2/setup.py` & `yaw_sweep_sg_cali-3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup
 # read the contents of your README file
 
 from pathlib import Path
-this_directory = Path(__file__).parent
+this_directory1 = Path(__file__).parent
+this_directory = this_directory1.joinpath('yaw_sweep_sg_cali')
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='yaw_sweep_sg_cali',
-version='2.2',
+version='3.0',
 description='Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.', 
 long_description = long_description,
 long_description_content_type='text/markdown',
 author='Bruno and Zahra',
 author_email='brofa@dtu.dk',
 packages=['yaw_sweep_sg_cali'],
 # packages_data={'yaw_sweep_sg_cali':['Data/V52_1min_data/*.txt', 'Data/V52_50Hz_data/*.txt','Data/V52_inputs.txt']}
```

### Comparing `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Calibration_factors.py` & `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Calibration_factors.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Curve_fitting.py` & `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Curve_fitting.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Load_data.py` & `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Load_data.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/SQL_utilities.py` & `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/SQL_utilities.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-2.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py` & `yaw_sweep_sg_cali-3.0/yaw_sweep_sg_cali/Yaw_sweep_identification.py`

 * *Files identical despite different names*

