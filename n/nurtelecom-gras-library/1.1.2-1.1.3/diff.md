# Comparing `tmp/nurtelecom_gras_library-1.1.2.tar.gz` & `tmp/nurtelecom_gras_library-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nurtelecom_gras_library-1.1.2.tar", last modified: Fri Feb  3 11:11:38 2023, max compression
+gzip compressed data, was "nurtelecom_gras_library-1.1.3.tar", last modified: Mon May  1 09:25:08 2023, max compression
```

## Comparing `nurtelecom_gras_library-1.1.2.tar` & `nurtelecom_gras_library-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-03 11:11:38.116603 nurtelecom_gras_library-1.1.2/
--rwxrwxrwx   0 root         (0) root         (0)      749 2023-02-03 11:11:38.118605 nurtelecom_gras_library-1.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      315 2022-12-06 06:19:22.000000 nurtelecom_gras_library-1.1.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-02-03 11:11:38.124604 nurtelecom_gras_library-1.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1324 2023-02-03 11:10:03.000000 nurtelecom_gras_library-1.1.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-03 11:11:37.771610 nurtelecom_gras_library-1.1.2/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-03 11:11:37.917609 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/
--rwxrwxrwx   0 root         (0) root         (0)     6898 2023-02-03 11:10:43.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/PLSQL_data_importer.py
--rwxrwxrwx   0 root         (0) root         (0)     2797 2023-02-03 10:05:29.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/PLSQL_geodata_importer.py
--rwxrwxrwx   0 root         (0) root         (0)      307 2023-01-27 03:29:34.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:01:23.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/additional_functions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-03 11:11:38.088606 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      749 2023-02-03 11:11:36.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      479 2023-02-03 11:11:36.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-02-03 11:11:36.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-02-03 11:11:36.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-02-03 11:11:36.000000 nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library.egg-info/top_level.txt
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.161090 nurtelecom_gras_library-1.1.3/
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      693 2023-05-01 09:25:08.161539 nurtelecom_gras_library-1.1.3/PKG-INFO
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      315 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/README.md
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      107 2023-05-01 09:25:08.163325 nurtelecom_gras_library-1.1.3/setup.cfg
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     1324 2023-05-01 09:24:31.000000 nurtelecom_gras_library-1.1.3/setup.py
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.136416 nurtelecom_gras_library-1.1.3/src/
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.149080 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     6927 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_data_importer.py
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     2797 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_geodata_importer.py
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      307 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/__init__.py
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     7399 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/additional_functions.py
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.160426 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      693 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/PKG-INFO
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      479 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/SOURCES.txt
+-rw-r--r--   0 kazamabeks   (501) staff       (20)        1 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/dependency_links.txt
+-rw-r--r--   0 kazamabeks   (501) staff       (20)       60 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/requires.txt
+-rw-r--r--   0 kazamabeks   (501) staff       (20)       24 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/top_level.txt
```

### Comparing `nurtelecom_gras_library-1.1.2/PKG-INFO` & `nurtelecom_gras_library-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nurtelecom_gras_library
-Version: 1.1.2
-Summary: UNKNOWN
+Version: 1.1.3
 Home-page: https://github.com/beksultantuleev/nurtelecom_gras_library.git
 Author: Beksultan Tuleev
 Author-email: kazamabeks@gmail.com
 License: MIT
-Description: UNKNOWN
 Keywords: NurTelecom
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nurtelecom_gras_library-1.1.2/setup.py` & `nurtelecom_gras_library-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='nurtelecom_gras_library',
-    version='1.1.2',
+    version='1.1.3',
     license='MIT',
     author="Beksultan Tuleev",
     author_email='kazamabeks@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/beksultantuleev/nurtelecom_gras_library.git',
     keywords='NurTelecom',
```

### Comparing `nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/PLSQL_data_importer.py` & `nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_data_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
                         VALUES({payload});
                     COMMIT;
                 END;
             '''
         return query
 
     def execute(self, query):
+        query = text(query)
         self.engine = create_engine(self.ENGINE_PATH_WIN_AUTH)
         self.conn = self.engine.connect()
         with self.engine.connect() as conn:
             conn.execute(text(query))  # text
             conn.close()
             print('Connection in execute is closed!')
         self.conn.close()
```

### Comparing `nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/PLSQL_geodata_importer.py` & `nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_geodata_importer.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library/additional_functions.py` & `nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/additional_functions.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.1.2/src/nurtelecom_gras_library.egg-info/PKG-INFO` & `nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nurtelecom-gras-library
-Version: 1.1.2
-Summary: UNKNOWN
+Version: 1.1.3
 Home-page: https://github.com/beksultantuleev/nurtelecom_gras_library.git
 Author: Beksultan Tuleev
 Author-email: kazamabeks@gmail.com
 License: MIT
-Description: UNKNOWN
 Keywords: NurTelecom
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

