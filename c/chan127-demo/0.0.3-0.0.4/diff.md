# Comparing `tmp/chan127-demo-0.0.3.tar.gz` & `tmp/chan127-demo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chan127-demo-0.0.3.tar", last modified: Sat Apr 29 11:42:07 2023, max compression
+gzip compressed data, was "chan127-demo-0.0.4.tar", last modified: Mon May  1 21:25:29 2023, max compression
```

## Comparing `chan127-demo-0.0.3.tar` & `chan127-demo-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 10:46:05.000000 chan127-demo-0.0.3/LICENSE
--rw-r--r--   0 cheukkaichan   (501) staff       (20)       31 2023-04-29 11:28:57.000000 chan127-demo-0.0.3/MANIFEST.in
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      199 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/PKG-INFO
-drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/chan127_demo.egg-info/
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      199 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/chan127_demo.egg-info/PKG-INFO
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      280 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/chan127_demo.egg-info/SOURCES.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        1 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/chan127_demo.egg-info/dependency_links.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)       55 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/chan127_demo.egg-info/entry_points.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)       13 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/chan127_demo.egg-info/requires.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        7 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/chan127_demo.egg-info/top_level.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)       38 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/setup.cfg
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      335 2023-04-29 11:41:59.000000 chan127-demo-0.0.3/setup.py
-drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:42:07.000000 chan127-demo-0.0.3/showdf/
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 10:47:13.000000 chan127-demo-0.0.3/showdf/__init__.py
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      341 2023-04-29 11:11:25.000000 chan127-demo-0.0.3/showdf/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:25:29.432401 chan127-demo-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:25:15.000000 chan127-demo-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 21:25:15.000000 chan127-demo-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 21:25:29.432401 chan127-demo-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 21:25:15.000000 chan127-demo-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:25:29.432401 chan127-demo-0.0.4/chan127_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 21:25:29.000000 chan127-demo-0.0.4/chan127_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-01 21:25:29.000000 chan127-demo-0.0.4/chan127_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:25:29.000000 chan127-demo-0.0.4/chan127_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 21:25:29.000000 chan127-demo-0.0.4/chan127_demo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 21:25:29.000000 chan127-demo-0.0.4/chan127_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 21:25:29.000000 chan127-demo-0.0.4/chan127_demo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:25:29.432401 chan127-demo-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-01 21:25:15.000000 chan127-demo-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:25:29.432401 chan127-demo-0.0.4/showdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:25:15.000000 chan127-demo-0.0.4/showdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-01 21:25:15.000000 chan127-demo-0.0.4/showdf/main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

