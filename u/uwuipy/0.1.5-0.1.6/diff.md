# Comparing `tmp/uwuipy-0.1.5.tar.gz` & `tmp/uwuipy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwuipy-0.1.5.tar", last modified: Sun Apr 30 21:29:59 2023, max compression
+gzip compressed data, was "uwuipy-0.1.6.tar", max compression
```

## Comparing `uwuipy-0.1.5.tar` & `uwuipy-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:59.175965 uwuipy-0.1.5/
--rwxrwxrwx   0 root         (0) root         (0)     1084 2022-07-30 16:51:45.000000 uwuipy-0.1.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     2293 2023-04-30 21:29:59.171766 uwuipy-0.1.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2018 2023-04-30 21:25:36.000000 uwuipy-0.1.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-30 21:29:59.175965 uwuipy-0.1.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-30 21:26:22.000000 uwuipy-0.1.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:58.897080 uwuipy-0.1.5/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:59.025250 uwuipy-0.1.5/src/uwuipy/
--rwxrwxrwx   0 root         (0) root         (0)       26 2022-07-30 17:42:55.000000 uwuipy-0.1.5/src/uwuipy/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1834 2023-04-30 21:25:36.000000 uwuipy-0.1.5/src/uwuipy/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     7620 2023-04-30 21:15:42.000000 uwuipy-0.1.5/src/uwuipy/uwuipy.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:59.139976 uwuipy-0.1.5/src/uwuipy.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2293 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      229 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0     1084 2022-07-30 16:51:45.360190 uwuipy-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0     2018 2023-04-30 21:25:36.914918 uwuipy-0.1.6/README.md
+-rwxr-xr-x   0        0        0      505 2023-04-30 22:22:54.298305 uwuipy-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0       26 2022-07-30 17:42:55.320171 uwuipy-0.1.6/uwuipy/__init__.py
+-rwxr-xr-x   0        0        0     1834 2023-04-30 21:25:36.915912 uwuipy-0.1.6/uwuipy/__main__.py
+-rwxr-xr-x   0        0        0     7620 2023-04-30 21:15:42.019576 uwuipy-0.1.6/uwuipy/uwuipy.py
+-rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 uwuipy-0.1.6/PKG-INFO
```

### Comparing `uwuipy-0.1.5/LICENSE` & `uwuipy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uwuipy-0.1.5/PKG-INFO` & `uwuipy-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: uwuipy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Allows the easy implementation of uwuifying words for applications like Discord bots and websites
-Home-page: https://github.com/Cuprum77/uwuipy
-Author: Cuprum77, diminDDL, R2Boyo25, ThatRedKite and pin-lee
 License: MIT
+Author: Cuprum77
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: homepage, https://github.com/Cuprum77/uwuipy
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 
 # uwuipy
 An advanced uwuifier for python.
 ## Install
 To install just use PyPI `pip install uwuipy`
 ## Usage
@@ -70,7 +74,8 @@
 print(uwu.uwuify(message))
 ```
 as you can see we only use one method `uwuify()` it accepts a string and returns an uwuified string as per the values set in the contructor.
 ## Contributing and Licence
 Feel free contribute to the [github repo](https://github.com/Cuprum77/uwuipy) of the project.
 
 Licenced under [MIT](https://github.com/Cuprum77/uwuipy/blob/main/LICENSE)
+
```

### Comparing `uwuipy-0.1.5/README.md` & `uwuipy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `uwuipy-0.1.5/src/uwuipy/__main__.py` & `uwuipy-0.1.6/uwuipy/__main__.py`

 * *Files identical despite different names*

### Comparing `uwuipy-0.1.5/src/uwuipy/uwuipy.py` & `uwuipy-0.1.6/uwuipy/uwuipy.py`

 * *Files identical despite different names*

