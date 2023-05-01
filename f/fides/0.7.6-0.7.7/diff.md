# Comparing `tmp/fides-0.7.6.tar.gz` & `tmp/fides-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fides-0.7.6.tar", last modified: Wed Apr 12 07:09:01 2023, max compression
+gzip compressed data, was "fides-0.7.7.tar", last modified: Mon May  1 13:09:13 2023, max compression
```

## Comparing `fides-0.7.6.tar` & `fides-0.7.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:09:01.442666 fides-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-04-12 07:09:01.442666 fides-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-04-12 07:09:01.000000 fides-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:09:01.442666 fides-0.7.6/fides/
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-12 07:09:01.000000 fides-0.7.6/fides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-04-12 07:09:01.000000 fides-0.7.6/fides/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20130 2023-04-12 07:09:01.000000 fides-0.7.6/fides/hessian_approximation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-12 07:09:01.000000 fides-0.7.6/fides/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    32025 2023-04-12 07:09:01.000000 fides-0.7.6/fides/minimize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-04-12 07:09:01.000000 fides-0.7.6/fides/stepback.py
--rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-04-12 07:09:01.000000 fides-0.7.6/fides/steps.py
--rw-r--r--   0 runner    (1001) docker     (122)    10253 2023-04-12 07:09:01.000000 fides-0.7.6/fides/subproblem.py
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-04-12 07:09:01.000000 fides-0.7.6/fides/trust_region.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-12 07:09:01.000000 fides-0.7.6/fides/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:09:01.442666 fides-0.7.6/fides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      367 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-12 07:09:01.000000 fides-0.7.6/fides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-12 07:09:01.442666 fides-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1755 2023-04-12 07:09:01.000000 fides-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:09:13.799842 fides-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-05-01 13:09:13.799842 fides-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-05-01 13:09:12.000000 fides-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:09:13.799842 fides-0.7.7/fides/
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-05-01 13:09:12.000000 fides-0.7.7/fides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-05-01 13:09:12.000000 fides-0.7.7/fides/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20130 2023-05-01 13:09:12.000000 fides-0.7.7/fides/hessian_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-05-01 13:09:12.000000 fides-0.7.7/fides/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32013 2023-05-01 13:09:12.000000 fides-0.7.7/fides/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-05-01 13:09:12.000000 fides-0.7.7/fides/stepback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-05-01 13:09:12.000000 fides-0.7.7/fides/steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10253 2023-05-01 13:09:12.000000 fides-0.7.7/fides/subproblem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-01 13:09:12.000000 fides-0.7.7/fides/trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-01 13:09:12.000000 fides-0.7.7/fides/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:09:13.799842 fides-0.7.7/fides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-01 13:09:13.000000 fides-0.7.7/fides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-01 13:09:13.799842 fides-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-05-01 13:09:12.000000 fides-0.7.7/setup.py
```

### Comparing `fides-0.7.6/PKG-INFO` & `fides-0.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fides
-Version: 0.7.6
+Version: 0.7.7
 Summary: python Trust Region Optimization
 Home-page: https://github.com/Fides-dev/fides
 Author: Fabian Froehlich
 Author-email: froehlichfab@gmail.com
 License: BSD-3-Clause
 Description: # Fides - A python package for Trust Region Optimization
         
