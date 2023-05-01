# Comparing `tmp/usefulib-1.0.4.tar.gz` & `tmp/usefulib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulib-1.0.4.tar", last modified: Wed Apr 26 16:25:48 2023, max compression
+gzip compressed data, was "usefulib-1.0.5.tar", last modified: Mon May  1 15:25:32 2023, max compression
```

## Comparing `usefulib-1.0.4.tar` & `usefulib-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.742083 usefulib-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-18 17:53:04.000000 usefulib-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3149 2023-04-26 16:25:48.742083 usefulib-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2434 2023-04-26 16:25:24.000000 usefulib-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 16:25:48.742083 usefulib-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3364 2023-04-26 16:24:56.000000 usefulib-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.710841 usefulib-1.0.4/usefulib/
--rw-rw-rw-   0        0        0      210 2023-04-26 16:25:16.000000 usefulib-1.0.4/usefulib/__init__.py
--rw-rw-rw-   0        0        0     4246 2023-04-26 16:25:07.000000 usefulib-1.0.4/usefulib/_usefulibs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.742083 usefulib-1.0.4/usefulib/temp_data/
--rw-rw-rw-   0        0        0      238 2023-04-26 16:25:05.000000 usefulib-1.0.4/usefulib/temp_data/__init__.py
--rw-rw-rw-   0        0        0     3276 2023-04-26 16:25:00.000000 usefulib-1.0.4/usefulib/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.726462 usefulib-1.0.4/usefulib.egg-info/
--rw-rw-rw-   0        0        0     3149 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 15:25:32.015899 usefulib-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-18 17:53:04.000000 usefulib-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3502 2023-05-01 15:25:32.014929 usefulib-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2820 2023-05-01 15:17:01.000000 usefulib-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 15:25:32.015899 usefulib-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3724 2023-05-01 15:14:46.000000 usefulib-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:25:31.996703 usefulib-1.0.5/usefulib/
+-rw-rw-rw-   0        0        0      211 2023-05-01 15:15:57.000000 usefulib-1.0.5/usefulib/__init__.py
+-rw-rw-rw-   0        0        0     6021 2023-05-01 15:15:53.000000 usefulib-1.0.5/usefulib/_usefulibs.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:25:32.013904 usefulib-1.0.5/usefulib/temp_data/
+-rw-rw-rw-   0        0        0      238 2023-05-01 15:16:02.000000 usefulib-1.0.5/usefulib/temp_data/__init__.py
+-rw-rw-rw-   0        0        0     4622 2023-05-01 15:15:46.000000 usefulib-1.0.5/usefulib/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:25:32.012903 usefulib-1.0.5/usefulib.egg-info/
+-rw-rw-rw-   0        0        0     3502 2023-05-01 15:25:31.000000 usefulib-1.0.5/usefulib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-01 15:25:31.000000 usefulib-1.0.5/usefulib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 15:25:31.000000 usefulib-1.0.5/usefulib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 15:25:31.000000 usefulib-1.0.5/usefulib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 15:25:31.000000 usefulib-1.0.5/usefulib.egg-info/top_level.txt
```

### Comparing `usefulib-1.0.4/LICENSE` & `usefulib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulib-1.0.4/PKG-INFO` & `usefulib-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usefulib
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of assorted methods to make small tasks easier.
 Home-page: UNKNOWN
 Author: Hamd Waseem
 Author-email: <codingboy.cw@gmail.com>
 License: UNKNOWN
 Keywords: python,useful,usefulib,collection
 Platform: UNKNOWN
@@ -18,22 +18,22 @@
 License-File: LICENSE
 
 
 <div align="center">
   <img src="https://github.com/hamdivazim/usefulib/raw/main/logo.png">
 </div>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/Python- >= 2.7 -blue?style=plastic.svg" alt="python versions" /></a>
