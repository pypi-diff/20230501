# Comparing `tmp/overloaded-iterables-0.6.2.tar.gz` & `tmp/overloaded-iterables-0.6.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.6.2.tar", last modified: Sun Apr 30 21:49:20 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.6.22.tar", last modified: Sun Apr 30 22:51:56 2023, max compression
```

## Comparing `overloaded-iterables-0.6.2.tar` & `overloaded-iterables-0.6.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.196779 overloaded-iterables-0.6.2/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     8130 2023-04-30 21:49:20.196779 overloaded-iterables-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     7417 2023-04-30 21:49:01.000000 overloaded-iterables-0.6.2/README.md
--rw-rw-rw-   0        0        0      111 2023-04-30 21:49:20.203783 overloaded-iterables-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-04-30 21:49:11.000000 overloaded-iterables-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.161779 overloaded-iterables-0.6.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.167775 overloaded-iterables-0.6.2/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.6.2/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    13051 2023-04-30 20:19:49.000000 overloaded-iterables-0.6.2/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:49:20.195776 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0     8130 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-30 21:49:20.000000 overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 22:51:56.383382 overloaded-iterables-0.6.22/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.6.22/LICENSE
+-rw-rw-rw-   0        0        0     8131 2023-04-30 22:51:56.384383 overloaded-iterables-0.6.22/PKG-INFO
+-rw-rw-rw-   0        0        0     7417 2023-04-30 21:49:01.000000 overloaded-iterables-0.6.22/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-30 22:51:56.385383 overloaded-iterables-0.6.22/setup.cfg
+-rw-rw-rw-   0        0        0     1478 2023-04-30 22:51:20.000000 overloaded-iterables-0.6.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:51:56.369384 overloaded-iterables-0.6.22/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 22:51:56.375382 overloaded-iterables-0.6.22/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.6.22/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    14035 2023-04-30 22:45:07.000000 overloaded-iterables-0.6.22/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:51:56.383382 overloaded-iterables-0.6.22/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0     8131 2023-04-30 22:51:56.000000 overloaded-iterables-0.6.22/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-30 22:51:56.000000 overloaded-iterables-0.6.22/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 22:51:56.000000 overloaded-iterables-0.6.22/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-30 22:51:56.000000 overloaded-iterables-0.6.22/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-30 22:51:56.000000 overloaded-iterables-0.6.22/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.6.2/LICENSE` & `overloaded-iterables-0.6.22/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.6.2/PKG-INFO` & `overloaded-iterables-0.6.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.6.2
+Version: 0.6.22
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
```

### Comparing `overloaded-iterables-0.6.2/README.md` & `overloaded-iterables-0.6.22/README.md`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.6.2/setup.py` & `overloaded-iterables-0.6.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         encoding="utf-8"
     )as file_obj:
         data = file_obj.read()
     return data
 
 setup(
     name='overloaded-iterables',
-    version='0.6.2',
+    version='0.6.22',
     description="Overloaded version of the built-in python classes: list and set to include some extra functionalities.",
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     license='MIT',
     author="Prithoo Medhi",
     author_email='prithoo11335@gmail.com',
     packages=find_packages('src'),
```

### Comparing `overloaded-iterables-0.6.2/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.6.22/src/overloaded_iterables/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,48 +99,56 @@
     def hist(
         self,
         bins: int = 10,
         title: str = 'Histogram',
         x_label: str = 'Values --->',
         y_label: str = 'Frequencies --->',
         save_dir: str = None,
+        color: str = '#0f0f0f',
         file_name: str = None,
         histtype: str = 'step',
         align: str = 'mid',
         orientation: str = 'vertical',
         log_scale: bool = False,
         show: bool = False,
+        dpi: int=300,
+        pad_inches: float=1,
         *args,
         **kwargs
     ) -> bool:
         """
         Draws and saves if required, the histogram of the frequency distribution of the elements of the OverloadedList object.
         """
         try:
             x_axis = array(self)
             plt.hist(
                 x=x_axis,
                 bins=bins,
                 histtype=histtype,
                 align=align,
                 orientation=orientation,
-                log=log_scale
+                log=log_scale,
+                color=color
             )
             plt.title(title)
             plt.xlabel(x_label)
             plt.ylabel(y_label)
-            if show:
-                plt.show()
 
-            if save_dir:
-                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow()}.PNG"
+            if save_dir and not show:
+                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow().timestamp()}.PNG"
                 save_path = path.join(
                     save_dir, file_name)
-                plt.savefig(save_path)
-
+                plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
+            elif show and not save_dir:
+                plt.show()
+            elif save_dir and show:
+                raise AttributeError(
+                    "Both `show` and `save_dir` cannot be defined."
+                )
+            
             return True
         except Exception as ex:
             raise ex
 
     def plot(
             self,
             title: str = 'Line Plot',
@@ -150,14 +158,16 @@
             file_name: str = None,
             color: str = '#000000',
             linewidth: float = 1,
             marker: str = ',',
             markerfacecolor: str = '#252525',
             marker_size: float = 1.0,
             show: bool = False,
+            dpi: int=300,
+            pad_inches: float=1,
             *args,
             **kwargs
     ):
         """
         Draws and saves if required, the line-plot of the frequency distribution of the elements of the OverloadedList object.
         """
         try:
@@ -165,22 +175,25 @@
             x_axis = array(x_axis)
             y_axis = array(y_axis)
             plt.plot(x_axis, y_axis, color=color, linewidth=linewidth, marker=marker,
                      markerfacecolor=markerfacecolor, markersize=marker_size)
             plt.title(title)
             plt.xlabel(x_label)
             plt.ylabel(y_label)
-            if show:
-                plt.show()
-
-            if save_dir:
-                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow()}.PNG"
+            if save_dir and not show:
+                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow().timestamp()}.PNG"
                 save_path = path.join(
                     save_dir, file_name)
-                plt.savefig(save_path)
+                plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
+            elif show and not save_dir:
+                plt.show()
+            elif save_dir and show:
+                raise AttributeError(
+                    "Both `show` and `save_dir` cannot be defined."
+                )
 
             return True
         except Exception as ex:
             raise ex
 
     def scatter(
             self,
@@ -190,36 +203,41 @@
             save_dir: str = None,
             file_name: str = None,
             size: List[float] = [1.25],
             color: str = '#000000',
             marker: str = ',',
             line_width: float = 2,
             show: bool = False,
+            dpi: int=300,
+            pad_inches: float=1,
             *args,
             **kwargs
     ):
         """
         Draws and saves if required, the scatter-plot of the frequency distribution of the elements of the OverloadedList object.
         """
         try:
             x_axis, y_axis = self.frequencies
             x_axis = array(x_axis)
             y_axis = array(y_axis)
             plt.scatter(x=x_axis, y=y_axis, s=array(size), color=color, marker=marker, linewidths=line_width)
             plt.title(title)
             plt.xlabel(x_label)
             plt.ylabel(y_label)
-            if show:
-                plt.show()
-
-            if save_dir:
-                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow()}.PNG"
+            if save_dir and not show:
+                file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__hist__{datetime.utcnow().timestamp()}.PNG"
                 save_path = path.join(
                     save_dir, file_name)
-                plt.savefig(save_path)
+                plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
+            elif show and not save_dir:
+                plt.show()
+            elif save_dir and show:
+                raise AttributeError(
+                    "Both `show` and `save_dir` cannot be defined."
+                )
 
             return True
         except Exception as ex:
             raise ex
 
     @property
     def _type(self):
```

### Comparing `overloaded-iterables-0.6.2/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.6.22/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.6.2
+Version: 0.6.22
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
```

