# Comparing `tmp/viso-sdk-python-0.0.5.tar.gz` & `tmp/viso-sdk-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viso-sdk-python-0.0.5.tar", last modified: Tue Apr 18 22:38:13 2023, max compression
+gzip compressed data, was "viso-sdk-python-0.0.6.tar", last modified: Mon May  1 20:21:51 2023, max compression
```

## Comparing `viso-sdk-python-0.0.5.tar` & `viso-sdk-python-0.0.6.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.026826 viso-sdk-python-0.0.5/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1311 2023-04-18 22:38:13.026826 viso-sdk-python-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.993823 viso-sdk-python-0.0.5/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7128 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.994823 viso-sdk-python-0.0.5/docs/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/ext/docstrings.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/ext/manager_tmpl.j2
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/viso.rst
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-docker.txt
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-docs.txt
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-lint.txt
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-18 22:38:13.027826 viso-sdk-python-0.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2531 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.996823 viso-sdk-python-0.0.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.996823 viso-sdk-python-0.0.5/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)     3314 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/fixtures/flow.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.997823 viso-sdk-python-0.0.5/tests/meta/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/meta/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/meta/test_ensure_type_hints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.997823 viso-sdk-python-0.0.5/tests/smoke/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/smoke/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/smoke/test_dists.py
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/test_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/test_status.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.002824 viso-sdk-python-0.0.5/viso_sdk/
--rw-r--r--   0 root         (0) root         (0)   128282 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138995 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/_version.c
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.007825 viso-sdk-python-0.0.5/viso_sdk/constants/
--rw-r--r--   0 root         (0) root         (0)   134253 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168423 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/constants.c
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/constants.py
--rw-r--r--   0 root         (0) root         (0)   122038 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/modules.c
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/modules.py
--rw-r--r--   0 root         (0) root         (0)   219738 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/variables.c
--rw-rw-rw-   0 root         (0) root         (0)     1502 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.009825 viso-sdk-python-0.0.5/viso_sdk/edge/
--rw-r--r--   0 root         (0) root         (0)   108989 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/edge/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/edge/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312878 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/edge/common.c
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/edge/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.013825 viso-sdk-python-0.0.5/viso_sdk/logging/
--rw-r--r--   0 root         (0) root         (0)   114597 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/logging/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)   275645 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/logging/logger.c
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/logging/logger.py
--rw-r--r--   0 root         (0) root         (0)   356104 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.c
--rw-rw-rw-   0 root         (0) root         (0)     4603 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.015825 viso-sdk-python-0.0.5/viso_sdk/mqtt/
--rw-r--r--   0 root         (0) root         (0)   113135 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/__init__.py
--rw-r--r--   0 root         (0) root         (0)   353758 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.c
--rw-rw-rw-   0 root         (0) root         (0)     3802 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.017825 viso-sdk-python-0.0.5/viso_sdk/nodered/
--rw-r--r--   0 root         (0) root         (0)   113205 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/__init__.py
--rw-r--r--   0 root         (0) root         (0)   377549 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/flow.c
--rw-rw-rw-   0 root         (0) root         (0)     5613 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.019826 viso-sdk-python-0.0.5/viso_sdk/redis/
--rw-r--r--   0 root         (0) root         (0)   113197 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/redis/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)   387846 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.c
--rw-rw-rw-   0 root         (0) root         (0)     4636 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.024826 viso-sdk-python-0.0.5/viso_sdk/visualize/
--rw-r--r--   0 root         (0) root         (0)   113212 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)   244344 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.c
--rw-rw-rw-   0 root         (0) root         (0)     2861 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.py
--rw-r--r--   0 root         (0) root         (0)   378258 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/palette.c
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/palette.py
--rw-r--r--   0 root         (0) root         (0)   472190 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.c
--rw-rw-rw-   0 root         (0) root         (0)     7621 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.026826 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1311 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.340527 viso-sdk-python-0.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-05-01 20:21:51.340527 viso-sdk-python-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.316525 viso-sdk-python-0.0.6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7128 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.317525 viso-sdk-python-0.0.6/docs/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/ext/docstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/ext/manager_tmpl.j2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/docs/viso.rst
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/requirements-docker.txt
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/requirements-docs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/requirements-lint.txt
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-01 20:21:51.341527 viso-sdk-python-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.318525 viso-sdk-python-0.0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.318525 viso-sdk-python-0.0.6/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/fixtures/flow.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.319525 viso-sdk-python-0.0.6/tests/meta/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/meta/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/meta/test_ensure_type_hints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.319525 viso-sdk-python-0.0.6/tests/smoke/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/smoke/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/smoke/test_dists.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/test_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tests/test_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.321525 viso-sdk-python-0.0.6/viso_sdk/
+-rw-r--r--   0 root         (0) root         (0)   128282 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138995 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/_version.c
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.324525 viso-sdk-python-0.0.6/viso_sdk/constants/
+-rw-r--r--   0 root         (0) root         (0)   134253 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/constants/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/constants/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168423 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/constants/constants.c
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/constants/constants.py
+-rw-r--r--   0 root         (0) root         (0)   122038 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/constants/modules.c
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/constants/modules.py
+-rw-r--r--   0 root         (0) root         (0)   219738 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/constants/variables.c
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/constants/variables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.326526 viso-sdk-python-0.0.6/viso_sdk/edge/
+-rw-r--r--   0 root         (0) root         (0)   108989 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/edge/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/edge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312878 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/edge/common.c
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/edge/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.329526 viso-sdk-python-0.0.6/viso_sdk/logging/
+-rw-r--r--   0 root         (0) root         (0)   114597 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/logging/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   275645 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/logging/logger.c
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/logging/logger.py
+-rw-r--r--   0 root         (0) root         (0)   356104 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/logging/status_logger.c
+-rw-rw-rw-   0 root         (0) root         (0)     4603 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/logging/status_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.331526 viso-sdk-python-0.0.6/viso_sdk/mqtt/
+-rw-r--r--   0 root         (0) root         (0)   113135 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/mqtt/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/mqtt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   353758 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/mqtt/mqtt_wrapper.c
+-rw-rw-rw-   0 root         (0) root         (0)     3802 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/mqtt/mqtt_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.333526 viso-sdk-python-0.0.6/viso_sdk/nodered/
+-rw-r--r--   0 root         (0) root         (0)   113205 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/nodered/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/nodered/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   377549 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/nodered/flow.c
+-rw-rw-rw-   0 root         (0) root         (0)     5613 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/nodered/flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.335526 viso-sdk-python-0.0.6/viso_sdk/redis/
+-rw-r--r--   0 root         (0) root         (0)   113197 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/redis/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   387846 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/redis/redis_wrapper.c
+-rw-rw-rw-   0 root         (0) root         (0)     4636 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/redis/redis_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.339527 viso-sdk-python-0.0.6/viso_sdk/visualize/
+-rw-r--r--   0 root         (0) root         (0)   113212 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   244344 2023-05-01 20:21:50.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/custom_font.c
+-rw-rw-rw-   0 root         (0) root         (0)     2861 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/custom_font.py
+-rw-r--r--   0 root         (0) root         (0)   378258 2023-05-01 20:21:51.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/palette.c
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/palette.py
+-rw-r--r--   0 root         (0) root         (0)   472190 2023-05-01 20:21:51.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/visualization.c
+-rw-rw-rw-   0 root         (0) root         (0)     7621 2023-05-01 20:21:37.000000 viso-sdk-python-0.0.6/viso_sdk/visualize/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:21:51.340527 viso-sdk-python-0.0.6/viso_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-05-01 20:21:51.000000 viso-sdk-python-0.0.6/viso_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-01 20:21:51.000000 viso-sdk-python-0.0.6/viso_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:21:51.000000 viso-sdk-python-0.0.6/viso_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-01 20:21:51.000000 viso-sdk-python-0.0.6/viso_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-01 20:21:51.000000 viso-sdk-python-0.0.6/viso_sdk_python.egg-info/top_level.txt
```

### Comparing `viso-sdk-python-0.0.5/COPYING` & `viso-sdk-python-0.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/PKG-INFO` & `viso-sdk-python-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viso-sdk-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: VisoSDK: A Python SDK for use in Viso containers
 Home-page: https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git
 Author: support@viso.ai
 Author-email: support@viso.ai
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `viso-sdk-python-0.0.5/docs/Makefile` & `viso-sdk-python-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/docs/conf.py` & `viso-sdk-python-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/docs/ext/docstrings.py` & `viso-sdk-python-0.0.6/docs/ext/docstrings.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/docs/ext/manager_tmpl.j2` & `viso-sdk-python-0.0.6/docs/ext/manager_tmpl.j2`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/docs/make.bat` & `viso-sdk-python-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/docs/viso.rst` & `viso-sdk-python-0.0.6/docs/viso.rst`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/setup.py` & `viso-sdk-python-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/tests/fixtures/flow.json` & `viso-sdk-python-0.0.6/tests/fixtures/flow.json`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/tests/meta/test_ensure_type_hints.py` & `viso-sdk-python-0.0.6/tests/meta/test_ensure_type_hints.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/tests/smoke/test_dists.py` & `viso-sdk-python-0.0.6/tests/smoke/test_dists.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/tests/test_flow.py` & `viso-sdk-python-0.0.6/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/tests/test_status.py` & `viso-sdk-python-0.0.6/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/tox.ini` & `viso-sdk-python-0.0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/__init__.py` & `viso-sdk-python-0.0.6/viso_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/_version.c` & `viso-sdk-python-0.0.6/viso_sdk/_version.c`

 * *Files 0% similar despite different names*

```diff
@@ -1289,15 +1289,15 @@
 static const char __pyx_k_now[] = "now";
 static const char __pyx_k_file[] = "__file__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_path[] = "path";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_year[] = "year";