-<a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
+<a style="display:inline;" href="#"><img src="https://img.shields.io/badge/pypi package- 1.0.5 -4DC71F?style=plastic.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.4</h1>
+<h1>usefulib v1.0.5</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ### GitHub Page: https://github.com/hamdivazim/usefulib
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
@@ -62,12 +62,15 @@
 
 ## What can it do?
 As an open-source library and can be contributed to by anyone, it offers a lot of simple functions to make writing code easier and quicker. A complete list of all usefulibs that are available can be found [here](https://github.com/hamdivazim/usefulib/blob/main/ALLFUNCTIONS.md).
 
 ## Support usefulib
 usefulib is full of contributions from the community! We're beginner-friendly here, so read the [contributing guidelines](https://github.com/hamdivazim/usefulib/blob/main/CONTRIBUTING.md) and give us your best usefulibs 😃!
 
+## View [the site](https://hamdivazim.github.io/usefulib/)
+Recently, usefulib's website launched at https://hamdivazim.github.io/usefulib/, feel free to report bugs or give feature requests, using the `web-issue` label. Or, take a look at [the discussion](https://github.com/hamdivazim/usefulib/discussions/13).
+
 ## License
 usefulib is licensed under the [GNU General Public License v3.0](https://github.com/hamdivazim/usefulib/blob/main/LICENSE).
```

### Comparing `usefulib-1.0.4/README.md` & `usefulib-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <div align="center">
   <img src="https://github.com/hamdivazim/usefulib/raw/main/logo.png">
 </div>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/Python- >= 2.7 -blue?style=plastic.svg" alt="python versions" /></a>
-<a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
+<a style="display:inline;" href="https://pypi.org/project/usefulib/"><img src="https://img.shields.io/badge/pypi package- 1.0.5 -4DC71F?style=plastic.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.4</h1>
+<h1>usefulib v1.0.5</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
 $ pip install usefulib
 ```
@@ -40,9 +40,12 @@
 
 ## What can it do?
 As an open-source library and can be contributed to by anyone, it offers a lot of simple functions to make writing code easier and quicker. A complete list of all usefulibs that are available can be found [here](https://github.com/hamdivazim/usefulib/blob/main/ALLFUNCTIONS.md).
 
 ## Support usefulib
 usefulib is full of contributions from the community! We're beginner-friendly here, so read the [contributing guidelines](https://github.com/hamdivazim/usefulib/blob/main/CONTRIBUTING.md) and give us your best usefulibs 😃!
 
+## View [the site](https://hamdivazim.github.io/usefulib/)
+Recently, usefulib's website launched at https://hamdivazim.github.io/usefulib/, feel free to report bugs or give feature requests, using the `web-issue` label. Or, take a look at [the discussion](https://github.com/hamdivazim/usefulib/discussions/13).
+
 ## License
 usefulib is licensed under the [GNU General Public License v3.0](https://github.com/hamdivazim/usefulib/blob/main/LICENSE).
```

### Comparing `usefulib-1.0.4/setup.py` & `usefulib-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = 'A collection of assorted methods to make small tasks easier.'
 LONG_DESCRIPTION = """
 <div align="center">
   <img src="https://github.com/hamdivazim/usefulib/raw/main/logo.png">
 </div>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/Python- >= 2.7 -blue?style=plastic.svg" alt="python versions" /></a>
-<a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
+<a style="display:inline;" href="#"><img src="https://img.shields.io/badge/pypi package- 1.0.5 -4DC71F?style=plastic.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.4</h1>
+<h1>usefulib v1.0.5</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ### GitHub Page: https://github.com/hamdivazim/usefulib
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
@@ -47,14 +47,17 @@
 
 ## What can it do?
 As an open-source library and can be contributed to by anyone, it offers a lot of simple functions to make writing code easier and quicker. A complete list of all usefulibs that are available can be found [here](https://github.com/hamdivazim/usefulib/blob/main/ALLFUNCTIONS.md).
 
 ## Support usefulib
 usefulib is full of contributions from the community! We're beginner-friendly here, so read the [contributing guidelines](https://github.com/hamdivazim/usefulib/blob/main/CONTRIBUTING.md) and give us your best usefulibs 😃!
 
+## View [the site](https://hamdivazim.github.io/usefulib/)
+Recently, usefulib's website launched at https://hamdivazim.github.io/usefulib/, feel free to report bugs or give feature requests, using the `web-issue` label. Or, take a look at [the discussion](https://github.com/hamdivazim/usefulib/discussions/13).
+
 ## License
 usefulib is licensed under the [GNU General Public License v3.0](https://github.com/hamdivazim/usefulib/blob/main/LICENSE).
 
 """
 
 # Setting up
 setup(
@@ -62,15 +65,15 @@
     version=VERSION,
     author="Hamd Waseem",
     author_email="<codingboy.cw@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=["numpy"],
     keywords=['python', 'useful', 'usefulib', 'collection'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `usefulib-1.0.4/usefulib.egg-info/PKG-INFO` & `usefulib-1.0.5/usefulib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usefulib
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of assorted methods to make small tasks easier.
 Home-page: UNKNOWN
 Author: Hamd Waseem
 Author-email: <codingboy.cw@gmail.com>
 License: UNKNOWN
 Keywords: python,useful,usefulib,collection
 Platform: UNKNOWN
@@ -18,22 +18,22 @@
 License-File: LICENSE
 
 
 <div align="center">
   <img src="https://github.com/hamdivazim/usefulib/raw/main/logo.png">
 </div>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/Python- >= 2.7 -blue?style=plastic.svg" alt="python versions" /></a>
-<a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
+<a style="display:inline;" href="#"><img src="https://img.shields.io/badge/pypi package- 1.0.5 -4DC71F?style=plastic.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.4</h1>
+<h1>usefulib v1.0.5</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ### GitHub Page: https://github.com/hamdivazim/usefulib
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
@@ -62,12 +62,15 @@
 
 ## What can it do?
 As an open-source library and can be contributed to by anyone, it offers a lot of simple functions to make writing code easier and quicker. A complete list of all usefulibs that are available can be found [here](https://github.com/hamdivazim/usefulib/blob/main/ALLFUNCTIONS.md).
 
 ## Support usefulib
 usefulib is full of contributions from the community! We're beginner-friendly here, so read the [contributing guidelines](https://github.com/hamdivazim/usefulib/blob/main/CONTRIBUTING.md) and give us your best usefulibs 😃!
 
+## View [the site](https://hamdivazim.github.io/usefulib/)
+Recently, usefulib's website launched at https://hamdivazim.github.io/usefulib/, feel free to report bugs or give feature requests, using the `web-issue` label. Or, take a look at [the discussion](https://github.com/hamdivazim/usefulib/discussions/13).
+
 ## License
 usefulib is licensed under the [GNU General Public License v3.0](https://github.com/hamdivazim/usefulib/blob/main/LICENSE).
```

