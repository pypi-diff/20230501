# Comparing `tmp/nwebclient-1.0.79.tar.gz` & `tmp/nwebclient-1.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.79.tar", last modified: Thu Apr 27 11:54:57 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.80.tar", last modified: Mon May  1 06:03:06 2023, max compression
```

## Comparing `nwebclient-1.0.79.tar` & `nwebclient-1.0.80.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 11:54:57.555689 nwebclient-1.0.79/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.79/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-27 11:54:57.555689 nwebclient-1.0.79/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.79/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 11:54:57.545689 nwebclient-1.0.79/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.79/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.79/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3274 2023-04-26 10:42:29.000000 nwebclient-1.0.79/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10590 2023-04-27 10:43:05.000000 nwebclient-1.0.79/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5625 2023-04-26 11:35:41.000000 nwebclient-1.0.79/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.79/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 11:54:57.555689 nwebclient-1.0.79/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-27 11:54:57.555689 nwebclient-1.0.79/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-04-27 11:54:52.000000 nwebclient-1.0.79/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-01 06:03:06.043084 nwebclient-1.0.80/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.80/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-01 06:03:06.043084 nwebclient-1.0.80/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.80/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-01 06:03:06.033085 nwebclient-1.0.80/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.80/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.80/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3274 2023-04-26 10:42:29.000000 nwebclient-1.0.80/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10798 2023-05-01 06:01:24.000000 nwebclient-1.0.80/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5625 2023-04-26 11:35:41.000000 nwebclient-1.0.80/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.80/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-01 06:03:06.043084 nwebclient-1.0.80/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-01 06:03:05.000000 nwebclient-1.0.80/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-01 06:03:05.000000 nwebclient-1.0.80/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-01 06:03:05.000000 nwebclient-1.0.80/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-01 06:03:05.000000 nwebclient-1.0.80/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-01 06:03:05.000000 nwebclient-1.0.80/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-01 06:03:05.000000 nwebclient-1.0.80/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-01 06:03:06.043084 nwebclient-1.0.80/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-01 06:02:57.000000 nwebclient-1.0.80/setup.py
```

### Comparing `nwebclient-1.0.79/LICENSE` & `nwebclient-1.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.79/PKG-INFO` & `nwebclient-1.0.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.79
+Version: 1.0.80
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.79/README.md` & `nwebclient-1.0.80/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.79/nwebclient/__init__.py` & `nwebclient-1.0.80/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.79/nwebclient/__main__.py` & `nwebclient-1.0.80/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.79/nwebclient/crypt.py` & `nwebclient-1.0.80/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.79/nwebclient/sd.py` & `nwebclient-1.0.80/nwebclient/sd.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,21 @@
             res = requests.post(result_url, params=params, files=files)
             print(res.text)
             os.remove('data.db')
         self.info("End: "+time.strftime("%Y-%m-%d, %H:%M:%S", time.localtime()))
         return i
     def executeFromUrl(self, url, askForMore= True):
         res = requests.get(url)
-        data = json.loads(res.text)
+        try:
+            data = json.loads(res.text)
+        except:
+            self.info("Error: JSON Decode Error");
+            self.info(res.text)
+            self.info("Error: JSON Decode Error");
+            return 0
         i = self.executeJobs(data)
         if i > 0 and askForMore:
             self.info('Asking for more Work')
             i = i + self.executeFromUrl(url, True)
         return i
     def info(self, message):
         print("[INFO] " + message)
@@ -209,15 +215,16 @@
         self.loaded_model = model
         self.api.set_options(options)
     def __str__(self):
         return f'ImageGen {self.generator} {self.model_id} {self.prefix}'
     def __repr__(self):
         return f'ImageGen(generator=\'{self.generator}\', model_id=\'{self.model_id}\', prefix=\'{self.prefix}\')'
     def toSdJob(count:50):
-        return {prefix:self.prefix, prompt:self.prompt, count:count, height: self.height, self.width: width}
+        data = {prefix:self.prefix, prompt:self.prompt, count:count, height: self.height, self.width: width}
+        return data
             
         
 class ImageGenProcess(ticker.FileExtObserver):
     ext = ".sdjob"
     def __init__(self, generator=None):
         if generator is None:
             generator = ImageGen()
```

### Comparing `nwebclient-1.0.79/nwebclient/sdb.py` & `nwebclient-1.0.80/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.79/nwebclient/ticker.py` & `nwebclient-1.0.80/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.79/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.80/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.79
+Version: 1.0.80
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.79/setup.py` & `nwebclient-1.0.80/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.79",
+    version="1.0.80",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