-static const char __pyx_k_0_0_5[] = "0.0.5";
+static const char __pyx_k_0_0_6[] = "0.0.6";
 static const char __pyx_k_LGPL3[] = "LGPL3";
 static const char __pyx_k_email[] = "__email__";
 static const char __pyx_k_title[] = "__title__";
 static const char __pyx_k_author[] = "__author__";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_abspath[] = "abspath";
 static const char __pyx_k_cur_dir[] = "_cur_dir";
@@ -1309,15 +1309,15 @@
 static const char __pyx_k_Viso_ai_team[] = "Viso.ai team";
 static const char __pyx_k_Constant_file[] = "\n    Constant file\n";
 static const char __pyx_k_Copyright_2020[] = "Copyright 2020-";
 static const char __pyx_k_viso_sdk_python[] = "viso-sdk-python";
 static const char __pyx_k_s_carlyon_viso_ai[] = "s.carlyon@viso.ai";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_viso_ai_AG_info_viso_ai[] = " viso.ai AG <info@viso.ai>";
-static PyObject *__pyx_kp_u_0_0_5;
+static PyObject *__pyx_kp_u_0_0_6;
 static PyObject *__pyx_kp_u_Copyright_2020;
 static PyObject *__pyx_n_u_LGPL3;
 static PyObject *__pyx_kp_u_Viso_ai_team;
 static PyObject *__pyx_n_s_abspath;
 static PyObject *__pyx_n_s_author;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_copyright;
