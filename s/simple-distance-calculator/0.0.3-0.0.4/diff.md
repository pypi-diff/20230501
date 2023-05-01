# Comparing `tmp/simple_distance_calculator-0.0.3.tar.gz` & `tmp/simple_distance_calculator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_distance_calculator-0.0.3.tar", last modified: Sun Apr 30 12:03:09 2023, max compression
+gzip compressed data, was "simple_distance_calculator-0.0.4.tar", last modified: Mon May  1 16:28:18 2023, max compression
```

## Comparing `simple_distance_calculator-0.0.3.tar` & `simple_distance_calculator-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.956183 simple_distance_calculator-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-04-29 21:15:11.000000 simple_distance_calculator-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1302 2023-04-30 12:03:09.956757 simple_distance_calculator-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-04-30 12:02:21.000000 simple_distance_calculator-0.0.3/README.txt
--rw-rw-rw-   0        0        0       95 2023-04-29 21:01:23.000000 simple_distance_calculator-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      378 2023-04-30 12:03:09.961679 simple_distance_calculator-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-04-30 12:02:55.000000 simple_distance_calculator-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.929731 simple_distance_calculator-0.0.3/simple_distance_calculator/
--rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.3/simple_distance_calculator/__init__.py
--rw-rw-rw-   0        0        0     1871 2023-04-28 19:34:41.000000 simple_distance_calculator-0.0.3/simple_distance_calculator/distance.py
-drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.950795 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/
--rw-rw-rw-   0        0        0     1302 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-30 12:03:09.000000 simple_distance_calculator-0.0.3/simple_distance_calculator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 12:03:09.954906 simple_distance_calculator-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2085 2023-04-29 21:05:06.000000 simple_distance_calculator-0.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:28:18.493961 simple_distance_calculator-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-04-29 21:15:11.000000 simple_distance_calculator-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3548 2023-05-01 16:28:18.494958 simple_distance_calculator-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-05-01 16:23:12.000000 simple_distance_calculator-0.0.4/README.txt
+-rw-rw-rw-   0        0        0       95 2023-04-29 21:01:23.000000 simple_distance_calculator-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      378 2023-05-01 16:28:18.497414 simple_distance_calculator-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      494 2023-05-01 16:27:31.000000 simple_distance_calculator-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:28:18.470317 simple_distance_calculator-0.0.4/simple_distance_calculator/
+-rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.4/simple_distance_calculator/__init__.py
+-rw-rw-rw-   0        0        0     1871 2023-04-28 19:34:41.000000 simple_distance_calculator-0.0.4/simple_distance_calculator/distance.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:28:18.489140 simple_distance_calculator-0.0.4/simple_distance_calculator.egg-info/
+-rw-rw-rw-   0        0        0     3548 2023-05-01 16:28:18.000000 simple_distance_calculator-0.0.4/simple_distance_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-01 16:28:18.000000 simple_distance_calculator-0.0.4/simple_distance_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 16:28:18.000000 simple_distance_calculator-0.0.4/simple_distance_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-01 16:28:18.000000 simple_distance_calculator-0.0.4/simple_distance_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 16:28:18.492040 simple_distance_calculator-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-27 17:58:57.000000 simple_distance_calculator-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2085 2023-04-29 21:05:06.000000 simple_distance_calculator-0.0.4/tests/test.py
```

### Comparing `simple_distance_calculator-0.0.3/LICENSE.txt` & `simple_distance_calculator-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_distance_calculator-0.0.3/simple_distance_calculator/distance.py` & `simple_distance_calculator-0.0.4/simple_distance_calculator/distance.py`

 * *Files identical despite different names*

### Comparing `simple_distance_calculator-0.0.3/tests/test.py` & `simple_distance_calculator-0.0.4/tests/test.py`

 * *Files identical despite different names*

