# Comparing `tmp/datamachine-0.1.0.tar.gz` & `tmp/datamachine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.1.0.tar", last modified: Sat Apr 29 23:12:35 2023, max compression
+gzip compressed data, was "datamachine-0.1.1.tar", last modified: Mon May  1 19:13:58 2023, max compression
```

## Comparing `datamachine-0.1.0.tar` & `datamachine-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 23:12:35.984408 datamachine-0.1.0/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4018 2023-04-29 23:12:35.985492 datamachine-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3494 2023-04-29 21:05:10.000000 datamachine-0.1.0/README.md
--rw-rw-rw-   0        0        0      582 2023-04-29 23:12:04.000000 datamachine-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      569 2023-04-29 23:12:35.986503 datamachine-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 23:12:35.955684 datamachine-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 23:12:35.969260 datamachine-0.1.0/src/datamachine/
--rw-rw-rw-   0        0        0      271 2023-04-29 02:02:57.000000 datamachine-0.1.0/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0    11255 2023-04-29 23:01:33.000000 datamachine-0.1.0/src/datamachine/_modular.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:12:35.983842 datamachine-0.1.0/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0     4018 2023-04-29 23:12:35.000000 datamachine-0.1.0/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-04-29 23:12:35.000000 datamachine-0.1.0/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 23:12:35.000000 datamachine-0.1.0/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 23:12:35.000000 datamachine-0.1.0/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:58.941597 datamachine-0.1.1/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4713 2023-05-01 19:13:58.942993 datamachine-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4189 2023-05-01 19:13:21.000000 datamachine-0.1.1/README.md
+-rw-rw-rw-   0        0        0      582 2023-05-01 16:25:32.000000 datamachine-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      569 2023-05-01 19:13:58.950097 datamachine-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:58.906065 datamachine-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:58.919173 datamachine-0.1.1/src/datamachine/
+-rw-rw-rw-   0        0        0      271 2023-04-29 02:02:57.000000 datamachine-0.1.1/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0    11255 2023-04-29 23:01:33.000000 datamachine-0.1.1/src/datamachine/_modular.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:58.940608 datamachine-0.1.1/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0     4713 2023-05-01 19:13:58.000000 datamachine-0.1.1/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-05-01 19:13:58.000000 datamachine-0.1.1/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 19:13:58.000000 datamachine-0.1.1/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 19:13:58.000000 datamachine-0.1.1/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.1.0/LICENSE` & `datamachine-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.1.0/PKG-INFO` & `datamachine-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,112 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.1.0
+Version: 0.1.1
 Summary: Modular Notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave@benevolentmachines.org>
 Project-URL: Project, https://github.com/dave-killough/datamachine
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="left" >
-  <img src="https://storage.googleapis.com/benevolentmachines/datamachine2.svg" 
-       title="BenevolentMachines.Org">
+  <img src="https://storage.googleapis.com/benevolentmachines/datamachine.svg" 
+       title="datamachine">
 </p>
 
-## Welcome to the Machine!
+## Modular Notebooks
 
-datamachine is a powerful Python package that allows you to execute cloud Python notebooks with parameters and import cloud notebooks as modules. With datamachine, you can reference notebooks from various sources such as local files, Colab links, Github links, and HTTP links, and execute or import them with ease. You can also assign codes to files or links and store them in a library, which is a collection of codes and their corresponding links. Libraries are stored in JSON format with a dictionary of notebooks to their links. 
+Imagine an easy way to reuse Python notebooks in the cloud. datamachine is a useful Python package that enables you to import notebooks as modules and execute Python notebooks with parameters. With datamachine, you can load notebooks from various sources such as local files, Colab links, and Github links, and then execute or import them with ease. You can also organize notebooks into libraries that use simple codes for easy access to commonly used notebooks. 
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/dm_overview.png">
+</p>
 
 ## Features
 
-- Execute cloud notebooks with parameters: With datamachine, you can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
+- **Import notebooks as modules**: Importing notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
 
