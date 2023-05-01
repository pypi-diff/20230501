# Comparing `tmp/burp-ui-agent-1.0.0.tar.gz` & `tmp/burp-ui-agent-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burp-ui-agent-1.0.0.tar", last modified: Sun Nov  6 20:58:49 2022, max compression
+gzip compressed data, was "burp-ui-agent-1.1.0.tar", last modified: Mon May  1 19:46:47 2023, max compression
```

## Comparing `burp-ui-agent-1.0.0.tar` & `burp-ui-agent-1.1.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.494587 burp-ui-agent-1.0.0/
--rw-r--r--   0 master    (1000) master    (1000)      152 2019-11-04 21:35:27.000000 burp-ui-agent-1.0.0/MANIFEST.in
--rw-r--r--   0 master    (1000) master    (1000)      776 2022-11-06 20:58:49.494587 burp-ui-agent-1.0.0/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)       44 2017-05-09 16:54:40.000000 burp-ui-agent-1.0.0/README
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.486587 burp-ui-agent-1.0.0/burp_ui_agent.egg-info/
--rw-r--r--   0 master    (1000) master    (1000)      776 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burp_ui_agent.egg-info/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)     1941 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burp_ui_agent.egg-info/SOURCES.txt
--rw-r--r--   0 master    (1000) master    (1000)        1 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burp_ui_agent.egg-info/dependency_links.txt
--rw-r--r--   0 master    (1000) master    (1000)       59 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burp_ui_agent.egg-info/entry_points.txt
--rw-r--r--   0 master    (1000) master    (1000)       74 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burp_ui_agent.egg-info/requires.txt
--rw-r--r--   0 master    (1000) master    (1000)       13 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burp_ui_agent.egg-info/top_level.txt
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.486587 burp-ui-agent-1.0.0/burpui_agent/
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/RELEASE
--rw-r--r--   0 master    (1000) master    (1000)        6 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/VERSION
--rw-r--r--   0 master    (1000) master    (1000)      278 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     2649 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/__main__.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.486587 burp-ui-agent-1.0.0/burpui_agent/__pycache__/
--rw-r--r--   0 master    (1000) master    (1000)      421 2021-05-14 20:26:36.000000 burp-ui-agent-1.0.0/burpui_agent/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 master    (1000) master    (1000)      429 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 master    (1000) master    (1000)      994 2021-05-14 20:26:36.000000 burp-ui-agent-1.0.0/burpui_agent/__pycache__/desc.cpython-36.pyc
--rw-r--r--   0 master    (1000) master    (1000)     1008 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/__pycache__/desc.cpython-39.pyc
--rw-r--r--   0 master    (1000) master    (1000)     2059 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/_compat.py
--rw-r--r--   0 master    (1000) master    (1000)     1202 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/_json.py
--rw-r--r--   0 master    (1000) master    (1000)    10045 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/config.py
--rw-r--r--   0 master    (1000) master    (1000)    23767 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/datastructures.py
--rw-r--r--   0 master    (1000) master    (1000)     2769 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/decorators.py
--rw-r--r--   0 master    (1000) master    (1000)      964 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/desc.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.486587 burp-ui-agent-1.0.0/burpui_agent/engines/
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/engines/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    14172 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/engines/agent.py
--rw-r--r--   0 master    (1000) master    (1000)      871 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/exceptions.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.486587 burp-ui-agent-1.0.0/burpui_agent/misc/
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/misc/__init__.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.490587 burp-ui-agent-1.0.0/burpui_agent/misc/backend/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.490587 burp-ui-agent-1.0.0/burpui_agent/misc/backend/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    47313 2021-10-06 15:22:17.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    30603 2021-10-06 15:22:17.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    41268 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    23473 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/multi.py
--rw-r--r--   0 master    (1000) master    (1000)    38355 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/parallel.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.490587 burp-ui-agent-1.0.0/burpui_agent/misc/backend/utils/
--rw-r--r--   0 master    (1000) master    (1000)        0 2019-11-04 21:35:27.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/utils/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    12736 2021-10-06 15:22:17.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/utils/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)      398 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/backend/utils/constant.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.490587 burp-ui-agent-1.0.0/burpui_agent/misc/parser/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.490587 burp-ui-agent-1.0.0/burpui_agent/misc/parser/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    37465 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    13883 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    43592 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/doc.py
--rw-r--r--   0 master    (1000) master    (1000)    17679 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/interface.py
--rw-r--r--   0 master    (1000) master    (1000)     8075 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/openssl.py
--rw-r--r--   0 master    (1000) master    (1000)    57168 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/burpui_agent/misc/parser/utils.py
--rw-r--r--   0 master    (1000) master    (1000)     2912 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/security.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.490587 burp-ui-agent-1.0.0/burpui_agent/tools/
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/tools/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     3289 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/tools/logging.py
--rw-r--r--   0 master    (1000) master    (1000)     8183 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/burpui_agent/utils.py
--rw-r--r--   0 master    (1000) master    (1000)       73 2022-11-06 20:58:49.000000 burp-ui-agent-1.0.0/requirements.txt
--rw-r--r--   0 master    (1000) master    (1000)       38 2022-11-06 20:58:49.494587 burp-ui-agent-1.0.0/setup.cfg
--rwxr-xr-x   0 master    (1000) master    (1000)     5429 2021-09-17 12:05:45.000000 burp-ui-agent-1.0.0/setup.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.482586 burp-ui-agent-1.0.0/share/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.482586 burp-ui-agent-1.0.0/share/burpui/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:58:49.490587 burp-ui-agent-1.0.0/share/burpui/etc/
--rw-r--r--   0 master    (1000) master    (1000)     2912 2019-11-04 21:35:27.000000 burp-ui-agent-1.0.0/share/burpui/etc/buiagent.sample.cfg
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/
+-rw-r--r--   0 master    (1000) master    (1000)      152 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/MANIFEST.in
+-rw-r--r--   0 master    (1000) master    (1000)      776 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)       44 2017-05-09 16:54:40.000000 burp-ui-agent-1.1.0/README
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.401666 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/
+-rw-r--r--   0 master    (1000) master    (1000)      776 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)     1941 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 master    (1000) master    (1000)        1 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 master    (1000) master    (1000)       59 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/entry_points.txt
+-rw-r--r--   0 master    (1000) master    (1000)       74 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/requires.txt
+-rw-r--r--   0 master    (1000) master    (1000)       13 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/top_level.txt
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.401666 burp-ui-agent-1.1.0/burpui_agent/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/RELEASE
+-rw-r--r--   0 master    (1000) master    (1000)        6 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/VERSION
+-rw-r--r--   0 master    (1000) master    (1000)      278 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     2648 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__main__.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/__pycache__/
+-rw-r--r--   0 master    (1000) master    (1000)      421 2021-05-14 20:26:36.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 master    (1000) master    (1000)      429 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 master    (1000) master    (1000)      994 2021-05-14 20:26:36.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-36.pyc
+-rw-r--r--   0 master    (1000) master    (1000)     1008 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-39.pyc
+-rw-r--r--   0 master    (1000) master    (1000)     2058 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/_compat.py
+-rw-r--r--   0 master    (1000) master    (1000)     1202 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/_json.py
+-rw-r--r--   0 master    (1000) master    (1000)    10045 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/config.py
+-rw-r--r--   0 master    (1000) master    (1000)    23767 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/datastructures.py
+-rw-r--r--   0 master    (1000) master    (1000)     2768 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/decorators.py
+-rw-r--r--   0 master    (1000) master    (1000)      964 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/desc.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/engines/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/engines/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    14171 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/engines/agent.py
+-rw-r--r--   0 master    (1000) master    (1000)      871 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/exceptions.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/misc/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/misc/__init__.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/misc/backend/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    47346 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    30620 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    41267 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    23472 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/multi.py
+-rw-r--r--   0 master    (1000) master    (1000)    38354 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/parallel.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    12735 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)      398 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/constant.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/parser/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    37464 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    13883 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    43592 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/doc.py
+-rw-r--r--   0 master    (1000) master    (1000)    17679 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)     8075 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/openssl.py
+-rw-r--r--   0 master    (1000) master    (1000)    57165 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/utils.py
+-rw-r--r--   0 master    (1000) master    (1000)     2913 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/security.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/tools/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/tools/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     3289 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/tools/logging.py
+-rw-r--r--   0 master    (1000) master    (1000)     8182 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/utils.py
+-rw-r--r--   0 master    (1000) master    (1000)       73 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/requirements.txt
+-rw-r--r--   0 master    (1000) master    (1000)       38 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/setup.cfg
+-rwxr-xr-x   0 master    (1000) master    (1000)     5429 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/setup.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.393665 burp-ui-agent-1.1.0/share/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.393665 burp-ui-agent-1.1.0/share/burpui/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/share/burpui/etc/
+-rw-r--r--   0 master    (1000) master    (1000)     2912 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/share/burpui/etc/buiagent.sample.cfg
```

### Comparing `burp-ui-agent-1.0.0/PKG-INFO` & `burp-ui-agent-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui-agent
-Version: 1.0.0
+Version: 1.1.0
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-agent-1.0.0/burp_ui_agent.egg-info/PKG-INFO` & `burp-ui-agent-1.1.0/burp_ui_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui-agent
-Version: 1.0.0
+Version: 1.1.0
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-agent-1.0.0/burp_ui_agent.egg-info/SOURCES.txt` & `burp-ui-agent-1.1.0/burp_ui_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/__main__.py` & `burp-ui-agent-1.1.0/burpui_agent/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 
 .. module:: burpui.__main__
     :platform: Unix
     :synopsis: Burp-UI main module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+import logging
 import os
 import sys
