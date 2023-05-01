# Comparing `tmp/sayhellox123-0.5.tar.gz` & `tmp/sayhellox123-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayhellox123-0.5.tar", last modified: Mon May  1 16:21:12 2023, max compression
+gzip compressed data, was "sayhellox123-0.6.tar", last modified: Mon May  1 16:24:14 2023, max compression
```

## Comparing `sayhellox123-0.5.tar` & `sayhellox123-0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 16:21:12.907905 sayhellox123-0.5/
--rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 16:21:12.907777 sayhellox123-0.5/PKG-INFO
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 16:21:12.907184 sayhellox123-0.5/helloworld/
--rw-r--r--   0 manosriram   (501) staff       (20)       25 2023-05-01 16:21:01.000000 sayhellox123-0.5/helloworld/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)      177 2023-05-01 15:43:15.000000 sayhellox123-0.5/helloworld/a.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 16:21:12.907640 sayhellox123-0.5/sayhellox123.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 16:21:12.000000 sayhellox123-0.5/sayhellox123.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      191 2023-05-01 16:21:12.000000 sayhellox123-0.5/sayhellox123.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-01 16:21:12.000000 sayhellox123-0.5/sayhellox123.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       11 2023-05-01 16:21:12.000000 sayhellox123-0.5/sayhellox123.egg-info/top_level.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-01 16:21:12.907944 sayhellox123-0.5/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)      144 2023-05-01 16:21:09.000000 sayhellox123-0.5/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 16:24:14.607259 sayhellox123-0.6/
+-rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 16:24:14.607135 sayhellox123-0.6/PKG-INFO
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 16:24:14.606412 sayhellox123-0.6/helloworld/
+-rw-r--r--   0 manosriram   (501) staff       (20)       25 2023-05-01 16:21:01.000000 sayhellox123-0.6/helloworld/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      177 2023-05-01 15:43:15.000000 sayhellox123-0.6/helloworld/a.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-01 16:24:14.606984 sayhellox123-0.6/sayhellox123.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)       86 2023-05-01 16:24:14.000000 sayhellox123-0.6/sayhellox123.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      230 2023-05-01 16:24:14.000000 sayhellox123-0.6/sayhellox123.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-01 16:24:14.000000 sayhellox123-0.6/sayhellox123.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       54 2023-05-01 16:24:14.000000 sayhellox123-0.6/sayhellox123.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       11 2023-05-01 16:24:14.000000 sayhellox123-0.6/sayhellox123.egg-info/top_level.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-01 16:24:14.607295 sayhellox123-0.6/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)      255 2023-05-01 16:24:11.000000 sayhellox123-0.6/setup.py
```

