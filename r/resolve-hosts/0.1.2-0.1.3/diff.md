# Comparing `tmp/resolve-hosts-0.1.2.tar.gz` & `tmp/resolve-hosts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolve-hosts-0.1.2.tar", last modified: Fri Mar  3 03:34:53 2023, max compression
+gzip compressed data, was "resolve-hosts-0.1.3.tar", last modified: Mon May  1 00:19:18 2023, max compression
```

## Comparing `resolve-hosts-0.1.2.tar` & `resolve-hosts-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-03-03 03:34:53.665672 resolve-hosts-0.1.2/
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      731 2023-02-23 07:31:43.000000 resolve-hosts-0.1.2/LICENSE
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     2799 2023-03-03 03:34:53.665672 resolve-hosts-0.1.2/PKG-INFO
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     2473 2023-03-02 08:28:41.000000 resolve-hosts-0.1.2/README.md
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      588 2023-03-02 08:29:22.000000 resolve-hosts-0.1.2/pyproject.toml
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-03-03 03:34:53.665672 resolve-hosts-0.1.2/resolve_hosts.egg-info/
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     2799 2023-03-03 03:34:53.000000 resolve-hosts-0.1.2/resolve_hosts.egg-info/PKG-INFO
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      273 2023-03-03 03:34:53.000000 resolve-hosts-0.1.2/resolve_hosts.egg-info/SOURCES.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)        1 2023-03-03 03:34:53.000000 resolve-hosts-0.1.2/resolve_hosts.egg-info/dependency_links.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       81 2023-03-03 03:34:53.000000 resolve-hosts-0.1.2/resolve_hosts.egg-info/entry_points.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       25 2023-03-03 03:34:53.000000 resolve-hosts-0.1.2/resolve_hosts.egg-info/requires.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       14 2023-03-03 03:34:53.000000 resolve-hosts-0.1.2/resolve_hosts.egg-info/top_level.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     2942 2023-03-02 08:49:22.000000 resolve-hosts-0.1.2/resolve_hosts.py
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       38 2023-03-03 03:34:53.665672 resolve-hosts-0.1.2/setup.cfg
+drwxr-xr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-05-01 00:19:18.955117 resolve-hosts-0.1.3/
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)      731 2023-04-30 21:57:18.000000 resolve-hosts-0.1.3/LICENSE
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)     2799 2023-05-01 00:19:18.954117 resolve-hosts-0.1.3/PKG-INFO
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)     2473 2023-04-30 21:57:18.000000 resolve-hosts-0.1.3/README.md
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)      588 2023-05-01 00:17:08.000000 resolve-hosts-0.1.3/pyproject.toml
+drwxr-xr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-05-01 00:19:18.954117 resolve-hosts-0.1.3/resolve_hosts.egg-info/
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)     2799 2023-05-01 00:19:18.000000 resolve-hosts-0.1.3/resolve_hosts.egg-info/PKG-INFO
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)      291 2023-05-01 00:19:18.000000 resolve-hosts-0.1.3/resolve_hosts.egg-info/SOURCES.txt
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)        1 2023-05-01 00:19:18.000000 resolve-hosts-0.1.3/resolve_hosts.egg-info/dependency_links.txt
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)       81 2023-05-01 00:19:18.000000 resolve-hosts-0.1.3/resolve_hosts.egg-info/entry_points.txt
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)       25 2023-05-01 00:19:18.000000 resolve-hosts-0.1.3/resolve_hosts.egg-info/requires.txt
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)       14 2023-05-01 00:19:18.000000 resolve-hosts-0.1.3/resolve_hosts.egg-info/top_level.txt
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)     3303 2023-05-01 00:17:08.000000 resolve-hosts-0.1.3/resolve_hosts.py
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)       38 2023-05-01 00:19:18.955117 resolve-hosts-0.1.3/setup.cfg
+drwxr-xr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-05-01 00:19:18.954117 resolve-hosts-0.1.3/tests/
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)       92 2023-05-01 00:17:08.000000 resolve-hosts-0.1.3/tests/test_nop.py
```

### Comparing `resolve-hosts-0.1.2/LICENSE` & `resolve-hosts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resolve-hosts-0.1.2/PKG-INFO` & `resolve-hosts-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resolve-hosts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Resolve list of DNS hostnames.
 Author-email: Darren Spruell <dspruell@sancho2k.net>
 Project-URL: Homepage, https://github.com/dspruell/resolve-hosts
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `resolve-hosts-0.1.2/README.md` & `resolve-hosts-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `resolve-hosts-0.1.2/pyproject.toml` & `resolve-hosts-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resolve-hosts"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Darren Spruell", email="dspruell@sancho2k.net" },
 ]
 description = "Resolve list of DNS hostnames."
 readme = "README.md"
 dependencies = [
     "dnspython",
```

### Comparing `resolve-hosts-0.1.2/resolve_hosts.egg-info/PKG-INFO` & `resolve-hosts-0.1.3/resolve_hosts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resolve-hosts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Resolve list of DNS hostnames.
 Author-email: Darren Spruell <dspruell@sancho2k.net>
 Project-URL: Homepage, https://github.com/dspruell/resolve-hosts
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `resolve-hosts-0.1.2/resolve_hosts.py` & `resolve-hosts-0.1.3/resolve_hosts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,51 @@
-"Resolve list of DNS hostnames."
+"""Resolve list of DNS hostnames."""
 
 import argparse
+from importlib.metadata import version
 from ipaddress import ip_address
 import logging
 import sys
 
 from dns.resolver import Resolver, resolve, NXDOMAIN
 from tabulate import tabulate
 
 try:
     from ujson import dumps as json_dumps
 except ImportError:
     from json import dumps as json_dumps
 
 
+__application_name__ = "resolve-hosts"
+__version__ = version(__application_name__)
+
 logging.basicConfig(level=logging.INFO, format="[%(levelname)s] %(message)s")
 
 
 def resolve_servers(servers: list) -> list:
-    "Return IP addresses of input DNS servers, after resolving any hostnames."
+    """
+    Resolve specified resolvers.
 
+    Return IP addresses of input DNS servers, after resolving any
+    hostnames.
+    """
     results = []
     for s in servers:
         try:
             ip_address(s)
             results.append(s)
         except ValueError:
             r = resolve(s)
             for addr in r:
                 results.append(str(addr))
     return results
 
 
 def cli():
+    """Run main CLI."""
     description = "Resolve list of DNS hostnames."
     epilog = (
         "Additional resolvers may be specified by passing multiple "
         "--server options."
     )
     parser = argparse.ArgumentParser(description=description, epilog=epilog)
     parser.add_argument(
@@ -54,14 +63,21 @@
     )
     parser.add_argument(
         "-j", "--json", action="store_true", help="output JSON data"
     )
     parser.add_argument(
         "-d", "--debug", action="store_true", help="enable debug output"
     )
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version=__version__,
+        help="print package version",
+    )
     args = parser.parse_args()
 
     if args.debug:
         logging.getLogger().setLevel(logging.DEBUG)
 
     logging.debug(
         "configured to use resolver(s): %s",
```

