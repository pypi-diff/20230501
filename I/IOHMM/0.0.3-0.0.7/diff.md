# Comparing `tmp/IOHMM-0.0.3.tar.gz` & `tmp/IOHMM-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IOHMM-0.0.3.tar", last modified: Fri Feb  5 17:34:16 2021, max compression
+gzip compressed data, was "IOHMM-0.0.7.tar", last modified: Mon May  1 06:03:53 2023, max compression
```

## Comparing `IOHMM-0.0.3.tar` & `IOHMM-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 mogengyin   (501) staff       (20)        0 2021-02-05 17:34:16.594061 IOHMM-0.0.3/
-drwxr-xr-x   0 mogengyin   (501) staff       (20)        0 2021-02-05 17:34:16.591019 IOHMM-0.0.3/IOHMM/
--rw-r--r--   0 mogengyin   (501) staff       (20)    34782 2021-02-01 04:40:13.000000 IOHMM-0.0.3/IOHMM/IOHMM.py
--rw-r--r--   0 mogengyin   (501) staff       (20)      764 2021-02-05 05:39:27.000000 IOHMM-0.0.3/IOHMM/__init__.py
--rw-r--r--   0 mogengyin   (501) staff       (20)    10223 2021-02-01 04:40:13.000000 IOHMM-0.0.3/IOHMM/forward_backward.py
--rw-r--r--   0 mogengyin   (501) staff       (20)    55038 2021-02-05 06:27:24.000000 IOHMM-0.0.3/IOHMM/linear_models.py
-drwxr-xr-x   0 mogengyin   (501) staff       (20)        0 2021-02-05 17:34:16.593809 IOHMM-0.0.3/IOHMM.egg-info/
--rw-r--r--   0 mogengyin   (501) staff       (20)      995 2021-02-05 17:34:16.000000 IOHMM-0.0.3/IOHMM.egg-info/PKG-INFO
--rw-r--r--   0 mogengyin   (501) staff       (20)      278 2021-02-05 17:34:16.000000 IOHMM-0.0.3/IOHMM.egg-info/SOURCES.txt
--rw-r--r--   0 mogengyin   (501) staff       (20)        1 2021-02-05 17:34:16.000000 IOHMM-0.0.3/IOHMM.egg-info/dependency_links.txt
--rw-r--r--   0 mogengyin   (501) staff       (20)      168 2021-02-05 17:34:16.000000 IOHMM-0.0.3/IOHMM.egg-info/requires.txt
--rw-r--r--   0 mogengyin   (501) staff       (20)        6 2021-02-05 17:34:16.000000 IOHMM-0.0.3/IOHMM.egg-info/top_level.txt
--rw-r--r--   0 mogengyin   (501) staff       (20)        1 2021-02-05 17:34:16.000000 IOHMM-0.0.3/IOHMM.egg-info/zip-safe
--rw-r--r--   0 mogengyin   (501) staff       (20)      995 2021-02-05 17:34:16.594204 IOHMM-0.0.3/PKG-INFO
--rw-r--r--   0 mogengyin   (501) staff       (20)     5445 2021-02-01 04:40:13.000000 IOHMM-0.0.3/README.md
--rw-r--r--   0 mogengyin   (501) staff       (20)      111 2021-02-05 17:34:16.594735 IOHMM-0.0.3/setup.cfg
--rw-r--r--   0 mogengyin   (501) staff       (20)     1606 2021-02-05 06:59:17.000000 IOHMM-0.0.3/setup.py
+drwxr-xr-x   0 mogengyin   (501) staff       (20)        0 2023-05-01 06:03:53.874995 IOHMM-0.0.7/
+drwxr-xr-x   0 mogengyin   (501) staff       (20)        0 2023-05-01 06:03:53.868018 IOHMM-0.0.7/IOHMM/
+-rw-rw-r--   0 mogengyin   (501) staff       (20)    34782 2023-05-01 05:40:06.000000 IOHMM-0.0.7/IOHMM/IOHMM.py
+-rw-rw-r--   0 mogengyin   (501) staff       (20)      764 2023-05-01 05:40:06.000000 IOHMM-0.0.7/IOHMM/__init__.py
+-rw-rw-r--   0 mogengyin   (501) staff       (20)    10223 2023-05-01 05:40:06.000000 IOHMM-0.0.7/IOHMM/forward_backward.py
+-rw-rw-r--   0 mogengyin   (501) staff       (20)    55044 2023-05-01 05:40:06.000000 IOHMM-0.0.7/IOHMM/linear_models.py
+drwxr-xr-x   0 mogengyin   (501) staff       (20)        0 2023-05-01 06:03:53.874451 IOHMM-0.0.7/IOHMM.egg-info/
+-rw-r--r--   0 mogengyin   (501) staff       (20)     1006 2023-05-01 06:03:53.000000 IOHMM-0.0.7/IOHMM.egg-info/PKG-INFO
+-rw-r--r--   0 mogengyin   (501) staff       (20)      286 2023-05-01 06:03:53.000000 IOHMM-0.0.7/IOHMM.egg-info/SOURCES.txt
+-rw-r--r--   0 mogengyin   (501) staff       (20)        1 2023-05-01 06:03:53.000000 IOHMM-0.0.7/IOHMM.egg-info/dependency_links.txt
+-rw-r--r--   0 mogengyin   (501) staff       (20)      167 2023-05-01 06:03:53.000000 IOHMM-0.0.7/IOHMM.egg-info/requires.txt
+-rw-r--r--   0 mogengyin   (501) staff       (20)        6 2023-05-01 06:03:53.000000 IOHMM-0.0.7/IOHMM.egg-info/top_level.txt
+-rw-r--r--   0 mogengyin   (501) staff       (20)        1 2023-05-01 05:48:54.000000 IOHMM-0.0.7/IOHMM.egg-info/zip-safe
+-rw-rw-r--   0 mogengyin   (501) staff       (20)     1535 2023-05-01 05:40:06.000000 IOHMM-0.0.7/LICENCE
+-rw-r--r--   0 mogengyin   (501) staff       (20)     1006 2023-05-01 06:03:53.875112 IOHMM-0.0.7/PKG-INFO
+-rw-rw-r--   0 mogengyin   (501) staff       (20)     5445 2023-05-01 05:40:06.000000 IOHMM-0.0.7/README.md
+-rw-rw-r--   0 mogengyin   (501) staff       (20)      111 2023-05-01 06:03:53.876577 IOHMM-0.0.7/setup.cfg
+-rw-rw-r--   0 mogengyin   (501) staff       (20)     1605 2023-05-01 06:02:05.000000 IOHMM-0.0.7/setup.py
```

### Comparing `IOHMM-0.0.3/IOHMM/IOHMM.py` & `IOHMM-0.0.7/IOHMM/IOHMM.py`

 * *Files identical despite different names*

### Comparing `IOHMM-0.0.3/IOHMM/__init__.py` & `IOHMM-0.0.7/IOHMM/__init__.py`

 * *Files identical despite different names*

### Comparing `IOHMM-0.0.3/IOHMM/forward_backward.py` & `IOHMM-0.0.7/IOHMM/forward_backward.py`

 * *Files identical despite different names*

### Comparing `IOHMM-0.0.3/IOHMM/linear_models.py` & `IOHMM-0.0.7/IOHMM/linear_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,15 +617,15 @@
         def _estimate_dispersion():
             """
             Estimate dispersion matrix based on the fitted model
             Returns
             -------
             dispersion matrix: array of shape (n_targets, n_targets), 2d
             """
