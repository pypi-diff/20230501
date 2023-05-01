# Comparing `tmp/locbuf-0.0.6.tar.gz` & `tmp/locbuf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/locbuf-0.0.6.tar", last modified: Sun Apr 10 11:46:52 2022, max compression
+gzip compressed data, was "dist/locbuf-0.0.7.tar", last modified: Mon May  1 13:28:10 2023, max compression
```

## Comparing `locbuf-0.0.6.tar` & `locbuf-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wenzhu     (501) staff       (20)        0 2022-04-10 11:46:52.000000 locbuf-0.0.6/
--rw-r--r--   0 wenzhu     (501) staff       (20)      268 2022-04-10 11:46:52.000000 locbuf-0.0.6/PKG-INFO
-drwxr-xr-x   0 wenzhu     (501) staff       (20)        0 2022-04-10 11:46:52.000000 locbuf-0.0.6/locbuf/
--rw-r--r--   0 wenzhu     (501) staff       (20)     7193 2022-04-10 11:40:33.000000 locbuf-0.0.6/locbuf/locbuf.py
--rw-r--r--   0 wenzhu     (501) staff       (20)       94 2022-04-10 11:39:24.000000 locbuf-0.0.6/locbuf/__init__.py
--rw-r--r--   0 wenzhu     (501) staff       (20)      417 2022-04-10 11:45:04.000000 locbuf-0.0.6/setup.py
--rw-r--r--   0 wenzhu     (501) staff       (20)       59 2022-04-10 11:46:52.000000 locbuf-0.0.6/setup.cfg
-drwxr-xr-x   0 wenzhu     (501) staff       (20)        0 2022-04-10 11:46:52.000000 locbuf-0.0.6/locbuf.egg-info/
--rw-r--r--   0 wenzhu     (501) staff       (20)      268 2022-04-10 11:46:51.000000 locbuf-0.0.6/locbuf.egg-info/PKG-INFO
--rw-r--r--   0 wenzhu     (501) staff       (20)      193 2022-04-10 11:46:52.000000 locbuf-0.0.6/locbuf.egg-info/SOURCES.txt
--rw-r--r--   0 wenzhu     (501) staff       (20)       13 2022-04-10 11:46:51.000000 locbuf-0.0.6/locbuf.egg-info/requires.txt
--rw-r--r--   0 wenzhu     (501) staff       (20)        7 2022-04-10 11:46:51.000000 locbuf-0.0.6/locbuf.egg-info/top_level.txt
--rw-r--r--   0 wenzhu     (501) staff       (20)        1 2022-04-10 11:46:51.000000 locbuf-0.0.6/locbuf.egg-info/dependency_links.txt
+drwxr-xr-x   0 wenzhu     (501) staff       (20)        0 2023-05-01 13:28:10.000000 locbuf-0.0.7/
+-rw-r--r--   0 wenzhu     (501) staff       (20)      268 2023-05-01 13:28:10.000000 locbuf-0.0.7/PKG-INFO
+drwxr-xr-x   0 wenzhu     (501) staff       (20)        0 2023-05-01 13:28:10.000000 locbuf-0.0.7/locbuf/
+-rw-r--r--   0 wenzhu     (501) staff       (20)     7194 2023-05-01 13:23:52.000000 locbuf-0.0.7/locbuf/locbuf.py
+-rw-r--r--   0 wenzhu     (501) staff       (20)       94 2023-05-01 09:25:43.000000 locbuf-0.0.7/locbuf/__init__.py
+-rw-r--r--   0 wenzhu     (501) staff       (20)      417 2023-05-01 13:24:09.000000 locbuf-0.0.7/setup.py
+-rw-r--r--   0 wenzhu     (501) staff       (20)       59 2023-05-01 13:28:10.000000 locbuf-0.0.7/setup.cfg
+drwxr-xr-x   0 wenzhu     (501) staff       (20)        0 2023-05-01 13:28:10.000000 locbuf-0.0.7/locbuf.egg-info/
+-rw-r--r--   0 wenzhu     (501) staff       (20)      268 2023-05-01 13:28:10.000000 locbuf-0.0.7/locbuf.egg-info/PKG-INFO
+-rw-r--r--   0 wenzhu     (501) staff       (20)      193 2023-05-01 13:28:10.000000 locbuf-0.0.7/locbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 wenzhu     (501) staff       (20)       13 2023-05-01 13:28:10.000000 locbuf-0.0.7/locbuf.egg-info/requires.txt
+-rw-r--r--   0 wenzhu     (501) staff       (20)        7 2023-05-01 13:28:10.000000 locbuf-0.0.7/locbuf.egg-info/top_level.txt
+-rw-r--r--   0 wenzhu     (501) staff       (20)        1 2023-05-01 13:28:10.000000 locbuf-0.0.7/locbuf.egg-info/dependency_links.txt
```

### Comparing `locbuf-0.0.6/locbuf/locbuf.py` & `locbuf-0.0.7/locbuf/locbuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,28 +99,28 @@
         return df
 
     # decorate method
     # ------------------------------------------------------------------
     #
     def csv_buffer(self, tag=None, dfdt_arg=None, strt_arg=None, end_arg=None):
         def decorate(func, *args):
-            @wraps(func)            
+            @wraps(func)
             def wrapper(instance, *args, **kwargs):
                 funcname = func.__qualname__
                 filename = '{}.csv'.format(kwargs.get(tag) or funcname)
                 stockfile = list((self.tmp_path / funcname).glob(filename))
                 # --- no tmp file yet, request and save ---
                 if not stockfile:
                     logger.info('new file {} -> {}'.format(funcname, filename))
                     reqdf = func(instance, *args, **kwargs)
                     drydf = self._normalize_df(reqdf, dfdt_arg)
                     self._save_csv(drydf, self.tmp_path / funcname / filename)
                     return drydf
                 stockfile = stockfile.pop()
-                csv_df = self._normalize_df(pd.read_csv(stockfile), dfdt_arg)
+                csv_df = self._normalize_df(pd.read_csv(stockfile, index_col=0), dfdt_arg)
                 # --- func has no date-arg, use ctime ---
                 if not strt_arg or not end_arg:
                     logger.info('func has no date-args, use mtime method')
                     if self._is_overtimed(stockfile):
                         # --- update csv file ---
                         logger.info('{} overtimed, renew'.format(stockfile))
                         df = func(instance, *args, **kwargs)
```

