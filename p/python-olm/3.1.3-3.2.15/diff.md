# Comparing `tmp/python-olm-3.1.3.tar.gz` & `tmp/python-olm-3.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-olm-3.1.3.tar", last modified: Wed Jun 26 08:21:52 2019, max compression
+gzip compressed data, was "python-olm-3.2.15.tar", last modified: Mon May  1 16:48:26 2023, max compression
```

## Comparing `python-olm-3.1.3.tar` & `python-olm-3.2.15.tar`

### file list

```diff
@@ -1,53 +1,505 @@
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/
--rw-r--r--   0 poljar    (1000) poljar    (1000)      138 2018-11-24 12:32:58.000000 python-olm-3.1.3/.gitignore
--rw-r--r--   0 poljar    (1000) poljar    (1000)      115 2019-04-10 13:18:07.000000 python-olm-3.1.3/MANIFEST.in
--rw-r--r--   0 poljar    (1000) poljar    (1000)     2051 2019-06-26 08:21:07.000000 python-olm-3.1.3/Makefile
--rw-r--r--   0 poljar    (1000) poljar    (1000)      290 2019-06-26 08:21:52.000000 python-olm-3.1.3/PKG-INFO
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4686 2018-11-24 12:32:58.000000 python-olm-3.1.3/README.md
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/docs/
--rw-r--r--   0 poljar    (1000) poljar    (1000)      596 2018-10-02 22:08:38.000000 python-olm-3.1.3/docs/Makefile
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4935 2018-10-02 22:08:38.000000 python-olm-3.1.3/docs/conf.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)       65 2018-10-02 22:08:38.000000 python-olm-3.1.3/docs/index.html
--rw-r--r--   0 poljar    (1000) poljar    (1000)      338 2018-10-02 22:08:38.000000 python-olm-3.1.3/docs/index.rst
--rw-r--r--   0 poljar    (1000) poljar    (1000)      771 2018-11-24 12:32:58.000000 python-olm-3.1.3/docs/make.bat
--rw-r--r--   0 poljar    (1000) poljar    (1000)      544 2018-10-02 22:08:38.000000 python-olm-3.1.3/docs/olm.rst
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/dummy/
--rw-r--r--   0 poljar    (1000) poljar    (1000)       97 2018-11-24 12:32:42.000000 python-olm-3.1.3/dummy/README
--rw-r--r--   0 poljar    (1000) poljar    (1000)        0 2018-11-24 12:32:42.000000 python-olm-3.1.3/dummy/stddef.h
--rw-r--r--   0 poljar    (1000) poljar    (1000)        0 2018-11-24 12:32:42.000000 python-olm-3.1.3/dummy/stdint.h
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/include/
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/include/olm/
--rw-r--r--   0 poljar    (1000) poljar    (1000)    10899 2019-06-26 08:21:51.000000 python-olm-3.1.3/include/olm/olm.h
--rw-r--r--   0 poljar    (1000) poljar    (1000)     3776 2019-06-26 08:21:51.000000 python-olm-3.1.3/include/olm/pk.h
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1544 2019-06-26 08:21:51.000000 python-olm-3.1.3/include/olm/sas.h
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/olm/
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1441 2019-04-22 20:00:55.000000 python-olm-3.1.3/olm/__init__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)      352 2019-06-26 08:21:07.000000 python-olm-3.1.3/olm/__version__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     2343 2019-06-26 08:21:07.000000 python-olm-3.1.3/olm/_compat.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     2251 2018-10-02 22:08:38.000000 python-olm-3.1.3/olm/_finalize.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     9818 2019-03-29 13:43:02.000000 python-olm-3.1.3/olm/account.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    19067 2019-06-26 08:21:07.000000 python-olm-3.1.3/olm/group_session.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    14833 2019-06-26 08:21:07.000000 python-olm-3.1.3/olm/pk.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     7840 2019-06-26 08:21:07.000000 python-olm-3.1.3/olm/sas.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    18570 2019-06-26 08:21:07.000000 python-olm-3.1.3/olm/session.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4457 2019-06-26 08:21:07.000000 python-olm-3.1.3/olm/utility.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1955 2019-04-10 13:18:07.000000 python-olm-3.1.3/olm_build.py
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/python_olm.egg-info/
--rw-r--r--   0 poljar    (1000) poljar    (1000)      290 2019-06-26 08:21:51.000000 python-olm-3.1.3/python_olm.egg-info/PKG-INFO
--rw-r--r--   0 poljar    (1000) poljar    (1000)      784 2019-06-26 08:21:51.000000 python-olm-3.1.3/python_olm.egg-info/SOURCES.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)        1 2019-06-26 08:21:51.000000 python-olm-3.1.3/python_olm.egg-info/dependency_links.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)        1 2019-06-26 08:21:51.000000 python-olm-3.1.3/python_olm.egg-info/not-zip-safe
--rw-r--r--   0 poljar    (1000) poljar    (1000)       53 2019-06-26 08:21:51.000000 python-olm-3.1.3/python_olm.egg-info/requires.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)       12 2019-06-26 08:21:51.000000 python-olm-3.1.3/python_olm.egg-info/top_level.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)       19 2019-06-20 11:51:24.000000 python-olm-3.1.3/requirements.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)      162 2019-06-26 08:21:52.000000 python-olm-3.1.3/setup.cfg
--rw-r--r--   0 poljar    (1000) poljar    (1000)      736 2019-04-09 07:49:30.000000 python-olm-3.1.3/setup.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)       83 2019-06-20 11:59:56.000000 python-olm-3.1.3/test-requirements.txt
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2019-06-26 08:21:52.000000 python-olm-3.1.3/tests/
--rw-r--r--   0 poljar    (1000) poljar    (1000)     3373 2019-06-20 11:59:56.000000 python-olm-3.1.3/tests/account_test.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4343 2019-06-26 08:21:07.000000 python-olm-3.1.3/tests/group_session_test.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     2296 2019-06-26 08:21:07.000000 python-olm-3.1.3/tests/pk_test.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     3006 2019-04-10 13:18:07.000000 python-olm-3.1.3/tests/sas_test.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     5218 2019-06-26 08:21:07.000000 python-olm-3.1.3/tests/session_test.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)      716 2019-06-20 11:59:56.000000 python-olm-3.1.3/tests/utils_test.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)      920 2019-06-20 11:51:24.000000 python-olm-3.1.3/tox.ini
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.023883 python-olm-3.2.15/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      199 2023-05-01 16:47:20.000000 python-olm-3.2.15/MANIFEST.in
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      316 2023-05-01 16:48:26.023883 python-olm-3.2.15/PKG-INFO
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5027 2023-05-01 15:38:39.000000 python-olm-3.2.15/README.md
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.979884 python-olm-3.2.15/include/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.983884 python-olm-3.2.15/include/olm/
+-rw-r--r--   0 hubert    (1000) hubert    (1000)      974 2023-05-01 16:00:02.000000 python-olm-3.2.15/include/olm/error.h
+-rw-r--r--   0 hubert    (1000) hubert    (1000)    12652 2023-05-01 16:00:02.000000 python-olm-3.2.15/include/olm/olm.h
+-rw-r--r--   0 hubert    (1000) hubert    (1000)     4241 2023-05-01 16:00:02.000000 python-olm-3.2.15/include/olm/pk.h
+-rw-r--r--   0 hubert    (1000) hubert    (1000)     2007 2023-05-01 16:00:02.000000 python-olm-3.2.15/include/olm/sas.h
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.983884 python-olm-3.2.15/libolm/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4117 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    15630 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/Makefile
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.983884 python-olm-3.2.15/libolm/cmake/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      301 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/cmake/OlmConfig.cmake.in
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       35 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/common.mk
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.979884 python-olm-3.2.15/libolm/include/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.987884 python-olm-3.2.15/libolm/include/olm/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6609 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/account.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2213 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/base64.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2280 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/base64.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4439 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/cipher.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6006 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/crypto.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2920 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/error.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     7880 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/inbound_group_session.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3045 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/list.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2859 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/megolm.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1009 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/memory.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2527 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/memory.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2635 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/message.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3747 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/message.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    20043 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/olm.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      146 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/olm.hh
+-rw-r--r--   0 hubert    (1000) hubert    (1000)      822 2023-05-01 15:58:55.000000 python-olm-3.2.15/libolm/include/olm/olm_export.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6012 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/outbound_group_session.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3366 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/pickle.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3743 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/pickle.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2314 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/pickle_encoding.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    10463 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/pk.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6172 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/ratchet.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6039 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/sas.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6282 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/session.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1933 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/include/olm/utility.hh
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.987884 python-olm-3.2.15/libolm/lib/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.987884 python-olm-3.2.15/libolm/lib/crypto-algorithms/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1576 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/README.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    41647 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/aes.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     7589 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/aes.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     9660 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/aes_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1236 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/arcfour.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1237 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/arcfour.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1632 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/arcfour_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3936 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/base64.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1175 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/base64.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2458 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/base64_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    16451 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/blowfish.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1294 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/blowfish.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2633 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/blowfish_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    12621 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/des.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1484 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/des.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3374 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/des_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3142 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/md2.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1076 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/md2.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2115 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/md2_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5832 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/md5.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1186 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/md5.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2097 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/md5_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1265 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/rot-13.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      761 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/rot-13.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1381 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/rot-13_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3941 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/sha1.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1203 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/sha1.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2083 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/sha1_test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5283 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/sha256.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1215 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/sha256.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2408 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/crypto-algorithms/sha256_test.c
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.987884 python-olm-3.2.15/libolm/lib/curve25519-donna/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      209 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/.gitignore
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2091 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/LICENSE.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2294 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/Makefile
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1253 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/README
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.991884 python-olm-3.2.15/libolm/lib/curve25519-donna/contrib/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3173 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/contrib/Curve25519Donna.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1178 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/contrib/Curve25519Donna.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2599 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/contrib/Curve25519Donna.java
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2767 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/contrib/make-snippets
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    13539 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/curve25519-donna-c64.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    31699 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/curve25519-donna.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      618 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/curve25519-donna.podspec
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.983884 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.991884 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       89 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/__init__.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2961 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/curve25519module.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1522 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/keys.py
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.991884 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/test/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)        0 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/test/__init__.py
+-rwxrwxr-x   0 hubert    (1000) hubert    (1000)     3910 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/test/test_curve25519.py
+-rwxrwxr-x   0 hubert    (1000) hubert    (1000)     1242 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/python-src/curve25519/test/test_speed.py
+-rwxrwxr-x   0 hubert    (1000) hubert    (1000)     1483 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/setup.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      926 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/speed-curve25519.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1238 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/test-curve25519.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1167 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/test-noncanon.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1884 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/test-sc-curve25519.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       69 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna/test-sc-curve25519.s
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      377 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/curve25519-donna.h
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.991884 python-olm-3.2.15/libolm/lib/doctest/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2171 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.clang-format
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      172 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.editorconfig
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       12 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.gitattributes
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.991884 python-olm-3.2.15/libolm/lib/doctest/.github/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       72 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.github/FUNDING.yml
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      833 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.github/issue_template.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1046 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.github/pull_request_template.md
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.991884 python-olm-3.2.15/libolm/lib/doctest/.github/workflows/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2357 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    17153 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.github/workflows/main.yml
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      705 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.github/workflows/vsenv.bat
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      394 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.gitignore
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    19367 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/.travis.yml
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    58180 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/CHANGELOG.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6219 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2562 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/CONTRIBUTING.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1086 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/LICENSE.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    10622 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/README.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)        0 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/WORKSPACE
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3700 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/appveyor.yml
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.983884 python-olm-3.2.15/libolm/lib/doctest/doc/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     9788 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/assertions.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    12540 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/benchmarks.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3085 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/build-systems.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    11448 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/commandline.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    16090 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/configuration.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6817 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/extensions.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    14474 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/faq.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8316 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/features.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2630 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/logging.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3583 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/main.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     7230 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/parameterized-tests.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1750 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/readme.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4983 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/reporters.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    12444 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/roadmap.html
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      725 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/README.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8075 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/index.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2413 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/strapdown.css
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    46095 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/strapdown.js
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/themes/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    15961 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/themes/bootstrap-responsive.min.css
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    98164 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/themes/bootstrap.min.css
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   119189 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/themes/cyborg.min.css
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   109790 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/strapdown.js/themes/united.min.css
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5504 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/stringification.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8638 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/testcases.html
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    11630 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/html_generated/tutorial.html
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     9622 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/assertions.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    12369 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/benchmarks.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2918 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/build-systems.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    11270 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/commandline.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    15903 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/configuration.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6664 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/extensions.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    14268 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/faq.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8092 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/features.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2479 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/logging.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3427 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/main.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     7081 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/parameterized-tests.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1556 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/readme.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4821 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/reporters.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    12277 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/roadmap.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5353 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/stringification.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8480 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/testcases.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    11474 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doc/markdown/tutorial.md
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/doctest/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      729 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doctest/BUILD.bazel
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   305882 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doctest/doctest.h
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/doctest/extensions/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4138 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doctest/extensions/doctest_mpi.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      929 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doctest/extensions/doctest_util.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8149 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doctest/extensions/mpi_reporter.h
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/doctest/parts/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   165848 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doctest/parts/doctest.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   139686 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/doctest/parts/doctest_fwd.h
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.995884 python-olm-3.2.15/libolm/lib/doctest/examples/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.999884 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6688 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      378 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/alternative_macros.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6136 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/assertion_macros.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2806 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/asserts_used_outside_of_tests.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2237 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/concurrency.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3533 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/doctest_proxy.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2190 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/enums.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1500 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/header.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2475 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/logging.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1594 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/main.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      598 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace1.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      518 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace2.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      469 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace3.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      719 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace4.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      768 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace5.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      817 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace6.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      849 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace7.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      900 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace8.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      985 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/namespace9.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      338 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/no_failures.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3056 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/reporters_and_listeners.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4088 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/stringification.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4086 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/subcases.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2433 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/templated_test_cases.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2226 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_cases_and_suites.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.007883 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      731 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/abort_after.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      679 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/abort_after_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1220 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/abort_after_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2637 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/all_binary.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      255 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/all_binary_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5865 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/all_binary_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      257 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/alternative_macros.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      349 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/alternative_macros.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      949 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/alternative_macros.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     9276 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/assertion_macros.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    11307 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/assertion_macros.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    19166 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/assertion_macros.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      817 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/asserts_used_outside_of_tests.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      709 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/asserts_used_outside_of_tests.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      946 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/asserts_used_outside_of_tests.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      142 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/count.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       39 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/count_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      305 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/count_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2198 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/coverage_maxout.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2480 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/coverage_maxout.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3785 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/coverage_maxout.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       14 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/disabled.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       14 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/disabled_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       14 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/disabled_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      257 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/doctest_proxy.h.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      149 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/doctest_proxy.h_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      386 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/doctest_proxy.h_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2307 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/enums.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3239 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/enums.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4923 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/enums.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      257 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_1.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      149 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_1_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      386 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_1_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      268 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_2.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      149 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_2_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    12284 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_2_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1000 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_3.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      959 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_3_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2444 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/filter_3_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1030 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/first_last.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      738 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/first_last_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1249 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/first_last_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      730 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/header.h.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      462 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/header.h_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1424 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/header.h_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3798 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/help.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       39 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/help_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      262 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/help_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      233 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_reporters.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       39 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_reporters_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      469 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_reporters_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      411 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_test_cases.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       39 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_test_cases_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      854 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_test_cases_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      353 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_test_suites.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       39 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_test_suites_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      389 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/list_test_suites_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3060 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/logging.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2365 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/logging.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5096 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/logging.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      257 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/main.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      249 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/main.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      594 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/main.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3512 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/minimal.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1948 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/minimal_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      253 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/minimal_no_fail.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      492 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/minimal_no_fail_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1435 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/minimal_no_fail_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5659 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/minimal_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3791 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_1.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2062 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_1_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5924 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_1_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3552 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_2.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1948 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_2_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5659 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_2_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      257 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_3.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      149 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_3_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      386 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/order_3_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      257 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/reporters_and_listeners.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      149 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/reporters_and_listeners.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      386 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/reporters_and_listeners.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1620 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/stringification.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1906 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/stringification.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2744 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/stringification.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6059 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/subcases.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4682 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/subcases.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     9555 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/subcases.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1499 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/templated_test_cases.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2600 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/templated_test_cases.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4546 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/templated_test_cases.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3552 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/test_cases_and_suites.cpp.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1948 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/test_cases_and_suites.cpp_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5659 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/test_cases_and_suites.cpp_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       37 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/version.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       39 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/version_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      278 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/all_features/test_output/version_xml.txt
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.007883 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5085 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      148 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/default.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      796 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/foo.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      796 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/main.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      167 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/return42.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.007883 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/test_output/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1321 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/test_output/same_tests_multiple_configurations.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      605 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/test_output/same_tests_multiple_configurations_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2211 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/test_output/same_tests_multiple_configurations_xml.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      178 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/test_runner.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.007883 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1556 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6730 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      226 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/lib_1_src1.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      226 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/lib_1_src2.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      225 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/lib_2_src.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      130 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/main.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.007883 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/test_output/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      358 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/test_output/exe_with_static_libs.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      524 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/test_output/exe_with_static_libs_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1158 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/exe_with_static_libs/test_output/exe_with_static_libs_xml.txt
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1184 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      452 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/dll.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      329 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/implementation.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      332 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/implementation_2.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2089 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/main.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      734 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/plugin.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/test_output/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      985 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/test_output/executable_dll_and_plugin.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      940 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/test_output/executable_dll_and_plugin_junit.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2324 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/executable_dll_and_plugin/test_output/executable_dll_and_plugin_xml.txt
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.983884 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/dll/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      444 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/dll/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      541 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/dll/dll.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       86 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/dll/dll.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      318 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/dll/exporting.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      901 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/dll/main.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/executable/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      284 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/executable/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      970 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/installed_doctest_cmake/executable/main.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/examples/mpi/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      276 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/mpi/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      416 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/mpi/main.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1082 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/mpi/mpi.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1391 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/examples/range_based_execution.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      265 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/meson.build
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/scripts/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/scripts/bench/
+-rwxrwxr-x   0 hubert    (1000) hubert    (1000)     9007 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/bench/bench.py
+-rwxrwxr-x   0 hubert    (1000) hubert    (1000)     2138 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/bench/run_all.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1467 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/bench/tests.json
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/scripts/cmake/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      204 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/cmake/Config.cmake.in
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      979 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/cmake/assemble_single_header.cmake
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8964 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/cmake/common.cmake
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     7762 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/cmake/doctest.cmake
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3688 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/cmake/doctestAddTests.cmake
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2952 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/cmake/exec_test.cmake
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5776 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/coverage_maxout.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.011883 python-olm-3.2.15/libolm/lib/doctest/scripts/data/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    14823 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/article.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    12719 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/article2.txt
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.015883 python-olm-3.2.15/libolm/lib/doctest/scripts/data/benchmarks/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    87578 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/benchmarks/asserts.png
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    59660 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/benchmarks/header.png
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    54083 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/benchmarks/implement.png
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    54023 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/benchmarks/runtime_assert.png
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    53696 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/benchmarks/runtime_info.png
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    42312 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/cover.png
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    31396 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/cover_888px_wide.png
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   114301 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/initial_release_traffic.png
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.015883 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2050 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/icon_1.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3204 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/icon_2.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3355 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/icon_3.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1765 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/icon_4.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3012 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/icon_5.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2837 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/icon_6.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    18723 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/logo_1.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    23999 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/logo_2.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    18576 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/logo_3.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    22351 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/logo_4.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    18932 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/logo_5.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    27235 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/logo_6.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    20338 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/logo/logo_7.svg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   431258 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/using_doctest_888px_wide.gif
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)  1078012 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/data/youtube-cppcon-talk-thumbnail.png
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:25.983884 python-olm-3.2.15/libolm/lib/doctest/scripts/development_only/
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.015883 python-olm-3.2.15/libolm/lib/doctest/scripts/development_only/doctest/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      115 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/development_only/doctest/doctest.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1237 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/generate_html.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      322 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/hello_world.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.015883 python-olm-3.2.15/libolm/lib/doctest/scripts/how_stuff_works/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      257 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/how_stuff_works/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2078 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/how_stuff_works/how_captures_work.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1910 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/how_stuff_works/how_exception_translators_work.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2563 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/how_stuff_works/how_subcases_work.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1581 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/how_stuff_works/testing_crash_scenarios.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.015883 python-olm-3.2.15/libolm/lib/doctest/scripts/playground/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      364 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/playground/CMakeLists.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      944 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/playground/main.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      183 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/playground/test.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3313 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/random_dev_notes.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1082 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/release_process.md
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      298 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/update_changelog.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1721 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/update_stuff.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)        5 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/doctest/scripts/version.txt
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.015883 python-olm-3.2.15/libolm/lib/ed25519/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   127488 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/ed25519_32.dll
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   112128 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/ed25519_64.dll
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5786 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/readme.md
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.019883 python-olm-3.2.15/libolm/lib/ed25519/src/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1789 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/add_scalar.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1251 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/ed25519.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    38757 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/fe.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      980 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/fe.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2518 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/fixedint.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    10367 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/ge.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1683 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/ge.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1817 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/key_exchange.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      380 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/keypair.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    97787 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/precomp_data.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    22930 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/sc.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      266 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/sc.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      643 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/seed.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    11088 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/sha512.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      488 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/sha512.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      827 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/sign.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1367 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/src/verify.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4674 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/lib/ed25519/test.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      295 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/olm.pc.in
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.019883 python-olm-3.2.15/libolm/src/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    17860 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/account.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5777 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/base64.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4550 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/cipher.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     9242 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/crypto.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      838 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/ed25519.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1328 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/error.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    16084 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/inbound_group_session.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4666 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/megolm.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1268 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/memory.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    10871 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/message.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    22891 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/olm.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    10760 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/outbound_group_session.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6714 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/pickle.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3061 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/pickle_encoding.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    16138 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/pk.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    19065 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/ratchet.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6121 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/sas.c
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    16951 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/session.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1742 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/src/utility.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.019883 python-olm-3.2.15/libolm/tests/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      797 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/CMakeLists.txt
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.023883 python-olm-3.2.15/libolm/tests/include/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)   305882 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/include/doctest.h
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1162 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/include/testing.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1338 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/include/utils.hh
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2695 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_base64.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     7050 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_crypto.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    13852 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_group_session.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1864 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_list.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     5473 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_megolm.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     3228 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_message.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    26930 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_olm.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2713 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_olm_decrypt.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      489 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_olm_sha256.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2335 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_olm_signature.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     6680 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_olm_using_malloc.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8229 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_pk.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     7308 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_ratchet.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4076 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_sas.cpp
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4177 2023-05-01 15:38:39.000000 python-olm-3.2.15/libolm/tests/test_session.cpp
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.023883 python-olm-3.2.15/olm/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     1441 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/__init__.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      422 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/__version__.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2343 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/_compat.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2213 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/_finalize.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    11873 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/account.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    18946 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/group_session.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    14583 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/pk.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)        0 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/py.typed
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     8454 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/sas.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    19187 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/session.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     4399 2023-05-01 15:38:39.000000 python-olm-3.2.15/olm/utility.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)     2760 2023-05-01 16:47:20.000000 python-olm-3.2.15/olm_build.py
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      432 2023-05-01 15:38:39.000000 python-olm-3.2.15/pyproject.toml
+drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2023-05-01 16:48:26.023883 python-olm-3.2.15/python_olm.egg-info/
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      316 2023-05-01 16:48:25.000000 python-olm-3.2.15/python_olm.egg-info/PKG-INFO
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)    23099 2023-05-01 16:48:25.000000 python-olm-3.2.15/python_olm.egg-info/SOURCES.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)        1 2023-05-01 16:48:25.000000 python-olm-3.2.15/python_olm.egg-info/dependency_links.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)        1 2023-05-01 16:48:25.000000 python-olm-3.2.15/python_olm.egg-info/not-zip-safe
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       46 2023-05-01 16:48:25.000000 python-olm-3.2.15/python_olm.egg-info/requires.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)       12 2023-05-01 16:48:25.000000 python-olm-3.2.15/python_olm.egg-info/top_level.txt
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      162 2023-05-01 16:48:26.023883 python-olm-3.2.15/setup.cfg
+-rw-rw-r--   0 hubert    (1000) hubert    (1000)      772 2023-05-01 15:38:39.000000 python-olm-3.2.15/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-olm-3.1.3/README.md` & `python-olm-3.2.15/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,26 @@
 
 An example of the implementation of the Olm and Megolm cryptographic protocol
 can be found in the Matrix protocol for which the implementation guide can be
 found [here][6].
 
 The full API reference can be found [here][7].
 