-            mu, wendog = _rescale_data(self.predict(X), Y, sample_weight)
+            mu, wendog, _ = _rescale_data(self.predict(X), Y, sample_weight)
             wresid = mu - wendog
             return np.dot(wresid.T, wresid) / np.sum(sample_weight)
 
         def _estimate_stderr():
             """
             Estimate standard deviation of the coefficients.
             Returns
@@ -641,15 +641,15 @@
             regression-coefficients-in-weighted-least-squares-method
             http://pj.freefaculty.org/guides/stat/Regression/GLS/GLS-1-guide.pdf
             https://stats.stackexchange.com/questions/27033/in-r-given-an-output-from-
             optim-with-a-hessian-matrix-how-to-calculate-paramet
             http://msekce.karlin.mff.cuni.cz/~vorisek/Seminar/0910l/jonas.pdf
             """
             if self.reg_method is None or self.alpha < EPS:
-                wexog, wendog = _rescale_data(X_train, Y, sample_weight)
+                wexog, wendog, _ = _rescale_data(X_train, Y, sample_weight)
                 stderr = np.zeros((self.n_targets, X_train.shape[1]))
                 try:
                     XWX_inverse_XW_sqrt = np.linalg.inv(np.dot(wexog.T, wexog)).dot(wexog.T)
                 except np.linalg.linalg.LinAlgError:
                     logging.warning('Covariance matrix is singular, cannot estimate stderr.')
                     return None
                 sqrt_diag_XWX_inverse_XW_sqrt_W_XWX_inverse_XW_sqrt = np.sqrt(np.diag(
```

### Comparing `IOHMM-0.0.3/IOHMM.egg-info/PKG-INFO` & `IOHMM-0.0.7/IOHMM.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: IOHMM
-Version: 0.0.3
+Version: 0.0.7
 Summary: A python library for Input Output Hidden Markov Models
 Home-page: https://github.com/Mogeng/IOHMM
 Author: Mogeng Yin
 Author-email: mogengyin@berkeley.edu
 License: BSD License
-Description: UNKNOWN
 Keywords: python hidden-markov-model graphical-models sequence-to-sequence machine-learning linear-models sequence-labeling supervised-learning semi-supervised-learning unsupervised-learning time-series scikit-learn statsmodels
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: tests
+License-File: LICENCE
+
+UNKNOWN
+
```

### Comparing `IOHMM-0.0.3/PKG-INFO` & `IOHMM-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: IOHMM
-Version: 0.0.3
+Version: 0.0.7
 Summary: A python library for Input Output Hidden Markov Models
 Home-page: https://github.com/Mogeng/IOHMM
 Author: Mogeng Yin
 Author-email: mogengyin@berkeley.edu
 License: BSD License
-Description: UNKNOWN
 Keywords: python hidden-markov-model graphical-models sequence-to-sequence machine-learning linear-models sequence-labeling supervised-learning semi-supervised-learning unsupervised-learning time-series scikit-learn statsmodels
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: tests
+License-File: LICENCE
+
+UNKNOWN
+
```

### Comparing `IOHMM-0.0.3/README.md` & `IOHMM-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `IOHMM-0.0.3/setup.py` & `IOHMM-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 setup(
     name="IOHMM",
-    version="0.0.3",
+    version="0.0.7",
     description='A python library for Input Output Hidden Markov Models',
     url='https://github.com/Mogeng/IOHMM',
     author='Mogeng Yin',
     author_email='mogengyin@berkeley.edu',
     license='BSD License',
     packages=['IOHMM'],
     install_requires=[
         'numpy >= 1.20.0',
         'future >= 0.18.2',
         'pandas >= 1.2.1',
-        'scikit-learn >= 0.24.1',
+        'scikit-learn >= 1.2.2',
         'scipy >= 1.6.0',
         'statsmodels >= 0.12.2',
     ],
     extras_require={
         'tests': [
             'flake8>=3.8.4',
             'mock>=3.9.1',
```

