# Comparing `tmp/HACKERTBILIB-0.0.5.tar.gz` & `tmp/HACKERTBILIB-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HACKERTBILIB-0.0.5.tar", last modified: Mon May  1 17:12:12 2023, max compression
+gzip compressed data, was "HACKERTBILIB-0.0.5a0.tar", last modified: Mon May  1 17:38:47 2023, max compression
```

## Comparing `HACKERTBILIB-0.0.5.tar` & `HACKERTBILIB-0.0.5a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:12:12.485071 HACKERTBILIB-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-01 17:12:12.469440 HACKERTBILIB-0.0.5/HACKERTBILIB.egg-info/
--rw-rw-rw-   0        0        0      487 2023-05-01 17:12:12.000000 HACKERTBILIB-0.0.5/HACKERTBILIB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-01 17:12:12.000000 HACKERTBILIB-0.0.5/HACKERTBILIB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:12:12.000000 HACKERTBILIB-0.0.5/HACKERTBILIB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:12:12.000000 HACKERTBILIB-0.0.5/HACKERTBILIB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      487 2023-05-01 17:12:12.485071 HACKERTBILIB-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-01 17:12:12.485071 HACKERTBILIB-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-05-01 13:23:01.000000 HACKERTBILIB-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 17:38:47.398561 HACKERTBILIB-0.0.5a0/
+drwxrwxrwx   0        0        0        0 2023-05-01 17:38:47.387555 HACKERTBILIB-0.0.5a0/HACKERTBILIB.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-05-01 17:38:47.000000 HACKERTBILIB-0.0.5a0/HACKERTBILIB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-01 17:38:47.000000 HACKERTBILIB-0.0.5a0/HACKERTBILIB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 17:38:47.000000 HACKERTBILIB-0.0.5a0/HACKERTBILIB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 17:38:47.000000 HACKERTBILIB-0.0.5a0/HACKERTBILIB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      489 2023-05-01 17:38:47.398561 HACKERTBILIB-0.0.5a0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-01 17:38:47.398561 HACKERTBILIB-0.0.5a0/setup.cfg
+-rw-rw-rw-   0        0        0      624 2023-05-01 17:33:31.000000 HACKERTBILIB-0.0.5a0/setup.py
```

### Comparing `HACKERTBILIB-0.0.5/setup.py` & `HACKERTBILIB-0.0.5a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='HACKERTBILIB',
-  version='0.0.5',
+  version='0.0.5a',
   description='Python extenctions and functions',
   author='Tobias Vastak as HACKERT_BI',
   author_email='tobias.vastak@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='HACEXTENCIONS',
   packages=find_packages(),
```