-- Import cloud notebooks as modules: Importing cloud notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
+- **Execute notebooks with parameters**: You can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
 
-- Library and Index: datamachine supports library and index features, making it easier to organize your code. You can store collections of code and their corresponding links in a library and index them for easy access.
+- **Libraries**: datamachine supports user-defined libraries that will make your reusable notebook modules much easier to publish and use by others.   
 
-- JSON support: All libraries and indexes are stored in JSON format, making it easy to read, write, and share with others.
+- **Notebook sources**: You can currently source public notebooks from GitHub, Colab, and notebooks in your local file system.  I plan on adding secure notebook access and extending storage options to S3, Azure, GCP, and other cloud-based systems.  Please add an issue to GitHub if you're intersted in support for a particular source.  
 
 ## Installation
 
 To install datamachine, run the following command:
 
 ``` python
-%pip install datamachine
+pip install datamachine
 ```
 
 ## Importing datamachine
 
-Once you've installed datamachine, you can import it.  
-The convention is to name the module instance `dm`.  
+Once you've installed datamachine, you can import it. The convention is to name the module instance `dm`.  
 
 ```python
 import datamachine as dm
 ```
+
+### Notebook Locations
+
+datamachine currrently supports notebook links from Github, Google Colab, local file paths, and public `https` links with raw content.  
 ### Importing a Notebook as a Module
 
 To import a notebook as a module, use the `import_notebook` function:
 
 ```python
 nbo = dm.import_notebook(
     "https://colab.research.google.com/drive/1y7x3BDkmaz6k93QjENanKHudLV8xB96Q?usp=sharing",
 )
 ```
 
-This command imports the notebook located at `"./module.ipynb"` as a module named `"nbo"`.
+This function imports the notebook located at the specified location and returns a module reference like the native import command.  The Colab notebook used above provides sample analytics that can be accessed by using methods in the module.  For instance, you could run the following function
+
+```python
+nbo.monthly_rulings()
+```
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/dm_module2.gif">
+</p>
+
+
 ### Executing a Notebook
 
 To execute a notebook with parameters, use the `execute_notebook` function:
 
 ```python
 import datamachine as dm
-dm.execute_notebook(
-    "execute.ipynb", html="output.html",
-    params={"EIN": "200549531","TYPE": "summary"},
+dm.execute_notebook("execute.ipynb", 
+    html="output.html",
+    params={
+        "EIN": "200549531",
+        "TYPE": "summary"
+    },
 )
 ```
 
 This function executes the notebook located at `"execute.ipynb"` with the parameter `"EIN"` 
 set to `"200549531"`. The output is saved in an HTML file named `"output.html"`.
 
-In order to receive the EIN parameter in the executed notebook, simply invoke 
-the `execute_params` function with a passed dictionary containing the parameter.
+In order to receive the EIN and TYPE parameters in the executed notebook, simply invoke 
+the `execute_params` function with a passed dictionary containing the parameters.
 This function provides the test values when you're directly running the notebook, 
 and uses the passed values when invoked via `execute_notebook`.    
 ```python
 import datamachine as dm
-params = dm.execute_params({"EIN": "454547709","TYPE": "detail"})
+params = dm.execute_params({
+    "EIN": "454547709",
+    "TYPE": "detail"
+})
 EIN = params["EIN"]
 ```
 
 
 
 ## Conclusion
 
-datamachine is a powerful tool for anyone who works with cloud Python notebooks. With its flexible features and easy-to-use commands, datamachine makes it easy to execute and import notebooks from various sources, store collections of code and their corresponding links in a library, and organize your code with an index. So why wait? Install datamachine today and take your cloud notebook experience to the next level!
+datamachine is a powerful tool for anyone who wants to reuse Python notebooks. With its flexible features and easy-to-use commands, datamachine makes it easy to execute and import notebooks from various sources, store collections of code and their corresponding links in a library, and organize your code with an index. So why wait? Install datamachine today and take your notebook experience to the next level!
```

### Comparing `datamachine-0.1.0/README.md` & `datamachine-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,97 @@
 <p align="left" >
