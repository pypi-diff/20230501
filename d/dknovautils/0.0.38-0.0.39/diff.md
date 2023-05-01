# Comparing `tmp/dknovautils-0.0.38.tar.gz` & `tmp/dknovautils-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.38.tar", last modified: Fri Apr 28 15:26:29 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.39.tar", last modified: Mon May  1 03:42:34 2023, max compression
```

## Comparing `dknovautils-0.0.38.tar` & `dknovautils-0.0.39.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 15:26:29.000000 dknovautils-0.0.38/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 15:26:29.000000 dknovautils-0.0.38/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2474 2023-04-28 15:25:46.000000 dknovautils-0.0.38/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7672 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.38/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.38/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.38/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.38/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.38/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.38/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-28 15:26:29.000000 dknovautils-0.0.38/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-28 15:26:28.000000 dknovautils-0.0.38/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.38/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-28 15:26:29.000000 dknovautils-0.0.38/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.38/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-28 15:26:29.000000 dknovautils-0.0.38/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1158 2023-04-28 15:26:28.000000 dknovautils-0.0.38/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-01 03:42:34.000000 dknovautils-0.0.39/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-01 03:42:34.000000 dknovautils-0.0.39/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2902 2023-05-01 03:41:15.000000 dknovautils-0.0.39/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8010 2023-05-01 03:42:30.000000 dknovautils-0.0.39/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.39/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.39/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-01 03:42:30.000000 dknovautils-0.0.39/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.39/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.39/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.39/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.39/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-01 03:42:34.000000 dknovautils-0.0.39/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-01 03:42:33.000000 dknovautils-0.0.39/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-05-01 03:42:33.000000 dknovautils-0.0.39/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-01 03:42:33.000000 dknovautils-0.0.39/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-01 03:42:33.000000 dknovautils-0.0.39/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-01 03:42:33.000000 dknovautils-0.0.39/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.39/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-05-01 03:42:34.000000 dknovautils-0.0.39/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.39/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-01 03:42:34.000000 dknovautils-0.0.39/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1158 2023-05-01 03:42:30.000000 dknovautils-0.0.39/setup.py
```

### Comparing `dknovautils-0.0.38/dknovautils/commons.py` & `dknovautils-0.0.39/dknovautils/commons.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,26 @@
 
     global _log_inited
     if not _log_inited:
         _log_inited = True
 
         # 只在没有配置的时候起作用 不会重复执行
         logging.basicConfig(level=logging.NOTSET,
+                            # datefmt=AT._default_time_format,
+                            datefmt=AT.STRFMT_ISO_SEC_A,
                             format=AT._LOG_FORMAT_106)
+        
+        '''
+        
+    formatter = logging.Formatter('%(asctime)s.%(msecs)03d-%(name)s-%(filename)s-[line:%(lineno)d]'
+                                  '-%(levelname)s-[日志信息]: %(message)s',
+                                  datefmt='%Y-%m-%d,%H:%M:%S')
+  
+        
+        '''
 
     # 采用这个将级别提升一下。不知为何 NotSET的设置没有生效 并不会打印。
     if level == LLevel.Trace:
         level = LLevel.Debug
 
     logging.log(level.value, obj)
```

### Comparing `dknovautils-0.0.38/dknovautils/dkat.py` & `dknovautils-0.0.39/dknovautils/dkat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.0.38'
+DkAppVer = '0.0.39'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
@@ -60,18 +60,24 @@
         return mloggerFun
 
     _LOG_FORMAT_100 = "%(asctime)s - %(levelname)s - %(message)s"
     _DATE_FORMAT_100 = "%m/%d/%Y %H:%M:%S %p"
     # _DATE_FORMAT_iso_simple = "%m/%d/%Y %H:%M:%S %p"
 
     STRFMT_ISO_COMPACT_SIMPLE = "%Y%m%dT%H%M%S"
-    STRFMT_ISO_COMPACT_ALL_A = "%Y%m%dT%H%M%SS%f"
+    STRFMT_ISO_COMPACT_ALL_A = "%Y%m%dT%H%M%SS%fZ%Z"
     STRFMT_ISO_ALL_A = "%Y-%m-%dT%H:%M:%S.%f%Z"
+    STRFMT_ISO_SEC_A = "%Y-%m-%dT%H:%M:%S"
 
-    _LOG_FORMAT_106 = '%(asctime)s %(name)s %(threadName)s %(levelname)s %(message)s'
+    STRFMT_LOGGER_MS_A = "%Y-%m-%d %H:%M:%S.%f"    
+
+    _default_time_format = '%Y-%m-%d %H:%M:%S'
+
+
+    _LOG_FORMAT_106 = '%(asctime)s.%(msecs)03d %(name)s %(threadName)s [%(levelname)s] %(message)s'
 
     '''
     
     dtstr = datetime.now().strftime("%Y%m%dT%H%M%S")
 
         
     '''
@@ -179,24 +185,26 @@
     print("date and time =", dts)
     
     
     '''
 
     @staticmethod
     def sdf_isocompact_format_datetime(dt=None, *, precise: str = 's'):
-        assert precise in ['a', 'd', 's'], 'err5554 bad precise'
+        assert precise in ['d', 's','ms','a'], 'err5554 bad precise'
 
         if dt is not None:
             AT.unsupported()
 
         dt = AT._now_dt()
         dts = dt.strftime(AT.STRFMT_ISO_COMPACT_ALL_A)
 
         if precise == 'a':
             pass
+        elif precise == 'ms':
+            dts = dts[:(8+0+1+6+4)]        
         elif precise == 's':
             dts = dts[:(8+0+1+6)]
         elif precise == 'd':
             dts = dts[:(8)]
         else:
             AT.never()
 
@@ -222,28 +230,31 @@
 
 "yyyy-MM-ddTHH:mm:ss"
 
 date -I
 
 d date
 s seconds
+ms millis
 a all
 
         '''
-        assert precise in ['a', 'd', 's'], 'err5554 bad precise'
+        assert precise in ['d', 's','ms','a'], 'err5554 bad precise'
 
         if dt is not None:
             dt = datetime.fromtimestamp(dt/1000, tz=None)
         else:
             dt = datetime.now()
 
         dts = dt.strftime(AT.STRFMT_ISO_ALL_A)
 
         if precise == 'a':
             pass
+        elif precise == 'ms':
+            dts = dts[:(10+1+8+4)]        
         elif precise == 's':
             dts = dts[:(10+1+8)]
         elif precise == 'd':
             dts = dts[:(10)]
         else:
             AT.never()
```

### Comparing `dknovautils-0.0.38/dknovautils/dkfiles.py` & `dknovautils-0.0.39/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.38/dknovautils/dkipy.py` & `dknovautils-0.0.39/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.38/dknovautils/dk_imports.py` & `dknovautils-0.0.39/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.38/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.39/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.38
+Version: 0.0.39
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.38/PKG-INFO` & `dknovautils-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.38
+Version: 0.0.39
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.38/setup.py` & `dknovautils-0.0.39/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.38'
+DkAppVer = '0.0.39'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