+# Installation instructions
+
+To install from the source package, you will need:
+
+- cmake (recommended) or GNU make
+- a C/C++ compiler
+
+You can then run `pip install python-olm`.
+
+This should work in UNIX-like environments, including macOS, and may work in
+other environments too, but is known to not work yet in Windows.
+
 # Accounts
 
 Accounts create and hold the central identity of the Olm protocol, they consist of a fingerprint and identity
 key pair. They also produce one time keys that are used to start peer to peer
 encrypted communication channels.
 
 ## Account Creation
@@ -153,9 +165,9 @@
 >>> restored = InboundGroupSession.from_pickle(pickle)
 ```
 [1]: https://git.matrix.org/git/olm/about/
 [2]: https://git.matrix.org/git/olm/tree/python?id=f8c61b8f8432d0b0b38d57f513c5048fb42f22ab
 [3]: https://cffi.readthedocs.io/en/latest/
 [4]: https://git.matrix.org/git/olm/about/docs/olm.rst
 [5]: https://git.matrix.org/git/olm/about/docs/megolm.rst
-[6]: https://matrix.org/docs/guides/e2e_implementation.html
+[6]: https://matrix.org/docs/guides/end-to-end-encryption-implementation-guide
 [7]: https://poljar.github.io/python-olm/html/index.html
```