-import logging
-
 from argparse import ArgumentParser
 
 ROOT = os.path.dirname(os.path.realpath(__file__))
 # Try to load modules from our current env first
 sys.path.insert(0, os.path.join(ROOT, ".."))
 
 from burpui_agent.tools.logging import logger
@@ -59,15 +58,15 @@
         metavar="<FILE>",
     )
 
     options = parser.parse_args()
 
     if options.version:
         from burpui_agent import __title__
-        from burpui_agent.desc import __version__, __release__
+        from burpui_agent.desc import __release__, __version__
 
         ver = "{}: v{}".format(mname or __title__, __version__)
         if options.log:
             ver = "{} ({})".format(ver, __release__)
         print(ver)
         sys.exit(0)
 
@@ -80,17 +79,17 @@
     """
     options = parse_args()
     agent(options)
 
 
 def agent(options=None):
     import trio
+    from burpui_agent._compat import patch_json
     from burpui_agent.engines.agent import BUIAgent as Agent
     from burpui_agent.utils import lookup_file
-    from burpui_agent._compat import patch_json
 
     patch_json()
 
     if not options:
         options = parse_args(name="bui-agent")
 
     conf = ["buiagent.cfg", "buiagent.sample.cfg"]
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/__pycache__/desc.cpython-36.pyc` & `burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/__pycache__/desc.cpython-39.pyc` & `burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Nov  6 20:58:49 2022 UTC, .py size: 964 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0920 6863 c403 0000  a........ hc....
+00000000: 610d 0d0a 0000 0000 2717 5064 c403 0000  a.......'.Pd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6403 5a02 6404  Z.d.d.l.Z.d.Z.d.
 00000040: 5a03 6405 5a04 6406 5a05 6407 5a00 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a06 6409 5a07 6508 6501 6a09 a00a 6501  Z.d.Z.e.e.j...e.
 00000060: 6a09 a00b 6501 6a09 a00c 650d a101 a101  j...e.j...e.....
 00000070: 640a a102 8301 a00e a100 a00f a100 5a10  d.............Z.
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/_compat.py` & `burp-ui-agent-1.1.0/burpui_agent/_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
     :platform: Unix
     :synopsis: Burp-UI compatibility module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import pickle  # noqa
-
-from urllib.parse import unquote, quote, urlparse, urljoin  # noqa
+from urllib.parse import quote, unquote, urljoin, urlparse  # noqa
 
 text_type = str
 string_types = (str,)
 
 
 def to_bytes(text):
     """Transform string to bytes."""
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/_json.py` & `burp-ui-agent-1.1.0/burpui_agent/_json.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/config.py` & `burp-ui-agent-1.1.0/burpui_agent/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 .. module:: burpui.config
     :platform: Unix
     :synopsis: Burp-UI config module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import codecs
 import os
 import re
-import codecs
+
 import configobj
 import validate
 
 from .tools.logging import logger
 
 
 class BUIConfig(dict):
@@ -110,15 +111,14 @@
             with codecs.open(source, "r", "utf-8", errors="ignore") as config:
                 ori = [x.rstrip("\n") for x in config.readlines()]
             if ori:
                 with codecs.open(conffile, "w", "utf-8", errors="ignore") as config:
                     found = False
                     for line in ori:
                         if re.match(r"^\s*(#|;)+\s*\[{}\]".format(section), line):
-
                             config.write("[{}]\n".format(section))
                             found = True
                         else:
                             config.write("{}\n".format(line))
 
                     if not found:
                         config.write("[{}]\n".format(section))
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/datastructures.py` & `burp-ui-agent-1.1.0/burpui_agent/datastructures.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/decorators.py` & `burp-ui-agent-1.1.0/burpui_agent/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 .. module:: burpui.decorators
     :platform: Unix
     :synopsis: Burp-UI decorators module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import time
 import datetime
-
+import time
 from functools import wraps
 
 
 def browser_cache(expires=None):
     """Add Flask cache response headers based on expires in seconds.
 
     If expires is None, caching will be disabled.
