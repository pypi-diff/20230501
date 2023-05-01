# Comparing `tmp/Prepup-0.0.5.tar.gz` & `tmp/prepup-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Prepup-0.0.5.tar", last modified: Sun Apr 30 17:20:39 2023, max compression
+gzip compressed data, was "prepup-0.0.6.tar", last modified: Mon May  1 00:41:12 2023, max compression
```

## Comparing `Prepup-0.0.5.tar` & `prepup-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.395629 Prepup-0.0.5/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 Prepup-0.0.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 Prepup-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 Prepup-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      929 2023-04-30 17:20:39.395629 Prepup-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.385038 Prepup-0.0.5/Prepup.egg-info/
--rw-rw-rw-   0        0        0      929 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      219 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 17:20:39.000000 Prepup-0.0.5/Prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 Prepup-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.390745 Prepup-0.0.5/prepup/
--rw-rw-rw-   0        0        0      148 2023-04-29 20:41:27.000000 Prepup-0.0.5/prepup/__init__.py
--rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 Prepup-0.0.5/prepup/common.py
--rw-rw-rw-   0        0        0     5349 2023-04-29 22:20:45.000000 Prepup-0.0.5/prepup/prepup.py
--rw-rw-rw-   0        0        0      202 2023-04-30 15:45:11.000000 Prepup-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-04-30 17:20:39.397582 Prepup-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3633 2023-04-30 17:20:10.000000 Prepup-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 17:20:39.394652 Prepup-0.0.5/tests/
--rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 Prepup-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 Prepup-0.0.5/tests/test_prepup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.133244 prepup-0.0.6/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      493 2023-05-01 00:41:12.132266 prepup-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.114599 prepup-0.0.6/prepup/
+-rw-rw-rw-   0        0        0     5353 2023-04-30 23:58:51.000000 prepup-0.0.6/prepup/__init__.py
+-rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 prepup-0.0.6/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.126393 prepup-0.0.6/prepup.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-01 00:41:12.000000 prepup-0.0.6/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      212 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 00:41:12.134216 prepup-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3162 2023-05-01 00:40:12.000000 prepup-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.130311 prepup-0.0.6/tests/
+-rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 prepup-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.6/tests/test_prepup.py
```

### Comparing `Prepup-0.0.5/LICENSE` & `prepup-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Prepup-0.0.5/prepup/common.py` & `prepup-0.0.6/prepup/common.py`

 * *Files identical despite different names*

### Comparing `Prepup-0.0.5/prepup/prepup.py` & `prepup-0.0.6/prepup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,9 +126,9 @@
         crafter.correlation_n()
 
         h_8 = Figlet(font='term')
         print(colored(h_8.renderText("\nExecution Time..."),'light_blue'))
         end_n = time.time()-start
         print("Operations Comepleted Successfully in {0} {1}".format(end_n,"seconds"))
                 
-if __name__ == '__main__':
-    main()
+# if __name__ == '__main__':
+#     main()
```

### Comparing `Prepup-0.0.5/setup.py` & `prepup-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,40 +55,31 @@
 #     version='0.0.2',
 #     zip_safe=False,
 # )
 
 import setuptools
 
 setuptools.setup(
-    name="Prepup",
-    version="0.0.5",
-    license='MIT',
+    name="prepup",
+    version="0.0.6",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
-    description="Prepup is a free, open-source package that lets you open, explore, visualize and pre-process datasets in your computer's terminal.",
-    url='https://github.com/sudhanshumukherjeexx/prepup',
-    keywords=['DATA PREPROCESSING','TERMINAL', 'DATA SCIENCE', 'EDA'],
+    description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
             "prepup = prepup.prepup:main",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.5",
     install_requires=[
         "argparse",
         "polars",
         "termcolor",
         "pyfiglet",
         "blessed",
         "imbalanced_learn",
@@ -96,15 +87,14 @@
         "joblib",
         "matplotlib",
         "nbclient",
         "nbformat",
         "numpy",
         "pandas",
         "plotext",
-        "polars",
         "prefect",
         "prefect_jupyter",
         "pydantic",
         "pyfiglet",
         "pytest",
         "scikit_learn",
         "scipy",
```