### Comparing `python-olm-3.1.3/include/olm/olm.h` & `python-olm-3.2.15/include/olm/olm.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,107 @@
 # 1 "../include/olm/olm.h"
 # 1 "<built-in>"
 # 1 "<command-line>"
-# 31 "<command-line>"
 # 1 "/usr/include/stdc-predef.h" 1 3 4
-# 32 "<command-line>" 2
+# 1 "<command-line>" 2
 # 1 "../include/olm/olm.h"
 # 19 "../include/olm/olm.h"
 # 1 "dummy/stddef.h" 1
 # 20 "../include/olm/olm.h" 2
 # 1 "dummy/stdint.h" 1
 # 21 "../include/olm/olm.h" 2
 
+# 1 "dummy/olm/error.h" 1
+# 23 "../include/olm/olm.h" 2
 # 1 "../include/olm/inbound_group_session.h" 1
 # 18 "../include/olm/inbound_group_session.h"
 # 1 "dummy/stddef.h" 1
 # 19 "../include/olm/inbound_group_session.h" 2
 # 1 "dummy/stdint.h" 1
 # 20 "../include/olm/inbound_group_session.h" 2
 
+# 1 "dummy/olm/error.h" 1
+# 22 "../include/olm/inbound_group_session.h" 2
+
+# 1 "../include/olm/olm_export.h" 1
+# 24 "../include/olm/inbound_group_session.h" 2
+
 
 
 
 
 typedef struct OlmInboundGroupSession OlmInboundGroupSession;
 
 
