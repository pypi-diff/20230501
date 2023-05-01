# Comparing `tmp/shareddata-2.0.0.tar.gz` & `tmp/shareddata-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.0.0.tar", last modified: Sat Apr 29 13:15:40 2023, max compression
+gzip compressed data, was "shareddata-2.0.1.tar", last modified: Mon May  1 18:23:06 2023, max compression
```

## Comparing `shareddata-2.0.0.tar` & `shareddata-2.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.565590 shareddata-2.0.0/
--rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1218 2023-04-29 13:15:40.565590 shareddata-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-02-15 20:29:49.000000 shareddata-2.0.0/README.md
--rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-04-29 13:15:40.566592 shareddata-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.542592 shareddata-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.554592 shareddata-2.0.0/src/SharedData/
--rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.0/src/SharedData/Defaults.py
--rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.0/src/SharedData/Logger.py
--rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.0/src/SharedData/LoggerConsumerProcess.py
--rw-rw-rw-   0        0        0    11426 2023-04-14 14:51:54.000000 shareddata-2.0.0/src/SharedData/Metadata.py
--rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/MultiProc.py
--rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/SeriesLib.py
--rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.0/src/SharedData/SharedData.py
--rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.0/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-rw-   0        0        0    11230 2023-03-26 19:43:51.000000 shareddata-2.0.0/src/SharedData/SharedDataAWSS3.py
--rw-rw-rw-   0        0        0     6283 2023-04-25 18:26:16.000000 shareddata-2.0.0/src/SharedData/SharedDataFeeder.py
--rw-rw-rw-   0        0        0    11229 2023-03-09 15:11:52.000000 shareddata-2.0.0/src/SharedData/SharedDataFrame.py
--rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.0/src/SharedData/SharedDataPeriod.py
--rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/SharedDataRealTime.py
--rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-rw-   0        0        0    46626 2023-04-28 21:14:34.000000 shareddata-2.0.0/src/SharedData/SharedDataTable.py
--rw-rw-rw-   0        0        0    18042 2023-03-20 11:50:36.000000 shareddata-2.0.0/src/SharedData/SharedDataTimeSeries.py
--rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.564590 shareddata-2.0.0/src/shareddata.egg-info/
--rw-rw-rw-   0        0        0     1218 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      793 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 18:23:06.543358 shareddata-2.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1218 2023-05-01 18:23:06.543358 shareddata-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-02-15 20:29:49.000000 shareddata-2.0.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-05-01 18:23:06.546358 shareddata-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 18:23:06.514358 shareddata-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 18:23:06.532359 shareddata-2.0.1/src/SharedData/
+-rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.1/src/SharedData/Defaults.py
+-rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.1/src/SharedData/Logger.py
+-rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.1/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-rw-   0        0        0    11426 2023-04-14 14:51:54.000000 shareddata-2.0.1/src/SharedData/Metadata.py
+-rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.1/src/SharedData/MultiProc.py
+-rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.1/src/SharedData/SeriesLib.py
+-rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.1/src/SharedData/SharedData.py
+-rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.1/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-rw-   0        0        0    11230 2023-03-26 19:43:51.000000 shareddata-2.0.1/src/SharedData/SharedDataAWSS3.py
+-rw-rw-rw-   0        0        0     6283 2023-04-25 18:26:16.000000 shareddata-2.0.1/src/SharedData/SharedDataFeeder.py
+-rw-rw-rw-   0        0        0    11229 2023-03-09 15:11:52.000000 shareddata-2.0.1/src/SharedData/SharedDataFrame.py
+-rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.1/src/SharedData/SharedDataPeriod.py
+-rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.1/src/SharedData/SharedDataRealTime.py
+-rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.1/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-rw-   0        0        0    46669 2023-05-01 18:15:41.000000 shareddata-2.0.1/src/SharedData/SharedDataTable.py
+-rw-rw-rw-   0        0        0    18042 2023-03-20 11:50:36.000000 shareddata-2.0.1/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.1/src/SharedData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 18:23:06.542359 shareddata-2.0.1/src/shareddata.egg-info/
+-rw-rw-rw-   0        0        0     1218 2023-05-01 18:23:06.000000 shareddata-2.0.1/src/shareddata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-05-01 18:23:06.000000 shareddata-2.0.1/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 18:23:06.000000 shareddata-2.0.1/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-05-01 18:23:06.000000 shareddata-2.0.1/src/shareddata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 18:23:06.000000 shareddata-2.0.1/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.0.0/LICENSE` & `shareddata-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/PKG-INFO` & `shareddata-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.0
+Version: 2.0.1
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.0/README.md` & `shareddata-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/Defaults.py` & `shareddata-2.0.1/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/Logger.py` & `shareddata-2.0.1/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.0.1/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/Metadata.py` & `shareddata-2.0.1/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/MultiProc.py` & `shareddata-2.0.1/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SeriesLib.py` & `shareddata-2.0.1/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedData.py` & `shareddata-2.0.1/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.0.1/src/SharedData/SharedDataAWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.0.1/src/SharedData/SharedDataAWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataFeeder.py` & `shareddata-2.0.1/src/SharedData/SharedDataFeeder.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataFrame.py` & `shareddata-2.0.1/src/SharedData/SharedDataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataPeriod.py` & `shareddata-2.0.1/src/SharedData/SharedDataPeriod.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataRealTime.py` & `shareddata-2.0.1/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.0.1/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataTable.py` & `shareddata-2.0.1/src/SharedData/SharedDataTable.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,16 @@
 
         descr = self.hdr['descr'].decode(encoding='UTF-8',errors='ignore')
         self.recnames = descr.split(';')[0].split(',')
         self.recformats = descr.split(';')[1].split(',')
         self.recdtype = np.dtype({'names':self.recnames,'formats':self.recformats})
         self.records = SharedNumpy((self.hdr['recordssize'],),\
             dtype=self.recdtype,buffer=self.shm.buf, offset=nb_hdr+nb_pkey)
-        self.records.master = self        
+        self.records.master = self
+        self.release() # release semaphore       
         
     def malloc(self,records=None, mtime=None):
         tini=time.time()
         
         path, shm_name = self.get_path(iswrite=True)
         # test if shared memory already exists        
         try:
```

### Comparing `shareddata-2.0.0/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.0.1/src/SharedData/SharedDataTimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.0/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.0.1/src/shareddata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.0
+Version: 2.0.1
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.0/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.0.1/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