-  <img src="https://storage.googleapis.com/benevolentmachines/datamachine2.svg" 
-       title="BenevolentMachines.Org">
+  <img src="https://storage.googleapis.com/benevolentmachines/datamachine.svg" 
+       title="datamachine">
 </p>
 
-## Welcome to the Machine!
+## Modular Notebooks
 
-datamachine is a powerful Python package that allows you to execute cloud Python notebooks with parameters and import cloud notebooks as modules. With datamachine, you can reference notebooks from various sources such as local files, Colab links, Github links, and HTTP links, and execute or import them with ease. You can also assign codes to files or links and store them in a library, which is a collection of codes and their corresponding links. Libraries are stored in JSON format with a dictionary of notebooks to their links. 
+Imagine an easy way to reuse Python notebooks in the cloud. datamachine is a useful Python package that enables you to import notebooks as modules and execute Python notebooks with parameters. With datamachine, you can load notebooks from various sources such as local files, Colab links, and Github links, and then execute or import them with ease. You can also organize notebooks into libraries that use simple codes for easy access to commonly used notebooks. 
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/dm_overview.png">
+</p>
 
 ## Features
 
-- Execute cloud notebooks with parameters: With datamachine, you can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
+- **Import notebooks as modules**: Importing notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
 
-- Import cloud notebooks as modules: Importing cloud notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
+- **Execute notebooks with parameters**: You can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
 
-- Library and Index: datamachine supports library and index features, making it easier to organize your code. You can store collections of code and their corresponding links in a library and index them for easy access.
+- **Libraries**: datamachine supports user-defined libraries that will make your reusable notebook modules much easier to publish and use by others.   
 
-- JSON support: All libraries and indexes are stored in JSON format, making it easy to read, write, and share with others.
+- **Notebook sources**: You can currently source public notebooks from GitHub, Colab, and notebooks in your local file system.  I plan on adding secure notebook access and extending storage options to S3, Azure, GCP, and other cloud-based systems.  Please add an issue to GitHub if you're intersted in support for a particular source.  
 
 ## Installation
 
 To install datamachine, run the following command:
 
 ``` python
-%pip install datamachine
+pip install datamachine
 ```
 
 ## Importing datamachine
 
-Once you've installed datamachine, you can import it.  
-The convention is to name the module instance `dm`.  
+Once you've installed datamachine, you can import it. The convention is to name the module instance `dm`.  
 
 ```python
 import datamachine as dm
 ```
+
+### Notebook Locations
+
+datamachine currrently supports notebook links from Github, Google Colab, local file paths, and public `https` links with raw content.  
 ### Importing a Notebook as a Module
 
 To import a notebook as a module, use the `import_notebook` function:
 
 ```python
 nbo = dm.import_notebook(
     "https://colab.research.google.com/drive/1y7x3BDkmaz6k93QjENanKHudLV8xB96Q?usp=sharing",
 )
 ```
 
-This command imports the notebook located at `"./module.ipynb"` as a module named `"nbo"`.
+This function imports the notebook located at the specified location and returns a module reference like the native import command.  The Colab notebook used above provides sample analytics that can be accessed by using methods in the module.  For instance, you could run the following function
+
+```python
+nbo.monthly_rulings()
+```
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/dm_module2.gif">
+</p>
+
+
 ### Executing a Notebook
 
 To execute a notebook with parameters, use the `execute_notebook` function:
 
 ```python
 import datamachine as dm
-dm.execute_notebook(
-    "execute.ipynb", html="output.html",
-    params={"EIN": "200549531","TYPE": "summary"},
+dm.execute_notebook("execute.ipynb", 
+    html="output.html",
+    params={
+        "EIN": "200549531",
+        "TYPE": "summary"
+    },
 )
 ```
 
 This function executes the notebook located at `"execute.ipynb"` with the parameter `"EIN"` 
 set to `"200549531"`. The output is saved in an HTML file named `"output.html"`.
 
