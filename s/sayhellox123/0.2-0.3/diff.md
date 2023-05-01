# Comparing `tmp/sayhellox123-0.2.tar.gz` & `tmp/sayhellox123-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayhellox123-0.2.tar", last modified: Mon May  1 15:43:45 2023, max compression
+gzip compressed data, was "sayhellox123-0.3.tar", last modified: Mon May  1 15:48:02 2023, max compression
```

## Comparing `sayhellox123-0.2.tar` & `sayhellox123-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 15:43:45.319854 sayhellox123-0.2/
--rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 15:43:45.319705 sayhellox123-0.2/PKG-INFO
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 15:43:45.319107 sayhellox123-0.2/helloworld/
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-01 15:43:13.000000 sayhellox123-0.2/helloworld/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)      177 2023-05-01 15:43:15.000000 sayhellox123-0.2/helloworld/a.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 15:43:45.319557 sayhellox123-0.2/sayhellox123.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 15:43:45.000000 sayhellox123-0.2/sayhellox123.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      191 2023-05-01 15:43:45.000000 sayhellox123-0.2/sayhellox123.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-01 15:43:45.000000 sayhellox123-0.2/sayhellox123.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       11 2023-05-01 15:43:45.000000 sayhellox123-0.2/sayhellox123.egg-info/top_level.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-01 15:43:45.319891 sayhellox123-0.2/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)      144 2023-05-01 15:43:39.000000 sayhellox123-0.2/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 15:48:02.657410 sayhellox123-0.3/
+-rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 15:48:02.657286 sayhellox123-0.3/PKG-INFO
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 15:48:02.656672 sayhellox123-0.3/helloworld/
+-rw-r--r--   0 manosriram   (501) staff       (20)       25 2023-05-01 15:47:43.000000 sayhellox123-0.3/helloworld/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      177 2023-05-01 15:43:15.000000 sayhellox123-0.3/helloworld/a.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 15:48:02.657131 sayhellox123-0.3/sayhellox123.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 15:48:02.000000 sayhellox123-0.3/sayhellox123.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      191 2023-05-01 15:48:02.000000 sayhellox123-0.3/sayhellox123.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-01 15:48:02.000000 sayhellox123-0.3/sayhellox123.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       11 2023-05-01 15:48:02.000000 sayhellox123-0.3/sayhellox123.egg-info/top_level.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-01 15:48:02.657442 sayhellox123-0.3/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)      144 2023-05-01 15:47:55.000000 sayhellox123-0.3/setup.py
```