@@ -45,14 +45,12 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fides Version: 0.7.6 Summary: python Trust Region
+Metadata-Version: 2.1 Name: fides Version: 0.7.7 Summary: python Trust Region
 Optimization Home-page: https://github.com/Fides-dev/fides Author: Fabian
 Froehlich Author-email: froehlichfab@gmail.com License: BSD-3-Clause
 Description: # Fides - A python package for Trust Region Optimization [PyPI
 version] [Code_coverage] [ReadTheDocs_status] [DOI] ## About Fides Fides
 implements an Interior Trust Region Reflective for boundary constrained
 optimization problems based on the papers [ColemanLi1994](https://doi.org/
 10.1007/BF01582221) and [ColemanLi1996](http://dx.doi.org/10.1137/0806023).
@@ -15,11 +15,10 @@
 and Broyden class iterative Hessian Approximation schemes * SSM, TSSM, FX,
 GNSBFGS and custom hybrid Hessian Approximations schemes Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Software Development ::
 Libraries Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
```

### Comparing `fides-0.7.6/README.md` & `fides-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides/constants.py` & `fides-0.7.7/fides/constants.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides/hessian_approximation.py` & `fides-0.7.7/fides/hessian_approximation.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides/logging.py` & `fides-0.7.7/fides/logging.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides/minimize.py` & `fides-0.7.7/fides/minimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,41 +523,41 @@
         gnorm = norm(grad)
         stepsx = step.ss + step.ss0
         nsx = norm(stepsx)
 
         if self.tr_ratio > self.get_option(Options.MU) and \
                 np.abs(fval - self.fval) < fatol + frtol*np.abs(self.fval):
             self.exitflag = ExitFlag.FTOL
-            self.logger.warning(
+            self.logger.info(
                 'Stopping as function difference '
                 f'{np.abs(self.fval - fval):.2E} was smaller than specified '
                 f'tolerances (atol={fatol:.2E}, rtol={frtol:.2E})'
             )
             converged = True
 
         elif self.iteration > 1 and nsx < xtol:
             self.exitflag = ExitFlag.XTOL
-            self.logger.warning(
+            self.logger.info(
                 'Stopping as norm of step '
                 f'{nsx} was smaller than specified '
                 f'tolerance (tol={xtol:.2E})'
             )
             converged = True
 
         elif gnorm <= gatol:
             self.exitflag = ExitFlag.GTOL
-            self.logger.warning(
+            self.logger.info(
                 'Stopping as gradient norm satisfies absolute convergence '
                 f'criteria: {gnorm:.2E} < {gatol:.2E}'
             )
             converged = True
 
         elif gnorm <= grtol * np.abs(self.fval):
             self.exitflag = ExitFlag.GTOL
-            self.logger.warning(
+            self.logger.info(
                 'Stopping as gradient norm satisfies relative convergence '
                 f'criteria: {gnorm:.2E} < {grtol:.2E} * '
                 f'{np.abs(self.fval):.2E}'
             )
             converged = True
 
         self.converged = converged
```

### Comparing `fides-0.7.6/fides/stepback.py` & `fides-0.7.7/fides/stepback.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides/steps.py` & `fides-0.7.7/fides/steps.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides/subproblem.py` & `fides-0.7.7/fides/subproblem.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides/trust_region.py` & `fides-0.7.7/fides/trust_region.py`

 * *Files identical despite different names*

### Comparing `fides-0.7.6/fides.egg-info/PKG-INFO` & `fides-0.7.7/fides.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fides
-Version: 0.7.6
+Version: 0.7.7
 Summary: python Trust Region Optimization
 Home-page: https://github.com/Fides-dev/fides
 Author: Fabian Froehlich
 Author-email: froehlichfab@gmail.com
 License: BSD-3-Clause
 Description: # Fides - A python package for Trust Region Optimization
         
@@ -45,14 +45,12 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fides Version: 0.7.6 Summary: python Trust Region
+Metadata-Version: 2.1 Name: fides Version: 0.7.7 Summary: python Trust Region
 Optimization Home-page: https://github.com/Fides-dev/fides Author: Fabian
 Froehlich Author-email: froehlichfab@gmail.com License: BSD-3-Clause
 Description: # Fides - A python package for Trust Region Optimization [PyPI
 version] [Code_coverage] [ReadTheDocs_status] [DOI] ## About Fides Fides
 implements an Interior Trust Region Reflective for boundary constrained
 optimization problems based on the papers [ColemanLi1994](https://doi.org/
 10.1007/BF01582221) and [ColemanLi1996](http://dx.doi.org/10.1137/0806023).
@@ -15,11 +15,10 @@
 and Broyden class iterative Hessian Approximation schemes * SSM, TSSM, FX,
 GNSBFGS and custom hybrid Hessian Approximations schemes Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Software Development ::
 Libraries Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
```

### Comparing `fides-0.7.6/setup.py` & `fides-0.7.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,13 +33,11 @@
       classifiers=['Development Status :: 5 - Production/Stable',
                    'Intended Audience :: Science/Research',
                    'Topic :: Software Development :: Libraries',
                    'License :: OSI Approved :: BSD License',
                    'Programming Language :: Python',
                    'Programming Language :: Python :: 3',
                    'Programming Language :: Python :: 3 :: Only',
-                   'Programming Language :: Python :: 3.7',
-                   'Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
                    'Programming Language :: Python :: 3.11'],
-      python_requires='>=3.7')
+      python_requires='>=3.9')
```