-In order to receive the EIN parameter in the executed notebook, simply invoke 
-the `execute_params` function with a passed dictionary containing the parameter.
+In order to receive the EIN and TYPE parameters in the executed notebook, simply invoke 
+the `execute_params` function with a passed dictionary containing the parameters.
 This function provides the test values when you're directly running the notebook, 
 and uses the passed values when invoked via `execute_notebook`.    
 ```python
 import datamachine as dm
-params = dm.execute_params({"EIN": "454547709","TYPE": "detail"})
+params = dm.execute_params({
+    "EIN": "454547709",
+    "TYPE": "detail"
+})
 EIN = params["EIN"]
 ```
 
 
 
 ## Conclusion
 
-datamachine is a powerful tool for anyone who works with cloud Python notebooks. With its flexible features and easy-to-use commands, datamachine makes it easy to execute and import notebooks from various sources, store collections of code and their corresponding links in a library, and organize your code with an index. So why wait? Install datamachine today and take your cloud notebook experience to the next level!
+datamachine is a powerful tool for anyone who wants to reuse Python notebooks. With its flexible features and easy-to-use commands, datamachine makes it easy to execute and import notebooks from various sources, store collections of code and their corresponding links in a library, and organize your code with an index. So why wait? Install datamachine today and take your notebook experience to the next level!
```

### Comparing `datamachine-0.1.0/pyproject.toml` & `datamachine-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamachine"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = []
 authors = [
   { name="Dave Killough", email="dave@benevolentmachines.org" },
 ]
 description = "Modular Notebooks"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `datamachine-0.1.0/setup.cfg` & `datamachine-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 616d 6163 6869 6e65 0d0a   = datamachine..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 300d  version = 0.1.0.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 310d  version = 0.1.1.
 00000030: 0a61 7574 686f 7220 3d20 4461 7665 204b  .author = Dave K
 00000040: 696c 6c6f 7567 680d 0a61 7574 686f 725f  illough..author_
 00000050: 656d 6169 6c20 3d20 6461 7665 2e6b 696c  email = dave.kil
 00000060: 6c6f 7567 6840 676d 6169 6c2e 636f 6d0d  lough@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 204d  .description = M
 00000080: 6f64 756c 6172 204e 6f74 6562 6f6f 6b73  odular Notebooks
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `datamachine-0.1.0/src/datamachine/_modular.py` & `datamachine-0.1.1/src/datamachine/_modular.py`

 * *Files identical despite different names*

### Comparing `datamachine-0.1.0/src/datamachine.egg-info/PKG-INFO` & `datamachine-0.1.1/src/datamachine.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,112 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.1.0
+Version: 0.1.1
 Summary: Modular Notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave@benevolentmachines.org>
 Project-URL: Project, https://github.com/dave-killough/datamachine
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="left" >
-  <img src="https://storage.googleapis.com/benevolentmachines/datamachine2.svg" 
-       title="BenevolentMachines.Org">
+  <img src="https://storage.googleapis.com/benevolentmachines/datamachine.svg" 
+       title="datamachine">
 </p>
 
-## Welcome to the Machine!
+## Modular Notebooks
 
-datamachine is a powerful Python package that allows you to execute cloud Python notebooks with parameters and import cloud notebooks as modules. With datamachine, you can reference notebooks from various sources such as local files, Colab links, Github links, and HTTP links, and execute or import them with ease. You can also assign codes to files or links and store them in a library, which is a collection of codes and their corresponding links. Libraries are stored in JSON format with a dictionary of notebooks to their links. 
+Imagine an easy way to reuse Python notebooks in the cloud. datamachine is a useful Python package that enables you to import notebooks as modules and execute Python notebooks with parameters. With datamachine, you can load notebooks from various sources such as local files, Colab links, and Github links, and then execute or import them with ease. You can also organize notebooks into libraries that use simple codes for easy access to commonly used notebooks. 
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/dm_overview.png">
+</p>
 
 ## Features
 
-- Execute cloud notebooks with parameters: With datamachine, you can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
+- **Import notebooks as modules**: Importing notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
 