@@ -26,21 +25,21 @@
         @app.route('/map')
         @browser_cache(expires=60)
         def index():
             return render_template('index.html')
 
     """
     from wsgiref.handlers import format_date_time
+
     from flask import g
     from flask_restx.utils import unpack
 
     def cache_decorator(view):
         @wraps(view)
         def cache_func(*args, **kwargs):
-
             resp, code, headers = unpack(view(*args, **kwargs))
             now = datetime.datetime.now()
 
             headers["Last-Modified"] = format_date_time(time.mktime(now.timetuple()))
 
             failure = code - 200 >= 100  # this is not a successful answer
             do_not_cache = getattr(g, "DONOTCACHE", False)
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/desc.py` & `burp-ui-agent-1.1.0/burpui_agent/desc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/engines/agent.py` & `burp-ui-agent-1.1.0/burpui_agent/engines/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 .. module:: burpui.engines.agent
     :platform: Unix
     :synopsis: Burp-UI agent module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import json
+import logging
 import os
+import ssl
 import struct
 import sys
-import ssl
-import json
-import logging
 import time
+from functools import partial
 
 import trio
 
-from functools import partial
-
-from ..exceptions import BUIserverException
-from ..misc.backend.interface import BUIbackend
 from .._compat import pickle, to_bytes, to_unicode
 from ..config import config
 from ..desc import __version__
+from ..exceptions import BUIserverException
+from ..misc.backend.interface import BUIbackend
 
 # TODO: sendfile is not yet supported by trio
 # try:
 #     from sendfile import sendfile
 #     USE_SENDFILE = True
 # except ImportError:
 #     USE_SENDFILE = False
@@ -265,16 +264,16 @@
                         os.unlink(path)
                         res = json.dumps(True)
                 else:
                     callback = getattr(self.client, j["func"])
                     if j["args"]:
                         if "pickled" in j and j["pickled"]:
                             # de-serialize arguments if needed
-                            import hmac
                             import hashlib
+                            import hmac
                             from base64 import b64decode
 
                             pickles = to_bytes(j["args"])
                             key = "{}{}".format(self.password, j["func"])
                             key = to_bytes(key)
                             bytes_pickles = pickles
                             digest = hmac.new(
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/exceptions.py` & `burp-ui-agent-1.1.0/burpui_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/.ropeproject/config.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/.ropeproject/globalnames` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/burp1.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 .. module:: burpui.misc.backend.burp1
     :platform: Unix
     :synopsis: Burp-UI burp1 backend module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import re
-import os
-import socket
-import time
 import datetime
 import json
+import os
+import re
 import shutil
+import socket
 import subprocess
 import tempfile
+import time
+from shlex import quote
 
-from .interface import BUIbackend
-from ..parser.burp1 import Parser
-from ...utils import human_readable as _hr, BUIcompress, utc_to_local
-from ...security import sanitize_string
+from ..._compat import to_bytes, to_unicode, unquote
 from ...exceptions import BUIserverException
-from ..._compat import unquote, to_unicode, to_bytes
-
-from shlex import quote
+from ...security import sanitize_string
+from ...utils import BUIcompress
+from ...utils import human_readable as _hr
+from ...utils import utc_to_local
+from ..parser.burp1 import Parser
+from .interface import BUIbackend
 
 
 class Burp(BUIbackend):
     """The :class:`burpui.misc.backend.burp1.Burp` class provides a consistent
     backend for ``burp-1`` servers.
 
     It implements the :class:`burpui.misc.backend.interface.BUIbackend` class
