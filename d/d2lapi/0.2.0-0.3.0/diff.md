# Comparing `tmp/d2lapi-0.2.0.tar.gz` & `tmp/d2lapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2lapi-0.2.0.tar", last modified: Mon May  1 01:31:24 2023, max compression
+gzip compressed data, was "d2lapi-0.3.0.tar", last modified: Mon May  1 01:33:34 2023, max compression
```

## Comparing `d2lapi-0.2.0.tar` & `d2lapi-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.036586 d2lapi-0.2.0/
--rw-rw-rw-   0        0        0      119 2023-04-14 03:33:14.000000 d2lapi-0.2.0/.gitignore
--rw-rw-rw-   0        0        0    47875 2023-05-01 00:55:58.000000 d2lapi-0.2.0/D2L_Data_Converter_Logo.png
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.000683 d2lapi-0.2.0/DataFiles/
--rw-rw-rw-   0        0        0    20313 2023-04-14 03:33:14.000000 d2lapi-0.2.0/DataFiles/ExampleData_AnswerKey.csv
--rw-rw-rw-   0        0        0   285845 2023-04-14 03:33:14.000000 d2lapi-0.2.0/DataFiles/ExampleData_QuizAttemptDetails.csv
--rw-rw-rw-   0        0        0   162364 2023-04-14 03:33:14.000000 d2lapi-0.2.0/DataFiles/ExampleData_Survey.csv
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.003675 d2lapi-0.2.0/Examples/
--rw-rw-rw-   0        0        0        0 2023-04-14 03:33:14.000000 d2lapi-0.2.0/Examples/.gitkeep
--rw-rw-rw-   0        0        0   864769 2023-05-01 00:55:58.000000 d2lapi-0.2.0/Examples/UsageExamples.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.006666 d2lapi-0.2.0/Figures/
--rw-rw-rw-   0        0        0        0 2023-04-14 03:33:14.000000 d2lapi-0.2.0/Figures/.gitkeep
--rw-rw-rw-   0        0        0    30002 2023-05-01 01:06:56.000000 d2lapi-0.2.0/Figures/Bar_Visualization.ipynb
--rw-rw-rw-   0        0        0     5089 2023-05-01 00:55:58.000000 d2lapi-0.2.0/INSTALL.md
--rw-rw-rw-   0        0        0     1148 2023-05-01 00:55:58.000000 d2lapi-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      200 2023-05-01 01:31:24.036586 d2lapi-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3187 2023-05-01 00:55:58.000000 d2lapi-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.011655 d2lapi-0.2.0/Reports/
--rw-rw-rw-   0        0        0     2841 2023-05-01 00:55:58.000000 d2lapi-0.2.0/Reports/Conda_Installation_Instructions.md
--rw-rw-rw-   0        0        0      503 2023-04-14 03:33:14.000000 d2lapi-0.2.0/Reports/Instruction of import functions.md
--rw-rw-rw-   0        0        0     3531 2023-05-01 00:55:58.000000 d2lapi-0.2.0/Reports/UsageRequirementsLimitations.md
--rw-rw-rw-   0        0        0     5321 2023-04-24 03:29:31.000000 d2lapi-0.2.0/TestGUI.py
--rw-rw-rw-   0        0        0      187 2023-05-01 00:55:58.000000 d2lapi-0.2.0/environment.yml
--rw-rw-rw-   0        0        0      165 2023-04-24 03:26:17.000000 d2lapi-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      380 2023-05-01 01:31:24.038582 d2lapi-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       77 2023-04-24 03:26:17.000000 d2lapi-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.014645 d2lapi-0.2.0/src/
--rw-rw-rw-   0        0        0     6148 2023-04-01 19:05:10.000000 d2lapi-0.2.0/src/.DS_Store
--rw-rw-rw-   0        0        0    32656 2023-05-01 01:27:46.000000 d2lapi-0.2.0/src/Widget-Based_GUI_WithLabelKeys.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.021628 d2lapi-0.2.0/src/d2lapi/
--rw-rw-rw-   0        0        0     1705 2023-05-01 01:25:21.000000 d2lapi-0.2.0/src/d2lapi/D2L_Widgets.py
--rw-rw-rw-   0        0        0    19801 2023-04-24 03:53:40.000000 d2lapi-0.2.0/src/d2lapi/Final_Quiz.py
--rw-rw-rw-   0        0        0     9706 2023-04-24 03:53:40.000000 d2lapi-0.2.0/src/d2lapi/Final_Survey.py
--rw-rw-rw-   0        0        0    12496 2023-04-24 01:50:13.000000 d2lapi-0.2.0/src/d2lapi/Visualization_Bar.py
--rw-rw-rw-   0        0        0        0 2023-04-24 01:50:13.000000 d2lapi-0.2.0/src/d2lapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.029605 d2lapi-0.2.0/src/d2lapi.egg-info/
--rw-rw-rw-   0        0        0      200 2023-05-01 01:31:23.000000 d2lapi-0.2.0/src/d2lapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      885 2023-05-01 01:31:23.000000 d2lapi-0.2.0/src/d2lapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:31:23.000000 d2lapi-0.2.0/src/d2lapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 01:31:23.000000 d2lapi-0.2.0/src/d2lapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 01:31:24.035589 d2lapi-0.2.0/src/test/
--rw-rw-rw-   0        0        0        0 2023-04-01 19:05:10.000000 d2lapi-0.2.0/src/test/.gitkeep
--rw-rw-rw-   0        0        0        2 2023-04-01 19:05:10.000000 d2lapi-0.2.0/src/test/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-04-24 03:29:31.000000 d2lapi-0.2.0/src/test/test_cases_quiz.py
--rw-rw-rw-   0        0        0     2664 2023-04-24 03:29:31.000000 d2lapi-0.2.0/src/test/test_cases_survey.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.862289 d2lapi-0.3.0/
+-rw-rw-rw-   0        0        0      119 2023-04-14 03:33:14.000000 d2lapi-0.3.0/.gitignore
+-rw-rw-rw-   0        0        0    47875 2023-05-01 00:55:58.000000 d2lapi-0.3.0/D2L_Data_Converter_Logo.png
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.800454 d2lapi-0.3.0/DataFiles/
+-rw-rw-rw-   0        0        0    20313 2023-04-14 03:33:14.000000 d2lapi-0.3.0/DataFiles/ExampleData_AnswerKey.csv
+-rw-rw-rw-   0        0        0   285845 2023-04-14 03:33:14.000000 d2lapi-0.3.0/DataFiles/ExampleData_QuizAttemptDetails.csv
+-rw-rw-rw-   0        0        0   162364 2023-04-14 03:33:14.000000 d2lapi-0.3.0/DataFiles/ExampleData_Survey.csv
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.803447 d2lapi-0.3.0/Examples/
+-rw-rw-rw-   0        0        0        0 2023-04-14 03:33:14.000000 d2lapi-0.3.0/Examples/.gitkeep
+-rw-rw-rw-   0        0        0   864769 2023-05-01 00:55:58.000000 d2lapi-0.3.0/Examples/UsageExamples.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.807435 d2lapi-0.3.0/Figures/
+-rw-rw-rw-   0        0        0        0 2023-04-14 03:33:14.000000 d2lapi-0.3.0/Figures/.gitkeep
+-rw-rw-rw-   0        0        0    10917 2023-05-01 01:32:31.000000 d2lapi-0.3.0/Figures/Bar_Visualization.ipynb
+-rw-rw-rw-   0        0        0    21950 2023-05-01 01:32:42.000000 d2lapi-0.3.0/Final_Report.md
+-rw-rw-rw-   0        0        0     5089 2023-05-01 00:55:58.000000 d2lapi-0.3.0/INSTALL.md
+-rw-rw-rw-   0        0        0     1148 2023-05-01 00:55:58.000000 d2lapi-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      200 2023-05-01 01:33:34.862289 d2lapi-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3187 2023-05-01 00:55:58.000000 d2lapi-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.814417 d2lapi-0.3.0/Reports/
+-rw-rw-rw-   0        0        0     2841 2023-05-01 00:55:58.000000 d2lapi-0.3.0/Reports/Conda_Installation_Instructions.md
+-rw-rw-rw-   0        0        0      503 2023-04-14 03:33:14.000000 d2lapi-0.3.0/Reports/Instruction of import functions.md
+-rw-rw-rw-   0        0        0     3531 2023-05-01 00:55:58.000000 d2lapi-0.3.0/Reports/UsageRequirementsLimitations.md
+-rw-rw-rw-   0        0        0     5321 2023-04-24 03:29:31.000000 d2lapi-0.3.0/TestGUI.py
+-rw-rw-rw-   0        0        0      187 2023-05-01 00:55:58.000000 d2lapi-0.3.0/environment.yml
+-rw-rw-rw-   0        0        0      165 2023-04-24 03:26:17.000000 d2lapi-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      380 2023-05-01 01:33:34.865281 d2lapi-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       77 2023-04-24 03:26:17.000000 d2lapi-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.818406 d2lapi-0.3.0/src/
+-rw-rw-rw-   0        0        0     6148 2023-04-01 19:05:10.000000 d2lapi-0.3.0/src/.DS_Store
+-rw-rw-rw-   0        0        0    15606 2023-05-01 01:32:31.000000 d2lapi-0.3.0/src/Widget-Based_GUI_WithLabelKeys.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.828379 d2lapi-0.3.0/src/d2lapi/
+-rw-rw-rw-   0        0        0     1714 2023-05-01 01:32:31.000000 d2lapi-0.3.0/src/d2lapi/D2L_Widgets.py
+-rw-rw-rw-   0        0        0    19801 2023-04-24 03:53:40.000000 d2lapi-0.3.0/src/d2lapi/Final_Quiz.py
+-rw-rw-rw-   0        0        0     9706 2023-04-24 03:53:40.000000 d2lapi-0.3.0/src/d2lapi/Final_Survey.py
+-rw-rw-rw-   0        0        0    12496 2023-04-24 01:50:13.000000 d2lapi-0.3.0/src/d2lapi/Visualization_Bar.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:50:13.000000 d2lapi-0.3.0/src/d2lapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.851320 d2lapi-0.3.0/src/d2lapi.egg-info/
+-rw-rw-rw-   0        0        0      200 2023-05-01 01:33:34.000000 d2lapi-0.3.0/src/d2lapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-05-01 01:33:34.000000 d2lapi-0.3.0/src/d2lapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 01:33:34.000000 d2lapi-0.3.0/src/d2lapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 01:33:34.000000 d2lapi-0.3.0/src/d2lapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 01:33:34.858300 d2lapi-0.3.0/src/test/
+-rw-rw-rw-   0        0        0        0 2023-04-01 19:05:10.000000 d2lapi-0.3.0/src/test/.gitkeep
+-rw-rw-rw-   0        0        0        2 2023-04-01 19:05:10.000000 d2lapi-0.3.0/src/test/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-04-24 03:29:31.000000 d2lapi-0.3.0/src/test/test_cases_quiz.py
+-rw-rw-rw-   0        0        0     2664 2023-04-24 03:29:31.000000 d2lapi-0.3.0/src/test/test_cases_survey.py
```

### Comparing `d2lapi-0.2.0/D2L_Data_Converter_Logo.png` & `d2lapi-0.3.0/D2L_Data_Converter_Logo.png`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/DataFiles/ExampleData_AnswerKey.csv` & `d2lapi-0.3.0/DataFiles/ExampleData_AnswerKey.csv`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/DataFiles/ExampleData_QuizAttemptDetails.csv` & `d2lapi-0.3.0/DataFiles/ExampleData_QuizAttemptDetails.csv`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/DataFiles/ExampleData_Survey.csv` & `d2lapi-0.3.0/DataFiles/ExampleData_Survey.csv`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/Examples/UsageExamples.ipynb` & `d2lapi-0.3.0/Examples/UsageExamples.ipynb`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/INSTALL.md` & `d2lapi-0.3.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/LICENSE` & `d2lapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/README.md` & `d2lapi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/Reports/Conda_Installation_Instructions.md` & `d2lapi-0.3.0/Reports/Conda_Installation_Instructions.md`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/Reports/UsageRequirementsLimitations.md` & `d2lapi-0.3.0/Reports/UsageRequirementsLimitations.md`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/TestGUI.py` & `d2lapi-0.3.0/TestGUI.py`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/src/.DS_Store` & `d2lapi-0.3.0/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/src/d2lapi/D2L_Widgets.py` & `d2lapi-0.3.0/src/d2lapi/D2L_Widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     inputs:
     input_file_widget_value: result from file upload widget - .csv that was uploaded
     
     outputs:
     final_content: byte object that can be passed into pd.read_csv
     '''
     try:
-        input_file = list(input_file_widget_value)[0]
+        input_file = list(input_file_widget_value.values())[0]
         input_file_content = input_file['content']
         final_content = io.BytesIO(input_file_content)
         return final_content
     except IndexError:
         return ''
 
 def run_1(self):
```

### Comparing `d2lapi-0.2.0/src/d2lapi/Final_Quiz.py` & `d2lapi-0.3.0/src/d2lapi/Final_Quiz.py`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/src/d2lapi/Final_Survey.py` & `d2lapi-0.3.0/src/d2lapi/Final_Survey.py`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/src/d2lapi/Visualization_Bar.py` & `d2lapi-0.3.0/src/d2lapi/Visualization_Bar.py`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/src/d2lapi.egg-info/SOURCES.txt` & `d2lapi-0.3.0/src/d2lapi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 D2L_Data_Converter_Logo.png
+Final_Report.md
 INSTALL.md
 LICENSE
 README.md
 TestGUI.py
 environment.yml
 pyproject.toml
 setup.cfg
```

### Comparing `d2lapi-0.2.0/src/test/test_cases_quiz.py` & `d2lapi-0.3.0/src/test/test_cases_quiz.py`

 * *Files identical despite different names*

### Comparing `d2lapi-0.2.0/src/test/test_cases_survey.py` & `d2lapi-0.3.0/src/test/test_cases_survey.py`

 * *Files identical despite different names*

