# Comparing `tmp/CryptoLyzer-0.8.5.tar.gz` & `tmp/CryptoLyzer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/usr/src/dist/tmps4N1pr/CryptoLyzer-0.8.5.tar", last modified: Thu Apr  6 07:00:19 2023, max compression
+gzip compressed data, was "CryptoLyzer-0.9.0.tar", last modified: Mon May  1 08:45:42 2023, max compression
```

## Comparing `CryptoLyzer-0.8.5.tar` & `CryptoLyzer-0.9.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/
--rw-r--r--   0 root         (0) root         (0)     3950 2023-04-05 22:12:02.000000 CryptoLyzer-0.8.5/setup.py
--rw-r--r--   0 root         (0) root         (0)     8624 2023-03-29 21:08:45.000000 CryptoLyzer-0.8.5/CONTRIBUTING.rst
--rw-rw-r--   0 root         (0) root         (0)    16726 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     6029 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/CryptoLyzer.egg-info/
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/CryptoLyzer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/CryptoLyzer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     6029 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/CryptoLyzer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/CryptoLyzer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1818 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/CryptoLyzer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      296 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/CryptoLyzer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    11919 2023-04-05 22:12:05.000000 CryptoLyzer-0.8.5/CHANGELOG.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/cryptolyzer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/
--rw-r--r--   0 root         (0) root         (0)    14786 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/extensions.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/sigalgos.py
--rw-r--r--   0 root         (0) root         (0)     8608 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/ciphers.py
--rw-r--r--   0 root         (0) root         (0)     5834 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/curves.py
--rw-r--r--   0 root         (0) root         (0)     4689 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/pubkeyreq.py
--rw-r--r--   0 root         (0) root         (0)    10170 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/dhparams.py
--rw-r--r--   0 root         (0) root         (0)    11621 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/all.py
--rw-r--r--   0 root         (0) root         (0)    10841 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/pubkeys.py
--rw-r--r--   0 root         (0) root         (0)    21549 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/server.py
--rw-r--r--   0 root         (0) root         (0)    49217 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/client.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3244 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/analyzer.py
--rw-r--r--   0 root         (0) root         (0)     8512 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/vulnerabilities.py
--rw-rw-r--   0 root         (0) root         (0)      270 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/exception.py
--rw-r--r--   0 root         (0) root         (0)    14994 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/simulations.py
--rw-r--r--   0 root         (0) root         (0)     9279 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/tls/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/cryptolyzer/ja3/
--rw-r--r--   0 root         (0) root         (0)     1657 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/ja3/generate.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/ja3/decode.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/ja3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      514 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/ja3/analyzer.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-04-06 06:59:39.000000 CryptoLyzer-0.8.5/cryptolyzer/__setup__.py
--rwxr-xr-x   0 root         (0) root         (0)     3682 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/cryptolyzer/httpx/
--rw-r--r--   0 root         (0) root         (0)     1713 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/httpx/headers.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/httpx/client.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/httpx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2022-12-29 22:47:54.000000 CryptoLyzer-0.8.5/cryptolyzer/httpx/analyzer.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/httpx/transfer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/cryptolyzer/hassh/
--rw-r--r--   0 root         (0) root         (0)     1451 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/hassh/generate.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/hassh/__init__.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/hassh/analyzer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/cryptolyzer/common/
--rw-r--r--   0 root         (0) root         (0)    13527 2022-12-29 22:26:08.000000 CryptoLyzer-0.8.5/cryptolyzer/common/curves.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/common/result.py
--rw-r--r--   0 root         (0) root         (0)    15739 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/common/prime.py
--rw-r--r--   0 root         (0) root         (0)   112140 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/common/dhparam.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/common/utils.py
--rw-r--r--   0 root         (0) root         (0)     4253 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/common/application.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6602 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/common/analyzer.py
--rw-r--r--   0 root         (0) root         (0)     9130 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/common/transfer.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     8977 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/common/x509.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/
--rw-r--r--   0 root         (0) root         (0)     6110 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/ciphers.py
--rw-r--r--   0 root         (0) root         (0)     5797 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/dhparams.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/all.py
--rw-r--r--   0 root         (0) root         (0)     4593 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/pubkeys.py
--rw-r--r--   0 root         (0) root         (0)     6819 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/server.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/client.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1060 2022-12-29 22:26:08.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/analyzer.py
--rw-rw-r--   0 root         (0) root         (0)     1178 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/transfer.py
--rw-rw-r--   0 root         (0) root         (0)      360 2022-03-20 16:52:35.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/exception.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-01-08 12:18:44.000000 CryptoLyzer-0.8.5/cryptolyzer/ssh/versions.py
--rw-r--r--   0 root         (0) root         (0)      153 2023-04-05 22:12:05.000000 CryptoLyzer-0.8.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2835 2023-03-29 21:08:45.000000 CryptoLyzer-0.8.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:00:19.000000 CryptoLyzer-0.8.5/test/
--rw-r--r--   0 root         (0) root         (0)    10361 2023-04-05 22:10:42.000000 CryptoLyzer-0.8.5/test/test_main.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-03-29 21:08:45.000000 CryptoLyzer-0.8.5/MANIFEST.in
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:42.002791 CryptoLyzer-0.9.0/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    12274 2023-04-29 11:50:32.000000 CryptoLyzer-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8624 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/CONTRIBUTING.rst
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.975790 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5325 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1849 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        1 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      108 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/entry_points.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      346 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/requires.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       12 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/top_level.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)    16726 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/LICENSE.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       39 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/MANIFEST.in
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5325 2023-05-01 08:45:42.001791 CryptoLyzer-0.9.0/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2835 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/README.rst
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.976790 CryptoLyzer-0.9.0/cryptolyzer/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/__init__.py
+-rwxr-xr-x   0 coroner   (1000) coroner   (1000)     3682 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/__main__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      348 2023-04-29 11:50:32.000000 CryptoLyzer-0.9.0/cryptolyzer/__setup__.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.982790 CryptoLyzer-0.9.0/cryptolyzer/common/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/common/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6603 2023-04-29 07:52:32.000000 CryptoLyzer-0.9.0/cryptolyzer/common/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4478 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/common/application.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    13527 2022-12-29 22:26:08.000000 CryptoLyzer-0.9.0/cryptolyzer/common/curves.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)   112140 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/dhparam.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2191 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    15739 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/prime.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4115 2023-04-29 07:15:07.000000 CryptoLyzer-0.9.0/cryptolyzer/common/result.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    13229 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/common/transfer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1902 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/common/utils.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8977 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/x509.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.984790 CryptoLyzer-0.9.0/cryptolyzer/hassh/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/hassh/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      442 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/hassh/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1451 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/hassh/generate.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.985790 CryptoLyzer-0.9.0/cryptolyzer/httpx/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2855 2022-12-29 22:47:54.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2365 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/client.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1713 2023-04-10 13:51:15.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/headers.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1286 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/transfer.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.987790 CryptoLyzer-0.9.0/cryptolyzer/ja3/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/__init__.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      514 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4143 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/decode.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1657 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/generate.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.991790 CryptoLyzer-0.9.0/cryptolyzer/ssh/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3478 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/all.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1060 2022-12-29 22:26:08.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6110 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/ciphers.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    14712 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/client.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5797 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/dhparams.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      360 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4593 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/pubkeys.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6808 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/server.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)     1178 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/transfer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1741 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/versions.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:42.000790 CryptoLyzer-0.9.0/cryptolyzer/tls/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    11621 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/all.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3244 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4712 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/application.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8608 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/ciphers.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    54508 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/client.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5834 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/curves.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    10170 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/dhparams.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      270 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    14786 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/extensions.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4689 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeyreq.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    10841 2023-04-24 23:04:12.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeys.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    24496 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/server.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3705 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/sigalgos.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    14994 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/simulations.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     9279 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/versions.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8512 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/vulnerabilities.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      224 2023-04-29 12:32:57.000000 CryptoLyzer-0.9.0/requirements.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2023-05-01 08:45:42.002791 CryptoLyzer-0.9.0/setup.cfg
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3950 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/setup.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:42.001791 CryptoLyzer-0.9.0/test/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    10361 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/test/test_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `CryptoLyzer-0.8.5/setup.py` & `CryptoLyzer-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/CONTRIBUTING.rst` & `CryptoLyzer-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/LICENSE.txt` & `CryptoLyzer-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/PKG-INFO` & `CryptoLyzer-0.9.0/CryptoLyzer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,22 @@
 Metadata-Version: 2.1
 Name: CryptoLyzer
-Version: 0.8.5
+Version: 0.9.0
 Summary: Fast and flexible cryptographic protocol analyzer
-Home-page: UNKNOWN
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
-Project-URL: Source, https://gitlab.com/coroner/cryptolyzer
-Project-URL: Documentation, https://cryptolyzer.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/coroner/cryptolyzer
-Project-URL: Issues, https://gitlab.com/coroner/cryptolyzer/-/issues
 Project-URL: Changelog, https://cryptolyzer.readthedocs.io/en/latest/changelog
-Description: **CryptoLyzer** is a fast and flexible server cryptographic settings analyzer library for Python with an easy-to-use
-        `command line interface <https://en.wikipedia.org/wiki/Command-line_interface>`__ with both human-readable
-        (`Markdown <https://en.wikipedia.org/wiki/Markdown>`__) and
-        machine-readable (`JSON <https://en.wikipedia.org/wiki/JSON>`__) output.  It works with multiple cryptographic protocols
-        (`SSL <https://en.wikipedia.org/wiki/Transport_Layer_Security#SSL_1.0,_2.0,_and_3.0>`__/
-        `TLS <https://en.wikipedia.org/wiki/Transport_Layer_Security>`__,
-        `opportunistic TLS <https://en.wikipedia.org/wiki/Opportunistic_TLS>`__,
-        `SSH <https://en.wikipedia.org/wiki/Secure_Shell>`__) and analyzes additional security mechanisms
-        (`web security <https://infosec.mozilla.org/guidelines/web_security>`__ related
-        `HTTP response header fields <https://en.wikipedia.org/wiki/List_of_HTTP_header_fields#Response_fields>`__,
-        `JA3 tag <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__) or `HASSH
-        tag <https://engineering.salesforce.com/open-sourcing-hassh-abed3ae5044c/>`__).
-        
-        Usage
-        -----
-        
-        Pip
-        ^^^
-        
-        .. code:: shell
-        
-           pip install cryptolyzer
-        
-           cryptolyze tls all www.example.com
-           cryptolyze tls1_2 ciphers www.example.com
-           cryptolyze ssh2 ciphers www.example.com
-           cryptolyze http headers www.example.com
-        
-        Docker
-        ^^^^^^
-        
-        .. code:: shell
-        
-           docker run --rm coroner/cryptolyzer tls all www.example.com
-           docker run --rm coroner/cryptolyzer tls1_2 ciphers www.example.com
-           docker run --rm coroner/cryptolyzer ssh2 ciphers www.example.com
-           docker run --rm coroner/cryptolyzer http headers www.example.com
-        
-        .. code:: shell
-        
-           docker run -ti --rm -p 127.0.0.1:4433:4433 coroner/cryptolyzer ja3 generate 127.0.0.1:4433
-           openssl s_client -connect 127.0.0.1:4433
-        
-           docker run -ti --rm -p 127.0.0.1:2121:2121 coroner/cryptolyzer ja3 generate ftp://127.0.0.1:2121
-           openssl s_client -starttls ftp -connect 127.0.0.1:2121
-        
-        .. code:: shell
-        
-           docker run -ti --rm -p 127.0.0.1:2222:4433 coroner/cryptolyzer hassh generate 127.0.0.1:2222
-           openssl s_client -connect 127.0.0.1:2222
-        
-        Support
-        -------
-        
-        Python implementation
-        ^^^^^^^^^^^^^^^^^^^^^
-        
-        -  CPython (2.7, 3.3+)
-        -  PyPy (2.7, 3.5+)
-        
-        Operating systems
-        ^^^^^^^^^^^^^^^^^
-        
-        -  Linux
-        -  macOS
-        -  Windows
-        
-        Social Media
-        ------------
-        
-        -  `Twitter <https://twitter.com/CryptoLyzer>`__
-        -  `Facebook <https://www.facebook.com/cryptolyzer>`__
-        
-        Credits
-        -------
-        
-        Icons made by `Freepik <https://www.flaticon.com/authors/freepik>`__ from `Flaticon <https://www.flaticon.com/>`__.
-        
-        License
-        -------
-        
-        The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
-        
-        A non-comprehensive, but straightforward description of MPL 2.0 can be found at
-        `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
-        
+Project-URL: Documentation, https://cryptolyzer.readthedocs.io/en/latest/
+Project-URL: Issues, https://gitlab.com/coroner/cryptolyzer/-/issues
+Project-URL: Source, https://gitlab.com/coroner/cryptolyzer
 Keywords: ssl tls gost ja3 hassh https pop3 smtp imap ftp rdp xmpp jabber ldap sieve ssh hsts
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -132,9 +44,96 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-Provides-Extra: pylint
 Provides-Extra: pep8
+Provides-Extra: pylint
+License-File: LICENSE.txt
+
+**CryptoLyzer** is a fast and flexible server cryptographic settings analyzer library for Python with an easy-to-use
+`command line interface <https://en.wikipedia.org/wiki/Command-line_interface>`__ with both human-readable
+(`Markdown <https://en.wikipedia.org/wiki/Markdown>`__) and
+machine-readable (`JSON <https://en.wikipedia.org/wiki/JSON>`__) output.  It works with multiple cryptographic protocols
+(`SSL <https://en.wikipedia.org/wiki/Transport_Layer_Security#SSL_1.0,_2.0,_and_3.0>`__/
+`TLS <https://en.wikipedia.org/wiki/Transport_Layer_Security>`__,
+`opportunistic TLS <https://en.wikipedia.org/wiki/Opportunistic_TLS>`__,
+`SSH <https://en.wikipedia.org/wiki/Secure_Shell>`__) and analyzes additional security mechanisms
+(`web security <https://infosec.mozilla.org/guidelines/web_security>`__ related
+`HTTP response header fields <https://en.wikipedia.org/wiki/List_of_HTTP_header_fields#Response_fields>`__,
+`JA3 tag <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__) or `HASSH
+tag <https://engineering.salesforce.com/open-sourcing-hassh-abed3ae5044c/>`__).
+
+Usage
+-----
+
+Pip
+^^^
+
+.. code:: shell
+
+   pip install cryptolyzer
+
+   cryptolyze tls all www.example.com
+   cryptolyze tls1_2 ciphers www.example.com
+   cryptolyze ssh2 ciphers www.example.com
+   cryptolyze http headers www.example.com
+
+Docker
+^^^^^^
+
+.. code:: shell
+
+   docker run --rm coroner/cryptolyzer tls all www.example.com
+   docker run --rm coroner/cryptolyzer tls1_2 ciphers www.example.com
+   docker run --rm coroner/cryptolyzer ssh2 ciphers www.example.com
+   docker run --rm coroner/cryptolyzer http headers www.example.com
+
+.. code:: shell
+
+   docker run -ti --rm -p 127.0.0.1:4433:4433 coroner/cryptolyzer ja3 generate 127.0.0.1:4433
+   openssl s_client -connect 127.0.0.1:4433
+
+   docker run -ti --rm -p 127.0.0.1:2121:2121 coroner/cryptolyzer ja3 generate ftp://127.0.0.1:2121
+   openssl s_client -starttls ftp -connect 127.0.0.1:2121
+
+.. code:: shell
+
+   docker run -ti --rm -p 127.0.0.1:2222:4433 coroner/cryptolyzer hassh generate 127.0.0.1:2222
+   openssl s_client -connect 127.0.0.1:2222
+
+Support
+-------
+
+Python implementation
+^^^^^^^^^^^^^^^^^^^^^
+
+-  CPython (2.7, 3.3+)
+-  PyPy (2.7, 3.5+)
+
+Operating systems
+^^^^^^^^^^^^^^^^^
+
+-  Linux
+-  macOS
+-  Windows
+
+Social Media
+------------
+
+-  `Twitter <https://twitter.com/CryptoLyzer>`__
+-  `Facebook <https://www.facebook.com/cryptolyzer>`__
+
+Credits
+-------
+
+Icons made by `Freepik <https://www.flaticon.com/authors/freepik>`__ from `Flaticon <https://www.flaticon.com/>`__.
+
+License
+-------
+
+The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
+
+A non-comprehensive, but straightforward description of MPL 2.0 can be found at
+`Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
```

### Comparing `CryptoLyzer-0.8.5/CryptoLyzer.egg-info/PKG-INFO` & `CryptoLyzer-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,22 @@
 Metadata-Version: 2.1
 Name: CryptoLyzer
-Version: 0.8.5
+Version: 0.9.0
 Summary: Fast and flexible cryptographic protocol analyzer
-Home-page: UNKNOWN
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
-Project-URL: Source, https://gitlab.com/coroner/cryptolyzer
-Project-URL: Documentation, https://cryptolyzer.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/coroner/cryptolyzer
-Project-URL: Issues, https://gitlab.com/coroner/cryptolyzer/-/issues
 Project-URL: Changelog, https://cryptolyzer.readthedocs.io/en/latest/changelog
-Description: **CryptoLyzer** is a fast and flexible server cryptographic settings analyzer library for Python with an easy-to-use
-        `command line interface <https://en.wikipedia.org/wiki/Command-line_interface>`__ with both human-readable
-        (`Markdown <https://en.wikipedia.org/wiki/Markdown>`__) and
-        machine-readable (`JSON <https://en.wikipedia.org/wiki/JSON>`__) output.  It works with multiple cryptographic protocols
-        (`SSL <https://en.wikipedia.org/wiki/Transport_Layer_Security#SSL_1.0,_2.0,_and_3.0>`__/
-        `TLS <https://en.wikipedia.org/wiki/Transport_Layer_Security>`__,
-        `opportunistic TLS <https://en.wikipedia.org/wiki/Opportunistic_TLS>`__,
-        `SSH <https://en.wikipedia.org/wiki/Secure_Shell>`__) and analyzes additional security mechanisms
-        (`web security <https://infosec.mozilla.org/guidelines/web_security>`__ related
-        `HTTP response header fields <https://en.wikipedia.org/wiki/List_of_HTTP_header_fields#Response_fields>`__,
-        `JA3 tag <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__) or `HASSH
-        tag <https://engineering.salesforce.com/open-sourcing-hassh-abed3ae5044c/>`__).
-        
-        Usage
-        -----
-        
-        Pip
-        ^^^
-        
-        .. code:: shell
-        
-           pip install cryptolyzer
-        
-           cryptolyze tls all www.example.com
-           cryptolyze tls1_2 ciphers www.example.com
-           cryptolyze ssh2 ciphers www.example.com
-           cryptolyze http headers www.example.com
-        
-        Docker
-        ^^^^^^
-        
-        .. code:: shell
-        
-           docker run --rm coroner/cryptolyzer tls all www.example.com
-           docker run --rm coroner/cryptolyzer tls1_2 ciphers www.example.com
-           docker run --rm coroner/cryptolyzer ssh2 ciphers www.example.com
-           docker run --rm coroner/cryptolyzer http headers www.example.com
-        
-        .. code:: shell
-        
-           docker run -ti --rm -p 127.0.0.1:4433:4433 coroner/cryptolyzer ja3 generate 127.0.0.1:4433
-           openssl s_client -connect 127.0.0.1:4433
-        
-           docker run -ti --rm -p 127.0.0.1:2121:2121 coroner/cryptolyzer ja3 generate ftp://127.0.0.1:2121
-           openssl s_client -starttls ftp -connect 127.0.0.1:2121
-        
-        .. code:: shell
-        
-           docker run -ti --rm -p 127.0.0.1:2222:4433 coroner/cryptolyzer hassh generate 127.0.0.1:2222
-           openssl s_client -connect 127.0.0.1:2222
-        
-        Support
-        -------
-        
-        Python implementation
-        ^^^^^^^^^^^^^^^^^^^^^
-        
-        -  CPython (2.7, 3.3+)
-        -  PyPy (2.7, 3.5+)
-        
-        Operating systems
-        ^^^^^^^^^^^^^^^^^
-        
-        -  Linux
-        -  macOS
-        -  Windows
-        
-        Social Media
-        ------------
-        
-        -  `Twitter <https://twitter.com/CryptoLyzer>`__
-        -  `Facebook <https://www.facebook.com/cryptolyzer>`__
-        
-        Credits
-        -------
-        
-        Icons made by `Freepik <https://www.flaticon.com/authors/freepik>`__ from `Flaticon <https://www.flaticon.com/>`__.
-        
-        License
-        -------
-        
-        The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
-        
-        A non-comprehensive, but straightforward description of MPL 2.0 can be found at
-        `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
-        
+Project-URL: Documentation, https://cryptolyzer.readthedocs.io/en/latest/
+Project-URL: Issues, https://gitlab.com/coroner/cryptolyzer/-/issues
+Project-URL: Source, https://gitlab.com/coroner/cryptolyzer
 Keywords: ssl tls gost ja3 hassh https pop3 smtp imap ftp rdp xmpp jabber ldap sieve ssh hsts
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -132,9 +44,96 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-Provides-Extra: pylint
 Provides-Extra: pep8
+Provides-Extra: pylint
+License-File: LICENSE.txt
+
+**CryptoLyzer** is a fast and flexible server cryptographic settings analyzer library for Python with an easy-to-use
+`command line interface <https://en.wikipedia.org/wiki/Command-line_interface>`__ with both human-readable
+(`Markdown <https://en.wikipedia.org/wiki/Markdown>`__) and
+machine-readable (`JSON <https://en.wikipedia.org/wiki/JSON>`__) output.  It works with multiple cryptographic protocols
+(`SSL <https://en.wikipedia.org/wiki/Transport_Layer_Security#SSL_1.0,_2.0,_and_3.0>`__/
+`TLS <https://en.wikipedia.org/wiki/Transport_Layer_Security>`__,
+`opportunistic TLS <https://en.wikipedia.org/wiki/Opportunistic_TLS>`__,
+`SSH <https://en.wikipedia.org/wiki/Secure_Shell>`__) and analyzes additional security mechanisms
+(`web security <https://infosec.mozilla.org/guidelines/web_security>`__ related
+`HTTP response header fields <https://en.wikipedia.org/wiki/List_of_HTTP_header_fields#Response_fields>`__,
+`JA3 tag <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__) or `HASSH
+tag <https://engineering.salesforce.com/open-sourcing-hassh-abed3ae5044c/>`__).
+
+Usage
+-----
+
+Pip
+^^^
+
+.. code:: shell
+
+   pip install cryptolyzer
+
+   cryptolyze tls all www.example.com
+   cryptolyze tls1_2 ciphers www.example.com
+   cryptolyze ssh2 ciphers www.example.com
+   cryptolyze http headers www.example.com
+
+Docker
+^^^^^^
+
+.. code:: shell
+
+   docker run --rm coroner/cryptolyzer tls all www.example.com
+   docker run --rm coroner/cryptolyzer tls1_2 ciphers www.example.com
+   docker run --rm coroner/cryptolyzer ssh2 ciphers www.example.com
+   docker run --rm coroner/cryptolyzer http headers www.example.com
+
+.. code:: shell
+
+   docker run -ti --rm -p 127.0.0.1:4433:4433 coroner/cryptolyzer ja3 generate 127.0.0.1:4433
+   openssl s_client -connect 127.0.0.1:4433
+
+   docker run -ti --rm -p 127.0.0.1:2121:2121 coroner/cryptolyzer ja3 generate ftp://127.0.0.1:2121
+   openssl s_client -starttls ftp -connect 127.0.0.1:2121
+
+.. code:: shell
+
+   docker run -ti --rm -p 127.0.0.1:2222:4433 coroner/cryptolyzer hassh generate 127.0.0.1:2222
+   openssl s_client -connect 127.0.0.1:2222
+
+Support
+-------
+
+Python implementation
+^^^^^^^^^^^^^^^^^^^^^
+
+-  CPython (2.7, 3.3+)
+-  PyPy (2.7, 3.5+)
+
+Operating systems
+^^^^^^^^^^^^^^^^^
+
+-  Linux
+-  macOS
+-  Windows
+
+Social Media
+------------
+
+-  `Twitter <https://twitter.com/CryptoLyzer>`__
+-  `Facebook <https://www.facebook.com/cryptolyzer>`__
+
+Credits
+-------
+
+Icons made by `Freepik <https://www.flaticon.com/authors/freepik>`__ from `Flaticon <https://www.flaticon.com/>`__.
+
+License
+-------
+
+The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
+
+A non-comprehensive, but straightforward description of MPL 2.0 can be found at
+`Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
```

### Comparing `CryptoLyzer-0.8.5/CryptoLyzer.egg-info/SOURCES.txt` & `CryptoLyzer-0.9.0/CryptoLyzer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 cryptolyzer/ssh/pubkeys.py
 cryptolyzer/ssh/server.py
 cryptolyzer/ssh/transfer.py
 cryptolyzer/ssh/versions.py
 cryptolyzer/tls/__init__.py
 cryptolyzer/tls/all.py
 cryptolyzer/tls/analyzer.py
+cryptolyzer/tls/application.py
 cryptolyzer/tls/ciphers.py
 cryptolyzer/tls/client.py
 cryptolyzer/tls/curves.py
 cryptolyzer/tls/dhparams.py
 cryptolyzer/tls/exception.py
 cryptolyzer/tls/extensions.py
 cryptolyzer/tls/pubkeyreq.py
```

### Comparing `CryptoLyzer-0.8.5/CHANGELOG.rst` & `CryptoLyzer-0.9.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Changelog
 =========
 
+0.9.0 - 2023-04-29
+------------------
+
+-  TLS (``tls``)
+
+   -  Generic
+
+      -  `OpenVPN <https://en.wikipedia.org/wiki/OpenVPN>`__ support (#85)
+
 0.8.5 - 2023-04-02
 ------------------
 
 -  TLS (``tls``)
 
-  -  Simulations (``simulations``)
+   -  Simulations (``simulations``)
 
-    -  checker for client compatibility (#92)
+      -  checker for client compatibility (#92)
 
-       -  `Chromium <https://en.wikipedia.org/wiki/Chromium_(web_browser)>`__
-       -  `Firefox <https://en.wikipedia.org/wiki/Firefox>`__
-       -  `Opera <https://en.wikipedia.org/wiki/Opera_(web_browser)>`__
+         -  `Chromium <https://en.wikipedia.org/wiki/Chromium_(web_browser)>`__
+         -  `Firefox <https://en.wikipedia.org/wiki/Firefox>`__
+         -  `Opera <https://en.wikipedia.org/wiki/Opera_(web_browser)>`__
 
 0.8.4 - 2023-01-22
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Generic
+   -  Generic
 
-    -  MySQL support (#54)
+      -  MySQL support (#54)
 
-  -  Vulnerabilities (``vulns``)
+   -  Vulnerabilities (``vulns``)
 
-    -  checker for well-known vulnerabilities (#93)
+      -  checker for well-known vulnerabilities (#93)
 
       -  Anonymous Diffie-Hellman
       -  DHEat attack
       -  DROWN attack
       -  Early TLS version
       -  Export grade ciphers
       -  FREAK attack
@@ -47,136 +56,136 @@
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Generic
+   -  Generic
 
    -  RDP hybrid mode support (#109)
 
 0.8.2 - 2022-10-10
 ------------------
 
 Features
 ~~~~~~~~
 
 -  Generic
 
-  -  Diffie-Hellman
+   -  Diffie-Hellman
 
-    -  add builtin Diffie-Hellman parameters of several application servers (#104)
-    -  add logging support to make it possible to follow up the analysis process (#58)
+      -  add builtin Diffie-Hellman parameters of several application servers (#104)
+      -  add logging support to make it possible to follow up the analysis process (#58)
 
 -  SSH (``ssh``)
 
-  -  HASSH (``hassh``)
+   -  HASSH (``hassh``)
 
-    -  tag generation support for servers (#97)
-    -  tag generation support for clients (#96)
+      -  tag generation support for servers (#97)
+      -  tag generation support for clients (#96)
 
-  -  Public Keys (``pubkeys``)
+   -  Public Keys (``pubkeys``)
 
-    -  host certificate support (#69)
+      -  host certificate support (#69)
 
 -  TLS (``tls``)
 
-  -  Diffie-Hellman (``dhparams``)
+   -  Diffie-Hellman (``dhparams``)
 
-    -  support finite field Diffie-Hellman ephemeral (FFDHE) parameter negotiation defined in RFC 7919 (#98)
+      -  support finite field Diffie-Hellman ephemeral (FFDHE) parameter negotiation defined in RFC 7919 (#98)
 
 Notable fixes
 ~~~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Extensions (``extensions``)
+   -  Extensions (``extensions``)
 
-    -  Clock accuracy check works even if difference is negative (#103)
+      -  Clock accuracy check works even if difference is negative (#103)
 
-  -  Signature Algorithms (``sigalgos``)
+   -  Signature Algorithms (``sigalgos``)
 
-    -  Not supported signature algorithms are not listed anymore (#102)
+      -  Not supported signature algorithms are not listed anymore (#102)
 
 0.8.1 - 2022-03-23
 ------------------
 
 -  JA3 (``ja3``)
 
-  -  Generate (``generate``)
+   -  Generate (``generate``)
 
-    -  support NNTP clients (#83)
-    -  support SMTP/LMTP clients (#82)
-    -  support POP3 clients (#81)
-    -  support FTP clients (#80)
-    -  support Sieve clients (#79)
-    -  support PostgreSQL clients (#78)
-    -  support LDAP clients (#77)
+      -  support NNTP clients (#83)
+      -  support SMTP/LMTP clients (#82)
+      -  support POP3 clients (#81)
+      -  support FTP clients (#80)
+      -  support Sieve clients (#79)
+      -  support PostgreSQL clients (#78)
+      -  support LDAP clients (#77)
 
 0.8.0 - 2022-01-18
 ------------------
 
 -  SSH (``ssh``)
 
-  -  Public Keys (``pubkeys``)
+   -  Public Keys (``pubkeys``)
 
-    -  add analyzer for checking SSH server against used
-       `host keys <https://datatracker.ietf.org/doc/html/rfc4253#section-6.6>`__ (#34)
+      -  add analyzer for checking SSH server against used
+         `host keys <https://datatracker.ietf.org/doc/html/rfc4253#section-6.6>`__ (#34)
 
-  -  Versions (``versions``)
+   -  Versions (``versions``)
 
-    -  identify application server and version (#71)
+      -  identify application server and version (#71)
 
 0.7.3 - 2021-12-26
 ------------------
 
 Features
 ~~~~~~~~
 
 -  SSH (``ssh``)
 
-  -  Generic
+   -  Generic
 
-    -  Add all command to SSH
+      -  Add all command to SSH
 
 Notable fixes
 ~~~~~~~~~~~~~
 
 -  Generic
 
-  -  Diffie-Hellman
+   -  Diffie-Hellman
 
-    -  Handle Diffie-Hellman parameter q value comparision well (#74)
+      -  Handle Diffie-Hellman parameter q value comparision well (#74)
 
 -  TLS (``tls``)
 
-  -  Generic
+   -  Generic
 
-    -  Handle multi-line greeting message in the case of SMTP servers (#72)
+      -  Handle multi-line greeting message in the case of SMTP servers (#72)
 
-  -  Diffie-Hellman (``dhparams``)
+   -  Diffie-Hellman (``dhparams``)
 
-    -  Add safe prime attribute to well-known DH params as there is an RFC (5144) which defines unsafe prime (#73)
+      -  Add safe prime attribute to well-known DH params as there is an RFC (5144) which defines unsafe prime (#73)
 
-  -  Public Keys (``pubkeys``)
+   -  Public Keys (``pubkeys``)
 
-    -  Handle missing certificates message well during an anonymous Diffie-Hellman key exchange (#66)
+      -  Handle missing certificates message well during an anonymous Diffie-Hellman key exchange (#66)
 
 0.7.2 - 2021-10-07
 ------------------
 
 Features
 ~~~~~~~~
 
 -  SSH (``ssh``)
 
-  -  Diffie-Hellman (``dhparams``)
+   -  Diffie-Hellman (``dhparams``)
 
-    -  add group exchange algorithms supported by the server to the result (#53)
+      -  add group exchange algorithms supported by the server to the result (#53)
 
 Other
 ~~~~~
 
 -  switch to Markdown format in changelog, readme and contributing
 -  update contributing to the latest version from contribution-guide.org
 -  add summary of the project to the readme
@@ -185,180 +194,181 @@
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  LMTP opportunistic TLS (``STARTTLS``) support (#56)
-  -  NNTP opportunistic TLS (``STARTTLS``) support (#7)
-  -  PostgreSQL opportunistic TLS (``STARTTLS``) support (#55)
+   -  LMTP opportunistic TLS (``STARTTLS``) support (#56)
+   -  NNTP opportunistic TLS (``STARTTLS``) support (#7)
+   -  PostgreSQL opportunistic TLS (``STARTTLS``) support (#55)
 
 Notable fixes
 ~~~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Generic
+   -  Generic
 
-    -  Use DH ephemeral keys that are mathematically correct during a TLS 1.3 handshake to increase stability (#57)
+      -  Use DH ephemeral keys that are mathematically correct during a TLS 1.3 handshake to increase stability (#57)
 
-  -  Ciphers (``ciphers``)
+   -  Ciphers (``ciphers``)
 
-    -  No fallback mechanism is used to check cipher suites if server honors long cipher suite lists (#59)
+      -  No fallback mechanism is used to check cipher suites if server honors long cipher suite lists (#59)
 
 0.7.0 - 2021-09-02
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Extensions (``extensions``)
+   -  Extensions (``extensions``)
 
-    -  add analyzer checking which `application-layer protocols <https://www.rfc-editor.org/rfc/rfc5077.html>`__ are
-       supported (#45)
-    -  add analyzer checking whether `encrypt-then-MAC <https://www.rfc-editor.org/rfc/rfc7366.html>`__ mode is
-       supported (#45)
-    -  add analyzer checking whether `extended master secret <https://www.rfc-editor.org/rfc/rfc7627.html>`__ is
-       supported (#45)
-    -  add analyzer checking which `next protocols <https://tools.ietf.org/id/draft-agl-tls-nextprotoneg-03.html>`__ are
-       supported (#45)
-    -  add analyzer checking whether `renegotiation indication <https://www.rfc-editor.org/rfc/rfc5746.html>`__ is
-       supported (#45)
-    -  add analyzer checking whether `session ticket <https://www.rfc-editor.org/rfc/rfc5077.html>`__ is supported (#45)
+      -  add analyzer checking which `application-layer protocols <https://www.rfc-editor.org/rfc/rfc5077.html>`__ are
+         supported (#45)
+      -  add analyzer checking whether `encrypt-then-MAC <https://www.rfc-editor.org/rfc/rfc7366.html>`__ mode is
+         supported (#45)
+      -  add analyzer checking whether `extended master secret <https://www.rfc-editor.org/rfc/rfc7627.html>`__ is
+         supported (#45)
+      -  add analyzer checking which `next protocols <https://tools.ietf.org/id/draft-agl-tls-nextprotoneg-03.html>`__
+         are supported (#45)
+      -  add analyzer checking whether `renegotiation indication <https://www.rfc-editor.org/rfc/rfc5746.html>`__ is
+         supported (#45)
+      -  add analyzer checking whether `session ticket <https://www.rfc-editor.org/rfc/rfc5077.html>`__ is supported
+         (#45)
 
-  -  Sieve opportunistic TLS (``STARTTLS``) support (#9)
+   -  Sieve opportunistic TLS (``STARTTLS``) support (#9)
 
 -  SSH (``ssh``)
 
-  -  Diffie-Hellman (``dhparams``)
+   -  Diffie-Hellman (``dhparams``)
 
-    -  check which DH parameter sizes supported by the server by group exchange (#53)
-    -  check which DH parameter sizes supported by the server by key exchange (#53)
+      -  check which DH parameter sizes supported by the server by group exchange (#53)
+      -  check which DH parameter sizes supported by the server by key exchange (#53)
 
 Notable fixes
 ~~~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Generic
+   -  Generic
 
-    -  handle server long cipher suite, signature algorithm list intolerance (#52)
+      -  handle server long cipher suite, signature algorithm list intolerance (#52)
 
 0.6.0 - 2021-05-27
 ------------------
 
 Improvements
 ~~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Ciphers (``ciphers``)
+   -  Ciphers (``ciphers``)
 
-    -  add TLS 1.3 support (#35)
+      -  add TLS 1.3 support (#35)
 
-  -  Elliptic Curves (``curves``)
+   -  Elliptic Curves (``curves``)
 
-    -  add TLS 1.3 support (#35)
+      -  add TLS 1.3 support (#35)
 
-  -  Diffie-Hellman (``dhparams``)
+   -  Diffie-Hellman (``dhparams``)
 
-    -  add TLS 1.3 support (#35)
+      -  add TLS 1.3 support (#35)
 
-  -  Signature Algorithms (``sigalgos``)
+   -  Signature Algorithms (``sigalgos``)
 
-    -  add TLS 1.3 support (#35)
+      -  add TLS 1.3 support (#35)
 
-  -  Versions (``versions``)
+   -  Versions (``versions``)
 
-    -  add TLS 1.3 support (#35)
+      -  add TLS 1.3 support (#35)
 
 0.5.0 - 2021-04-08
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-    -  add analyzer (``all``) for running all TLS analysis at once (#40)
+   -  add analyzer (``all``) for running all TLS analysis at once (#40)
 
 -  SSH (``ssh2``)
 
-    -  add analyzer for checking SSH servers against
-       `negotiated algorithms <https://tools.ietf.org/html/rfc4253#section-7.1>`__ (#33)
+   -  add analyzer for checking SSH servers against
+      `negotiated algorithms <https://tools.ietf.org/html/rfc4253#section-7.1>`__ (#33)
 
 Usability
 ~~~~~~~~~
 
 -  Generic
 
-  -  use human readable algorithms names in Markdown output (#48)
-  -  command line interface gives error output instead of traceback on exception (#49)
+   -  use human readable algorithms names in Markdown output (#48)
+   -  command line interface gives error output instead of traceback on exception (#49)
 
 0.4.0 - 2021-01-30
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  add analyzer for checking whether TLS server requires client certificate for authentication (#36)
-  -  `LDAP <https://en.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol>`__ support (#25)
+   -  add analyzer for checking whether TLS server requires client certificate for authentication (#36)
+   -  `LDAP <https://en.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol>`__ support (#25)
 
 Notable fixes
 ~~~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Generic
+   -  Generic
 
-    -  handle that a server indicates handshake failure by sending close notify alert (#44)
-    -  handle that a server does not respect lack of the signature algorithms extension (#43)
+      -  handle that a server indicates handshake failure by sending close notify alert (#44)
+      -  handle that a server does not respect lack of the signature algorithms extension (#43)
 
-  -  Versions (``versions``)
+   -  Versions (``versions``)
 
-    -  handle that a server supports only non-RSA public keys (#41)
+      -  handle that a server supports only non-RSA public keys (#41)
 
 Performance
 ~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Cipher Suites (``ciphers``)
+   -  Cipher Suites (``ciphers``)
 
-    -  speed up TLS supported curve check (#39)
+      -  speed up TLS supported curve check (#39)
 
 0.3.1 - 2020-09-15
 ------------------
 
 Features
 ~~~~~~~~
 
 -  Generic
 
-  -  `Markdown <https://en.wikipedia.org/wiki/Markdown>`__ output format (#30)
+   -  `Markdown <https://en.wikipedia.org/wiki/Markdown>`__ output format (#30)
 
 -  TLS (``tls``)
 
-  -  `XMPP (Jabber) <https://en.wikipedia.org/wiki/XMPP>`__ support (#26)
-  -  Cipher Suites (``ciphers``)
+   -  `XMPP (Jabber) <https://en.wikipedia.org/wiki/XMPP>`__ support (#26)
+   -  Cipher Suites (``ciphers``)
 
-    -  `GOST <https://en.wikipedia.org/wiki/GOST>`__ (national standards of the Russian Federation and CIS countries)
-       support for TLS cipher suite checker (#32)
+      -  `GOST <https://en.wikipedia.org/wiki/GOST>`__ (national standards of the Russian Federation and CIS countries)
+         support for TLS cipher suite checker (#32)
 
 Notable fixes
 ~~~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  fix several uncertain test cases (#28)
+   -  fix several uncertain test cases (#28)
 
 Refactor
 ~~~~~~~~
 
 -  remove unnecessary unicode conversions (#29)
 -  switch from `cryptography <https://cryptography.io>`__ to `certvalidator <https://github.com/wbond/certvalidator>`__
 
@@ -366,22 +376,22 @@
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  RDP support (#21)
+   -  RDP support (#21)
 
 -  JA3 (``ja3``)
 
-  -  `JA3 fingerprint <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__ decoding
-     support (#22)
-  -  `JA3 fingerprint <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__
-     generatoin support (#23)
+   -  `JA3 fingerprint <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__
+      decoding support (#22)
+   -  `JA3 fingerprint <https://engineering.salesforce.com/tls-fingerprinting-with-ja3-and-ja3s-247362855967>`__
+      generatoin support (#23)
 
 Notable fixes
 ~~~~~~~~~~~~~
 
 -  FTP server check cause Python traceback on connection close (#27)
 
 Refactor
@@ -393,64 +403,64 @@
 ------------------
 
 Features
 ~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Diffie-Hellman (``dhparams``)
+   -  Diffie-Hellman (``dhparams``)
 
-    -  check whether server uses `safe prime <https://en.wikipedia.org/wiki/Safe_prime>`__ as DH parameter to avoid
-       `small subgroup confinement attack <https://en.wikipedia.org/wiki/Small_subgroup_confinement_attack>`__ (#13)
-    -  check whether server uses well-known (RFC defined) DH parameter (#13)
-    -  check whether server reuse the DH parameter (#13)
+      -  check whether server uses `safe prime <https://en.wikipedia.org/wiki/Safe_prime>`__ as DH parameter to avoid
+         `small subgroup confinement attack <https://en.wikipedia.org/wiki/Small_subgroup_confinement_attack>`__ (#13)
+      -  check whether server uses well-known (RFC defined) DH parameter (#13)
+      -  check whether server reuse the DH parameter (#13)
 
-  -  FTP opportunistic TLS (``STARTTLS``) support (#8)
+   -  FTP opportunistic TLS (``STARTTLS``) support (#8)
 
 Notable Fixes
 ~~~~~~~~~~~~~
 
 -  TLS (``tls``)
 
-  -  Cipher Suites (``ciphers``)
+   -  Cipher Suites (``ciphers``)
 
-    -  handle server long cipher suite list intolerance
-    -  fix cipher suite preference order calculation (#18)
+      -  handle server long cipher suite list intolerance
+      -  fix cipher suite preference order calculation (#18)
 
-  -  Elliptic Curves (``curves``)
+   -  Elliptic Curves (``curves``)
 
-    -  fix result when server does not support named group extension
+      -  fix result when server does not support named group extension
 
-  -  Public Keys (``pubkeys``)
+   -  Public Keys (``pubkeys``)
 
-    -  handle cross signed key in the certificate chain
-    -  fix JSON output in case of expired certificates (#15)
-    -  handle the case when only a self-singed CA is served as certificate (#17)
-    -  handle the case when CA with no basic constraint is served (#20)
+      -  handle cross signed key in the certificate chain
+      -  fix JSON output in case of expired certificates (#15)
+      -  handle the case when only a self-singed CA is served as certificate (#17)
+      -  handle the case when CA with no basic constraint is served (#20)
 
-  -  handle rarely/incorrectly used TLS alerts
-  -  handle when there is no response from server (#11)
-  -  handle scheme other than tls in URL argument of the command line tool (#3)
-  -  handle plain text response to TLS handshake initiation (#19)
-  -  add default port for opportunistic TLS schemes (#6)
-  -  uniform timeout handling in TLS clients (#12)
+   -  handle rarely/incorrectly used TLS alerts
+   -  handle when there is no response from server (#11)
+   -  handle scheme other than tls in URL argument of the command line tool (#3)
+   -  handle plain text response to TLS handshake initiation (#19)
+   -  add default port for opportunistic TLS schemes (#6)
+   -  uniform timeout handling in TLS clients (#12)
 
 Other
 ^^^^^
 
 -  improve unit tests (100% code coverage)
 -  Docker support and ready-to-use container on DockerHub
    (`coroner/cryprolyzer <https://hub.docker.com/r/coroner/cryptolyzer>`__)
 -  build packages to several Linux distributions on `Open Build Service <https://build.opensuse.org/>`__
 
-  -  Debian (10, Testing)
-  -  Raspbian (10)
-  -  Ubuntu (19.10)
-  -  Fedora (29, 30, 31, Rawhide)
-  -  Mageia (7, Cauldron)
+   -  Debian (10, Testing)
+   -  Raspbian (10)
+   -  Ubuntu (19.10)
+   -  Fedora (29, 30, 31, Rawhide)
+   -  Mageia (7, Cauldron)
 
 -  IP address can be set to hostname in command line (#10)
 -  fix several Python packaging issues
 
 0.1.0 - 2019-03-20
 ------------------
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/extensions.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/extensions.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/sigalgos.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/sigalgos.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/ciphers.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/ciphers.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/curves.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/curves.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/pubkeyreq.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeyreq.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/dhparams.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/dhparams.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/all.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/all.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/pubkeys.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeys.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/server.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 import attr
 
 import six
 
 from cryptodatahub.common.algorithm import BlockCipher
 from cryptodatahub.common.exception import InvalidValue
 
-from cryptoparser.common.exception import NotEnoughData
+from cryptoparser.common.exception import InvalidType, NotEnoughData
 
 from cryptoparser.tls.extension import TlsExtensionType, TlsExtensionSupportedVersionsServer
 from cryptoparser.tls.ldap import (
     LDAPResultCode,
     LDAPExtendedRequestStartTLS,
     LDAPExtendedResponseStartTLS,
 )
 from cryptoparser.tls.mysql import (
     MySQLCapability,
     MySQLHandshakeSslRequest,
     MySQLHandshakeV10,
     MySQLRecord,
     MySQLVersion,
 )
+from cryptoparser.tls.openvpn import (
+    OpenVpnPacketHardResetServerV2,
+    OpenVpnOpCode,
+)
 from cryptoparser.tls.postgresql import SslRequest, Sync
 from cryptoparser.tls.rdp import (
     TPKT,
     COTPConnectionConfirm,
     COTPConnectionRequest,
     RDPProtocol,
     RDPNegotiationRequest,
@@ -51,14 +55,18 @@
     TlsSubprotocolMessageParser,
 )
 from cryptoparser.tls.version import TlsProtocolVersion, TlsVersion
 
 from cryptolyzer.__setup__ import __title__, __version__
 from cryptolyzer.common.exception import NetworkError, NetworkErrorType, SecurityError, SecurityErrorType
 from cryptolyzer.common.application import L7ServerBase, L7ServerHandshakeBase, L7ServerConfigurationBase
+from cryptolyzer.common.transfer import L4ServerTCP, L4ServerUDP
+from cryptolyzer.common.utils import buffer_flush, buffer_is_plain_text
+
+from cryptolyzer.tls.application import L7OpenVpnBase
 
 
 @attr.s
 class TlsServerConfiguration(L7ServerConfigurationBase):
     protocol_versions = attr.ib(
         converter=sorted,
         default=[TlsProtocolVersion(version) for version in TlsVersion],
@@ -90,76 +98,71 @@
 
     def _init_l7(self):
         pass
 
     def _deinit_l7(self):
         pass
 
-    def _get_handshake_class(self, l4_transfer):
+    def _get_handshake_class(self):
         if self.configuration.fallback_to_ssl:
             try:
-                l4_transfer.receive(TlsRecord.HEADER_SIZE)
+                self.receive(TlsRecord.HEADER_SIZE)
             except NotEnoughData as e:
                 six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
 
             try:
-                TlsRecord.parse_header(l4_transfer.buffer)
+                TlsRecord.parse_header(self.buffer)
                 handshake_class = TlsServerHandshake
             except InvalidValue:
                 handshake_class = SslServerHandshake
         else:
             handshake_class = TlsServerHandshake
 
         return handshake_class
 
     def _do_handshake(self, last_handshake_message_type):
         try:
             self._init_l7()
         except (NotEnoughData, InvalidValue, NetworkError, SecurityError):
-            self.l4_transfer.close()
+            self.l4_transfer.close_client()
             return {}
 
         try:
-            handshake_class = self._get_handshake_class(self.l4_transfer)
-            handshake_object = handshake_class(self.l4_transfer, self.configuration)
+            handshake_class = self._get_handshake_class()
+            handshake_object = handshake_class(self, self.configuration)
         except NetworkError:
-            self.l4_transfer.close()
+            self.l4_transfer.close_client()
             return {}
 
         try:
             handshake_object.do_handshake(last_handshake_message_type)
         finally:
             self._deinit_l7()
-            self.l4_transfer.close()
+            self.l4_transfer.close_client()
 
         return handshake_object.client_messages
 
     def do_handshake(self, last_handshake_message_type=TlsHandshakeType.CLIENT_HELLO):
         return self._do_handshakes(last_handshake_message_type)
 
 
-@attr.s
 class L7ServerStartTlsBase(L7ServerTlsBase):
     @classmethod
     @abc.abstractmethod
     def get_scheme(cls):
         raise NotImplementedError()
 
     @classmethod
     @abc.abstractmethod
     def get_default_port(cls):
         raise NotImplementedError()
 
 
 @attr.s
 class TlsServer(L7ServerHandshakeBase):
-    @staticmethod
-    def _is_message_plain_text(transfer):
-        return transfer.buffer and transfer.buffer_is_plain_text
-
     @abc.abstractmethod
     def _parse_record(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def _parse_message(self, record):
         raise NotImplementedError()
@@ -236,49 +239,49 @@
             if TlsHandshakeType.CLIENT_HELLO not in self.client_messages:
                 self._handle_error(TlsAlertLevel.FATAL, TlsAlertDescription.UNEXPECTED_MESSAGE)
                 raise StopIteration()
 
         if message.get_handshake_type() == TlsHandshakeType.CLIENT_HELLO:
             protocol_version = self._check_protocol_version(message)
             server_hello = self._prepare_server_hello(message, protocol_version)
-            self.l4_transfer.send(TlsRecord(server_hello.compose()).compose())
+            self.l7_transfer.send(TlsRecord(server_hello.compose()).compose())
 
         if self._last_processed_message_type == last_handshake_message_type:
             self._handle_error(TlsAlertLevel.WARNING, TlsAlertDescription.CLOSE_NOTIFY)
             raise StopIteration()
 
     def _process_non_handshake_message(self, message):
         self._handle_error(TlsAlertLevel.FATAL, TlsAlertDescription.UNEXPECTED_MESSAGE)
         raise StopIteration()
 
     def _process_plain_text_message(self):
-        if self._is_message_plain_text(self.l4_transfer):
+        if self.l7_transfer.buffer_is_plain_text:
             self._handle_error(TlsAlertLevel.WARNING, TlsAlertDescription.DECRYPT_ERROR)
             raise StopIteration()
 
     def _process_invalid_message(self):
         self._process_plain_text_message()
 
         self._handle_error(TlsAlertLevel.WARNING, TlsAlertDescription.DECRYPT_ERROR)
         raise StopIteration()
 
     def _handle_error(self, alert_level, alert_description):
         if self.configuration.close_on_error:
-            self.l4_transfer.close()
+            self.l7_transfer.l4_transfer.close_client()
         else:
-            self.l4_transfer.send(TlsRecord(
+            self.l7_transfer.send(TlsRecord(
                 TlsAlertMessage(alert_level, alert_description).compose(),
                 content_type=TlsContentType.ALERT,
             ).compose())
 
     def _parse_record(self):
-        record = TlsRecord.parse_exact_size(self.l4_transfer.buffer)
+        record, parsed_length = TlsRecord.parse_immutable(self.l7_transfer.buffer)
         is_handshake = record.content_type == TlsContentType.HANDSHAKE
 
-        return record, is_handshake
+        return record, parsed_length, is_handshake
 
     def _parse_message(self, record):
         subprotocol_parser = TlsSubprotocolMessageParser(record.content_type)
         message, _ = subprotocol_parser.parse(record.fragment)
 
         return message
 
@@ -295,43 +298,43 @@
         self.client_messages[self._last_processed_message_type] = message
 
         server_hello = SslHandshakeServerHello(
             certificate=b'fake certificate',
             cipher_kinds=message.cipher_kinds,
             connection_id=b'fake connection id',
         )
-        self.l4_transfer.send(SslRecord(server_hello).compose())
+        self.l7_transfer.send(SslRecord(server_hello).compose())
 
         if self._last_processed_message_type == last_handshake_message_type:
             self._handle_error(SslErrorType.NO_CIPHER_ERROR)
             raise StopIteration()
 
     def _process_non_handshake_message(self, message):
         self._handle_error(SslErrorType.NO_CIPHER_ERROR)
         raise StopIteration()
 
     def _process_plain_text_message(self):
-        if self._is_message_plain_text(self.l4_transfer):
+        if self.l7_transfer.buffer_is_plain_text:
             self._handle_error(SslErrorType.NO_CIPHER_ERROR)
             raise StopIteration()
 
     def _process_invalid_message(self):
         self._process_plain_text_message()
 
         self._handle_error(SslErrorType.NO_CIPHER_ERROR)
         raise StopIteration()
 
     def _handle_error(self, error_type):
-        self.l4_transfer.send(SslRecord(SslErrorMessage(error_type)).compose())
+        self.l7_transfer.send(SslRecord(SslErrorMessage(error_type)).compose())
 
     def _parse_record(self):
-        record = SslRecord.parse_exact_size(self.l4_transfer.buffer)
+        record, parsed_length = SslRecord.parse_immutable(self.l7_transfer.buffer)
         is_handshake = record.message.get_message_type() != SslMessageType.ERROR
 
-        return record, is_handshake
+        return record, parsed_length, is_handshake
 
     def _parse_message(self, record):
         return record.message
 
 
 class L7ServerTls(L7ServerTlsBase):
     @classmethod
@@ -349,33 +352,33 @@
         return 'rdp'
 
     @classmethod
     def get_default_port(cls):
         return 3389
 
     def _init_l7(self):
-        self.l4_transfer.receive(TPKT.HEADER_SIZE)
+        self.receive(TPKT.HEADER_SIZE)
         try:
-            TPKT.parse_exact_size(self.l4_transfer.buffer)
+            TPKT.parse_exact_size(self.buffer)
         except NotEnoughData as e:
-            self.l4_transfer.receive(e.bytes_needed)
+            self.receive(e.bytes_needed)
 
-        tpkt = TPKT.parse_exact_size(self.l4_transfer.buffer)
+        tpkt = TPKT.parse_exact_size(self.buffer)
         cotp = COTPConnectionRequest.parse_exact_size(tpkt.message)
         neg_req = RDPNegotiationRequest.parse_exact_size(cotp.user_data)
         if RDPProtocol.SSL not in neg_req.protocol:
             raise SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY)
 
-        self.l4_transfer.flush_buffer()
+        self.flush_buffer()
 
         neg_resp = RDPNegotiationResponse([], [RDPProtocol.SSL, ])
         cotp = COTPConnectionConfirm(src_ref=cotp.src_ref, user_data=neg_resp.compose())
         tpkt = TPKT(version=3, message=cotp.compose())
         request_bytes = tpkt.compose()
-        self.l4_transfer.send(request_bytes)
+        self.send(request_bytes)
 
     def _deinit_l7(self):
         pass
 
 
 class L7ServerTlsLDAP(L7ServerStartTlsBase):
     _EXTENDED_RESPONSE_STARTLS_BYTES = LDAPExtendedResponseStartTLS(LDAPResultCode.SUCCESS).compose()
@@ -385,24 +388,24 @@
         return 'ldap'
 
     @classmethod
     def get_default_port(cls):
         return 3389
 
     def _init_l7(self):
-        self.l4_transfer.receive(LDAPExtendedRequestStartTLS.HEADER_SIZE)
+        self.receive(LDAPExtendedRequestStartTLS.HEADER_SIZE)
         try:
-            LDAPExtendedRequestStartTLS.parse_exact_size(self.l4_transfer.buffer)
+            LDAPExtendedRequestStartTLS.parse_exact_size(self.buffer)
         except NotEnoughData as e:
-            self.l4_transfer.receive(e.bytes_needed)
+            self.receive(e.bytes_needed)
 
-        LDAPExtendedRequestStartTLS.parse_exact_size(self.l4_transfer.buffer)
-        self.l4_transfer.flush_buffer()
+        LDAPExtendedRequestStartTLS.parse_exact_size(self.buffer)
+        self.flush_buffer()
 
-        self.l4_transfer.send(self._EXTENDED_RESPONSE_STARTLS_BYTES)
+        self.send(self._EXTENDED_RESPONSE_STARTLS_BYTES)
 
     def _deinit_l7(self):
         pass
 
 
 class L7ServerTlsPostgreSQL(L7ServerStartTlsBase):
     _SSL_REQUEST_BYTES = SslRequest().compose()
@@ -413,20 +416,20 @@
         return 'postgresql'
 
     @classmethod
     def get_default_port(cls):
         return 5432
 
     def _init_l7(self):
-        self.l4_transfer.receive(len(self._SSL_REQUEST_BYTES))
-        if self.l4_transfer.buffer != self._SSL_REQUEST_BYTES:
+        self.receive(len(self._SSL_REQUEST_BYTES))
+        if self.buffer != self._SSL_REQUEST_BYTES:
             raise SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY)
-        self.l4_transfer.flush_buffer()
+        self.flush_buffer()
 
-        self.l4_transfer.send(self._SYNC_BYTES)
+        self.send(self._SYNC_BYTES)
 
     def _deinit_l7(self):
         pass
 
 
 class L7ServerTlsMySQL(L7ServerStartTlsBase):
     _SERVER_HANDSHAKE_RECORD_BYTES = MySQLRecord(0, MySQLHandshakeV10(
@@ -442,24 +445,24 @@
         return 'mysql'
 
     @classmethod
     def get_default_port(cls):
         return 3306
 
     def _init_l7(self):
-        self.l4_transfer.send(self._SERVER_HANDSHAKE_RECORD_BYTES)
+        self.send(self._SERVER_HANDSHAKE_RECORD_BYTES)
 
-        self.l4_transfer.receive(MySQLRecord.HEADER_SIZE)
+        self.receive(MySQLRecord.HEADER_SIZE)
         try:
-            MySQLRecord.parse_exact_size(self.l4_transfer.buffer)
+            MySQLRecord.parse_exact_size(self.buffer)
         except NotEnoughData as e:
-            self.l4_transfer.receive(e.bytes_needed)
+            self.receive(e.bytes_needed)
 
-        record, parsed_length = MySQLRecord.parse_immutable(self.l4_transfer.buffer)
-        self.l4_transfer.flush_buffer(parsed_length)
+        record, parsed_length = MySQLRecord.parse_immutable(self.buffer)
+        self.flush_buffer(parsed_length)
 
         ssl_request = MySQLHandshakeSslRequest.parse_exact_size(record.packet_bytes)
         if not set([MySQLCapability.CLIENT_SSL, MySQLCapability.CLIENT_SECURE_CONNECTION]) & ssl_request.capabilities:
             raise SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY)
 
     def _deinit_l7(self):
         pass
@@ -502,29 +505,29 @@
     @classmethod
     def _get_software_name(cls):
         return '{} {}'.format(__title__, __version__).encode('ascii')
 
     def _init_l7(self):
         greeting = self._get_greeting()
         if greeting:
-            self.l4_transfer.send(greeting)
+            self.send(greeting)
 
         self.l4_transfer.receive_line()
         capabilities_request_prefix = self._get_capabilities_request_prefix()
-        if capabilities_request_prefix and self.l4_transfer.buffer.startswith(capabilities_request_prefix):
+        if capabilities_request_prefix and self.buffer.startswith(capabilities_request_prefix):
             self.l4_transfer.flush_buffer()
             self.l4_transfer.send(self._get_capabilities_response())
             self.l4_transfer.receive_line()
 
         starttls_request_prefix = self._get_starttls_request_prefix()
-        if not self.l4_transfer.buffer.startswith(starttls_request_prefix):
+        if not self.buffer.startswith(starttls_request_prefix):
             raise SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY)
-        self.l4_transfer.flush_buffer()
+        self.flush_buffer()
 
-        self.l4_transfer.send(self._get_starttls_response())
+        self.send(self._get_starttls_response())
 
 
 class L7ServerTlsSieve(L7ServerStartTlsTextBase):
     @classmethod
     def get_scheme(cls):
         return 'sieve'
 
@@ -718,7 +721,114 @@
             b'200 ' + cls._get_software_name() + b' Welcome!',
             b'',
         ])
 
     @classmethod
     def _get_starttls_response(cls):
         return b'382 Continue with TLS negotiation\r\n'
+
+
+@attr.s
+class L7ServerStartTlsOpenVpnBase(L7ServerStartTlsBase, L7OpenVpnBase):
+    session_id = attr.ib(
+        init=False, default=0xff58585858585858,
+        validator=attr.validators.instance_of(six.integer_types)
+    )
+    client_packet_id = attr.ib(
+        init=False, default=0x00000000,
+        validator=attr.validators.instance_of(six.integer_types)
+    )
+    remote_session_id = attr.ib(
+        init=False, default=None,
+        validator=attr.validators.optional(attr.validators.instance_of(six.integer_types))
+    )
+    _buffer = attr.ib(init=False)
+
+    def __attrs_post_init__(self):
+        super(L7ServerStartTlsOpenVpnBase, self).__attrs_post_init__()
+
+        self._buffer = bytearray()
+
+    @classmethod
+    @abc.abstractmethod
+    def get_scheme(cls):
+        raise NotImplementedError()
+
+    @classmethod
+    @abc.abstractmethod
+    def get_default_port(cls):
+        raise NotImplementedError()
+
+    def _reset_session(self):
+        packets = self._receive_packets(self.l4_transfer)
+        packet_hard_reset_client = packets[0]
+
+        if packet_hard_reset_client.get_op_code() != OpenVpnOpCode.HARD_RESET_CLIENT_V2:
+            raise InvalidValue(
+                packet_hard_reset_client.get_op_code(), type(self), 'op_code'
+            )
+
+        self.remote_session_id = packet_hard_reset_client.session_id
+        packet_hard_reset_server = OpenVpnPacketHardResetServerV2(
+            self.session_id,
+            self.remote_session_id,
+            [packet_hard_reset_client.packet_id],
+            0
+        )
+        self._send_packet(self.l4_transfer, packet_hard_reset_server)
+
+    def _init_l7(self):
+        try:
+            self._reset_session()
+        except (InvalidValue, InvalidType, NotEnoughData) as e:
+            six.raise_from(SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY), e)
+
+    def send(self, sendable_bytes):
+        return self._send_bytes(self.l4_transfer, sendable_bytes)
+
+    def receive(self, receivable_byte_num):
+        received_bytes = self._receive_packet_bytes(self.l4_transfer, receivable_byte_num)
+        self._buffer += received_bytes
+        return len(received_bytes)
+
+    def flush_buffer(self, byte_num=None):
+        self._buffer = buffer_flush(self._buffer, byte_num)
+
+    @property
+    def buffer_is_plain_text(self):
+        return buffer_is_plain_text(self._buffer)
+
+    @property
+    def buffer(self):
+        return self._buffer
+
+    @classmethod
+    def _is_tcp(cls):
+        return issubclass(cls._get_transfer_class(), L4ServerTCP)
+
+
+class L7ServerTlsOpenVpn(L7ServerStartTlsOpenVpnBase):
+    @classmethod
+    def get_scheme(cls):
+        return 'openvpn'
+
+    @classmethod
+    def get_default_port(cls):
+        return 1194
+
+    @classmethod
+    def _get_transfer_class(cls):
+        return L4ServerUDP
+
+
+class L7ServerTlsOpenVpnTcp(L7ServerStartTlsOpenVpnBase):
+    @classmethod
+    def get_scheme(cls):
+        return 'openvpntcp'
+
+    @classmethod
+    def get_default_port(cls):
+        return 443
+
+    @classmethod
+    def _get_transfer_class(cls):
+        return L4ServerTCP
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/client.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,27 +57,34 @@
     TlsExtensionSignatureAlgorithms,
     TlsExtensionSignatureAlgorithmsCert,
     TlsExtensionSupportedVersionsClient,
     TlsExtensionsClient,
     TlsKeyShareEntry,
     TlsNamedCurve,
 )
+from cryptoparser.tls.openvpn import (
+    OpenVpnPacketAckV1,
+    OpenVpnPacketHardResetClientV2,
+)
 
 from cryptoparser.tls.record import TlsRecord, SslRecord
 from cryptoparser.tls.version import TlsVersion, TlsProtocolVersion
 
 from cryptolyzer.common.dhparam import (
     WellKnownDHParams,
     get_dh_ephemeral_key_forged,
     get_ecdh_ephemeral_key_forged,
     int_to_bytes,
 )
 from cryptolyzer.common.exception import NetworkError, NetworkErrorType, SecurityError, SecurityErrorType
+from cryptolyzer.common.transfer import L4ClientTCP, L4ClientUDP, L7TransferBase
+from cryptolyzer.common.utils import buffer_flush, buffer_is_plain_text
+
+from cryptolyzer.tls.application import L7OpenVpnBase
 from cryptolyzer.tls.exception import TlsAlert
-from cryptolyzer.common.transfer import L4ClientTCP, L7TransferBase
 
 
 NAMED_CURVE_TO_RFC7919_WELL_KNOWN = {
     TlsNamedCurve.FFDHE2048: WellKnownDHParams.RFC7919_2048_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
     TlsNamedCurve.FFDHE3072: WellKnownDHParams.RFC7919_3072_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
     TlsNamedCurve.FFDHE4096: WellKnownDHParams.RFC7919_4096_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
     TlsNamedCurve.FFDHE6144: WellKnownDHParams.RFC7919_6144_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
@@ -1377,80 +1384,89 @@
                     message.cipher_suite.value.last_version == TlsVersion.TLS1_3):
                 raise StopIteration()
 
         if handshake_type == last_handshake_message_type:
             raise StopIteration
 
     @classmethod
-    def _process_non_handshake_message(cls, content_type, message):
-        if content_type != TlsContentType.ALERT:
+    def _process_non_handshake_message(cls, content_type, message, last_handshake_message_type):
+        if content_type == TlsContentType.ALERT:
+            if (message.level == TlsAlertLevel.FATAL or
+                    message.description == TlsAlertDescription.CLOSE_NOTIFY):
+                raise TlsAlert(message.description)
+        elif last_handshake_message_type is None and content_type == TlsContentType.CHANGE_CIPHER_SPEC:
+            raise StopIteration
+        else:
             raise TlsAlert(TlsAlertDescription.UNEXPECTED_MESSAGE)
 
-        if (message.level == TlsAlertLevel.FATAL or
-                message.description == TlsAlertDescription.CLOSE_NOTIFY):
-            raise TlsAlert(message.description)
-
     @classmethod
     def _process_invalid_message(cls, transfer):
         cls.raise_response_error(transfer)
 
     @classmethod
     def _send_hello(cls, transfer, hello_message, record_version):
         tls_record_bytes = TlsRecord(hello_message.compose(), record_version, TlsContentType.HANDSHAKE).compose()
         try:
             transfer.send(tls_record_bytes)
-        except socket.timeout as e:
-            six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
+        except BaseException as e:  # pylint: disable=broad-except
+            if e.__class__.__name__ == 'TimeoutError' or isinstance(e, socket.timeout):
+                six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
+
+            raise e
 
     def do_handshake(
             self,
             transfer,
             hello_message,
             record_version=TlsProtocolVersion(TlsVersion.SSL3),
             last_handshake_message_type=TlsHandshakeType.SERVER_HELLO_DONE
     ):
         self.server_messages = {}
+        transfer.flush_buffer()
         self._send_hello(transfer, hello_message, record_version)
 
-        record_buffer = bytearray()
+        receivable_byte_num = 0
+        message_buffer = bytearray()
         while True:
             try:
-                while True:
-                    record, parsed_length = TlsRecord.parse_immutable(transfer.buffer)
-                    record_buffer += record.fragment
-                    transfer.flush_buffer(parsed_length)
-
-                    if not transfer.buffer:
-                        break
+                record, parsed_length = TlsRecord.parse_immutable(transfer.buffer)
+                message_buffer += record.fragment
+                transfer.flush_buffer(parsed_length)
 
                 subprotocol_parser = TlsSubprotocolMessageParser(record.content_type)
 
-                while record_buffer:
-                    message, parsed_length = subprotocol_parser.parse(record_buffer)
-                    record_buffer = record_buffer[parsed_length:]
+                while message_buffer:
+                    try:
+                        message, parsed_length = subprotocol_parser.parse(message_buffer)
+                    except NotEnoughData:
+                        # another record should be received
+                        break
+
+                    message_buffer = message_buffer[parsed_length:]
 
                     if record.content_type == TlsContentType.HANDSHAKE:
                         self._process_handshake_message(
                             hello_message.protocol_version, message, last_handshake_message_type
                         )
                     else:
-                        self._process_non_handshake_message(record.content_type, message)
+                        self._process_non_handshake_message(record.content_type, message, last_handshake_message_type)
 
-                receivable_byte_num = 0
+                # transfer buffer may contain another record or another record should be received
+                continue
             except NotEnoughData as e:
                 receivable_byte_num = e.bytes_needed
             except (InvalidType, InvalidValue):
                 self._process_invalid_message(transfer)
             except StopIteration:
                 return
 
             try:
                 transfer.receive(receivable_byte_num)
             except NotEnoughData as e:
-                if transfer.buffer or record_buffer:
+                if transfer.buffer:
                     six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
 
                 six.raise_from(NetworkError(NetworkErrorType.NO_RESPONSE), e)
 
 
 @attr.s
 class SslError(ValueError):
@@ -1513,7 +1529,160 @@
                                         TlsAlertDescription.INTERNAL_ERROR,
                                     ]:
                                 six.raise_from(NetworkError(NetworkErrorType.NO_RESPONSE), e)
 
                         six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
                 else:
                     six.raise_from(NetworkError(NetworkErrorType.NO_RESPONSE), e)
+
+
+@attr.s
+class ClientOpenVpnBase(L7ClientTlsBase, L7OpenVpnBase):
+    SESSION_ID = 0xff58585858585858
+
+    _buffer = attr.ib(init=False)
+
+    def __attrs_post_init__(self):
+        super(ClientOpenVpnBase, self).__attrs_post_init__()
+
+        self._buffer = bytearray()
+
+        if self.session_id is None:
+            self.session_id = int(self.SESSION_ID)
+
+    @classmethod
+    @abc.abstractmethod
+    def get_scheme(cls):
+        raise NotImplementedError()
+
+    @classmethod
+    @abc.abstractmethod
+    def get_default_port(cls):
+        raise NotImplementedError()
+
+    def _reset_session(self):
+        self.flush_buffer()
+        self.client_packet_id = 0x00000000
+        self.remote_session_id = None
+        self.session_id += 1
+        packet_client_hard_reset = OpenVpnPacketHardResetClientV2(
+            self.session_id,
+            self.client_packet_id
+        )
+        self._send_packet(self.l4_transfer, packet_client_hard_reset)
+
+        packets = self._receive_packets(self.l4_transfer)
+        packet_hard_reset_server = packets[0]
+
+        if (packet_hard_reset_server.remote_session_id is not None and
+                packet_hard_reset_server.remote_session_id != self.session_id):
+            raise InvalidValue(
+                packet_hard_reset_server.remote_session_id, type(self), 'session_id'
+            )
+
+        self.session_id = packet_hard_reset_server.remote_session_id
+        self.remote_session_id = packet_hard_reset_server.session_id
+        packet_ack_server_hard_reset = OpenVpnPacketAckV1(
+            self.session_id,
+            self.remote_session_id,
+            [packet_hard_reset_server.packet_id, ]
+        )
+        self._send_packet(self.l4_transfer, packet_ack_server_hard_reset)
+
+    def do_ssl_handshake(self, hello_message, last_handshake_message_type=SslMessageType.SERVER_HELLO):
+        return self._do_handshake(
+            SslClientHandshake(),
+            hello_message,
+            TlsVersion.SSL2,
+            last_handshake_message_type
+        )
+
+    def do_tls_handshake(
+            self,
+            hello_message,
+            record_version=TlsProtocolVersion(TlsVersion.TLS1),
+            last_handshake_message_type=TlsHandshakeType.SERVER_HELLO
+    ):
+        return self._do_handshake(
+            TlsClientOpenVpn(),
+            hello_message,
+            record_version,
+            last_handshake_message_type
+        )
+
+    def _init_connection(self):
+        if self._is_tcp():
+            self.l4_transfer = L4ClientTCP(self.address, self.port, self.timeout, self.ip)
+        else:
+            self.l4_transfer = L4ClientUDP(self.address, self.port, self.timeout, self.ip)
+        self.l4_transfer.init_connection()
+
+        try:
+            self._reset_session()
+        except (InvalidValue, InvalidType, NotEnoughData) as e:
+            six.raise_from(SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY), e)
+
+    def send(self, sendable_bytes):
+        return self._send_bytes(self.l4_transfer, sendable_bytes)
+
+    def receive(self, receivable_byte_num):
+        total_received_byte_num = 0
+        while total_received_byte_num < receivable_byte_num:
+            try:
+                actual_received_bytes = self._receive_packet_bytes(self.l4_transfer, receivable_byte_num)
+            except NotEnoughData as e:
+                six.raise_from(NotEnoughData(receivable_byte_num - total_received_byte_num), e)
+            self._buffer += actual_received_bytes
+            total_received_byte_num += len(actual_received_bytes)
+
+        return len(actual_received_bytes)
+
+    def flush_buffer(self, byte_num=None):
+        self._buffer = buffer_flush(self._buffer, byte_num)
+
+    @property
+    def buffer_is_plain_text(self):
+        return buffer_is_plain_text(self._buffer)
+
+    @property
+    def buffer(self):
+        return self._buffer
+
+    @classmethod
+    def get_default_timeout(cls):
+        return 5
+
+
+class ClientOpenVpn(ClientOpenVpnBase):
+    @classmethod
+    def get_scheme(cls):
+        return 'openvpn'
+
+    @classmethod
+    def get_default_port(cls):
+        return 1194
+
+    @classmethod
+    def get_default_timeout(cls):
+        return 2
+
+    @classmethod
+    def _is_tcp(cls):
+        return False
+
+
+class ClientOpenVpnTcp(ClientOpenVpnBase):
+    @classmethod
+    def get_scheme(cls):
+        return 'openvpntcp'
+
+    @classmethod
+    def get_default_port(cls):
+        return 443
+
+    @classmethod
+    def _is_tcp(cls):
+        return True
+
+
+class TlsClientOpenVpn(TlsClientHandshake):
+    pass
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/analyzer.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/analyzer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/vulnerabilities.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/simulations.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/simulations.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/tls/versions.py` & `CryptoLyzer-0.9.0/cryptolyzer/tls/versions.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ja3/generate.py` & `CryptoLyzer-0.9.0/cryptolyzer/ja3/generate.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ja3/decode.py` & `CryptoLyzer-0.9.0/cryptolyzer/ja3/decode.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ja3/analyzer.py` & `CryptoLyzer-0.9.0/cryptolyzer/ja3/analyzer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/__main__.py` & `CryptoLyzer-0.9.0/cryptolyzer/__main__.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/httpx/headers.py` & `CryptoLyzer-0.9.0/cryptolyzer/httpx/headers.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/httpx/client.py` & `CryptoLyzer-0.9.0/cryptolyzer/httpx/client.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/httpx/analyzer.py` & `CryptoLyzer-0.9.0/cryptolyzer/httpx/analyzer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/httpx/transfer.py` & `CryptoLyzer-0.9.0/cryptolyzer/httpx/transfer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/hassh/generate.py` & `CryptoLyzer-0.9.0/cryptolyzer/hassh/generate.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/curves.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/curves.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/result.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/result.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/prime.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/prime.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/dhparam.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/dhparam.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/utils.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import ipaddress
 import logging
 import socket
+import string
 import sys
 
 import six
 
 from cryptolyzer import __setup__
 from cryptolyzer.common.exception import NetworkError, NetworkErrorType
 
@@ -52,7 +53,21 @@
         raise NetworkError(NetworkErrorType.NO_ADDRESS)
 
     if not ip:
         family = addresses[0][0]
         ip = addresses[0][1]
 
     return family, ip
+
+
+def buffer_is_plain_text(buffer):
+    try:
+        return all(c in string.printable for c in buffer.decode('utf-8'))
+    except UnicodeDecodeError:
+        return False
+
+
+def buffer_flush(buffer, byte_num):
+    if byte_num is None:
+        byte_num = len(buffer)
+
+    return buffer[byte_num:]
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/application.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import abc
-import socket
 
 import attr
 
 from cryptodatahub.common.exception import InvalidValue
 
 from cryptoparser.common.exception import NotEnoughData, InvalidType
 
-from cryptolyzer.common.transfer import L7TransferBase, L4TransferBase, L4ServerTCP
+from cryptolyzer.common.exception import NetworkError
+from cryptolyzer.common.transfer import L4TransferBase, L7TransferBase, L4ServerTCP
 
 
 class L7ServerConfigurationBase(object):
     pass
 
 
 @attr.s
@@ -34,49 +34,55 @@
 
     @classmethod
     @abc.abstractmethod
     def get_default_port(cls):
         raise NotImplementedError()
 
     def _init_connection(self):
-        self.l4_transfer = L4ServerTCP(self.address, self.port, self.timeout, self.ip)
+        l4_transfer_class = self._get_transfer_class()
+        self.l4_transfer = l4_transfer_class(self.address, self.port, self.timeout, self.ip)
         self.l4_transfer.init_connection()
 
-    def _get_handshake_class(self, l4_transfer):
+    @classmethod
+    def _get_transfer_class(cls):
+        return L4ServerTCP
+
+    @abc.abstractmethod
+    def _get_handshake_class(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def _do_handshake(self, last_handshake_message_type):
         raise NotImplementedError()
 
     def _do_handshakes(self, last_handshake_message_type):
         client_messages = []
         actual_handshake_count = 0
         while True:
-            self.l4_transfer.close()
+            self.l4_transfer.close_client()
 
             if self.max_handshake_count is not None and actual_handshake_count >= self.max_handshake_count:
                 break
 
             try:
                 self.l4_transfer.accept()
-            except socket.timeout:
+            except NetworkError:
                 break
 
             actual_handshake_count += 1
             client_messages.append(self._do_handshake(last_handshake_message_type))
 
         self._close_connection()
 
         return client_messages
 
 
 @attr.s
 class L7ServerHandshakeBase(object):
-    l4_transfer = attr.ib(validator=attr.validators.instance_of(L4TransferBase))
+    l7_transfer = attr.ib(validator=attr.validators.instance_of(L7TransferBase))
     configuration = attr.ib(validator=attr.validators.instance_of(L7ServerConfigurationBase))
     _last_processed_message_type = attr.ib(init=False, default=None)
     client_messages = attr.ib(init=False, default={})
 
     def _init_connection(self, last_handshake_message_type):
         pass
 
@@ -108,29 +114,30 @@
         self._last_processed_message_type = None
 
         self._init_connection(last_handshake_message_type)
 
         while True:
             try:
                 try:
-                    record, is_handshake = self._parse_record()
+                    record, parsed_length, is_handshake = self._parse_record()
                     message = self._parse_message(record)
-                    self.l4_transfer.flush_buffer()
-                    receivable_byte_num = 0
                 except NotEnoughData as e:
                     receivable_byte_num = e.bytes_needed
                 except (InvalidType, InvalidValue):
                     self._process_invalid_message()
                 else:
+                    self.l7_transfer.flush_buffer(parsed_length)
+                    receivable_byte_num = 0
+
                     if is_handshake:
                         self._process_handshake_message(message, last_handshake_message_type)
                     else:
                         self._process_non_handshake_message(message)
 
                 try:
-                    self.l4_transfer.receive(receivable_byte_num)
+                    self.l7_transfer.receive(receivable_byte_num)
                 except NotEnoughData:
                     self._process_not_enough_data()
 
                 continue
             except StopIteration:
                 break
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/analyzer.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,12 +221,12 @@
 class AnalyzerHttpBase(object):
     @classmethod
     def get_clients(cls):
         return list(get_leaf_classes(L7ClientHttpBase))
 
     @classmethod
     def get_default_scheme(cls):
-        return 'http'
+        return 'https'
 
     @abc.abstractmethod
     def analyze(self, analyzable, protocol_version):
         raise NotImplementedError()
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/transfer.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/transfer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,99 @@
 # -*- coding: utf-8 -*-
 
 import abc
 import socket
-import string
 
 import ipaddress
 import attr
 import six
 
 from cryptoparser.common.exception import NotEnoughData
 from cryptoparser.common.utils import get_leaf_classes
 
 from cryptolyzer.common.exception import NetworkError, NetworkErrorType, SecurityError
-from cryptolyzer.common.utils import resolve_address
+from cryptolyzer.common.utils import buffer_flush, buffer_is_plain_text, resolve_address
 
 
 @attr.s
 class L4TransferBase(object):
     address = attr.ib(validator=attr.validators.instance_of(six.string_types))
     port = attr.ib(validator=attr.validators.instance_of(int))
     timeout = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of((int, float))))
     ip = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of((
         six.string_types, ipaddress.IPv4Address, ipaddress.IPv6Address
     ))))
+    _family = attr.ib(init=False)
+    _buffer = attr.ib(init=False)
     _socket = attr.ib(
-        init=False, default=None, validator=attr.validators.optional(attr.validators.instance_of(socket.socket))
+        init=False, default=None,
+        validator=attr.validators.optional(attr.validators.instance_of(socket.socket))
     )
-    _buffer = attr.ib(init=False, default=bytearray(), validator=attr.validators.instance_of(bytearray))
-    _family = attr.ib(init=False)
 
     def __attrs_post_init__(self):
         if self.timeout is None:
             self.timeout = self.get_default_timeout()
-        self._socket = None
-        self._buffer = bytearray()
         self._family, self.ip = resolve_address(self.address, self.port, self.ip)
+        self._buffer = bytearray()
+
+    def __del__(self):
+        self.close()
 
-    def _close(self):
+    @staticmethod
+    def _close_socket(sock):
         try:
-            self._socket.close()
-        except (socket.error, socket.timeout):
-            pass
+            sock.close()
+        except BaseException as e:  # pylint: disable=broad-except
+            if e.__class__.__name__ != 'TimeoutError' and not isinstance(e, (socket.error, socket.timeout)):
+                raise e
 
     def close(self):
         if self._socket is not None:
-            self._close()
+            self._close_socket(self._socket)
             self._socket = None
 
+    @abc.abstractmethod
     def _send(self, sendable_bytes):
-        return self._socket.send(sendable_bytes)
+        raise NotImplementedError()
 
     @property
     def buffer(self):
         return bytearray(self._buffer)
 
     def flush_buffer(self, byte_num=None):
-        if byte_num is None:
-            byte_num = len(self._buffer)
-
-        self._buffer = self._buffer[byte_num:]
+        self._buffer = buffer_flush(self._buffer, byte_num)
 
     @property
     def buffer_is_plain_text(self):
-        try:
-            return all(c in string.printable for c in self._buffer.decode('utf-8'))
-        except UnicodeDecodeError:
-            return False
+        return buffer_is_plain_text(self._buffer)
 
     def init_connection(self, _socket=None):
         self.close()
 
         if _socket:
             self._socket = _socket
             self.ip, self.port = _socket.getsockname()[0:2]
         else:
             self._init_connection()
 
-    @abc.abstractmethod
-    def _init_connection(self):
-        raise NotImplementedError()
-
-    @classmethod
-    @abc.abstractmethod
-    def get_default_timeout(cls):
-        raise NotImplementedError()
-
-
-@attr.s
-class L4TransferTCP(L4TransferBase):
     def send(self, sendable_bytes):
         total_sent_byte_num = 0
         while total_sent_byte_num < len(sendable_bytes):
             actual_sent_byte_num = self._send(sendable_bytes[total_sent_byte_num:])
             if actual_sent_byte_num == 0:
                 raise NetworkError(NetworkErrorType.NO_CONNECTION)
             total_sent_byte_num += actual_sent_byte_num
 
         return total_sent_byte_num
 
     def receive(self, receivable_byte_num, flags=0):
         total_received_byte_num = 0
         while total_received_byte_num < receivable_byte_num:
             try:
-                actual_received_bytes = self._socket.recv(
+                actual_received_bytes = self._receive_bytes(
                     min(receivable_byte_num - total_received_byte_num, 1024), flags
                 )
                 self._buffer += actual_received_bytes
                 total_received_byte_num += len(actual_received_bytes)
             except socket.error:
                 actual_received_bytes = None
 
@@ -132,67 +119,212 @@
     def receive_line(self, max_line_length=None):
         return self.receive_until(b'\n', max_line_length - 1 if max_line_length is not None else None)
 
     @abc.abstractmethod
     def _init_connection(self):
         raise NotImplementedError()
 
+    @staticmethod
+    def _receive_bytes_from_tcp_socket(sock, receivable_byte_num, flags):
+        if sock is None:
+            raise NotEnoughData(receivable_byte_num)
 
-class L4ClientTCP(L4TransferTCP):
+        return sock.recv(receivable_byte_num, flags)
+
+    @abc.abstractmethod
+    def _receive_bytes(self, receivable_byte_num, flags):
+        raise NotImplementedError()
+
+    @classmethod
+    @abc.abstractmethod
+    def get_default_timeout(cls):
+        raise NotImplementedError()
+
+
+@attr.s
+class L4ClientBase(L4TransferBase):
+    @abc.abstractmethod
     def _init_connection(self):
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def _receive_bytes(self, receivable_byte_num, flags):
+        raise NotImplementedError()
+
+    @classmethod
+    @abc.abstractmethod
+    def get_default_timeout(cls):
+        raise NotImplementedError()
+
+    def _send(self, sendable_bytes):
+        return self._socket.send(sendable_bytes)
+
+
+class L4ClientTCP(L4ClientBase):
+    def _init_connection(self):
+        self._buffer = bytearray()
         try:
             self._socket = socket.create_connection((str(self.ip), self.port), self.timeout)
         except BaseException as e:  # pylint: disable=broad-except
             if e.__class__.__name__ == 'ConnectionRefusedError' or isinstance(e, (socket.error, socket.timeout)):
                 six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
 
             raise e
 
+    def _receive_bytes(self, receivable_byte_num, flags):
+        return self._receive_bytes_from_tcp_socket(self._socket, receivable_byte_num, flags)
+
+    @classmethod
+    def get_default_timeout(cls):
+        return 5
+
+
+class L4ClientUDP(L4ClientBase):
+    def _init_connection(self):
+        self._buffer = bytearray()
+        self._socket = socket.socket(self._family, socket.SOCK_DGRAM)
+        self._socket.settimeout(self.timeout)
+        self._socket.connect((str(self.ip), self.port))
+
+    def _receive_bytes(self, receivable_byte_num, flags):
+        msg_bytes = bytearray(1)
+        msg_byte_num = self._socket.recv_into(msg_bytes, 1, flags=socket.MSG_PEEK | socket.MSG_TRUNC)
+
+        msg_bytes = bytearray(msg_byte_num)
+        self._socket.recv_into(msg_bytes, msg_byte_num, flags=flags)
+
+        return msg_bytes
+
     @classmethod
     def get_default_timeout(cls):
         return 5
 
 
 @attr.s
-class L4ServerTCP(L4TransferTCP):
+class L4ServerBase(L4TransferBase):
     backlog = attr.ib(default=1, validator=attr.validators.instance_of(int))
-    _server_socket = attr.ib(init=False, default=None)
-    bind_port = attr.ib(init=False, default=None)
+
+    @classmethod
+    @abc.abstractmethod
+    def _get_socket_type(cls):
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def close_client(self):
+        raise NotImplementedError()
 
     def __del__(self):
-        if self._server_socket is not None:
-            self._server_socket.close()
+        super(L4ServerBase, self).__del__()
+
+        if self._socket is not None:
+            self._close_socket(self._socket)
+
+    def close(self):
+        self.close_client()
 
     def _init_connection(self):
+        socket_type = self._get_socket_type()
         try:
-            self._server_socket = socket.socket(self._family, socket.SOCK_STREAM)
-            self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            self._server_socket.settimeout(self.timeout)
-            self._server_socket.bind((self.ip, self.port))
-            self._server_socket.listen(self.backlog)
+            self._socket = socket.socket(self._family, socket_type)
+            self._socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self._socket.settimeout(self.timeout)
+            self._socket.bind((str(self.address), self.port))
+            if socket_type == socket.SOCK_STREAM:
+                self._socket.listen(self.backlog)
         except KeyboardInterrupt as e:
             six.raise_from(NetworkError(NetworkErrorType.NO_RESPONSE), e)
         except OverflowError as e:
             six.raise_from(NetworkError(NetworkErrorType.NO_ADDRESS), e)
         except (OSError, socket.error) as e:
             six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
 
-        self.bind_port = self._server_socket.getsockname()[1]
+    @property
+    def bind_address(self):
+        return self._socket.getsockname()[0]
 
-    def accept(self):
-        self._socket, _ = self._server_socket.accept()
-        self._socket.settimeout(self.get_default_timeout())
-        self.flush_buffer()
+    @property
+    def bind_port(self):
+        return self._socket.getsockname()[1]
 
     @classmethod
     def get_default_timeout(cls):
         return 1
 
 
 @attr.s
+class L4ServerTCP(L4ServerBase):
+    _client_socket = attr.ib(
+        init=False, default=None, validator=attr.validators.optional(attr.validators.instance_of(socket.socket))
+    )
+
+    @classmethod
+    def _get_socket_type(cls):
+        return socket.SOCK_STREAM
+
+    def accept(self):
+        try:
+            self._client_socket, _ = self._socket.accept()
+        except BaseException as e:  # pylint: disable=broad-except
+            six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
+
+        self._client_socket.settimeout(self.get_default_timeout())
+        self.flush_buffer()
+
+    def _receive_bytes(self, receivable_byte_num, flags):
+        return self._receive_bytes_from_tcp_socket(self._client_socket, receivable_byte_num, flags)
+
+    def _send(self, sendable_bytes):
+        return self._client_socket.send(sendable_bytes)
+
+    def close_client(self):
+        if self._client_socket is not None:
+            self._client_socket.close()
+            self._client_socket = None
+
+
+@attr.s
+class L4ServerUDP(L4ServerBase):
+    _client_address = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of((
+        ipaddress.IPv4Address, ipaddress.IPv6Address
+    ))))
+    _client_port = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of(int)))
+
+    @classmethod
+    def _get_socket_type(cls):
+        return socket.SOCK_DGRAM
+
+    def accept(self):
+        pass
+
+    def _send(self, sendable_bytes):
+        return self._socket.sendto(sendable_bytes, (self._client_address, self._client_port))
+
+    def _receive_bytes(self, receivable_byte_num, flags):
+        msg_bytes = bytearray(1)
+        msg_byte_num = self._socket.recv_into(msg_bytes, 1, flags=socket.MSG_PEEK | socket.MSG_TRUNC)
+
+        msg_bytes, client_address = self._socket.recvfrom(msg_byte_num, flags)
+
+        if self._client_address is None:
+            self._client_address, self._client_port = client_address[0:2]
+        elif client_address[0:2] != (self._client_address, self._client_port):
+            raise NotImplementedError()
+
+        return msg_bytes
+
+    def close(self):
+        super(L4ServerUDP, self).close()
+
+        self._client_address = None
+
+    def close_client(self):
+        pass
+
+
+@attr.s
 class L7TransferBase(object):
     address = attr.ib(validator=attr.validators.instance_of(six.string_types))
     port = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of(int)))
     timeout = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of((float, int))))
     ip = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of((
         six.string_types, ipaddress.IPv4Address, ipaddress.IPv6Address
     ))))
@@ -212,14 +344,17 @@
 
     def send(self, sendable_bytes):
         return self.l4_transfer.send(sendable_bytes)
 
     def receive(self, receivable_byte_num):
         return self.l4_transfer.receive(receivable_byte_num)
 
+    def receive_line(self, max_line_length=None):
+        return self.l4_transfer.receive_line(max_line_length)
+
     def flush_buffer(self, byte_num=None):
         self.l4_transfer.flush_buffer(byte_num)
 
     @property
     def buffer(self):
         return self.l4_transfer.buffer
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/exception.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/exception.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/common/x509.py` & `CryptoLyzer-0.9.0/cryptolyzer/common/x509.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/ciphers.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/ciphers.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/dhparams.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/dhparams.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/all.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/all.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/pubkeys.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/pubkeys.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/server.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,21 +79,21 @@
         raise NotImplementedError()
 
     @classmethod
     @abc.abstractmethod
     def get_default_port(cls):
         raise NotImplementedError()
 
-    def _get_handshake_class(self, l4_transfer):
+    def _get_handshake_class(self):
         return SshServerHandshake
 
     def _do_handshake(self, last_handshake_message_type):
         try:
-            handshake_class = self._get_handshake_class(self.l4_transfer)
-            handshake_object = handshake_class(self.l4_transfer, self.configuration)
+            handshake_class = self._get_handshake_class()
+            handshake_object = handshake_class(self, self.configuration)
             handshake_object.do_handshake(last_handshake_message_type)
         finally:
             self.l4_transfer.close()
 
         return handshake_object.client_messages
 
     def do_ssh_handshake(self, last_handshake_message_type=SshMessageCode.KEXINIT):
@@ -116,25 +116,25 @@
             self.configuration.compression_algorithms_client_to_server,
             self.configuration.compression_algorithms_server_to_client,
             self.configuration.languages_client_to_server,
             self.configuration.languages_server_to_client,
         )
 
         return self.do_key_exchange_init(
-            transfer=self.l4_transfer,
+            transfer=self.l7_transfer,
             protocol_message=protocol_message,
             key_exchange_init_message=key_exchange_init_message,
             last_handshake_message_type=last_handshake_message_type
         )
 
     def _parse_record(self):
-        record = SshRecordInit.parse_exact_size(self.l4_transfer.buffer)
+        record = SshRecordInit.parse_exact_size(self.l7_transfer.buffer)
         is_handshake = record.packet.get_message_code() == SshMessageCode.KEXINIT
 
-        return record, is_handshake
+        return record, len(self.l7_transfer.buffer), is_handshake
 
     def _parse_message(self, record):
         return record.packet
 
     def _process_handshake_message(self, message, last_handshake_message_type):
         self._last_processed_message_type = message.get_message_code()
         self.client_messages[self._last_processed_message_type] = message
@@ -155,15 +155,15 @@
         kwargs = {
             'reason': reason,
             'description': description,
         }
         if language is not None:
             kwargs['language'] = language
 
-        self.l4_transfer.send(SshRecordInit(SshDisconnectMessage(**kwargs)).compose())
+        self.l7_transfer.send(SshRecordInit(SshDisconnectMessage(**kwargs)).compose())
 
 
 class L7ServerSsh(L7ServerSshBase):
     def __attrs_post_init__(self):
         if self.configuration is None:
             self.configuration = SshServerConfiguration()
```

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/client.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/client.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/analyzer.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/analyzer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/transfer.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/transfer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/cryptolyzer/ssh/versions.py` & `CryptoLyzer-0.9.0/cryptolyzer/ssh/versions.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/README.rst` & `CryptoLyzer-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.8.5/test/test_main.py` & `CryptoLyzer-0.9.0/test/test_main.py`

 * *Files identical despite different names*