@@ -506,15 +507,15 @@
                 continue
             elif re.match(r"^-+$", line):
                 useful = True
                 continue
 
             found = False
             # this method is not optimal, but it is easy to read and to maintain
-            for (key, regex) in lookup_easy.items():
+            for key, regex in lookup_easy.items():
                 reg = re.search(regex, line)
                 if reg:
                     found = True
                     if key in ["start", "end"]:
                         backup[key] = int(
                             time.mktime(
                                 datetime.datetime.strptime(
@@ -522,15 +523,15 @@
                                 ).timetuple()
                             )
                         )
                     elif key == "duration":
                         tmp = reg.group(1).split(":")
                         tmp.reverse()
                         fields = [0] * 4
-                        for (i, val) in enumerate(tmp):
+                        for i, val in enumerate(tmp):
                             fields[i] = int(val)
                         seconds = 0
                         seconds += fields[0]
                         seconds += fields[1] * 60
                         seconds += fields[2] * (60 * 60)
                         seconds += fields[3] * (60 * 60 * 24)
                         backup[key] = seconds
@@ -539,15 +540,15 @@
                     # break the loop as soon as we find a match
                     break
 
             # if found is True, we already parsed the line so we can jump to the next one
             if found:
                 continue
 
-            for (key, regex) in lookup_complex.items():
+            for key, regex in lookup_complex.items():
                 reg = re.search(regex, line)
                 if reg:
                     # self.logger.debug("match[1]: '{0}'".format(reg.group(1)))
                     spl = re.split(r"\s+", reg.group(1))
                     if len(spl) < 5:
                         return {}
                     backup[key] = {
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/burp2.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp2.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 .. module:: burpui.misc.backend.burp2
     :platform: Unix
     :synopsis: Burp-UI burp2 backend module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import re
+import json
 import os
+import re
 import time
-import json
-
 from collections import OrderedDict
 
+from ..._compat import to_unicode
+from ...exceptions import BUIserverException
+from ...utils import human_readable as _hr
+from ...utils import utc_to_local
+from ..parser.burp2 import Parser
 from .burp1 import Burp as Burp1
 from .interface import BUIbackend
 from .utils.burp2 import Monitor
 from .utils.constant import BURP_REVERSE_COUNTERS, BURP_STATUS_FORMAT_V2
-from ..parser.burp2 import Parser
-from ...utils import human_readable as _hr, utc_to_local
-from ...exceptions import BUIserverException
-from ..._compat import to_unicode
 
 
 # Some functions are the same as in Burp1 backend
 class Burp(Burp1):
     """The :class:`burpui.misc.backend.burp2.Burp` class provides a consistent
     backend for ``burp-2`` servers.
 
@@ -297,15 +297,15 @@
             name = counter["name"]
             if name in translate:
                 name = translate[name]
             if counter["name"] in single:
                 result[name] = counter["count"]
             else:
                 result[name] = {}
-                for (key, val) in counts.items():
+                for key, val in counts.items():
                     if val in counter:
                         result[name][key] = counter[val]
                     else:
                         result[name][key] = 0
         if "start" in result and "end" in result:
             result["duration"] = result["end"] - result["start"]
             # convert utc timestamp to local
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/interface.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     :synopsis: Burp-UI backend interface.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import os
 import re
-
 from abc import ABCMeta, abstractmethod
 
 from ...tools.logging import logger
 
 G_BURPPORT = 4972
 G_BURPHOST = "::1"
 G_BURPBIN = "/usr/sbin/burp"
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/multi.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf8 -*-
-import re
-import socket
 import errno
 import json
+import re
+import socket
 import struct
 
 from werkzeug.datastructures import ImmutableMultiDict as _ImmutableMultiDict
 
-from .interface import BUIbackend
-from ..parser.interface import BUIparser
-from ...exceptions import BUIserverException
-from ..._compat import pickle, to_unicode, to_bytes
-from ...decorators import implement
+from ..._compat import pickle, to_bytes, to_unicode
 from ...datastructures import ImmutableMultiDict
-
+from ...decorators import implement
+from ...exceptions import BUIserverException
+from ..parser.interface import BUIparser
+from .interface import BUIbackend
 
 INTERFACE_METHODS = BUIbackend.__abstractmethods__
 PARSER_INTERFACE_METHODS = BUIparser.__abstractmethods__
 AGENT_VERSION_CAST = "0.4.9999"
 
 
 class ProxyCall(object):
@@ -552,16 +551,16 @@
         template=False,
         statictemplate=False,
         content="",
         agent=None,
     ):
         """See :func:`burpui.misc.backend.interface.BUIbackend.store_conf_cli`"""
         # serialize data as it is a nested dict
-        import hmac
         import hashlib
+        import hmac
         from base64 import b64encode
 
         if not isinstance(data, (_ImmutableMultiDict, ImmutableMultiDict)):
             msg = "Wrong data type"
             self.logger.warning(msg)
             raise BUIserverException(msg)
         vers = self._get_agent_version()
@@ -595,16 +594,16 @@
         }
         return json.loads(self.do_command(data))
 
     @implement
     def store_conf_srv(self, data, conf=None, agent=None):
         """See :func:`burpui.misc.backend.interface.BUIbackend.store_conf_srv`"""
         # serialize data as it is a nested dict
-        import hmac
         import hashlib
+        import hmac
         from base64 import b64encode
 
         if not isinstance(data, (_ImmutableMultiDict, ImmutableMultiDict)):
             msg = "Wrong data type"
             self.logger.warning(msg)
             raise BUIserverException(msg)
         vers = self._get_agent_version()
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/parallel.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 .. module:: burpui.misc.backend.parallel
     :platform: Unix
     :synopsis: Burp-UI parallel backend module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import json
 import os
 import re
-import json
 import ssl
-import time
-import trio
 import struct
-
+import time
 from asyncio import iscoroutinefunction
 from functools import partial
 
-from .burp2 import Burp as Burp2
-from .interface import BUIbackend, BUIBACKEND_INTERFACE_METHODS
-from .utils.constant import BURP_STATUS_FORMAT_V2
-from ..parser.burp2 import Parser
-from ...exceptions import BUIserverException
+import trio
+
+from ..._compat import to_bytes, to_unicode
 from ...decorators import implement, usetriorun
-from ...utils import utc_to_local
-from ..._compat import to_unicode, to_bytes
+from ...exceptions import BUIserverException
 from ...tools.logging import logger
+from ...utils import utc_to_local
+from ..parser.burp2 import Parser
+from .burp2 import Burp as Burp2
+from .interface import BUIBACKEND_INTERFACE_METHODS, BUIbackend
+from .utils.constant import BURP_STATUS_FORMAT_V2
 
 BUI_DEFAULTS = {
     "Parallel": {
         "host": "::1",
         "port": 11111,
         "ssl": True,
         "password": "password123456",
@@ -132,15 +132,14 @@
                 result = await self._do_process(data)
             self.connected = False
         else:
             result = await self._do_process(data)
         return result
 
     async def status(self, query, timeout=None, cache=True):
-
         request = {
             "query": query,
             "timeout": timeout,
             "cache": cache,
             "password": self.password,
         }
         request = json.dumps(request)
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/backend/utils/burp2.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/burp2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 .. module:: burpui.misc.backend.utils.burp2
     :platform: Unix
     :synopsis: Burp-UI burp utils module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import datetime
+import json
 import re
 import subprocess
-import json
-import datetime
-
 from select import select
 
 from ...._compat import to_bytes, to_unicode
 from ....exceptions import BUIserverException
 from ....security import sanitize_string
 from ....tools.logging import logger
 from .constant import (
     BURP_LIST_BATCH,
     BURP_MINIMAL_VERSION,
-    BURP_STATUS_FORMAT_V2,
     BURP_STATUS_DELIMITER,
+    BURP_STATUS_FORMAT_V2,
 )
 
 
 class Monitor(object):
     """The :class:`burpui.misc.backend.utils.burp2.Monitor` class provides a ``burp-2``
     Monitor object to interact with the server.
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/parser/.ropeproject/config.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/parser/burp1.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # -*- coding: utf8 -*-
 """
 .. module:: burpui.misc.parser.burp1
     :platform: Unix
     :synopsis: Burp-UI configuration file parser for Burp1.
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
-import re
-import os
-import json
 import codecs
+import json
+import os
+import re
 import shutil
-
 from glob import glob
 
-from .doc import Doc
-from .utils import Config
-from .openssl import OSSLConf, OSSLAuth
 from ...exceptions import BUIserverException
 from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN
+from .doc import Doc
+from .openssl import OSSLAuth, OSSLConf
+from .utils import Config
 
 
 class Parser(Doc):
     """:class:`burpui.misc.parser.burp1.Parser` provides a consistent interface
     to parse burp configuration files.
 
     It implements :class:`burpui.misc.parser.interface.BUIparser`.
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/parser/burp2.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf8 -*-
 """
 .. module:: burpui.misc.parser.burp2
     :platform: Unix
     :synopsis: Burp-UI configuration file parser for Burp2.
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+from ..backend.utils.constant import BURP_BIND_MULTIPLE, BURP_LISTEN_OPTION
 from .burp1 import Parser as Burp1
-from ..backend.utils.constant import BURP_LISTEN_OPTION, BURP_BIND_MULTIPLE
 
 
 def __(string):
     """dummy function to fake the translation"""
     return string
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/parser/doc.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/parser/doc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/parser/interface.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/parser/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/parser/openssl.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/parser/openssl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf8 -*-
 """
 .. module:: burpui.misc.parser.openssl
     :platform: Unix
     :synopsis: Burp-UI configuration file parser OpenSSL configuration.
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+import codecs
 import os
 import re
-import codecs
 import subprocess
-
 from hashlib import md5
+
 from OpenSSL import crypto
 
 from ...tools.logging import logger
 
 
 class OSSLAuth(object):
     """OpenSSL wrapper"""
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/misc/parser/utils.py` & `burp-ui-agent-1.1.0/burpui_agent/misc/parser/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 """
 .. module:: burpui.misc.parser.utils
     :platform: Unix
     :synopsis: Burp-UI configuration file parser utilities.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+import codecs
 import os
 import re
-import codecs
 import shutil
-
-from copy import copy
-from hashlib import md5
 from collections import OrderedDict
+from copy import copy
 from glob import glob
+from hashlib import md5
 
-from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN
-from ...security import sanitize_string
 from ...datastructures import MultiDict
-
+from ...security import sanitize_string
+from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN
 
 RESET_IDENTIFIER = "_reset_bui_CUSTOM"
 BEGIN_TEMPLATES = "BURP-UI TEMPLATES"
 END_TEMPLATES = "END TEMPLATES"
 
 
 class Option(object):
@@ -1510,15 +1508,14 @@
     def changed(self):
         for path, conf in self.files.items():
             if conf.changed:
                 return True
         return False
 
     def _parse(self):
-
         orig = self.files.copy()
         for root, conf in orig.items():
             conf.parse()
             for key, val in conf.flatten("include", False).items():
                 for path in val:
                     if not os.path.isabs(path):
                         path = os.path.join(os.path.dirname(root), path)
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/security.py` & `burp-ui-agent-1.1.0/burpui_agent/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. module:: burpui.security
     :platform: Unix
     :synopsis: Burp-UI security module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from ._compat import to_unicode, urlparse, urljoin
+from ._compat import to_unicode, urljoin, urlparse
 
 
 def sanitize_string(string, strict=True, paranoid=False):
     """Return a 'safe' version of the string (ie. remove malicious chars like
     '\n')
 
     :param string: String to escape
@@ -41,24 +41,25 @@
     :type app: :class:`burpui.engines.server.BUIServer`
     """
     if app.auth != "none":
         if request.headers.get("X-From-UI", False):
             return None
         auth = request.authorization
         if auth:
-            from flask import session, g
+            from flask import g, session
 
             app.logger.debug("Found Basic user: {}".format(auth.username))
             refresh = True
             if "login" in session and session["login"] == auth.username:
                 refresh = False
             session["language"] = request.headers.get("X-Language", "en")
             user = app.uhandler.user(auth.username, refresh)
             if user and user.active and user.login(auth.password):
                 from flask_login import login_user
+
                 from .sessions import session_manager
 
                 if "login" in session and session["login"] != auth.username:
                     session.clear()
                     session["login"] = auth.username
                     session["language"] = request.headers.get("X-Language", "en")
                 login_user(user)
```

### Comparing `burp-ui-agent-1.0.0/burpui_agent/tools/logging.py` & `burp-ui-agent-1.1.0/burpui_agent/tools/logging.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.0.0/burpui_agent/utils.py` & `burp-ui-agent-1.1.0/burpui_agent/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 .. module:: burpui.utils
     :platform: Unix
     :synopsis: Burp-UI utils module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import os
+import datetime
 import math
+import os
 import string
 import sys
-import datetime
-import zipfile
 import tarfile
-
+import zipfile
 from uuid import UUID
 
 NOTIF_OK = 0
 NOTIF_WARN = 1
 NOTIF_ERROR = 2
 NOTIF_INFO = 3
```

### Comparing `burp-ui-agent-1.0.0/setup.py` & `burp-ui-agent-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import os
 import re
-import sys
 import shutil
 import subprocess
+import sys
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 # only used to build the package
 CWD = os.path.dirname(os.path.realpath(__file__))
 ROOT = os.path.join(os.path.dirname(os.path.realpath(__file__)), "..", "..")
 
 raw_requirements = [
     "trio",
@@ -122,17 +122,17 @@
 """
 
 from burpui_agent import __title__
 from burpui_agent.desc import (
     __author__,
     __author_email__,
     __description__,
+    __license__,
     __url__,
     __version__,
-    __license__,
 )
 
 name = __title__
 author = __author__
 author_email = __author_email__
 description = __description__
 url = __url__
```

### Comparing `burp-ui-agent-1.0.0/share/burpui/etc/buiagent.sample.cfg` & `burp-ui-agent-1.1.0/share/burpui/etc/buiagent.sample.cfg`

 * *Files identical despite different names*