@@ -1384,15 +1384,15 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_0_0_5, __pyx_k_0_0_5, sizeof(__pyx_k_0_0_5), 0, 1, 0, 0},
+  {&__pyx_kp_u_0_0_6, __pyx_k_0_0_6, sizeof(__pyx_k_0_0_6), 0, 1, 0, 0},
   {&__pyx_kp_u_Copyright_2020, __pyx_k_Copyright_2020, sizeof(__pyx_k_Copyright_2020), 0, 1, 0, 0},
   {&__pyx_n_u_LGPL3, __pyx_k_LGPL3, sizeof(__pyx_k_LGPL3), 0, 1, 0, 1},
   {&__pyx_kp_u_Viso_ai_team, __pyx_k_Viso_ai_team, sizeof(__pyx_k_Viso_ai_team), 0, 1, 0, 0},
   {&__pyx_n_s_abspath, __pyx_k_abspath, sizeof(__pyx_k_abspath), 0, 0, 1, 1},
   {&__pyx_n_s_author, __pyx_k_author, sizeof(__pyx_k_author), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_copyright, __pyx_k_copyright, sizeof(__pyx_k_copyright), 0, 0, 1, 1},
@@ -1870,24 +1870,24 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_license, __pyx_n_u_LGPL3) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":15
  * __email__ = "s.carlyon@viso.ai"
  * __license__ = "LGPL3"
  * __title__ = "viso-sdk-python"             # <<<<<<<<<<<<<<
  * 
