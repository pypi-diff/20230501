# Comparing `tmp/zeroconf-0.58.2.tar.gz` & `tmp/zeroconf-0.59.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.58.2.tar", max compression
+gzip compressed data, was "zeroconf-0.59.0.tar", max compression
```

## Comparing `zeroconf-0.58.2.tar` & `zeroconf-0.59.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    49867 2023-04-26 05:56:37.776344 zeroconf-0.58.2/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-04-26 05:56:36.960330 zeroconf-0.58.2/COPYING
--rw-r--r--   0        0        0     4407 2023-04-26 05:56:36.960330 zeroconf-0.58.2/README.rst
--rw-r--r--   0        0        0     1060 2023-04-26 05:56:36.960330 zeroconf-0.58.2/build_ext.py
--rw-r--r--   0        0        0     6770 2023-04-26 05:56:36.960330 zeroconf-0.58.2/docs/Makefile
--rw-r--r--   0        0        0      234 2023-04-26 05:56:36.960330 zeroconf-0.58.2/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-04-26 05:56:36.960330 zeroconf-0.58.2/docs/conf.py
--rw-r--r--   0        0        0      991 2023-04-26 05:56:36.960330 zeroconf-0.58.2/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-04-26 05:56:37.852345 zeroconf-0.58.2/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-04-26 05:56:37.788344 zeroconf-0.58.2/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      511 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0     8493 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39043 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2061 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18218 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    25863 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2385 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    13655 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     1950 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17758 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22113 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    25364 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3964 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4469 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-04-26 05:56:36.964330 zeroconf-0.58.2/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-04-26 05:56:36.964330 zeroconf-0.58.2/tests/__init__.py
--rw-r--r--   0        0        0      668 2023-04-26 05:56:36.964330 zeroconf-0.58.2/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-04-26 05:56:36.964330 zeroconf-0.58.2/tests/services/__init__.py
--rw-r--r--   0        0        0    42950 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/services/test_browser.py
--rw-r--r--   0        0        0    45244 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/services/test_info.py
--rw-r--r--   0        0        0     4923 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/services/test_registry.py
--rw-r--r--   0        0        0     6273 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/services/test_types.py
--rw-r--r--   0        0        0    41883 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_cache.py
--rw-r--r--   0        0        0    29468 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_dns.py
--rw-r--r--   0        0        0     5022 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_exceptions.py
--rw-r--r--   0        0        0    63127 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_protocol.py
--rw-r--r--   0        0        0     9477 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-04-26 05:56:36.968330 zeroconf-0.58.2/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.58.2/setup.py
--rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 zeroconf-0.58.2/PKG-INFO
+-rw-r--r--   0        0        0    50156 2023-05-01 13:34:16.089610 zeroconf-0.59.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-05-01 13:34:15.241603 zeroconf-0.59.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-05-01 13:34:15.241603 zeroconf-0.59.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-05-01 13:34:15.245603 zeroconf-0.59.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-05-01 13:34:15.245603 zeroconf-0.59.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-05-01 13:34:15.245603 zeroconf-0.59.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-05-01 13:34:15.245603 zeroconf-0.59.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-05-01 13:34:15.245603 zeroconf-0.59.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-05-01 13:34:16.161610 zeroconf-0.59.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-05-01 13:34:16.097610 zeroconf-0.59.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      511 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0     8493 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39043 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2061 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18218 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    25863 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2412 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    13783 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     1950 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17758 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22113 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    25364 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3964 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-05-01 13:34:15.245603 zeroconf-0.59.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-05-01 13:34:15.249604 zeroconf-0.59.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4469 2023-05-01 13:34:15.249604 zeroconf-0.59.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-05-01 13:34:15.249604 zeroconf-0.59.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/__init__.py
+-rw-r--r--   0        0        0      668 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42950 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45244 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4923 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     6273 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    41883 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_cache.py
+-rw-r--r--   0        0        0    29468 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5022 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    63127 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     9477 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-05-01 13:34:15.249604 zeroconf-0.59.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.59.0/setup.py
+-rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 zeroconf-0.59.0/PKG-INFO
```

### Comparing `zeroconf-0.58.2/CHANGELOG.md` & `zeroconf-0.59.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.59.0 (2023-05-01)
+### Feature
+* Speed up decoding dns questions when processing incoming data ([#1168](https://github.com/python-zeroconf/python-zeroconf/issues/1168)) ([`f927190`](https://github.com/python-zeroconf/python-zeroconf/commit/f927190cb24f70fd7c825c6e12151fcc0daf3973))
+
 ## v0.58.2 (2023-04-26)
 ### Fix
 * Re-release to rebuild failed wheels ([#1165](https://github.com/python-zeroconf/python-zeroconf/issues/1165)) ([`4986271`](https://github.com/python-zeroconf/python-zeroconf/commit/498627166a4976f1d9d8cd1f3654b0d50272d266))
 
 ## v0.58.1 (2023-04-26)
 ### Fix
 * Reduce cast calls in service browser ([#1164](https://github.com/python-zeroconf/python-zeroconf/issues/1164)) ([`c0d65ae`](https://github.com/python-zeroconf/python-zeroconf/commit/c0d65aeae7037a18ed1149336f5e7bdb8b2dd8cf))
```

### Comparing `zeroconf-0.58.2/COPYING` & `zeroconf-0.59.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/README.rst` & `zeroconf-0.59.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/build_ext.py` & `zeroconf-0.59.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/docs/Makefile` & `zeroconf-0.59.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/docs/conf.py` & `zeroconf-0.59.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/docs/index.rst` & `zeroconf-0.59.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/pyproject.toml` & `zeroconf-0.59.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.58.2"
+version = "0.59.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.58.2/src/zeroconf/__init__.py` & `zeroconf-0.59.0/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.58.2'
+__version__ = '0.59.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.58.2/src/zeroconf/_cache.py` & `zeroconf-0.59.0/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_core.py` & `zeroconf-0.59.0/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_dns.pxd` & `zeroconf-0.59.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_dns.py` & `zeroconf-0.59.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_exceptions.py` & `zeroconf-0.59.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_handlers.py` & `zeroconf-0.59.0/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_history.py` & `zeroconf-0.59.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_logger.py` & `zeroconf-0.59.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.59.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.59.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files 13% similar despite different names*

```diff
@@ -34,29 +34,30 @@
 
 from .._dns cimport (
     DNSAddress,
     DNSEntry,
     DNSHinfo,
     DNSNsec,
     DNSPointer,
+    DNSQuestion,
     DNSRecord,
     DNSService,
     DNSText,
 )
 
 
 cdef class DNSIncoming:
 
     cdef bint _did_read_others
     cdef public unsigned int flags
-    cdef object offset
+    cdef cython.uint offset
     cdef public bytes data
     cdef unsigned int _data_len
     cdef public cython.dict name_cache
-    cdef public object questions
+    cdef public cython.list questions
     cdef object _answers
     cdef public object id
     cdef public cython.uint num_questions
     cdef public cython.uint num_answers
     cdef public cython.uint num_authorities
     cdef public cython.uint num_additionals
     cdef public object valid
```

### Comparing `zeroconf-0.58.2/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.59.0/src/zeroconf/_protocol/incoming.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,20 @@
             self.num_answers,
             self.num_authorities,
             self.num_additionals,
         ) = self._unpack(UNPACK_6H, 12)
 
     def _read_questions(self) -> None:
         """Reads questions section of packet"""
-        self.questions = [
-            DNSQuestion(self._read_name(), *self._unpack(UNPACK_HH, 4)) for _ in range(self.num_questions)
-        ]
+        for _ in range(self.num_questions):
+            name = self._read_name()
+            type_, class_ = UNPACK_HH(self.data, self.offset)
+            self.offset += 4
+            question = DNSQuestion(name, type_, class_)
+            self.questions.append(question)
 
     def _read_character_string(self) -> bytes:
         """Reads a character string from the packet"""
         length = self.data[self.offset]
         self.offset += 1
         return self._read_string(length)
```

### Comparing `zeroconf-0.58.2/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.59.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.59.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_services/__init__.py` & `zeroconf-0.59.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_services/browser.py` & `zeroconf-0.59.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_services/info.py` & `zeroconf-0.59.0/src/zeroconf/_services/info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_services/registry.py` & `zeroconf-0.59.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_services/types.py` & `zeroconf-0.59.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_updates.py` & `zeroconf-0.59.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_utils/__init__.py` & `zeroconf-0.59.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.59.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_utils/name.py` & `zeroconf-0.59.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_utils/net.py` & `zeroconf-0.59.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/_utils/time.py` & `zeroconf-0.59.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/asyncio.py` & `zeroconf-0.59.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/src/zeroconf/const.py` & `zeroconf-0.59.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/__init__.py` & `zeroconf-0.59.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/conftest.py` & `zeroconf-0.59.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/services/__init__.py` & `zeroconf-0.59.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/services/test_browser.py` & `zeroconf-0.59.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/services/test_info.py` & `zeroconf-0.59.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/services/test_registry.py` & `zeroconf-0.59.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/services/test_types.py` & `zeroconf-0.59.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_asyncio.py` & `zeroconf-0.59.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_cache.py` & `zeroconf-0.59.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_core.py` & `zeroconf-0.59.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_dns.py` & `zeroconf-0.59.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_exceptions.py` & `zeroconf-0.59.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_handlers.py` & `zeroconf-0.59.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_history.py` & `zeroconf-0.59.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_init.py` & `zeroconf-0.59.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_logger.py` & `zeroconf-0.59.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_protocol.py` & `zeroconf-0.59.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_services.py` & `zeroconf-0.59.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/test_updates.py` & `zeroconf-0.59.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/utils/__init__.py` & `zeroconf-0.59.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/utils/test_asyncio.py` & `zeroconf-0.59.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/utils/test_name.py` & `zeroconf-0.59.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/tests/utils/test_net.py` & `zeroconf-0.59.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.58.2/setup.py` & `zeroconf-0.59.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.58.2',
+    'version': '0.59.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.58.2/PKG-INFO` & `zeroconf-0.59.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.58.2
+Version: 0.59.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

