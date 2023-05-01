# Comparing `tmp/overloaded-iterables-0.7.0.tar.gz` & `tmp/overloaded-iterables-0.7.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.0.tar", last modified: Sun Apr 30 23:51:27 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.12.tar", last modified: Mon May  1 05:58:04 2023, max compression
```

## Comparing `overloaded-iterables-0.7.0.tar` & `overloaded-iterables-0.7.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 23:51:27.994984 overloaded-iterables-0.7.0/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     8130 2023-04-30 23:51:27.994984 overloaded-iterables-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     7417 2023-04-30 21:49:01.000000 overloaded-iterables-0.7.0/README.md
--rw-rw-rw-   0        0        0      111 2023-04-30 23:51:27.996987 overloaded-iterables-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-04-30 23:50:47.000000 overloaded-iterables-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 23:51:27.981985 overloaded-iterables-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 23:51:27.986987 overloaded-iterables-0.7.0/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.7.0/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    14722 2023-04-30 23:48:36.000000 overloaded-iterables-0.7.0/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-30 23:51:27.993987 overloaded-iterables-0.7.0/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0     8130 2023-04-30 23:51:27.000000 overloaded-iterables-0.7.0/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-30 23:51:27.000000 overloaded-iterables-0.7.0/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 23:51:27.000000 overloaded-iterables-0.7.0/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-30 23:51:27.000000 overloaded-iterables-0.7.0/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-30 23:51:27.000000 overloaded-iterables-0.7.0/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.277460 overloaded-iterables-0.7.12/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.12/LICENSE
+-rw-rw-rw-   0        0        0     8079 2023-05-01 05:58:04.277460 overloaded-iterables-0.7.12/PKG-INFO
+-rw-rw-rw-   0        0        0     7365 2023-05-01 05:45:35.000000 overloaded-iterables-0.7.12/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-01 05:58:04.279460 overloaded-iterables-0.7.12/setup.cfg
+-rw-rw-rw-   0        0        0     1497 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.263458 overloaded-iterables-0.7.12/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.268459 overloaded-iterables-0.7.12/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.7.12/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    15059 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.12/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.276459 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0     8079 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.0/LICENSE` & `overloaded-iterables-0.7.12/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.0/PKG-INFO` & `overloaded-iterables-0.7.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,15 @@
-Metadata-Version: 2.1
-Name: overloaded-iterables
-Version: 0.7.0
-Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
-Home-page: https://github.com/Arkiralor/overloaded_iterables
-Author: Prithoo Medhi
-Author-email: prithoo11335@gmail.com
-License: MIT
-Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
-Platform: windows
-Platform: ubuntu-linux
-Platform: mac-os
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Overloaded Iterables
 
