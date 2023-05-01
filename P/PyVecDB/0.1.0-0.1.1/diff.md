# Comparing `tmp/PyVecDB-0.1.0.tar.gz` & `tmp/PyVecDB-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVecDB-0.1.0.tar", last modified: Mon May  1 10:43:50 2023, max compression
+gzip compressed data, was "PyVecDB-0.1.1.tar", last modified: Mon May  1 11:19:41 2023, max compression
```

## Comparing `PyVecDB-0.1.0.tar` & `PyVecDB-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:43:50.655727 PyVecDB-0.1.0/
--rw-rw-rw-   0        0        0     2392 2023-05-01 10:43:50.655727 PyVecDB-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 10:43:50.625073 PyVecDB-0.1.0/PyVecDB.egg-info/
--rw-rw-rw-   0        0        0     2392 2023-05-01 10:43:50.000000 PyVecDB-0.1.0/PyVecDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-01 10:43:50.000000 PyVecDB-0.1.0/PyVecDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:43:50.000000 PyVecDB-0.1.0/PyVecDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 10:43:50.000000 PyVecDB-0.1.0/PyVecDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 10:43:50.000000 PyVecDB-0.1.0/PyVecDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1658 2023-05-01 10:33:10.000000 PyVecDB-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 10:43:50.655727 PyVecDB-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-01 10:42:28.000000 PyVecDB-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:43:50.655727 PyVecDB-0.1.0/src/
--rw-rw-rw-   0        0        0       29 2023-05-01 07:38:16.000000 PyVecDB-0.1.0/src/__init__.py
--rw-rw-rw-   0        0        0     1583 2023-05-01 07:47:53.000000 PyVecDB-0.1.0/src/data_object.py
--rw-rw-rw-   0        0        0      459 2023-04-30 14:04:33.000000 PyVecDB-0.1.0/src/database.py
--rw-rw-rw-   0        0        0     1742 2023-05-01 07:37:56.000000 PyVecDB-0.1.0/src/stress_test.py
--rw-rw-rw-   0        0        0     3875 2023-04-30 16:05:40.000000 PyVecDB-0.1.0/src/vector_db.py
--rw-rw-rw-   0        0        0     5102 2023-05-01 08:46:52.000000 PyVecDB-0.1.0/src/word_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:43:50.655727 PyVecDB-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-01 07:35:27.000000 PyVecDB-0.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/
+-rw-rw-rw-   0        0        0     2666 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/PyVecDB.egg-info/
+-rw-rw-rw-   0        0        0     2666 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1928 2023-05-01 11:15:48.000000 PyVecDB-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-01 11:18:13.000000 PyVecDB-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/src/
+-rw-rw-rw-   0        0        0       29 2023-05-01 07:38:16.000000 PyVecDB-0.1.1/src/__init__.py
+-rw-rw-rw-   0        0        0     1583 2023-05-01 07:47:53.000000 PyVecDB-0.1.1/src/data_object.py
+-rw-rw-rw-   0        0        0      459 2023-04-30 14:04:33.000000 PyVecDB-0.1.1/src/database.py
+-rw-rw-rw-   0        0        0     1742 2023-05-01 07:37:56.000000 PyVecDB-0.1.1/src/stress_test.py
+-rw-rw-rw-   0        0        0     3875 2023-04-30 16:05:40.000000 PyVecDB-0.1.1/src/vector_db.py
+-rw-rw-rw-   0        0        0     5102 2023-05-01 08:46:52.000000 PyVecDB-0.1.1/src/word_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:35:27.000000 PyVecDB-0.1.1/tests/__init__.py
```

### Comparing `PyVecDB-0.1.0/PKG-INFO` & `PyVecDB-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVecDB
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for efficient similarity search using high-dimensional vectors.
 Home-page: https://github.com/tyronenorth/PyVecDB
 Author: Your Name
 Author-email: north.tyronejr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -70,8 +70,15 @@
 
 Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) to get started.
 
 ## License
 
 PyVecDB is released under the [MIT License](LICENSE).
 
+## Support
+
+If you like my work consider buying me a coffee â˜• Support my work on Patreon or PayPal!
+
+[![Support me on Patreon](https://img.shields.io/badge/patreon-support-%23e85b46.svg?logo=patreon&style=for-the-badge)](https://www.patreon.com/SimulatedDev)
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyVecDB-0.1.0/PyVecDB.egg-info/PKG-INFO` & `PyVecDB-0.1.1/PyVecDB.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVecDB
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for efficient similarity search using high-dimensional vectors.
 Home-page: https://github.com/tyronenorth/PyVecDB
 Author: Your Name
 Author-email: north.tyronejr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -70,8 +70,15 @@
 
 Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) to get started.
 
 ## License
 
 PyVecDB is released under the [MIT License](LICENSE).
 
+## Support
+
+If you like my work consider buying me a coffee â˜• Support my work on Patreon or PayPal!
+
+[![Support me on Patreon](https://img.shields.io/badge/patreon-support-%23e85b46.svg?logo=patreon&style=for-the-badge)](https://www.patreon.com/SimulatedDev)
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyVecDB-0.1.0/README.md` & `PyVecDB-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -50,7 +50,14 @@
 ## Contributing
 
 Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) to get started.
 
 ## License
 
 PyVecDB is released under the [MIT License](LICENSE).
+
+## Support
+
+If you like my work consider buying me a coffee ☕ Support my work on Patreon or PayPal!
+
+[![Support me on Patreon](https://img.shields.io/badge/patreon-support-%23e85b46.svg?logo=patreon&style=for-the-badge)](https://www.patreon.com/SimulatedDev)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyVecDB-0.1.0/setup.py` & `PyVecDB-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="PyVecDB",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "annoy",
         "msgpack",
         "sqlite3",
     ],
     author="Your Name",
```

### Comparing `PyVecDB-0.1.0/src/data_object.py` & `PyVecDB-0.1.1/src/data_object.py`

 * *Files identical despite different names*

### Comparing `PyVecDB-0.1.0/src/stress_test.py` & `PyVecDB-0.1.1/src/stress_test.py`

 * *Files identical despite different names*

### Comparing `PyVecDB-0.1.0/src/vector_db.py` & `PyVecDB-0.1.1/src/vector_db.py`

 * *Files identical despite different names*

### Comparing `PyVecDB-0.1.0/src/word_generator.py` & `PyVecDB-0.1.1/src/word_generator.py`

 * *Files identical despite different names*