-- Import cloud notebooks as modules: Importing cloud notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
+- **Execute notebooks with parameters**: You can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
 
-- Library and Index: datamachine supports library and index features, making it easier to organize your code. You can store collections of code and their corresponding links in a library and index them for easy access.
+- **Libraries**: datamachine supports user-defined libraries that will make your reusable notebook modules much easier to publish and use by others.   
 
-- JSON support: All libraries and indexes are stored in JSON format, making it easy to read, write, and share with others.
+- **Notebook sources**: You can currently source public notebooks from GitHub, Colab, and notebooks in your local file system.  I plan on adding secure notebook access and extending storage options to S3, Azure, GCP, and other cloud-based systems.  Please add an issue to GitHub if you're intersted in support for a particular source.  
 
 ## Installation
 
 To install datamachine, run the following command:
 
 ``` python
-%pip install datamachine
+pip install datamachine
 ```
 
 ## Importing datamachine
 
-Once you've installed datamachine, you can import it.  
-The convention is to name the module instance `dm`.  
+Once you've installed datamachine, you can import it. The convention is to name the module instance `dm`.  
 
 ```python
 import datamachine as dm
 ```
+
+### Notebook Locations
+
+datamachine currrently supports notebook links from Github, Google Colab, local file paths, and public `https` links with raw content.  
 ### Importing a Notebook as a Module
 
 To import a notebook as a module, use the `import_notebook` function:
 
 ```python
 nbo = dm.import_notebook(
     "https://colab.research.google.com/drive/1y7x3BDkmaz6k93QjENanKHudLV8xB96Q?usp=sharing",
 )
 ```
 
-This command imports the notebook located at `"./module.ipynb"` as a module named `"nbo"`.
+This function imports the notebook located at the specified location and returns a module reference like the native import command.  The Colab notebook used above provides sample analytics that can be accessed by using methods in the module.  For instance, you could run the following function
+
+```python
+nbo.monthly_rulings()
+```
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/dm_module2.gif">
+</p>
+
+
 ### Executing a Notebook
 
 To execute a notebook with parameters, use the `execute_notebook` function:
 
 ```python
 import datamachine as dm
-dm.execute_notebook(
-    "execute.ipynb", html="output.html",
-    params={"EIN": "200549531","TYPE": "summary"},
+dm.execute_notebook("execute.ipynb", 
+    html="output.html",
+    params={
+        "EIN": "200549531",
+        "TYPE": "summary"
+    },
 )
 ```
 
 This function executes the notebook located at `"execute.ipynb"` with the parameter `"EIN"` 
 set to `"200549531"`. The output is saved in an HTML file named `"output.html"`.
 
-In order to receive the EIN parameter in the executed notebook, simply invoke 
-the `execute_params` function with a passed dictionary containing the parameter.
+In order to receive the EIN and TYPE parameters in the executed notebook, simply invoke 
+the `execute_params` function with a passed dictionary containing the parameters.
 This function provides the test values when you're directly running the notebook, 
 and uses the passed values when invoked via `execute_notebook`.    
 ```python
 import datamachine as dm
-params = dm.execute_params({"EIN": "454547709","TYPE": "detail"})
+params = dm.execute_params({
+    "EIN": "454547709",
+    "TYPE": "detail"
+})
 EIN = params["EIN"]
 ```
 
 
 
 ## Conclusion
 
-datamachine is a powerful tool for anyone who works with cloud Python notebooks. With its flexible features and easy-to-use commands, datamachine makes it easy to execute and import notebooks from various sources, store collections of code and their corresponding links in a library, and organize your code with an index. So why wait? Install datamachine today and take your cloud notebook experience to the next level!
+datamachine is a powerful tool for anyone who wants to reuse Python notebooks. With its flexible features and easy-to-use commands, datamachine makes it easy to execute and import notebooks from various sources, store collections of code and their corresponding links in a library, and organize your code with an index. So why wait? Install datamachine today and take your notebook experience to the next level!
```

