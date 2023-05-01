# Comparing `tmp/malbench-0.3.1.tar.gz` & `tmp/malbench-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malbench-0.3.1.tar", max compression
+gzip compressed data, was "malbench-0.3.2.tar", max compression
```

## Comparing `malbench-0.3.1.tar` & `malbench-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.1/data/banner.txt
--rw-r--r--   0        0        0      508 2023-04-25 12:39:55.627552 malbench-0.3.1/data/disclaimer.txt
--rw-r--r--   0        0        0        5 2023-05-01 04:29:10.898528 malbench-0.3.1/data/version.txt
--rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.1/malbench/__init__.py
--rw-r--r--   0        0        0     2905 2023-04-27 03:15:45.560814 malbench-0.3.1/malbench/__main__.py
--rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.1/malbench/args.py
--rw-r--r--   0        0        0     4830 2023-04-26 15:12:59.929156 malbench-0.3.1/malbench/malware.py
--rw-r--r--   0        0        0     8362 2023-04-27 03:29:38.237716 malbench-0.3.1/malbench/message.py
--rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.1/malbench/version.py
--rw-r--r--   0        0        0      894 2023-05-01 04:32:12.652571 malbench-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6927 2023-04-27 03:47:54.949752 malbench-0.3.1/README.md
--rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 malbench-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.2/data/banner.txt
+-rw-r--r--   0        0        0      508 2023-04-25 12:39:55.627552 malbench-0.3.2/data/disclaimer.txt
+-rw-r--r--   0        0        0        5 2023-05-01 04:55:31.656629 malbench-0.3.2/data/version.txt
+-rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.2/malbench/__init__.py
+-rw-r--r--   0        0        0     2905 2023-04-27 03:15:45.560814 malbench-0.3.2/malbench/__main__.py
+-rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.2/malbench/args.py
+-rw-r--r--   0        0        0     4830 2023-04-26 15:12:59.929156 malbench-0.3.2/malbench/malware.py
+-rw-r--r--   0        0        0     8362 2023-04-27 03:29:38.237716 malbench-0.3.2/malbench/message.py
+-rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.2/malbench/version.py
+-rw-r--r--   0        0        0      894 2023-05-01 04:55:40.662999 malbench-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7144 2023-05-01 04:55:05.817341 malbench-0.3.2/README.md
+-rw-r--r--   0        0        0     7870 1970-01-01 00:00:00.000000 malbench-0.3.2/PKG-INFO
```

### Comparing `malbench-0.3.1/data/banner.txt` & `malbench-0.3.2/data/banner.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.3.1/LICENSE` & `malbench-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `malbench-0.3.1/malbench/__main__.py` & `malbench-0.3.2/malbench/__main__.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.1/malbench/args.py` & `malbench-0.3.2/malbench/args.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.1/malbench/malware.py` & `malbench-0.3.2/malbench/malware.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.1/malbench/message.py` & `malbench-0.3.2/malbench/message.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.1/pyproject.toml` & `malbench-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "malbench"
-version = "0.3.1"
+version = "0.3.2"
 description = "A tool used for automating the analysis of malware samples against antivirus solutions."
 repository = "https://github.com/youkergav/Malbench"
 authors = ["Gavin Youker <youkergav@gmail.com>"]
 readme = "README.md"
 license = "LICENSE"
 include = ["data/*"]
 exclude = ["data/samples"]
```

### Comparing `malbench-0.3.1/README.md` & `malbench-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Malbench
 Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
 
 ## About
 
 
 ### Disclaimer 
-**:warning: WARNING**: Malbench is designed to run malicious code that can harm your computer. Malbench should only be run on secure and isolated environments by users who know what they are doing. Do **not** run Malbench on a computer or network that contains sensitive information or data that you are not willing to lose or become compromised. By downloading and/or using this software, you acknowledge and understand the risks of using this software; and assume full responsibility for any damages that may result from running Malbench.
+**⚠ WARNING**: Malbench is designed to run malicious code that can harm your computer. Malbench should only be run on secure and isolated environments by users who know what they are doing. Do **not** run Malbench on a computer or network that contains sensitive information or data that you are not willing to lose or become compromised. By downloading and/or using this software, you acknowledge and understand the risks of using this software; and assume full responsibility for any damages that may result from running Malbench.
 