+[![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
+
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
-## Specifications
-
-1. __Python Version:__
-
-    _Python v3.8+_
-
-2. __Code Coverage:__
-
-    ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
-
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
 2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
 
@@ -200,9 +174,7 @@
     - Arguments: `self`
     - Returns: `OverloadedList, OverloadedList`
     - Example:
 
         ```python
             values: Overloadedlist, frequencies: OverloadedList = obj.frequencies
         ```
-
-
```

### Comparing `overloaded-iterables-0.7.0/README.md` & `overloaded-iterables-0.7.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,33 @@
+Metadata-Version: 2.1
+Name: overloaded-iterables
+Version: 0.7.12
+Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
+Home-page: https://github.com/Arkiralor/overloaded_iterables
+Author: Prithoo Medhi
+Author-email: prithoo11335@gmail.com
+License: MIT
+Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
+Platform: windows
+Platform: ubuntu-linux
+Platform: mac-os
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Overloaded Iterables
 
+[![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
+
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
-## Specifications
-
-1. __Python Version:__
-
-    _Python v3.8+_
-
-2. __Code Coverage:__
-
-    ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
-
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
 2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
 
@@ -182,7 +192,9 @@
     - Arguments: `self`
     - Returns: `OverloadedList, OverloadedList`
     - Example:
 
         ```python
             values: Overloadedlist, frequencies: OverloadedList = obj.frequencies
         ```
+
+
```

### Comparing `overloaded-iterables-0.7.0/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.12/src/overloaded_iterables/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class OverloadedList(list):
     """
     Overloaded <list> class to add additional methods.
     """
     iZERO: int = 0
     fZERO: float = 0.0
+    TIME_FORMAT:str = '%Y-%m-%dT%H-%M-%S.%fZ%z'
 
     def mean(self) -> float:
         """
         Returns the arithmetic mean of the values in the OverloadedList.
         """
         return self.sum()/self.len
 
@@ -94,15 +95,15 @@
         elif _l > 1 and _l % 2 == 1:
             return _sorted[(_l)//2]
         else:
             return float()
 
     def hist(
         self,
-        bins: int = 10,
+        bins: int = 0,
         title: str = 'Histogram',
         x_label: str = 'Values --->',
         y_label: str = 'Frequencies --->',
         save_dir: str = None,
         color: str = '#0f0f0f',
         file_name: str = None,
         histtype: str = 'step',
@@ -116,32 +117,37 @@
         **kwargs
     ) -> bool:
         """
         Draws and saves if required, the histogram of the frequency distribution of the elements of the OverloadedList object.
         """
         try:
             x_axis = array(self)
+            if bins == 0:
+                bins = x_axis.__len__()//10
             plt.hist(
                 x=x_axis,
                 bins=bins,
                 histtype=histtype,
                 align=align,
                 orientation=orientation,
                 log=log_scale,
-                color=color
+                color=color,
+                rwidth=1
             )
             plt.title(title)
-            plt.xlabel(x_label)
-            plt.ylabel(y_label)
+            plt.xlabel(x_label, loc='center')
+            plt.ylabel(y_label, loc='center')
+            plt.grid(visible=True, which='both', axis='both')
 
             if save_dir and not show:
-                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow().timestamp()}.PNG"
-                save_path = path.join(
-                    save_dir, file_name)
+                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow().strftime(self.TIME_FORMAT)}.PNG"
+                save_path = path.join(save_dir, file_name)
+
                 plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
+
                 return file_name
             elif show and not save_dir:
                 plt.show()
             elif save_dir and show:
                 raise AttributeError(
                     "Both `show` and `save_dir` cannot be defined."
                 )
@@ -149,15 +155,14 @@
                 pass
             else:
                 raise ValueError("Something went wrong.")
             
             plt.clf()
             return True
         except Exception as ex:
-            plt.clf()
             raise ex
 
     def plot(
             self,
             title: str = 'Line Plot',
             x_label: str = 'Values --->',
             y_label: str = 'Frequencies --->',
@@ -182,35 +187,37 @@
             x_axis = array(x_axis)
             y_axis = array(y_axis)
             plt.plot(x_axis, y_axis, color=color, linewidth=linewidth, marker=marker,
                      markerfacecolor=markerfacecolor, markersize=marker_size)
             plt.title(title)
             plt.xlabel(x_label)
             plt.ylabel(y_label)
+            plt.grid(visible=True, which='both', axis='both')
+
             if save_dir and not show:
-                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow().timestamp()}.PNG"
-                save_path = path.join(
-                    save_dir, file_name)
+                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__plot__{datetime.utcnow().strftime(self.TIME_FORMAT)}.PNG"
+                save_path = path.join(save_dir, file_name)
+                
                 plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
+
                 return file_name
             elif show and not save_dir:
                 plt.show()
             elif save_dir and show:
                 raise AttributeError(
                     "Both `show` and `save_dir` cannot be defined."
                 )
             elif not show and not save_dir:
                 pass
             else:
                 raise ValueError("Something went wrong.")
-
+            
             plt.clf()
             return True
         except Exception as ex:
-            plt.clf()
             raise ex
 
     def scatter(
             self,
             title: str = 'Scatter Plot',
             x_label: str = 'Values --->',
             y_label: str = 'Frequencies --->',
@@ -233,19 +240,22 @@
             x_axis, y_axis = self.frequencies
             x_axis = array(x_axis)
             y_axis = array(y_axis)
             plt.scatter(x=x_axis, y=y_axis, s=array(size), color=color, marker=marker, linewidths=line_width)
             plt.title(title)
             plt.xlabel(x_label)
             plt.ylabel(y_label)
+            plt.grid(visible=True, which='both', axis='both')
+
             if save_dir and not show:
-                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow().timestamp()}.PNG"
-                save_path = path.join(
-                    save_dir, file_name)
+                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__scatter__{datetime.utcnow().strftime(self.TIME_FORMAT)}.PNG"
+                save_path = path.join(save_dir, file_name)
+                
                 plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
+
                 return file_name
             elif show and not save_dir:
                 plt.show()
             elif save_dir and show:
                 raise AttributeError(
                     "Both `show` and `save_dir` cannot be defined."
                 )
@@ -253,15 +263,14 @@
                 pass
             else:
                 raise ValueError("Something went wrong.")
             
             plt.clf()
             return True
         except Exception as ex:
-            plt.clf()
             raise ex
 
     @property
     def _type(self):
         """
         Return the type of the current OverloadedList object, which will of course, always be `OverloadedList`.
```

### Comparing `overloaded-iterables-0.7.0/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.0
+Version: 0.7.12
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -14,28 +14,20 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
+[![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
+
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
-## Specifications
-
-1. __Python Version:__
-
-    _Python v3.8+_
-
-2. __Code Coverage:__
-
-    ![_code coverage_](https://github.com/Arkiralor/overloaded_iterables/blob/master/media/screenshots/coverage.PNG?raw=true)
-
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
 2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
```