-size_t olm_inbound_group_session_size(void);
+ size_t olm_inbound_group_session_size(void);
 
 
 
 
 
 
-OlmInboundGroupSession * olm_inbound_group_session(
+ OlmInboundGroupSession * olm_inbound_group_session(
     void *memory
 );
 
 
 
 
-const char *olm_inbound_group_session_last_error(
+ const char *olm_inbound_group_session_last_error(
+    const OlmInboundGroupSession *session
+);
+
+
+
+
+ enum OlmErrorCode olm_inbound_group_session_last_error_code(
     const OlmInboundGroupSession *session
 );
 
 
-size_t olm_clear_inbound_group_session(
+ size_t olm_clear_inbound_group_session(
     OlmInboundGroupSession *session
 );
 
 
-size_t olm_pickle_inbound_group_session_length(
+ size_t olm_pickle_inbound_group_session_length(
     const OlmInboundGroupSession *session
 );
-# 64 "../include/olm/inbound_group_session.h"
-size_t olm_pickle_inbound_group_session(
+# 75 "../include/olm/inbound_group_session.h"
+ size_t olm_pickle_inbound_group_session(
     OlmInboundGroupSession *session,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
-# 80 "../include/olm/inbound_group_session.h"
-size_t olm_unpickle_inbound_group_session(
+# 91 "../include/olm/inbound_group_session.h"
+ size_t olm_unpickle_inbound_group_session(
     OlmInboundGroupSession *session,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
-# 97 "../include/olm/inbound_group_session.h"
-size_t olm_init_inbound_group_session(
+# 108 "../include/olm/inbound_group_session.h"
+ size_t olm_init_inbound_group_session(
     OlmInboundGroupSession *session,
 
     uint8_t const * session_key, size_t session_key_length
 );
-# 112 "../include/olm/inbound_group_session.h"
-size_t olm_import_inbound_group_session(
+# 123 "../include/olm/inbound_group_session.h"
+ size_t olm_import_inbound_group_session(
     OlmInboundGroupSession *session,
 
 
     uint8_t const * session_key, size_t session_key_length
 );
-# 129 "../include/olm/inbound_group_session.h"
-size_t olm_group_decrypt_max_plaintext_length(
+# 140 "../include/olm/inbound_group_session.h"
+ size_t olm_group_decrypt_max_plaintext_length(
     OlmInboundGroupSession *session,
     uint8_t * message, size_t message_length
 );
-# 153 "../include/olm/inbound_group_session.h"
-size_t olm_group_decrypt(
+# 164 "../include/olm/inbound_group_session.h"
+ size_t olm_group_decrypt(
     OlmInboundGroupSession *session,
 
 
 
     uint8_t * message, size_t message_length,
 
 
@@ -95,171 +109,185 @@
     uint32_t * message_index
 );
 
 
 
 
 
-size_t olm_inbound_group_session_id_length(
+ size_t olm_inbound_group_session_id_length(
     const OlmInboundGroupSession *session
 );
-# 181 "../include/olm/inbound_group_session.h"
-size_t olm_inbound_group_session_id(
+# 192 "../include/olm/inbound_group_session.h"
+ size_t olm_inbound_group_session_id(
     OlmInboundGroupSession *session,
     uint8_t * id, size_t id_length
 );
 
 
 
 
-uint32_t olm_inbound_group_session_first_known_index(
+ uint32_t olm_inbound_group_session_first_known_index(
     const OlmInboundGroupSession *session
 );
-# 202 "../include/olm/inbound_group_session.h"
-int olm_inbound_group_session_is_verified(
+# 213 "../include/olm/inbound_group_session.h"
+ int olm_inbound_group_session_is_verified(
     const OlmInboundGroupSession *session
 );
 
 
 
 
-size_t olm_export_inbound_group_session_length(
+ size_t olm_export_inbound_group_session_length(
     const OlmInboundGroupSession *session
 );
-# 225 "../include/olm/inbound_group_session.h"
-size_t olm_export_inbound_group_session(
+# 236 "../include/olm/inbound_group_session.h"
+ size_t olm_export_inbound_group_session(
     OlmInboundGroupSession *session,
     uint8_t * key, size_t key_length, uint32_t message_index
 );
-# 23 "../include/olm/olm.h" 2
+# 24 "../include/olm/olm.h" 2
 # 1 "../include/olm/outbound_group_session.h" 1
 # 18 "../include/olm/outbound_group_session.h"
 # 1 "dummy/stddef.h" 1
 # 19 "../include/olm/outbound_group_session.h" 2
 # 1 "dummy/stdint.h" 1
 # 20 "../include/olm/outbound_group_session.h" 2
 
+# 1 "dummy/olm/error.h" 1
+# 22 "../include/olm/outbound_group_session.h" 2
+
+
+
 
 
 
 
 typedef struct OlmOutboundGroupSession OlmOutboundGroupSession;
 
 
-size_t olm_outbound_group_session_size(void);
+ size_t olm_outbound_group_session_size(void);
 
 
 
 
 
 
-OlmOutboundGroupSession * olm_outbound_group_session(
+ OlmOutboundGroupSession * olm_outbound_group_session(
     void *memory
 );
 
 
 
 
-const char *olm_outbound_group_session_last_error(
+ const char *olm_outbound_group_session_last_error(
     const OlmOutboundGroupSession *session
 );
 
 
-size_t olm_clear_outbound_group_session(
+
+
+ enum OlmErrorCode olm_outbound_group_session_last_error_code(
+    const OlmOutboundGroupSession *session
+);
+
+
+ size_t olm_clear_outbound_group_session(
     OlmOutboundGroupSession *session
 );
 
 
-size_t olm_pickle_outbound_group_session_length(
+ size_t olm_pickle_outbound_group_session_length(
     const OlmOutboundGroupSession *session
 );
-# 64 "../include/olm/outbound_group_session.h"
-size_t olm_pickle_outbound_group_session(
+# 75 "../include/olm/outbound_group_session.h"
+ size_t olm_pickle_outbound_group_session(
     OlmOutboundGroupSession *session,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
-# 80 "../include/olm/outbound_group_session.h"
-size_t olm_unpickle_outbound_group_session(
+# 91 "../include/olm/outbound_group_session.h"
+ size_t olm_unpickle_outbound_group_session(
     OlmOutboundGroupSession *session,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
 
 
 
-size_t olm_init_outbound_group_session_random_length(
+ size_t olm_init_outbound_group_session_random_length(
     const OlmOutboundGroupSession *session
 );
 
 
 
 
 
 
-size_t olm_init_outbound_group_session(
+ size_t olm_init_outbound_group_session(
     OlmOutboundGroupSession *session,
     uint8_t *random, size_t random_length
 );
 
 
 
 
-size_t olm_group_encrypt_message_length(
+ size_t olm_group_encrypt_message_length(
     OlmOutboundGroupSession *session,
     size_t plaintext_length
 );
 
 
 
 
 
 
 
-size_t olm_group_encrypt(
+ size_t olm_group_encrypt(
     OlmOutboundGroupSession *session,
     uint8_t const * plaintext, size_t plaintext_length,
     uint8_t * message, size_t message_length
 );
 
 
 
 
 
-size_t olm_outbound_group_session_id_length(
+ size_t olm_outbound_group_session_id_length(
     const OlmOutboundGroupSession *session
 );
-# 138 "../include/olm/outbound_group_session.h"
-size_t olm_outbound_group_session_id(
+# 149 "../include/olm/outbound_group_session.h"
+ size_t olm_outbound_group_session_id(
     OlmOutboundGroupSession *session,
     uint8_t * id, size_t id_length
 );
 
 
 
 
 
 
 
-uint32_t olm_outbound_group_session_message_index(
+ uint32_t olm_outbound_group_session_message_index(
     OlmOutboundGroupSession *session
 );
 
 
 
 
-size_t olm_outbound_group_session_key_length(
+ size_t olm_outbound_group_session_key_length(
     const OlmOutboundGroupSession *session
 );
-# 170 "../include/olm/outbound_group_session.h"
-size_t olm_outbound_group_session_key(
+# 181 "../include/olm/outbound_group_session.h"
+ size_t olm_outbound_group_session_key(
     OlmOutboundGroupSession *session,
     uint8_t * key, size_t key_length
 );
-# 24 "../include/olm/olm.h" 2
+# 25 "../include/olm/olm.h" 2
+
+
 
 
 
 
 
 static const size_t OLM_MESSAGE_TYPE_PRE_KEY = 0;
 static const size_t OLM_MESSAGE_TYPE_MESSAGE = 1;
@@ -267,344 +295,411 @@
 typedef struct OlmAccount OlmAccount;
 typedef struct OlmSession OlmSession;
 typedef struct OlmUtility OlmUtility;
 
 
 
 
-void olm_get_library_version(uint8_t *major, uint8_t *minor, uint8_t *patch);
+ void olm_get_library_version(uint8_t *major, uint8_t *minor, uint8_t *patch);
 
 
-size_t olm_account_size(void);
+ size_t olm_account_size(void);
 
 
-size_t olm_session_size(void);
+ size_t olm_session_size(void);
 
 
-size_t olm_utility_size(void);
+ size_t olm_utility_size(void);
 
 
 
-OlmAccount * olm_account(
+ OlmAccount * olm_account(
     void * memory
 );
 
 
 
-OlmSession * olm_session(
+ OlmSession * olm_session(
     void * memory
 );
 
 
 
-OlmUtility * olm_utility(
+ OlmUtility * olm_utility(
     void * memory
 );
 
 
-size_t olm_error(void);
+ size_t olm_error(void);
 
 
 
-const char * olm_account_last_error(
-    OlmAccount * account
+ const char * olm_account_last_error(
+    OlmAccount const * account
 );
 
 
+ enum OlmErrorCode olm_account_last_error_code(
+    OlmAccount const * account
+);
 
-const char * olm_session_last_error(
-    OlmSession * session
+
+
+ const char * olm_session_last_error(
+    OlmSession const * session
+);
+
+
+ enum OlmErrorCode olm_session_last_error_code(
+    OlmSession const * session
 );
 
 
 
-const char * olm_utility_last_error(
-    OlmUtility * utility
+ const char * olm_utility_last_error(
+    OlmUtility const * utility
+);
+
+
+ enum OlmErrorCode olm_utility_last_error_code(
+    OlmUtility const * utility
 );
 
 
-size_t olm_clear_account(
+ size_t olm_clear_account(
     OlmAccount * account
 );
 
 
-size_t olm_clear_session(
+ size_t olm_clear_session(
     OlmSession * session
 );
 
 
-size_t olm_clear_utility(
+ size_t olm_clear_utility(
     OlmUtility * utility
 );
 
 
-size_t olm_pickle_account_length(
-    OlmAccount * account
+ size_t olm_pickle_account_length(
+    OlmAccount const * account
 );
 
 
-size_t olm_pickle_session_length(
-    OlmSession * session
+ size_t olm_pickle_session_length(
+    OlmSession const * session
 );
 
 
 
 
 
 
-size_t olm_pickle_account(
+ size_t olm_pickle_account(
     OlmAccount * account,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
 
 
 
 
 
 
-size_t olm_pickle_session(
+ size_t olm_pickle_session(
     OlmSession * session,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
 
 
 
 
 
 
 
-size_t olm_unpickle_account(
+ size_t olm_unpickle_account(
     OlmAccount * account,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
 
 
 
 
 
 
 
-size_t olm_unpickle_session(
+ size_t olm_unpickle_session(
     OlmSession * session,
     void const * key, size_t key_length,
     void * pickled, size_t pickled_length
 );
 
 
-size_t olm_create_account_random_length(
-    OlmAccount * account
+ size_t olm_create_account_random_length(
+    OlmAccount const * account
 );
 
 
 
 
-size_t olm_create_account(
+ size_t olm_create_account(
     OlmAccount * account,
     void * random, size_t random_length
 );
 
 
-size_t olm_account_identity_keys_length(
-    OlmAccount * account
+ size_t olm_account_identity_keys_length(
+    OlmAccount const * account
 );
 
 
 
 
 
-size_t olm_account_identity_keys(
+ size_t olm_account_identity_keys(
     OlmAccount * account,
     void * identity_keys, size_t identity_key_length
 );
 
 
 
-size_t olm_account_signature_length(
-    OlmAccount * account
+ size_t olm_account_signature_length(
+    OlmAccount const * account
 );
 
 
 
 
-size_t olm_account_sign(
+ size_t olm_account_sign(
     OlmAccount * account,
     void const * message, size_t message_length,
     void * signature, size_t signature_length
 );
 
 
-size_t olm_account_one_time_keys_length(
-    OlmAccount * account
+ size_t olm_account_one_time_keys_length(
+    OlmAccount const * account
 );
-# 225 "../include/olm/olm.h"
-size_t olm_account_one_time_keys(
+# 243 "../include/olm/olm.h"
+ size_t olm_account_one_time_keys(
     OlmAccount * account,
     void * one_time_keys, size_t one_time_keys_length
 );
-
-
-size_t olm_account_mark_keys_as_published(
+# 255 "../include/olm/olm.h"
+ size_t olm_account_mark_keys_as_published(
     OlmAccount * account
 );
 
 
-size_t olm_account_max_number_of_one_time_keys(
-    OlmAccount * account
+ size_t olm_account_max_number_of_one_time_keys(
+    OlmAccount const * account
 );
 
 
 
-size_t olm_account_generate_one_time_keys_random_length(
-    OlmAccount * account,
+ size_t olm_account_generate_one_time_keys_random_length(
+    OlmAccount const * account,
     size_t number_of_keys
 );
 
 
 
 
 
-size_t olm_account_generate_one_time_keys(
+ size_t olm_account_generate_one_time_keys(
     OlmAccount * account,
     size_t number_of_keys,
     void * random, size_t random_length
 );
 
 
-size_t olm_create_outbound_session_random_length(
-    OlmSession * session
+ size_t olm_account_generate_fallback_key_random_length(
+    OlmAccount const * account
 );
 
 
 
 
+ size_t olm_account_generate_fallback_key(
+    OlmAccount * account,
+    void * random, size_t random_length
+);
 
 
-size_t olm_create_outbound_session(
-    OlmSession * session,
+
+ size_t olm_account_fallback_key_length(
+    OlmAccount const * account
+);
+
+
+ size_t olm_account_fallback_key(
     OlmAccount * account,
+    void * fallback_key, size_t fallback_key_size
+);
+
+
+
+ size_t olm_account_unpublished_fallback_key_length(
+    OlmAccount const * account
+);
+
+
+
+ size_t olm_account_unpublished_fallback_key(
+    OlmAccount * account,
+    void * fallback_key, size_t fallback_key_size
+);
+
+
+
+
+
+
+ void olm_account_forget_old_fallback_key(
+    OlmAccount * account
+);
+
+
+
+ size_t olm_create_outbound_session_random_length(
+    OlmSession const * session
+);
+
+
+
+
+
+
+ size_t olm_create_outbound_session(
+    OlmSession * session,
+    OlmAccount const * account,
     void const * their_identity_key, size_t their_identity_key_length,
     void const * their_one_time_key, size_t their_one_time_key_length,
     void * random, size_t random_length
 );
-# 283 "../include/olm/olm.h"
-size_t olm_create_inbound_session(
+# 355 "../include/olm/olm.h"
+ size_t olm_create_inbound_session(
     OlmSession * session,
     OlmAccount * account,
     void * one_time_key_message, size_t message_length
 );
-# 297 "../include/olm/olm.h"
-size_t olm_create_inbound_session_from(
+
+
+
+
+ size_t olm_create_inbound_session_from(
     OlmSession * session,
     OlmAccount * account,
     void const * their_identity_key, size_t their_identity_key_length,
     void * one_time_key_message, size_t message_length
 );
 
 
-size_t olm_session_id_length(
-    OlmSession * session
+ size_t olm_session_id_length(
+    OlmSession const * session
 );
 
 
 
 
-size_t olm_session_id(
+ size_t olm_session_id(
     OlmSession * session,
     void * id, size_t id_length
 );
 
-int olm_session_has_received_message(
-    OlmSession *session
+ int olm_session_has_received_message(
+    OlmSession const *session
 );
-# 330 "../include/olm/olm.h"
-size_t olm_matches_inbound_session(
+# 395 "../include/olm/olm.h"
+ void olm_session_describe(OlmSession * session, char *buf, size_t buflen);
+# 406 "../include/olm/olm.h"
+ size_t olm_matches_inbound_session(
     OlmSession * session,
     void * one_time_key_message, size_t message_length
 );
-# 344 "../include/olm/olm.h"
-size_t olm_matches_inbound_session_from(
+# 420 "../include/olm/olm.h"
+ size_t olm_matches_inbound_session_from(
     OlmSession * session,
     void const * their_identity_key, size_t their_identity_key_length,
     void * one_time_key_message, size_t message_length
 );
 
 
 
 
-size_t olm_remove_one_time_keys(
+ size_t olm_remove_one_time_keys(
     OlmAccount * account,
     OlmSession * session
 );
 
 
 
 
 
-size_t olm_encrypt_message_type(
-    OlmSession * session
+ size_t olm_encrypt_message_type(
+    OlmSession const * session
 );
 
 
-size_t olm_encrypt_random_length(
-    OlmSession * session
+ size_t olm_encrypt_random_length(
+    OlmSession const * session
 );
 
 
 
-size_t olm_encrypt_message_length(
-    OlmSession * session,
+ size_t olm_encrypt_message_length(
+    OlmSession const * session,
     size_t plaintext_length
 );
 
 
 
 
 
 
 
-size_t olm_encrypt(
+ size_t olm_encrypt(
     OlmSession * session,
     void const * plaintext, size_t plaintext_length,
     void * random, size_t random_length,
     void * message, size_t message_length
 );
-# 399 "../include/olm/olm.h"
-size_t olm_decrypt_max_plaintext_length(
+# 475 "../include/olm/olm.h"
+ size_t olm_decrypt_max_plaintext_length(
     OlmSession * session,
     size_t message_type,
     void * message, size_t message_length
 );
-# 416 "../include/olm/olm.h"
-size_t olm_decrypt(
+# 492 "../include/olm/olm.h"
+ size_t olm_decrypt(
     OlmSession * session,
     size_t message_type,
     void * message, size_t message_length,
     void * plaintext, size_t max_plaintext_length
 );
 
 
-size_t olm_sha256_length(
-   OlmUtility * utility
+ size_t olm_sha256_length(
+   OlmUtility const * utility
 );
 
 
 
 
-size_t olm_sha256(
+ size_t olm_sha256(
     OlmUtility * utility,
     void const * input, size_t input_length,
     void * output, size_t output_length
 );
 
 
 
 
-size_t olm_ed25519_verify(
+ size_t olm_ed25519_verify(
     OlmUtility * utility,
     void const * key, size_t key_length,
     void const * message, size_t message_length,
     void * signature, size_t signature_length
 );
 void *memset(void *s, int c, size_t n);
```

### Comparing `python-olm-3.1.3/include/olm/pk.h` & `python-olm-3.2.15/include/olm/pk.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,219 +1,242 @@
 # 1 "../include/olm/pk.h"
 # 1 "<built-in>"
 # 1 "<command-line>"
-# 31 "<command-line>"
 # 1 "/usr/include/stdc-predef.h" 1 3 4
-# 32 "<command-line>" 2
+# 1 "<command-line>" 2
 # 1 "../include/olm/pk.h"
 # 19 "../include/olm/pk.h"
 # 1 "dummy/stddef.h" 1
 # 20 "../include/olm/pk.h" 2
 # 1 "dummy/stdint.h" 1
 # 21 "../include/olm/pk.h" 2
 
+# 1 "dummy/olm/error.h" 1
+# 23 "../include/olm/pk.h" 2
+
+# 1 "../include/olm/olm_export.h" 1
+# 25 "../include/olm/pk.h" 2
+
 
 
 
 
 typedef struct OlmPkEncryption OlmPkEncryption;
 
 
-size_t olm_pk_encryption_size(void);
+ size_t olm_pk_encryption_size(void);
 
 
 
-OlmPkEncryption *olm_pk_encryption(
+ OlmPkEncryption *olm_pk_encryption(
     void * memory
 );
 
 
 
-const char * olm_pk_encryption_last_error(
-    OlmPkEncryption * encryption
+ const char * olm_pk_encryption_last_error(
+    const OlmPkEncryption * encryption
 );
 
 
-size_t olm_clear_pk_encryption(
+
+ enum OlmErrorCode olm_pk_encryption_last_error_code(
+    const OlmPkEncryption * encryption
+);
+
+
+ size_t olm_clear_pk_encryption(
     OlmPkEncryption *encryption
 );
 
 
-size_t olm_pk_encryption_set_recipient_key(
+ size_t olm_pk_encryption_set_recipient_key(
     OlmPkEncryption *encryption,
     void const *public_key, size_t public_key_length
 );
 
 
 
-size_t olm_pk_ciphertext_length(
-    OlmPkEncryption *encryption,
+ size_t olm_pk_ciphertext_length(
+    const OlmPkEncryption *encryption,
     size_t plaintext_length
 );
 
 
-size_t olm_pk_mac_length(
-    OlmPkEncryption *encryption
+ size_t olm_pk_mac_length(
+    const OlmPkEncryption *encryption
 );
 
 
-size_t olm_pk_key_length(void);
+ size_t olm_pk_key_length(void);
 
 
-size_t olm_pk_encrypt_random_length(
-    OlmPkEncryption *encryption
+ size_t olm_pk_encrypt_random_length(
+    const OlmPkEncryption *encryption
 );
-# 84 "../include/olm/pk.h"
-size_t olm_pk_encrypt(
+# 94 "../include/olm/pk.h"
+ size_t olm_pk_encrypt(
     OlmPkEncryption *encryption,
     void const * plaintext, size_t plaintext_length,
     void * ciphertext, size_t ciphertext_length,
     void * mac, size_t mac_length,
     void * ephemeral_key, size_t ephemeral_key_size,
     const void * random, size_t random_length
 );
 
 typedef struct OlmPkDecryption OlmPkDecryption;
 
 
-size_t olm_pk_decryption_size(void);
+ size_t olm_pk_decryption_size(void);
 
 
 
-OlmPkDecryption *olm_pk_decryption(
+ OlmPkDecryption *olm_pk_decryption(
     void * memory
 );
 
 
 
-const char * olm_pk_decryption_last_error(
-    OlmPkDecryption * decryption
+ const char * olm_pk_decryption_last_error(
+    const OlmPkDecryption * decryption
 );
 
 
-size_t olm_clear_pk_decryption(
+
+ enum OlmErrorCode olm_pk_decryption_last_error_code(
+    const OlmPkDecryption * decryption
+);
+
+
+ size_t olm_clear_pk_decryption(
     OlmPkDecryption *decryption
 );
 
 
 
-size_t olm_pk_private_key_length(void);
+ size_t olm_pk_private_key_length(void);
 
 
 
-size_t olm_pk_generate_key_random_length(void);
-# 133 "../include/olm/pk.h"
-size_t olm_pk_key_from_private(
+ size_t olm_pk_generate_key_random_length(void);
+# 149 "../include/olm/pk.h"
+ size_t olm_pk_key_from_private(
     OlmPkDecryption * decryption,
     void * pubkey, size_t pubkey_length,
     const void * privkey, size_t privkey_length
 );
 
 
 
-size_t olm_pk_generate_key(
+ size_t olm_pk_generate_key(
     OlmPkDecryption * decryption,
     void * pubkey, size_t pubkey_length,
     const void * privkey, size_t privkey_length
 );
 
 
-size_t olm_pickle_pk_decryption_length(
-    OlmPkDecryption * decryption
+ size_t olm_pickle_pk_decryption_length(
+    const OlmPkDecryption * decryption
 );
 
 
 
 
 
 
-size_t olm_pickle_pk_decryption(
+ size_t olm_pickle_pk_decryption(
     OlmPkDecryption * decryption,
     void const * key, size_t key_length,
     void *pickled, size_t pickled_length
 );
-# 170 "../include/olm/pk.h"
-size_t olm_unpickle_pk_decryption(
+# 186 "../include/olm/pk.h"
+ size_t olm_unpickle_pk_decryption(
     OlmPkDecryption * decryption,
     void const * key, size_t key_length,
     void *pickled, size_t pickled_length,
     void *pubkey, size_t pubkey_length
 );
 
 
 
-size_t olm_pk_max_plaintext_length(
-    OlmPkDecryption * decryption,
+ size_t olm_pk_max_plaintext_length(
+    const OlmPkDecryption * decryption,
     size_t ciphertext_length
 );
 
 
 
 
 
 
-size_t olm_pk_decrypt(
+ size_t olm_pk_decrypt(
     OlmPkDecryption * decryption,
     void const * ephemeral_key, size_t ephemeral_key_length,
     void const * mac, size_t mac_length,
     void * ciphertext, size_t ciphertext_length,
     void * plaintext, size_t max_plaintext_length
 );
-# 205 "../include/olm/pk.h"
-size_t olm_pk_get_private_key(
+# 221 "../include/olm/pk.h"
+ size_t olm_pk_get_private_key(
     OlmPkDecryption * decryption,
     void *private_key, size_t private_key_length
 );
 
 typedef struct OlmPkSigning OlmPkSigning;
 
 
-size_t olm_pk_signing_size(void);
+ size_t olm_pk_signing_size(void);
 
 
 
-OlmPkSigning *olm_pk_signing(
+ OlmPkSigning *olm_pk_signing(
     void * memory
 );
 
 
 
-const char * olm_pk_signing_last_error(
-    OlmPkSigning * sign
+ const char * olm_pk_signing_last_error(
+    const OlmPkSigning * sign
+);
+
+
+
+ enum OlmErrorCode olm_pk_signing_last_error_code(
+    const OlmPkSigning * sign
 );
 
 
-size_t olm_clear_pk_signing(
+ size_t olm_clear_pk_signing(
     OlmPkSigning *sign
 );
-# 240 "../include/olm/pk.h"
-size_t olm_pk_signing_key_from_seed(
+# 262 "../include/olm/pk.h"
+ size_t olm_pk_signing_key_from_seed(
     OlmPkSigning * sign,
     void * pubkey, size_t pubkey_length,
     const void * seed, size_t seed_length
 );
 
 
 
 
-size_t olm_pk_signing_seed_length(void);
+ size_t olm_pk_signing_seed_length(void);
 
 
 
 
-size_t olm_pk_signing_public_key_length(void);
+ size_t olm_pk_signing_public_key_length(void);
 
 
 
 
-size_t olm_pk_signature_length(void);
+ size_t olm_pk_signature_length(void);
 
 
 
 
 
 
-size_t olm_pk_sign(
+ size_t olm_pk_sign(
     OlmPkSigning *sign,
     uint8_t const * message, size_t message_length,
     uint8_t * signature, size_t signature_length
 );
```

### Comparing `python-olm-3.1.3/include/olm/sas.h` & `python-olm-3.2.15/include/olm/sas.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,111 @@
 # 1 "../include/olm/sas.h"
 # 1 "<built-in>"
 # 1 "<command-line>"
-# 31 "<command-line>"
 # 1 "/usr/include/stdc-predef.h" 1 3 4
-# 32 "<command-line>" 2
+# 1 "<command-line>" 2
 # 1 "../include/olm/sas.h"
 # 20 "../include/olm/sas.h"
 # 1 "dummy/stddef.h" 1
 # 21 "../include/olm/sas.h" 2
-# 32 "../include/olm/sas.h"
+
+# 1 "dummy/olm/error.h" 1
+# 23 "../include/olm/sas.h" 2
+
+# 1 "../include/olm/olm_export.h" 1
+# 25 "../include/olm/sas.h" 2
+# 36 "../include/olm/sas.h"
 typedef struct OlmSAS OlmSAS;
 
 
 
-const char * olm_sas_last_error(
-    OlmSAS * sas
+ const char * olm_sas_last_error(
+    const OlmSAS * sas
+);
+
+
+
+ enum OlmErrorCode olm_sas_last_error_code(
+    const OlmSAS * sas
 );
 
 
-size_t olm_sas_size(void);
+ size_t olm_sas_size(void);
 
 
 
-OlmSAS * olm_sas(
+ OlmSAS * olm_sas(
     void * memory
 );
 
 
-size_t olm_clear_sas(
+ size_t olm_clear_sas(
     OlmSAS * sas
 );
 
 
-size_t olm_create_sas_random_length(
-    OlmSAS * sas
+ size_t olm_create_sas_random_length(
+    const OlmSAS * sas
 );
-# 70 "../include/olm/sas.h"
-size_t olm_create_sas(
+# 80 "../include/olm/sas.h"
+ size_t olm_create_sas(
     OlmSAS * sas,
     void * random, size_t random_length
 );
 
 
-size_t olm_sas_pubkey_length(OlmSAS * sas);
-# 88 "../include/olm/sas.h"
-size_t olm_sas_get_pubkey(
+ size_t olm_sas_pubkey_length(const OlmSAS * sas);
+# 98 "../include/olm/sas.h"
+ size_t olm_sas_get_pubkey(
     OlmSAS * sas,
     void * pubkey, size_t pubkey_length
 );
-# 103 "../include/olm/sas.h"
-size_t olm_sas_set_their_key(
+# 113 "../include/olm/sas.h"
+ size_t olm_sas_set_their_key(
     OlmSAS *sas,
     void * their_key, size_t their_key_length
 );
-# 118 "../include/olm/sas.h"
-size_t olm_sas_generate_bytes(
+
+
+
+
+
+
+ int olm_sas_is_their_key_set(
+    const OlmSAS *sas
+);
+# 140 "../include/olm/sas.h"
+ size_t olm_sas_generate_bytes(
     OlmSAS * sas,
     const void * info, size_t info_length,
     void * output, size_t output_length
 );
 
 
 
-size_t olm_sas_mac_length(
-    OlmSAS *sas
+ size_t olm_sas_mac_length(
+    const OlmSAS *sas
 );
-# 145 "../include/olm/sas.h"
-size_t olm_sas_calculate_mac(
+# 167 "../include/olm/sas.h"
+ size_t olm_sas_calculate_mac(
+    OlmSAS * sas,
+    const void * input, size_t input_length,
+    const void * info, size_t info_length,
+    void * mac, size_t mac_length
+);
+
+
+
+ size_t olm_sas_calculate_mac_fixed_base64(
     OlmSAS * sas,
     const void * input, size_t input_length,
     const void * info, size_t info_length,
     void * mac, size_t mac_length
 );
 
 
-size_t olm_sas_calculate_mac_long_kdf(
+ size_t olm_sas_calculate_mac_long_kdf(
     OlmSAS * sas,
     const void * input, size_t input_length,
     const void * info, size_t info_length,
     void * mac, size_t mac_length
 );
```

### Comparing `python-olm-3.1.3/olm/__init__.py` & `python-olm-3.2.15/olm/__init__.py`

 * *Files identical despite different names*

### Comparing `python-olm-3.1.3/olm/_compat.py` & `python-olm-3.2.15/olm/_compat.py`

 * *Files identical despite different names*

### Comparing `python-olm-3.1.3/olm/_finalize.py` & `python-olm-3.2.15/olm/_finalize.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 # OR OTHER DEALINGS IN THE SOFTWARE.
 
 """Finalization with weakrefs
 
 This is designed for avoiding __del__.
 """
-from __future__ import print_function
 
 import sys
 import traceback
 import weakref
 
 __author__ = "Benjamin Peterson <benjamin@python.org>"
```

### Comparing `python-olm-3.1.3/olm/account.py` & `python-olm-3.2.15/olm/account.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 """
 
 import json
 # pylint: disable=redefined-builtin,unused-import
 from builtins import bytes, super
 from typing import AnyStr, Dict, Optional, Type
 
-from future.utils import bytes_to_native_str
-
 # pylint: disable=no-name-in-module
 from _libolm import ffi, lib  # type: ignore
 
 from ._compat import URANDOM, to_bytearray
 from ._finalize import track_for_finalization
 
 # This is imported only for type checking purposes
@@ -89,16 +87,15 @@
 
 
     def _check_error(self, ret):
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(
-            ffi.string((lib.olm_account_last_error(self._account))))
+        last_error = ffi.string((lib.olm_account_last_error(self._account))).decode()
 
         raise OlmAccountError(last_error)
 
     def pickle(self, passphrase=""):
         # type: (Optional[str]) -> bytes
         """Store an Olm account.
 
@@ -205,15 +202,15 @@
                                      out_length))
         finally:
             # clear out copies of the message, which may be plaintext
             if bytes_message is not message:
                 for i in range(0, len(bytes_message)):
                     bytes_message[i] = 0
 
-        return bytes_to_native_str(ffi.unpack(out_buffer, out_length))
+        return ffi.unpack(out_buffer, out_length).decode()
 
     @property
     def max_one_time_keys(self):
         # type: () -> int
         """int: The maximum number of one-time keys the account can store."""
         return lib.olm_account_max_number_of_one_time_keys(self._account)
 
@@ -265,7 +262,60 @@
 
         Args:
             session(Session): An Olm Session object that was created with this
             account.
         """
         self._check_error(lib.olm_remove_one_time_keys(self._account,
                                                        session._session))
+
+    def generate_fallback_key(self):
+        # type: () -> None
+        """Generate a new fallback key
+
+        This will overwrite the existing fallback key, make sure that you upload
+        the fallback key before rotating again. Internally there are two slots
+        for the private part of the fallback key. Rotating without uploading
+        means that we'll remove a fallback key that may be still used on the
+        server side but has been removed on our side.
+
+        When we receive pre-key messages that use such a removed fallback key we
+        won't be able to create a new Olm session.
+        """
+        random_length = lib.olm_account_generate_fallback_key_random_length(
+            self._account
+        )
+        random = URANDOM(random_length)
+
+        self._check_error(
+            lib.olm_account_generate_fallback_key(
+                self._account, ffi.from_buffer(random), random_length
+            )
+        )
+
+    def forget_old_fallback_key(self):
+        """Forget about the old fallback key.
+
+        This should be called once you are reasonably certain that you will not
+        receive any more messages that use the old fallback key (e.g. 5 minutes
+        after the new fallback key has been published).
+        """
+        lib.olm_account_forget_old_fallback_key(self._account)
+
+    @property
+    def fallback_key(self):
+        """The public part of the current fallback for this account.
+
+        The fallback key can be uploaded alongside of the one-time keys. It can
+        be used instead of a one-time key to establish a new Olm Session. The
+        fallback key comes into play if all one-time keys have been used up due
+        to the client being offline and not replenishing the pool of one-time
+        keys.
+        """
+        out_length = lib.olm_account_unpublished_fallback_key_length(self._account)
+        out_buffer = ffi.new("char[]", out_length)
+
+        ret = lib.olm_account_unpublished_fallback_key(self._account, out_buffer, out_length)
+        self._check_error(ret)
+
+        fallback_key = ffi.unpack(out_buffer, out_length)
+
+        return json.loads(fallback_key)
```

### Comparing `python-olm-3.1.3/olm/group_session.py` & `python-olm-3.2.15/olm/group_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     >>> InboundGroupSession(outbound.session_key)
 """
 
 # pylint: disable=redefined-builtin,unused-import
 from builtins import bytes, super
 from typing import AnyStr, Optional, Tuple, Type
 
-from future.utils import bytes_to_native_str
-
 # pylint: disable=no-name-in-module
 from _libolm import ffi, lib  # type: ignore
 
 from ._compat import URANDOM, to_bytearray, to_bytes, to_unicode_str
 from ._finalize import track_for_finalization
 
 
@@ -167,16 +165,17 @@
         return obj
 
     def _check_error(self, ret):
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(ffi.string(
-            lib.olm_inbound_group_session_last_error(self._session)))
+        last_error = ffi.string(
+            lib.olm_inbound_group_session_last_error(self._session)
+        ).decode()
 
         raise OlmGroupSessionError(last_error)
 
     def decrypt(self, ciphertext, unicode_errors="replace"):
         # type: (AnyStr, str) -> Tuple[str, int]
         """Decrypt a message
 
@@ -248,15 +247,15 @@
         id_buffer = ffi.new("char[]", id_length)
         ret = lib.olm_inbound_group_session_id(
             self._session,
             id_buffer,
             id_length
         )
         self._check_error(ret)
-        return bytes_to_native_str(ffi.unpack(id_buffer, id_length))
+        return ffi.unpack(id_buffer, id_length).decode()
 
     @property
     def first_known_index(self):
         # type: () -> int
         """int: The first message index we know how to decrypt."""
         return lib.olm_inbound_group_session_first_known_index(self._session)
 
@@ -286,15 +285,15 @@
         ret = lib.olm_export_inbound_group_session(
             self._session,
             export_buffer,
             export_length,
             message_index
         )
         self._check_error(ret)
-        export_str = bytes_to_native_str(ffi.unpack(export_buffer, export_length))
+        export_str = ffi.unpack(export_buffer, export_length).decode()
 
         # clear out copies of the key
         lib.memset(export_buffer, 0, export_length)
 
         return export_str
 
     @classmethod
@@ -369,17 +368,17 @@
         self._check_error(ret)
 
     def _check_error(self, ret):
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(ffi.string(
+        last_error = ffi.string(
             lib.olm_outbound_group_session_last_error(self._session)
-        ))
+        ).decode()
 
         raise OlmGroupSessionError(last_error)
 
     def pickle(self, passphrase=""):
         # type: (Optional[str]) -> bytes
         """Store an outbound group session.
 
@@ -479,15 +478,15 @@
             self._check_error(ret)
         finally:
             # clear out copies of plaintext
             if byte_plaintext is not plaintext:
                 for i in range(0, len(byte_plaintext)):
                     byte_plaintext[i] = 0
 
-        return bytes_to_native_str(ffi.unpack(message_buffer, message_length))
+        return ffi.unpack(message_buffer, message_length).decode()
 
     @property
     def id(self):
         # type: () -> str
         """str: A base64 encoded identifier for this session."""
         id_length = lib.olm_outbound_group_session_id_length(self._session)
         id_buffer = ffi.new("char[]", id_length)
@@ -495,15 +494,15 @@
         ret = lib.olm_outbound_group_session_id(
             self._session,
             id_buffer,
             id_length
         )
         self._check_error(ret)
 
-        return bytes_to_native_str(ffi.unpack(id_buffer, id_length))
+        return ffi.unpack(id_buffer, id_length).decode()
 
     @property
     def message_index(self):
         # type: () -> int
         """int: The current message index of the session.
 
         Each message is encrypted with an increasing index. This is the index
@@ -525,8 +524,8 @@
         ret = lib.olm_outbound_group_session_key(
             self._session,
             key_buffer,
             key_length
         )
         self._check_error(ret)
 
-        return bytes_to_native_str(ffi.unpack(key_buffer, key_length))
+        return ffi.unpack(key_buffer, key_length).decode()
```

### Comparing `python-olm-3.1.3/olm/pk.py` & `python-olm-3.2.15/olm/pk.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     >>> ed25519_verify(signing.public_key, plaintext, signature)
 
 """
 
 from builtins import super
 from typing import AnyStr, Type
 
-from future.utils import bytes_to_native_str
-
 from _libolm import ffi, lib  # type: ignore
 
 from ._compat import URANDOM, to_bytearray, to_unicode_str
 from ._finalize import track_for_finalization
 
 
 class PkEncryptionError(Exception):
@@ -112,16 +110,17 @@
                 byte_key[i] = 0
 
     def _check_error(self, ret):  # pragma: no cover
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(
-            ffi.string(lib.olm_pk_encryption_last_error(self._pk_encryption)))
+        last_error = ffi.string(
+            lib.olm_pk_encryption_last_error(self._pk_encryption)
+        ).decode()
 
         raise PkEncryptionError(last_error)
 
     def encrypt(self, plaintext):
         # type: (AnyStr) -> PkMessage
         """Encrypt a message.
 
@@ -162,20 +161,17 @@
         finally:  # pragma: no cover
             # clear out copies of plaintext
             if byte_plaintext is not plaintext:
                 for i in range(0, len(byte_plaintext)):
                     byte_plaintext[i] = 0
 
         message = PkMessage(
-            bytes_to_native_str(
-                ffi.unpack(ephemeral_key, ephemeral_key_size)),
-            bytes_to_native_str(
-                ffi.unpack(mac, mac_length)),
-            bytes_to_native_str(
-                ffi.unpack(ciphertext, ciphertext_length))
+            ffi.unpack(ephemeral_key, ephemeral_key_size).decode(),
+            ffi.unpack(mac, mac_length).decode(),
+            ffi.unpack(ciphertext, ciphertext_length).decode(),
         )
         return message
 
 
 def _clear_pk_decryption(pk_struct):
     lib.olm_clear_pk_decryption(pk_struct)
 
@@ -213,26 +209,27 @@
 
         ret = lib.olm_pk_key_from_private(
             self._pk_decryption,
             key_buffer, key_length,
             random_buffer, random_length
         )
         self._check_error(ret)
-        self.public_key = bytes_to_native_str(ffi.unpack(
+        self.public_key: str = ffi.unpack(
             key_buffer,
             key_length
-        ))
+        ).decode()
 
     def _check_error(self, ret):
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(
-            ffi.string(lib.olm_pk_decryption_last_error(self._pk_decryption)))
+        last_error = ffi.string(
+            lib.olm_pk_decryption_last_error(self._pk_decryption)
+        ).decode()
 
         raise PkDecryptionError(last_error)
 
     def pickle(self, passphrase=""):
         # type: (str) -> bytes
         """Store a PkDecryption object.
 
@@ -263,15 +260,15 @@
             for i in range(0, len(byte_key)):
                 byte_key[i] = 0
 
         return ffi.unpack(pickle_buffer, pickle_length)
 
     @classmethod
     def from_pickle(cls, pickle, passphrase=""):
-        # types: (bytes, str) -> PkDecryption
+        # type: (bytes, str) -> PkDecryption
         """Restore a previously stored PkDecryption object.
 
         Creates a PkDecryption object from a pickled base64 string. Decrypts
         the pickled object using the supplied passphrase.
         Raises PkDecryptionError on failure. If the passphrase
         doesn't match the one used to encrypt the session then the error
         message for the exception will be "BAD_ACCOUNT_KEY". If the base64
@@ -302,23 +299,23 @@
 
         try:
             obj._check_error(ret)
         finally:
             for i in range(0, len(byte_key)):
                 byte_key[i] = 0
 
-        obj.public_key = bytes_to_native_str(ffi.unpack(
+        obj.public_key = ffi.unpack(
             pubkey_buffer,
             pubkey_length
-        ))
+        ).decode()
 
         return obj
 
     def decrypt(self, message, unicode_errors="replace"):
-        # type (PkMessage, str) -> str
+        # type: (PkMessage, str) -> str
         """Decrypt a previously encrypted Pk message.
 
         Returns the decrypted plaintext.
         Raises PkDecryptionError on failure.
 
         Args:
             message(PkMessage): the pk message to decrypt.
@@ -407,25 +404,22 @@
         )
 
         # zero out copies of the seed
         lib.memset(seed_buffer, 0, len(seed))
 
         self._check_error(ret)
 
-        self.public_key = bytes_to_native_str(
-            ffi.unpack(pubkey_buffer, pubkey_length)
-        )
+        self.public_key = ffi.unpack(pubkey_buffer, pubkey_length).decode()
 
     def _check_error(self, ret):
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(
-            ffi.string(lib.olm_pk_signing_last_error(self._pk_signing)))
+        last_error = ffi.string(lib.olm_pk_signing_last_error(self._pk_signing)).decode()
 
         raise PkSigningError(last_error)
 
     @classmethod
     def generate_seed(cls):
         # type: () -> bytes
         """Generate a random seed.
@@ -452,10 +446,8 @@
 
         ret = lib.olm_pk_sign(
             self._pk_signing,
             ffi.from_buffer(bytes_message), len(bytes_message),
             signature_buffer, signature_length)
         self._check_error(ret)
 
-        return bytes_to_native_str(
-            ffi.unpack(signature_buffer, signature_length)
-        )
+        return ffi.unpack(signature_buffer, signature_length).decode()
```

### Comparing `python-olm-3.1.3/olm/sas.py` & `python-olm-3.2.15/olm/sas.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,32 +30,20 @@
 
 """
 
 from builtins import bytes
 from functools import wraps
 from typing import Optional
 
-from future.utils import bytes_to_native_str
-
 from _libolm import ffi, lib
 
 from ._compat import URANDOM, to_bytearray, to_bytes
 from ._finalize import track_for_finalization
 
 
-def other_pubkey_set(func):
-    """Ensure that the other pubkey is added to the Sas object."""
-    @wraps(func)
-    def wrapper(self, *args, **kwargs):
-        if not self.other_key_set:
-            raise OlmSasError("The other public key isn't set.")
-        return func(self, *args, **kwargs)
-    return wrapper
-
-
 def _clear_sas(sas):
     # type: (ffi.cdata) -> None
     lib.olm_clear_sas(sas)
 
 
 class OlmSasError(Exception):
     """libolm Sas error exception."""
@@ -69,24 +57,19 @@
         """Create a new SAS object.
 
         Args:
             other_users_pubkey(str, optional): The other users public key, this
                 key is necesary to generate bytes for the authentication string
                 as well as to calculate the MAC.
 
-        Attributes:
-            other_key_set (bool): A boolean flag that tracks if we set the
-                other users public key for this SAS object.
-
         Raises OlmSasError on failure.
 
         """
         self._buf = ffi.new("char[]", lib.olm_sas_size())
         self._sas = lib.olm_sas(self._buf)
-        self.other_key_set = False
         track_for_finalization(self, self._sas, _clear_sas)
 
         random_length = lib.olm_create_sas_random_length(self._sas)
         random = URANDOM(random_length)
 
         self._create_sas(random, random_length)
 
@@ -103,16 +86,15 @@
         )
 
     def _check_error(self, ret):
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(
-            ffi.string((lib.olm_sas_last_error(self._sas))))
+        last_error = ffi.string((lib.olm_sas_last_error(self._sas))).decode()
 
         raise OlmSasError(last_error)
 
     @property
     def pubkey(self):
         # type: () -> str
         """Get the public key for the SAS object.
@@ -126,15 +108,22 @@
         pubkey_length = lib.olm_sas_pubkey_length(self._sas)
         pubkey_buffer = ffi.new("char[]", pubkey_length)
 
         self._check_error(
             lib.olm_sas_get_pubkey(self._sas, pubkey_buffer, pubkey_length)
         )
 
-        return bytes_to_native_str(ffi.unpack(pubkey_buffer, pubkey_length))
+        return ffi.unpack(pubkey_buffer, pubkey_length).decode()
+
+    @property
+    def other_key_set(self):
+        # type: () -> bool
+        """Check if the other user's pubkey has been set.
+        """
+        return lib.olm_sas_is_their_key_set(self._sas) == 1
 
     def set_their_pubkey(self, key):
         # type: (str) -> None
         """Set the public key of the other user.
 
         This sets the public key of the other user, it needs to be set before
         bytes can be generated for the authentication string and a MAC can be
@@ -151,17 +140,15 @@
         self._check_error(
             lib.olm_sas_set_their_key(
                 self._sas,
                 ffi.from_buffer(byte_key),
                 len(byte_key)
             )
         )
-        self.other_key_set = True
 
-    @other_pubkey_set
     def generate_bytes(self, extra_info, length):
         # type: (str, int) -> bytes
         """Generate bytes to use for the short authentication string.
 
         Args:
             extra_info (str): Extra information to mix in when generating the
                 bytes.
@@ -185,15 +172,14 @@
                 out_buffer,
                 length
             )
         )
 
         return ffi.unpack(out_buffer, length)
 
-    @other_pubkey_set
     def calculate_mac(self, message, extra_info):
         # type: (str, str) -> str
         """Generate a message authentication code based on the shared secret.
 
         Args:
             message (str): The message to produce the authentication code for.
             extra_info (str): Extra information to mix in when generating the
@@ -215,17 +201,50 @@
                 len(byte_message),
                 ffi.from_buffer(byte_info),
                 len(byte_info),
                 mac_buffer,
                 mac_length
             )
         )
-        return bytes_to_native_str(ffi.unpack(mac_buffer, mac_length))
+        return ffi.unpack(mac_buffer, mac_length).decode()
+
+    def calculate_mac_fixed_base64(self, message, extra_info):
+        # type: (str, str) -> str
+        """Generate a message authentication code based on the shared secret.
+
+        This function uses a fixed base64 encoding that is compatible with
+        other base64 implementations.
+
+        Args:
+            message (str): The message to produce the authentication code for.
+            extra_info (str): Extra information to mix in when generating the
+                MAC
+
+        Raises OlmSasError on failure.
+
+        """
+        byte_message = to_bytes(message)
+        byte_info = to_bytes(extra_info)
+
+        mac_length = lib.olm_sas_mac_length(self._sas)
+        mac_buffer = ffi.new("char[]", mac_length)
+
+        self._check_error(
+            lib.olm_sas_calculate_mac_fixed_base64(
+                self._sas,
+                ffi.from_buffer(byte_message),
+                len(byte_message),
+                ffi.from_buffer(byte_info),
+                len(byte_info),
+                mac_buffer,
+                mac_length
+            )
+        )
+        return ffi.unpack(mac_buffer, mac_length).decode()
 
-    @other_pubkey_set
     def calculate_mac_long_kdf(self, message, extra_info):
         # type: (str, str) -> str
         """Generate a message authentication code based on the shared secret.
 
         This function should not be used unless compatibility with an older
         non-tagged Olm version is required.
 
@@ -250,8 +269,8 @@
                 len(byte_message),
                 ffi.from_buffer(byte_info),
                 len(byte_info),
                 mac_buffer,
                 mac_length
             )
         )
-        return bytes_to_native_str(ffi.unpack(mac_buffer, mac_length))
+        return ffi.unpack(mac_buffer, mac_length).decode()
```

### Comparing `python-olm-3.1.3/olm/session.py` & `python-olm-3.2.15/olm/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 
 """
 
 # pylint: disable=redefined-builtin,unused-import
 from builtins import bytes, super
 from typing import AnyStr, Optional, Type
 
-from future.utils import bytes_to_native_str
-
 # pylint: disable=no-name-in-module
 from _libolm import ffi, lib  # type: ignore
 
 from ._compat import URANDOM, to_bytearray, to_bytes, to_unicode_str
 from ._finalize import track_for_finalization
 
 # This is imported only for type checking purposes
@@ -142,16 +140,15 @@
             self._session = self._session  # type: ffi.cdata
 
     def _check_error(self, ret):
         # type: (int) -> None
         if ret != lib.olm_error():
             return
 
-        last_error = bytes_to_native_str(
-            ffi.string(lib.olm_session_last_error(self._session)))
+        last_error = ffi.string(lib.olm_session_last_error(self._session)).decode()
 
         raise OlmSessionError(last_error)
 
     def pickle(self, passphrase=""):
         # type: (Optional[str]) -> bytes
         """Store an Olm session.
 
@@ -256,24 +253,24 @@
             # clear out copies of plaintext
             if byte_plaintext is not plaintext:
                 for i in range(0, len(byte_plaintext)):
                     byte_plaintext[i] = 0
 
         if message_type == lib.OLM_MESSAGE_TYPE_PRE_KEY:
             return OlmPreKeyMessage(
-                bytes_to_native_str(ffi.unpack(
+                ffi.unpack(
                     ciphertext_buffer,
                     ciphertext_length
-                )))
+                ).decode())
         elif message_type == lib.OLM_MESSAGE_TYPE_MESSAGE:
             return OlmMessage(
-                bytes_to_native_str(ffi.unpack(
+                ffi.unpack(
                     ciphertext_buffer,
                     ciphertext_length
-                )))
+                ).decode())
         else:  # pragma: no cover
             raise ValueError("Unknown message type")
 
     def decrypt(self, message, unicode_errors="replace"):
         # type: (_OlmMessage, str) -> str
         """Decrypts a message using the session. Returns the plaintext string
         on success. Raises OlmSessionError on failure. If the base64 couldn't
@@ -336,15 +333,15 @@
         """
         id_length = lib.olm_session_id_length(self._session)
         id_buffer = ffi.new("char[]", id_length)
 
         self._check_error(
             lib.olm_session_id(self._session, id_buffer, id_length)
         )
-        return bytes_to_native_str(ffi.unpack(id_buffer, id_length))
+        return ffi.unpack(id_buffer, id_length).decode()
 
     def matches(self, message, identity_key=None):
         # type: (OlmPreKeyMessage, Optional[AnyStr]) -> bool
         """Checks if the PRE_KEY message is for this in-bound session.
         This can happen if multiple messages are sent to this session before
         this session sends a message in reply. Returns True if the session
         matches. Returns False if the session does not match. Raises
@@ -387,14 +384,32 @@
                 self._session,
                 message_buffer, len(byte_ciphertext))
 
         self._check_error(ret)
 
         return bool(ret)
 
+    def describe(self, buffer_length=600):
+        # type: (int) -> str
+        """
+        Generate a string describing the internal state of an olm session
+        for debugging and logging purposes.
+
+        Args:
+            buffer_length(int): The size of buffer for the string.
+                If the buffer is not large enough to hold the entire string, it
+                will be truncated and will end with "...".  A buffer length of
+                600 will be enough to hold any output.
+        """
+        describe_buffer = ffi.new("char[]", buffer_length)
+        lib.olm_session_describe(
+            self._session, describe_buffer, buffer_length
+        )
+        return ffi.string(describe_buffer).decode()
+
 
 class InboundSession(Session):
     """Inbound Olm session for p2p encrypted communication.
     """
 
     def __new__(cls, account, message, identity_key=None):
         # type: (Account, OlmPreKeyMessage, Optional[AnyStr]) -> Session
```

### Comparing `python-olm-3.1.3/olm/utility.py` & `python-olm-3.2.15/olm/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,14 @@
     >>> ed25519_verify(signing_key, message, signature)
 
 """
 
 # pylint: disable=redefined-builtin,unused-import
 from typing import AnyStr, Type
 
-from future.utils import bytes_to_native_str
-
 # pylint: disable=no-name-in-module
 from _libolm import ffi, lib  # type: ignore
 
 from ._compat import to_bytearray, to_bytes
 from ._finalize import track_for_finalization
 
 
@@ -119,15 +117,15 @@
         hash = ffi.new("char[]", hash_length)
 
         ret = lib.olm_sha256(cls._utility, byte_input, len(byte_input),
                              hash, hash_length)
 
         cls._check_error(ret, OlmHashError)
 
-        return bytes_to_native_str(ffi.unpack(hash, hash_length))
+        return ffi.unpack(hash, hash_length).decode()
 
 
 def ed25519_verify(key, message, signature):
     # type: (AnyStr, AnyStr, AnyStr) -> None
     """Verify an ed25519 signature.
 
     Raises an OlmVerifyError if verification fails.
```

### Comparing `python-olm-3.1.3/olm_build.py` & `python-olm-3.2.15/olm_build.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,47 +11,66 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY
 # SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
 # RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF
 # CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
 # CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-from __future__ import unicode_literals
-
 import os
 import subprocess
 
 from cffi import FFI
 
 ffibuilder = FFI()
 PATH = os.path.dirname(__file__)
 
 DEVELOP = os.environ.get("DEVELOP")
 
-compile_args = ["-I../include"]
-link_args = ["-L../build"]
+compile_args = ["-Ilibolm/include"]
 
 if DEVELOP and DEVELOP.lower() in ["yes", "true", "1"]:
     link_args.append('-Wl,-rpath=../build')
 
-headers_build = subprocess.Popen("make headers", shell=True)
-headers_build.wait()
+# Try to build with cmake first, fall back to GNU make
+try:
+    subprocess.run(
+        ["cmake", ".", "-Bbuild", "-DBUILD_SHARED_LIBS=NO"],
+        cwd="libolm", check=True,
+    )
+    subprocess.run(
+        ["cmake", "--build", "build"],
+        cwd="libolm", check=True,
+    )
+except FileNotFoundError:
+    try:
+        # try "gmake" first because some systems have a non-GNU make
+        # installed as "make"
+        subprocess.run(["gmake", "static"], cwd="libolm", check=True)
+    except FileNotFoundError:
+        # some systems have GNU make installed without the leading "g"
+        # so give that a try (though this may fail if it isn't GNU make)
+        subprocess.run(["make", "static"], cwd="libolm", check=True)
 
 ffibuilder.set_source(
     "_libolm",
     r"""
         #include <olm/olm.h>
         #include <olm/inbound_group_session.h>
         #include <olm/outbound_group_session.h>
         #include <olm/pk.h>
         #include <olm/sas.h>
     """,
     libraries=["olm"],
+    library_dirs=[os.path.join("libolm", "build")],
     extra_compile_args=compile_args,
-    extra_link_args=link_args)
+    source_extension=".cpp", # we need to link the C++ standard library, so use a C++ extension
+)
+
+with open(os.path.join(PATH, "include/olm/error.h")) as f:
+    ffibuilder.cdef(f.read(), override=True)
 
 with open(os.path.join(PATH, "include/olm/olm.h")) as f:
     ffibuilder.cdef(f.read(), override=True)
 
 with open(os.path.join(PATH, "include/olm/pk.h")) as f:
     ffibuilder.cdef(f.read(), override=True)
```

### Comparing `python-olm-3.1.3/setup.py` & `python-olm-3.2.15/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,12 +20,14 @@
     url=about["__url__"],
     license=about["__license__"],
     packages=["olm"],
     setup_requires=["cffi>=1.0.0"],
     cffi_modules=["olm_build.py:ffibuilder"],
     install_requires=[
         "cffi>=1.0.0",
-        "future",
         "typing;python_version<'3.5'"
     ],
-    zip_safe=False
+    zip_safe=False,
+    package_data={
+        "olm": ["py.typed"]
+    }
 )
```