- * __version__ = "0.0.5"
+ * __version__ = "0.0.6"
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_title, __pyx_kp_u_viso_sdk_python) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":17
  * __title__ = "viso-sdk-python"
  * 
- * __version__ = "0.0.5"             # <<<<<<<<<<<<<<
+ * __version__ = "0.0.6"             # <<<<<<<<<<<<<<
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_0_5) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_0_6) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":1
  * """             # <<<<<<<<<<<<<<
  *     Constant file
  * """
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
```

### Comparing `viso-sdk-python-0.0.5/viso_sdk/constants/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/constants/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/constants/constants.c` & `viso-sdk-python-0.0.6/viso_sdk/constants/constants.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/constants/constants.py` & `viso-sdk-python-0.0.6/viso_sdk/constants/constants.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/constants/modules.c` & `viso-sdk-python-0.0.6/viso_sdk/constants/modules.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/constants/variables.c` & `viso-sdk-python-0.0.6/viso_sdk/constants/variables.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/constants/variables.py` & `viso-sdk-python-0.0.6/viso_sdk/constants/variables.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/edge/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/edge/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/edge/common.c` & `viso-sdk-python-0.0.6/viso_sdk/edge/common.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/edge/common.py` & `viso-sdk-python-0.0.6/viso_sdk/edge/common.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/logging/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/logging/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/logging/logger.c` & `viso-sdk-python-0.0.6/viso_sdk/logging/logger.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/logging/logger.py` & `viso-sdk-python-0.0.6/viso_sdk/logging/logger.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.c` & `viso-sdk-python-0.0.6/viso_sdk/logging/status_logger.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.py` & `viso-sdk-python-0.0.6/viso_sdk/logging/status_logger.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/mqtt/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/mqtt/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.c` & `viso-sdk-python-0.0.6/viso_sdk/mqtt/mqtt_wrapper.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.py` & `viso-sdk-python-0.0.6/viso_sdk/mqtt/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/nodered/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/nodered/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/nodered/flow.c` & `viso-sdk-python-0.0.6/viso_sdk/nodered/flow.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/nodered/flow.py` & `viso-sdk-python-0.0.6/viso_sdk/nodered/flow.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/redis/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/redis/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.c` & `viso-sdk-python-0.0.6/viso_sdk/redis/redis_wrapper.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.py` & `viso-sdk-python-0.0.6/viso_sdk/redis/redis_wrapper.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/visualize/__init__.c` & `viso-sdk-python-0.0.6/viso_sdk/visualize/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.c` & `viso-sdk-python-0.0.6/viso_sdk/visualize/custom_font.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.py` & `viso-sdk-python-0.0.6/viso_sdk/visualize/custom_font.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/visualize/palette.c` & `viso-sdk-python-0.0.6/viso_sdk/visualize/palette.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/visualize/palette.py` & `viso-sdk-python-0.0.6/viso_sdk/visualize/palette.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.c` & `viso-sdk-python-0.0.6/viso_sdk/visualize/visualization.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.py` & `viso-sdk-python-0.0.6/viso_sdk/visualize/visualization.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.5/viso_sdk_python.egg-info/PKG-INFO` & `viso-sdk-python-0.0.6/viso_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viso-sdk-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: VisoSDK: A Python SDK for use in Viso containers
 Home-page: https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git
 Author: support@viso.ai
 Author-email: support@viso.ai
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `viso-sdk-python-0.0.5/viso_sdk_python.egg-info/SOURCES.txt` & `viso-sdk-python-0.0.6/viso_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