-**:information_source: NOTE**: It is important to note that Malbench does not include any malware samples. Therefore, users are expected to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically; and that users have control over the types of malware being tested.
+**ℹ️ NOTE**: It is important to note that Malbench does not include any malware samples. Therefore, users are expected to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically; and that users have control over the types of malware being tested.
 
 ### Why Use Malbench?
 Malware detection tools are an essential component of any computer security strategy, but they are not foolproof. New techniques and methods are constantly being developed to evade detection. It is important to regularly test and evaluate the effectiveness of detection tools to ensure that we are keeping up with these evolving threats.
 
 With all the different features and algorithms of modern antivirus solutions, it can be hard to find practical and objective results on what-all they defend against. Malbench can be leveraged to bulk-test known malware samples against antivirus solutions to deliver real and practical results. This is done by automatically launching multiple malware payloads on a system and seeing what samples are detected and which ones were evaded. With Malbench, users can customize their testing to meet their specific needs, selecting the malware samples they want to run, and the duration of a test.
 
 ## Installation
@@ -39,15 +39,20 @@
     cd malbench
     ```
 4.  Install the required dependencies using Poetry:
     ```bash
     poetry install
     ```
     *Note: Please ensure the your PATH is configured for poetry*
-5. If using VSCode: First ensure the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) is installed. Open the `Malbench` folder in VSCode and ensure the Python interpreter is set to use the local poetry `.venv` (you may need to reload VSCode after this).
+5. Launch the virtual environment using one of the following methods:
+    - For general use, the virtual environment can be opened with:
+      ```
+      poetry shell
+      ```
+    - Alternatively, the virtual environment can be opened in VSCode. First ensure the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) is installed. Then, open the `Malbench` folder in VSCode and ensure the Python interpreter is set to use the local poetry `.venv` (you may need to reload VSCode after this).
 
 ## Usage
 To use Malbench, simply run the following command inside your virtual environment:
 ```bash
 python -m malbench /path/to/malware
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `malbench-0.3.1/PKG-INFO` & `malbench-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malbench
-Version: 0.3.1
+Version: 0.3.2
 Summary: A tool used for automating the analysis of malware samples against antivirus solutions.
 Home-page: https://github.com/youkergav/Malbench
 License: LICENSE
 Author: Gavin Youker
 Author-email: youkergav@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -22,17 +22,17 @@
 # Malbench
 Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
 
 ## About
 
 
 ### Disclaimer 
-**:warning: WARNING**: Malbench is designed to run malicious code that can harm your computer. Malbench should only be run on secure and isolated environments by users who know what they are doing. Do **not** run Malbench on a computer or network that contains sensitive information or data that you are not willing to lose or become compromised. By downloading and/or using this software, you acknowledge and understand the risks of using this software; and assume full responsibility for any damages that may result from running Malbench.
+**⚠ WARNING**: Malbench is designed to run malicious code that can harm your computer. Malbench should only be run on secure and isolated environments by users who know what they are doing. Do **not** run Malbench on a computer or network that contains sensitive information or data that you are not willing to lose or become compromised. By downloading and/or using this software, you acknowledge and understand the risks of using this software; and assume full responsibility for any damages that may result from running Malbench.
 
-**:information_source: NOTE**: It is important to note that Malbench does not include any malware samples. Therefore, users are expected to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically; and that users have control over the types of malware being tested.
+**ℹ️ NOTE**: It is important to note that Malbench does not include any malware samples. Therefore, users are expected to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically; and that users have control over the types of malware being tested.
 
 ### Why Use Malbench?
 Malware detection tools are an essential component of any computer security strategy, but they are not foolproof. New techniques and methods are constantly being developed to evade detection. It is important to regularly test and evaluate the effectiveness of detection tools to ensure that we are keeping up with these evolving threats.
 
 With all the different features and algorithms of modern antivirus solutions, it can be hard to find practical and objective results on what-all they defend against. Malbench can be leveraged to bulk-test known malware samples against antivirus solutions to deliver real and practical results. This is done by automatically launching multiple malware payloads on a system and seeing what samples are detected and which ones were evaded. With Malbench, users can customize their testing to meet their specific needs, selecting the malware samples they want to run, and the duration of a test.
 
 ## Installation
@@ -60,15 +60,20 @@
     cd malbench
     ```
 4.  Install the required dependencies using Poetry:
     ```bash
     poetry install
     ```
     *Note: Please ensure the your PATH is configured for poetry*
-5. If using VSCode: First ensure the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) is installed. Open the `Malbench` folder in VSCode and ensure the Python interpreter is set to use the local poetry `.venv` (you may need to reload VSCode after this).
+5. Launch the virtual environment using one of the following methods:
+    - For general use, the virtual environment can be opened with:
+      ```
+      poetry shell
+      ```
+    - Alternatively, the virtual environment can be opened in VSCode. First ensure the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) is installed. Then, open the `Malbench` folder in VSCode and ensure the Python interpreter is set to use the local poetry `.venv` (you may need to reload VSCode after this).
 
 ## Usage
 To use Malbench, simply run the following command inside your virtual environment:
 ```bash
 python -m malbench /path/to/malware
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

