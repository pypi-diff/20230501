# Comparing `tmp/orpc-client-0.1.3.tar.gz` & `tmp/orpc-client-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orpc-client-0.1.3.tar", last modified: Wed Dec 14 01:36:28 2022, max compression
+gzip compressed data, was "orpc-client-0.5.8.tar", last modified: Mon May  1 12:18:48 2023, max compression
```

## Comparing `orpc-client-0.1.3.tar` & `orpc-client-0.5.8.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-12-14 01:36:28.486123 orpc-client-0.1.3/
--rw-r--r--   0 test       (501) staff       (20)      136 2022-12-11 09:33:22.000000 orpc-client-0.1.3/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1435 2022-12-14 01:36:28.485942 orpc-client-0.1.3/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      852 2022-12-14 01:09:55.000000 orpc-client-0.1.3/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-12-14 01:36:28.485712 orpc-client-0.1.3/orpc_client.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1435 2022-12-14 01:36:28.000000 orpc-client-0.1.3/orpc_client.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      308 2022-12-14 01:36:28.000000 orpc-client-0.1.3/orpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-12-14 01:36:28.000000 orpc-client-0.1.3/orpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)       20 2022-12-14 01:36:28.000000 orpc-client-0.1.3/orpc_client.egg-info/entry_points.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-12-14 01:36:28.000000 orpc-client-0.1.3/orpc_client.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       40 2022-12-14 01:36:28.000000 orpc-client-0.1.3/orpc_client.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       12 2022-12-14 01:36:28.000000 orpc-client-0.1.3/orpc_client.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)     5682 2022-12-14 01:11:03.000000 orpc-client-0.1.3/orpc_client.py
--rw-r--r--   0 test       (501) staff       (20)       40 2022-12-14 01:15:16.000000 orpc-client-0.1.3/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2022-12-14 01:36:28.486170 orpc-client-0.1.3/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1493 2022-12-14 01:31:38.000000 orpc-client-0.1.3/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-01 12:18:48.016284 orpc-client-0.5.8/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2023-04-27 06:54:41.000000 orpc-client-0.5.8/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      148 2023-04-27 06:54:54.000000 orpc-client-0.5.8/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)      707 2023-05-01 12:18:48.016156 orpc-client-0.5.8/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      113 2023-05-01 12:18:16.000000 orpc-client-0.5.8/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-01 12:18:48.014991 orpc-client-0.5.8/orpc/
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-04-26 08:41:04.000000 orpc-client-0.5.8/orpc/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      647 2023-04-27 23:43:47.000000 orpc-client-0.5.8/orpc/asio.py
+-rw-r--r--   0 test       (501) staff       (20)     2796 2023-04-28 03:17:54.000000 orpc-client-0.5.8/orpc/client.py
+-rw-r--r--   0 test       (501) staff       (20)      211 2023-04-28 02:50:13.000000 orpc-client-0.5.8/orpc/exceptions.py
+-rw-r--r--   0 test       (501) staff       (20)     6432 2023-04-27 14:48:23.000000 orpc-client-0.5.8/orpc/protocol.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-01 12:18:48.015197 orpc-client-0.5.8/orpc/tests/
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-04-26 08:38:38.000000 orpc-client-0.5.8/orpc/tests/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     5202 2023-04-26 08:59:05.000000 orpc-client-0.5.8/orpc/tests/test_protocol.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-05-01 12:18:48.015969 orpc-client-0.5.8/orpc_client.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)      707 2023-05-01 12:18:47.000000 orpc-client-0.5.8/orpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      395 2023-05-01 12:18:47.000000 orpc-client-0.5.8/orpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-05-01 12:18:47.000000 orpc-client-0.5.8/orpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-05-01 12:18:47.000000 orpc-client-0.5.8/orpc_client.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       49 2023-05-01 12:18:47.000000 orpc-client-0.5.8/orpc_client.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)        5 2023-05-01 12:18:47.000000 orpc-client-0.5.8/orpc_client.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       49 2023-05-01 12:16:31.000000 orpc-client-0.5.8/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-05-01 12:18:48.016322 orpc-client-0.5.8/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1458 2023-05-01 12:18:10.000000 orpc-client-0.5.8/setup.py
```

### Comparing `orpc-client-0.1.3/setup.py` & `orpc-client-0.5.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 
 import os
 from io import open
 from setuptools import setup
 from setuptools import find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with open(os.path.join(here, 'README.md'), "r", encoding="utf-8") as fobj:
+with open(os.path.join(here, "README.md"), "r", encoding="utf-8") as fobj:
     long_description = fobj.read()
 
 requires = []
-with open(os.path.join(here, 'requirements.txt'), "r", encoding="utf-8") as fobj:
+with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="orpc-client",
-    version="0.1.3",
+    version="0.5.8",
     description="Open RPC client.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
     ],
-    keywords=["orpc", "rpc", "orpc client"],
+    keywords=["orpc", "open rpc", "open rpc client", "open rpc protocol"],
     install_requires=requires,
     packages=find_packages("."),
-    py_modules=["orpc_client",],
     zip_safe=False,
     include_package_data=True,
-    entry_points={
-        "console_scripts": [
-        ]
-    },
 )
```

