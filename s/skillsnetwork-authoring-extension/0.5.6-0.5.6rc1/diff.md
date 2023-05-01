# Comparing `tmp/skillsnetwork-authoring-extension-0.5.6.tar.gz` & `tmp/skillsnetwork-authoring-extension-0.5.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillsnetwork-authoring-extension-0.5.6.tar", last modified: Mon May  1 21:05:18 2023, max compression
+gzip compressed data, was "skillsnetwork-authoring-extension-0.5.6rc1.tar", last modified: Wed Apr 19 14:41:47 2023, max compression
```

## Comparing `skillsnetwork-authoring-extension-0.5.6.tar` & `skillsnetwork-authoring-extension-0.5.6rc1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.299780 skillsnetwork-authoring-extension-0.5.6/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.303780 skillsnetwork-authoring-extension-0.5.6/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.303780 skillsnetwork-authoring-extension-0.5.6/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/jupyter-config/server-config/skillsnetwork_authoring_extension.json
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:05:18.311780 skillsnetwork-authoring-extension-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.303780 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.303780 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-01 21:05:18.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-05-01 21:05:17.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/568.3e8305ffaf486d3cc564.js
--rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-05-01 21:05:17.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-01 21:05:17.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-01 21:05:17.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1175c035aa1c7085eb76.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 21:05:15.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-01 21:05:17.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-01 21:05:18.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 21:05:18.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:05:18.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:04:26.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 21:05:18.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 21:05:18.000000 skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/src/button/
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/button/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/button/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/config.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/dialog.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/src/menu/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/menu/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/sn-file-library.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/src/tools.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:05:18.307780 skillsnetwork-authoring-extension-0.5.6/style/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-01 21:03:49.000000 skillsnetwork-authoring-extension-0.5.6/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   218508 2023-05-01 21:05:01.000000 skillsnetwork-authoring-extension-0.5.6/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.738331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/server-config/skillsnetwork_authoring_extension.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-19 14:40:32.000000 skillsnetwork-authoring-extension-0.5.6rc1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 14:41:45.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:41:04.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/src/button/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/button/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/button/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/dialog.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/src/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/menu/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/sn-file-library.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/tools.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218440 2023-04-19 14:41:34.000000 skillsnetwork-authoring-extension-0.5.6rc1/yarn.lock
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/LICENSE` & `skillsnetwork-authoring-extension-0.5.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.6rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.6
+Version: 0.5.6rc1
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/README.md` & `skillsnetwork-authoring-extension-0.5.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/RELEASE.md` & `skillsnetwork-authoring-extension-0.5.6rc1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/package.json` & `skillsnetwork-authoring-extension-0.5.6rc1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.5.6-rc1'"}*

```diff
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.6"
+    "version": "0.5.6-rc1"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/pyproject.toml` & `skillsnetwork-authoring-extension-0.5.6rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/setup.py` & `skillsnetwork-authoring-extension-0.5.6rc1/setup.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/__init__.py` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/_version.py` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/_version.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/handlers.py` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/package.json` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1ebb17cfc896e2585599.js'}}",*

 * * "'version'": "'0.5.6-rc1'"}*

```diff
@@ -54,15 +54,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1175c035aa1c7085eb76.js",
+            "load": "static/remoteEntry.1ebb17cfc896e2585599.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "skillsnetwork-authoring-extension/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.6"
+    "version": "0.5.6-rc1"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/568.3e8305ffaf486d3cc564.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -38,17 +38,17 @@
                                             type: "application/x-ipynb+json"
                                         }),
                                         a = URL.createObjectURL(n),
                                         l = document.createElement("a");
                                     l.setAttribute("download", e.path), l.setAttribute("href", a), document.body.appendChild(l), l.click(), document.body.removeChild(l), URL.revokeObjectURL(a)
                                 }, a = new l.ToolbarButton({
                                     className: "download-lab-button",
-                                    label: "Download Notebook",
+                                    label: "Download",
                                     onClick: n,
-                                    tooltip: "Download the current notebook ipynb file to your local system"
+                                    tooltip: "Download Lab"
                                 }), s = new l.ToolbarButton({
                                     className: "publish-lab-button",
                                     label: "Publish on SN",
                                     onClick: o,
                                     tooltip: "Publish Lab"
                                 }), u = new l.ToolbarButton({
                                     className: "sn-file-library-button",
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1175c035aa1c7085eb76.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, m, b, g, y, w, k, _, S = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b, m, g, y, w, k, _ = {
             5367: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(1568))),
                         "./extension": () => t.e(568).then((() => () => t(1568))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -21,28 +21,28 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        x = {};
+        S = {};
 
-    function E(e) {
-        var r = x[e];
+    function x(e) {
+        var r = S[e];
         if (void 0 !== r) return r.exports;
-        var t = x[e] = {
+        var t = S[e] = {
             id: e,
             exports: {}
         };
-        return S[e](t, t.exports, E), t.exports
+        return _[e](t, t.exports, x), t.exports
     }
-    E.m = S, E.c = x, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
+    x.m = _, x.c = S, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
         e && !e.d && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
-    }, E.a = (o, a, i) => {
+    }, x.a = (o, a, i) => {
         var u;
         i && ((u = []).d = 1);
         var l, s, f, d = new Set,
             p = o.exports,
             c = new Promise(((e, r) => {
                 f = r, s = e
             }));
@@ -72,105 +72,104 @@
                 s = new Promise((r => {
                     (a = () => r(i)).r = 0;
                     var t = e => e !== u && !d.has(e) && (d.add(e), e && !e.d && (a.r++, e.push(a)));
                     l.map((r => r[e](t)))
                 }));
             return a.r ? s : i()
         }), (e => (e ? f(c[t] = e) : s(p), n(u)))), u && (u.d = 0)
-    }, E.n = e => {
+    }, x.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return E.d(r, {
+        return x.d(r, {
             a: r
         }), r
-    }, E.d = (e, r) => {
-        for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
+    }, x.d = (e, r) => {
+        for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        568: "3e8305ffaf486d3cc564",
+    }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
+        568: "d23144daea3f495050cb",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
     } [e] + ".js?v=" + {
-        568: "3e8305ffaf486d3cc564",
+        568: "d23144daea3f495050cb",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
-    } [e], E.g = function() {
+    } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork-authoring-extension:", E.l = (e, r, t, n) => {
+    }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork-authoring-extension:", x.l = (e, r, t, n) => {
         if (o[e]) o[e].push(r);
         else {
             var i, u;
             if (void 0 !== t)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
                     var f = l[s];
                     if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == a + t) {
                         i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
             var d = (r, t) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = o[e];
                     if (delete o[e], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(t))), r) return r(t)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, E.r = e => {
+    }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        E.S = {};
+        x.S = {};
         var e = {},
             r = {};
-        E.I = (t, n) => {
+        x.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                E.o(E.S, t) || (E.S[t] = {});
-                var a = E.S[t],
+                x.o(x.S, t) || (x.S[t] = {});
+                var a = x.S[t],
                     i = "skillsnetwork-authoring-extension",
                     u = (e, r, t, n) => {
                         var o = a[e] = a[e] || {},
                             u = o[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "0.21.4", (() => E.e(669).then((() => () => E(9669))))), u("skillsnetwork-authoring-extension", "0.5.6", (() => E.e(568).then((() => () => E(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "0.21.4", (() => x.e(669).then((() => () => x(9669))))), u("skillsnetwork-authoring-extension", "0.5.6-rc1", (() => x.e(568).then((() => () => x(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        E.g.importScripts && (e = E.g.location + "");
-        var r = E.g.document;
+        x.g.importScripts && (e = x.g.location + "");
+        var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            if (t.length)
-                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
+            t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), E.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), x.p = e
     })(), i = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, u = (e, r) => {
         e = i(e), r = i(r);
@@ -236,95 +235,93 @@
             c = p.pop.bind(p);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? s(h, r) : !c())
         }
         return !!c()
     }, f = (e, r) => {
-        var t = E.S[e];
-        if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = x.S[e];
+        if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
     }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
         var o = d(e, t);
-        return s(n, o) || v(p(e, t, o, n)), m(e[t][o])
+        return s(n, o) || "undefined" != typeof console && console.warn && console.warn(p(e, t, o, n)), v(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !s(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
-    }, v = e => {
-        "undefined" != typeof console && console.warn && console.warn(e)
-    }, m = e => (e.loaded = 1, e.get()), g = (b = e => function(r, t, n, o) {
-        var a = E.I(r);
-        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (f(e, t), c(r, 0, t, n)))), y = b(((e, r, t, n, o) => {
-        var a = r && E.o(r, t) && h(r, t, n);
-        return a ? m(a) : o()
-    })), w = {}, k = {
-        1123: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        3033: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        5344: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
-        5923: () => g("default", "@lumino/disposable", [1, 1, 10, 0]),
-        7986: () => g("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
-        8820: () => g("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        8832: () => g("default", "@lumino/widgets", [1, 1, 37, 2]),
-        9581: () => y("default", "axios", [2, 0, 21, 2], (() => E.e(669).then((() => () => E(9669)))))
-    }, _ = {
+    }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, n, o) {
+        var a = x.I(r);
+        return a && a.then ? a.then(e.bind(e, r, x.S[r], t, n, o)) : e(r, x.S[r], t, n, o)
+    })(((e, r, t, n) => (f(e, t), c(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
+        var a = r && x.o(r, t) && h(r, t, n);
+        return a ? v(a) : o()
+    })), y = {}, w = {
+        1123: () => m("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        3033: () => m("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        5344: () => m("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
+        5923: () => m("default", "@lumino/disposable", [1, 1, 10, 0]),
+        7986: () => m("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
+        8820: () => m("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        8832: () => m("default", "@lumino/widgets", [1, 1, 37, 2]),
+        9581: () => g("default", "axios", [2, 0, 21, 2], (() => x.e(669).then((() => () => x(9669)))))
+    }, k = {
         568: [1123, 3033, 5344, 5923, 7986, 8820, 8832, 9581]
-    }, E.f.consumes = (e, r) => {
-        E.o(_, e) && _[e].forEach((e => {
-            if (E.o(w, e)) return r.push(w[e]);
+    }, x.f.consumes = (e, r) => {
+        x.o(k, e) && k[e].forEach((e => {
+            if (x.o(y, e)) return r.push(y[e]);
             var t = r => {
-                    w[e] = 0, E.m[e] = t => {
-                        delete E.c[e], t.exports = r()
+                    y[e] = 0, x.m[e] = t => {
+                        delete x.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete w[e], E.m[e] = t => {
-                        throw delete E.c[e], r
+                    delete y[e], x.m[e] = t => {
+                        throw delete x.c[e], r
                     }
                 };
             try {
-                var o = k[e]();
-                o.then ? r.push(w[e] = o.then(t).catch(n)) : t(o)
+                var o = w[e]();
+                o.then ? r.push(y[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             340: 0
         };
-        E.f.j = (r, t) => {
-            var n = E.o(e, r) ? e[r] : void 0;
+        x.f.j = (r, t) => {
+            var n = x.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = E.p + E.u(r),
+                    var a = x.p + x.u(r),
                         i = new Error;
-                    E.l(a, (t => {
-                        if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    x.l(a, (t => {
+                        if (x.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
-                    u && u(E)
+                    for (n in i) x.o(i, n) && (x.m[n] = i[n]);
+                    u && u(x)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkskillsnetwork_authoring_extension = self.webpackChunkskillsnetwork_authoring_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), E.nc = void 0;
-    var j = E(5367);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["skillsnetwork-authoring-extension"] = j
+    })(), x.nc = void 0;
+    var E = x(5367);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["skillsnetwork-authoring-extension"] = E
 })();
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.6
+Version: 0.5.6rc1
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/skillsnetwork_authoring_extension.egg-info/SOURCES.txt` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 yarn.lock
 jupyter-config/nb-config/skillsnetwork_authoring_extension.json
 jupyter-config/server-config/skillsnetwork_authoring_extension.json
 skillsnetwork-authoring-extension/__init__.py
 skillsnetwork-authoring-extension/_version.py
 skillsnetwork-authoring-extension/handlers.py
 skillsnetwork-authoring-extension/labextension/package.json
-skillsnetwork-authoring-extension/labextension/static/568.3e8305ffaf486d3cc564.js
+skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js
 skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
 skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
-skillsnetwork-authoring-extension/labextension/static/remoteEntry.1175c035aa1c7085eb76.js
+skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js
 skillsnetwork-authoring-extension/labextension/static/style.js
 skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
 skillsnetwork_authoring_extension.egg-info/PKG-INFO
 skillsnetwork_authoring_extension.egg-info/SOURCES.txt
 skillsnetwork_authoring_extension.egg-info/dependency_links.txt
 skillsnetwork_authoring_extension.egg-info/not-zip-safe
 skillsnetwork_authoring_extension.egg-info/requires.txt
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/button/index.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/button/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 
         document.body.removeChild(link);
         URL.revokeObjectURL(url);
       };
 
       const downloadButton = new ToolbarButton({
         className: 'download-lab-button',
-        label: 'Download Notebook',
+        label: 'Download',
         onClick: download,
-        tooltip: 'Download the current notebook ipynb file to your local system'
+        tooltip: 'Download Lab'
       });
 
       const publishButton = new ToolbarButton({
         className: 'publish-lab-button',
         label: 'Publish on SN',
         onClick: start,
         tooltip: 'Publish Lab'
```

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/button/sample.json` & `skillsnetwork-authoring-extension-0.5.6rc1/src/button/sample.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/config.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/dialog.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/handler.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/menu/index.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/sn-file-library.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/src/tools.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/tools.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/tsconfig.json` & `skillsnetwork-authoring-extension-0.5.6rc1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.6/yarn.lock` & `skillsnetwork-authoring-extension-0.5.6rc1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -27,24 +27,24 @@
   integrity sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==
   dependencies:
     "@babel/helper-validator-identifier" "^7.18.6"
     chalk "^2.0.0"
     js-tokens "^4.0.0"
 
 "@babel/runtime@^7.1.2":
-  version "7.21.5"
-  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.21.5.tgz#8492dddda9644ae3bda3b45eabe87382caee7200"
-  integrity sha512-8jI69toZqqcsnqGGqwGS4Qb1VwLOEp4hz+CXPywcvjs60u3B4Pom/U/7rm4W8tMOYEB+E9wgD0mW1l3r8qlI9Q==
+  version "7.21.0"
+  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.21.0.tgz#5b55c9d394e5fcf304909a8b00c07dc217b56673"
+  integrity sha512-xwII0//EObnq89Ji5AKYQaRYiW/nZ3llSv29d49IuxPhKbtJoLP+9QUUZ4nVragQVtaVGeZrpB+ZtG/Pdy/POw==
   dependencies:
     regenerator-runtime "^0.13.11"
 
 "@blueprintjs/colors@^4.0.0-alpha.3":
-  version "4.1.22"
-  resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.1.22.tgz#033cbf03705100d5114d54161c225eec5cfeacfb"
-  integrity sha512-qcC7nWW9TTSS7aDxE5gbo9vrxo+IOpC6/Kzpi0rdOBYFDd02PppCdnCCjGYw1/IopSsZ9EWqDLmD7zuy0H+WEA==
+  version "4.1.21"
+  resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.1.21.tgz#622c56ac7f9af466680eafcdbaf26e5c9152ad3b"
+  integrity sha512-5csitaTn1xyHktMRyXAcvWzsbrgtP9pK7ZmYX9f0TGjB1UG5zNaTGLexX0aFqop44SpfsSP5mbA8xGBniy8nZA==
 
 "@blueprintjs/core@^3.36.0", "@blueprintjs/core@^3.54.0":
   version "3.54.0"
   resolved "https://registry.yarnpkg.com/@blueprintjs/core/-/core-3.54.0.tgz#7269f34eccdf0d2874377c5ad973ca2a31562221"
   integrity sha512-u2c1s6MNn0ocxhnC6CuiG5g3KV6b4cKUvSobznepA9SC3/AL1s3XOvT7DLWoHRv2B/vBOHFYEDzLw2/vlcGGZg==
   dependencies:
     "@blueprintjs/colors" "^4.0.0-alpha.3"
@@ -721,33 +721,33 @@
     "@lumino/virtualdom" "^1.14.3"
 
 "@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.12.1":
   version "1.12.1"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.12.1.tgz#79860c9937483ddf6cda87f6c2b9da8eb1a5d768"
   integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
 
-"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.1.1":
-  version "2.1.1"
-  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.1.tgz#e867a501f3564987a757005c81aa4b0d4ea5ff4c"
-  integrity sha512-OmEzvphZC/EVpFfwBkmcuzNwKXvkij6gJo1mbf4/tZMC1/8NO3aVnjK1FsgC0TlaGwMD1BLIFgGay2mC/I/cyQ==
+"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.1.0":
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.0.tgz#291ed11a1bd143bfd5a2f2638cfb27aefd1bd9ba"
+  integrity sha512-1pF3gaTxZY6P+Tixs2rd1aj5HgFOdH3RNupgsMaq0sFmxuvuSxaYhiK5/LB9evDN8a6HqHFeS6wVhVajSOJfDQ==
 
 "@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.4", "@lumino/disposable@^1.4.3":
   version "1.10.4"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
   integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/signaling" "^1.11.1"
 
 "@lumino/disposable@^1.10.0 || ^2.0.0-alpha.6":
-  version "2.1.1"
-  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.1.1.tgz#9c6dace68320538532ebd4fb91b159c532baf62e"
-  integrity sha512-zGl5hDDgDgPlrCN8b37gmNRjmYrTXnVq4WaseRtEgjj/en+gHLQW7sgTzkLgPj5rFaVETPkyrDTQ5uZVewFOAw==
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.1.0.tgz#54dfd2e8f361570b08751784b80751056816c66f"
+  integrity sha512-BFSNoNKxdX/qpN8cvL+5/I3MErzBUZYlqLuURSp4aTnqkVg4fYVOUo3E8fD/V9zQRu9pX0WzgTl8H0w0uVK6Gg==
   dependencies:
-    "@lumino/signaling" "^2.1.1"
+    "@lumino/signaling" "^2.1.0"
 
 "@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
   integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
 
 "@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.5":
@@ -789,21 +789,21 @@
   version "1.11.1"
   resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.11.1.tgz#438f447a1b644fd286549804f9851b5aec9679a2"
   integrity sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/properties" "^1.8.2"
 
-"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.1.1":
-  version "2.1.1"
-  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.1.1.tgz#aae22e4cfb8f99baaa54cefaf1555be2c4148f0f"
-  integrity sha512-EUPJlC/kis5DEPA4UxsJRPidGk4qcgS+rfQlYfGfA4Z6vR8nzcwU9WE0UIWdqo6GN7cLWR8lGLzZzyIGY3+qiA==
+"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.1.0":
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.1.0.tgz#82bddad7e074e757b5c9b5e0822278115f81beec"
+  integrity sha512-Vk2qPmuYn7TdEiqn/bmIrLNBaLmcuB09s+cI8FOxyEZvuW92fGP5P5H2C0rgqy9OT1mvZqobhkEvcCav8HdxxA==
   dependencies:
     "@lumino/algorithm" "^2.0.0"
-    "@lumino/coreutils" "^2.1.1"
+    "@lumino/coreutils" "^2.1.0"
 
 "@lumino/virtualdom@^1.14.0", "@lumino/virtualdom@^1.14.3":
   version "1.14.3"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
   integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
@@ -910,17 +910,17 @@
 
 "@types/minimist@^1.2.0":
   version "1.2.2"
   resolved "https://registry.yarnpkg.com/@types/minimist/-/minimist-1.2.2.tgz#ee771e2ba4b3dc5b372935d549fd9617bf345b8c"
   integrity sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==
 
 "@types/node@*":
-  version "18.16.3"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-18.16.3.tgz#6bda7819aae6ea0b386ebc5b24bdf602f1b42b01"
-  integrity sha512-OPs5WnnT1xkCBiuQrZA4+YAV4HEJejmHneyraIaxsbev5yCEr6KMwINNFP9wQeFIw8FWcoTqF3vQsa5CDaI+8Q==
+  version "18.15.11"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-18.15.11.tgz#b3b790f09cb1696cffcec605de025b088fa4225f"
+  integrity sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==
 
 "@types/node@^17.0.29":
   version "17.0.45"
   resolved "https://registry.yarnpkg.com/@types/node/-/node-17.0.45.tgz#2c0fafd78705e7a18b7906b5201a522719dc5190"
   integrity sha512-w+tIMs3rq2afQdsPJlODhoUEKzFP1ayaoyl1CcnwtIlsVe7K7bA1NGm4s3PraqTLlXnbIN84zuBlxBWo1u9BLw==
 
 "@types/normalize-package-data@^2.4.0":
@@ -1039,133 +1039,133 @@
   version "4.33.0"
   resolved "https://registry.yarnpkg.com/@typescript-eslint/visitor-keys/-/visitor-keys-4.33.0.tgz#2a22f77a41604289b7a186586e9ec48ca92ef1dd"
   integrity sha512-uqi/2aSz9g2ftcHWf8uLPJA70rUv6yuMW5Bohw+bwcuzaxQIHaKFZCKGoGXIrc9vkTJ3+0txM73K0Hq3d5wgIg==
   dependencies:
     "@typescript-eslint/types" "4.33.0"
     eslint-visitor-keys "^2.0.0"
 
-"@webassemblyjs/ast@1.11.5", "@webassemblyjs/ast@^1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/ast/-/ast-1.11.5.tgz#6e818036b94548c1fb53b754b5cae3c9b208281c"
-  integrity sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==
-  dependencies:
-    "@webassemblyjs/helper-numbers" "1.11.5"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.5"
-
-"@webassemblyjs/floating-point-hex-parser@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz#e85dfdb01cad16b812ff166b96806c050555f1b4"
-  integrity sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==
-
-"@webassemblyjs/helper-api-error@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz#1e82fa7958c681ddcf4eabef756ce09d49d442d1"
-  integrity sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==
-
-"@webassemblyjs/helper-buffer@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz#91381652ea95bb38bbfd270702351c0c89d69fba"
-  integrity sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==
-
-"@webassemblyjs/helper-numbers@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz#23380c910d56764957292839006fecbe05e135a9"
-  integrity sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==
+"@webassemblyjs/ast@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ast/-/ast-1.11.1.tgz#2bfd767eae1a6996f432ff7e8d7fc75679c0b6a7"
+  integrity sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==
+  dependencies:
+    "@webassemblyjs/helper-numbers" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+
+"@webassemblyjs/floating-point-hex-parser@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz#f6c61a705f0fd7a6aecaa4e8198f23d9dc179e4f"
+  integrity sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==
+
+"@webassemblyjs/helper-api-error@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz#1a63192d8788e5c012800ba6a7a46c705288fd16"
+  integrity sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==
+
+"@webassemblyjs/helper-buffer@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz#832a900eb444884cde9a7cad467f81500f5e5ab5"
+  integrity sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==
+
+"@webassemblyjs/helper-numbers@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz#64d81da219fbbba1e3bd1bfc74f6e8c4e10a62ae"
+  integrity sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==
   dependencies:
-    "@webassemblyjs/floating-point-hex-parser" "1.11.5"
-    "@webassemblyjs/helper-api-error" "1.11.5"
+    "@webassemblyjs/floating-point-hex-parser" "1.11.1"
+    "@webassemblyjs/helper-api-error" "1.11.1"
     "@xtuc/long" "4.2.2"
 
-"@webassemblyjs/helper-wasm-bytecode@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz#e258a25251bc69a52ef817da3001863cc1c24b9f"
-  integrity sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==
-
-"@webassemblyjs/helper-wasm-section@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz#966e855a6fae04d5570ad4ec87fbcf29b42ba78e"
-  integrity sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.5"
-    "@webassemblyjs/helper-buffer" "1.11.5"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.5"
-    "@webassemblyjs/wasm-gen" "1.11.5"
-
-"@webassemblyjs/ieee754@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz#b2db1b33ce9c91e34236194c2b5cba9b25ca9d60"
-  integrity sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==
+"@webassemblyjs/helper-wasm-bytecode@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz#f328241e41e7b199d0b20c18e88429c4433295e1"
+  integrity sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==
+
+"@webassemblyjs/helper-wasm-section@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz#21ee065a7b635f319e738f0dd73bfbda281c097a"
+  integrity sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-buffer" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/wasm-gen" "1.11.1"
+
+"@webassemblyjs/ieee754@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz#963929e9bbd05709e7e12243a099180812992614"
+  integrity sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==
   dependencies:
     "@xtuc/ieee754" "^1.2.0"
 
-"@webassemblyjs/leb128@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/leb128/-/leb128-1.11.5.tgz#482e44d26b6b949edf042a8525a66c649e38935a"
-  integrity sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==
+"@webassemblyjs/leb128@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/leb128/-/leb128-1.11.1.tgz#ce814b45574e93d76bae1fb2644ab9cdd9527aa5"
+  integrity sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==
   dependencies:
     "@xtuc/long" "4.2.2"
 
-"@webassemblyjs/utf8@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/utf8/-/utf8-1.11.5.tgz#83bef94856e399f3740e8df9f63bc47a987eae1a"
-  integrity sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==
-
-"@webassemblyjs/wasm-edit@^1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz#93ee10a08037657e21c70de31c47fdad6b522b2d"
-  integrity sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.5"
-    "@webassemblyjs/helper-buffer" "1.11.5"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.5"
-    "@webassemblyjs/helper-wasm-section" "1.11.5"
-    "@webassemblyjs/wasm-gen" "1.11.5"
-    "@webassemblyjs/wasm-opt" "1.11.5"
-    "@webassemblyjs/wasm-parser" "1.11.5"
-    "@webassemblyjs/wast-printer" "1.11.5"
-
-"@webassemblyjs/wasm-gen@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz#ceb1c82b40bf0cf67a492c53381916756ef7f0b1"
-  integrity sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.5"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.5"
-    "@webassemblyjs/ieee754" "1.11.5"
-    "@webassemblyjs/leb128" "1.11.5"
-    "@webassemblyjs/utf8" "1.11.5"
-
-"@webassemblyjs/wasm-opt@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz#b52bac29681fa62487e16d3bb7f0633d5e62ca0a"
-  integrity sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.5"
-    "@webassemblyjs/helper-buffer" "1.11.5"
-    "@webassemblyjs/wasm-gen" "1.11.5"
-    "@webassemblyjs/wasm-parser" "1.11.5"
-
-"@webassemblyjs/wasm-parser@1.11.5", "@webassemblyjs/wasm-parser@^1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz#7ba0697ca74c860ea13e3ba226b29617046982e2"
-  integrity sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.5"
-    "@webassemblyjs/helper-api-error" "1.11.5"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.5"
-    "@webassemblyjs/ieee754" "1.11.5"
-    "@webassemblyjs/leb128" "1.11.5"
-    "@webassemblyjs/utf8" "1.11.5"
-
-"@webassemblyjs/wast-printer@1.11.5":
-  version "1.11.5"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz#7a5e9689043f3eca82d544d7be7a8e6373a6fa98"
-  integrity sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==
+"@webassemblyjs/utf8@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/utf8/-/utf8-1.11.1.tgz#d1f8b764369e7c6e6bae350e854dec9a59f0a3ff"
+  integrity sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==
+
+"@webassemblyjs/wasm-edit@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz#ad206ebf4bf95a058ce9880a8c092c5dec8193d6"
+  integrity sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-buffer" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/helper-wasm-section" "1.11.1"
+    "@webassemblyjs/wasm-gen" "1.11.1"
+    "@webassemblyjs/wasm-opt" "1.11.1"
+    "@webassemblyjs/wasm-parser" "1.11.1"
+    "@webassemblyjs/wast-printer" "1.11.1"
+
+"@webassemblyjs/wasm-gen@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz#86c5ea304849759b7d88c47a32f4f039ae3c8f76"
+  integrity sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/ieee754" "1.11.1"
+    "@webassemblyjs/leb128" "1.11.1"
+    "@webassemblyjs/utf8" "1.11.1"
+
+"@webassemblyjs/wasm-opt@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz#657b4c2202f4cf3b345f8a4c6461c8c2418985f2"
+  integrity sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-buffer" "1.11.1"
+    "@webassemblyjs/wasm-gen" "1.11.1"
+    "@webassemblyjs/wasm-parser" "1.11.1"
+
+"@webassemblyjs/wasm-parser@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz#86ca734534f417e9bd3c67c7a1c75d8be41fb199"
+  integrity sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-api-error" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/ieee754" "1.11.1"
+    "@webassemblyjs/leb128" "1.11.1"
+    "@webassemblyjs/utf8" "1.11.1"
+
+"@webassemblyjs/wast-printer@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz#d0c73beda8eec5426f10ae8ef55cee5e7084c2f0"
+  integrity sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==
   dependencies:
-    "@webassemblyjs/ast" "1.11.5"
+    "@webassemblyjs/ast" "1.11.1"
     "@xtuc/long" "4.2.2"
 
 "@webpack-cli/configtest@^1.2.0":
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/@webpack-cli/configtest/-/configtest-1.2.0.tgz#7b20ce1c12533912c3b217ea68262365fa29a6f5"
   integrity sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==
 
@@ -1461,17 +1461,17 @@
 
 camelcase@^5.3.1:
   version "5.3.1"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-5.3.1.tgz#e3c9b31569e106811df242f715725a1f4c494320"
   integrity sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==
 
 caniuse-lite@^1.0.30001449:
-  version "1.0.30001482"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001482.tgz#8b3fad73dc35b2674a5c96df2d4f9f1c561435de"
-  integrity sha512-F1ZInsg53cegyjroxLNW9DmrEQ1SuGRTO1QlpA0o2/6OpQ0gFeDRoq1yFmnr8Sakn9qwwt9DmbxHB6w167OSuQ==
+  version "1.0.30001480"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001480.tgz#9bbd35ee44c2480a1e3a3b9f4496f5066817164a"
+  integrity sha512-q7cpoPPvZYgtyC4VaBSN0Bt+PJ4c4EYRf0DrduInOz2SkFpHD5p3LnvEpqBp7UnJn+8x1Ogl1s38saUxe+ihQQ==
 
 chalk@^2.0.0, chalk@^2.3.0, chalk@^2.4.1:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -1805,17 +1805,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.284:
-  version "1.4.378"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.378.tgz#73431ffd5fffebc18b4e897fac2e7d4ae6d559d9"
-  integrity sha512-RfCD26kGStl6+XalfX3DGgt3z2DNwJS5DKRHCpkPq5T/PqpZMPB1moSRXuK9xhkt/sF57LlpzJgNoYl7mO7Z6w==
+  version "1.4.368"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.368.tgz#75901f97d3e23da2e66feb1e61fbb8e70ac96430"
+  integrity sha512-e2aeCAixCj9M7nJxdB/wDjO6mbYX+lJJxSJCXDzlr5YPGYVofuJwGN9nKg2o6wWInjX6XmxRinn3AeJMK81ltw==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emojis-list@^3.0.0:
@@ -1829,18 +1829,18 @@
   integrity sha512-QKrV0iKR6MZVJV08QY0wp1e7vF6QbhnbQhb07bwpEyuz4uZiZgPlEGdkCROuFkUwdxlFaiPIhjyarH1ee/3vhw==
   dependencies:
     abstract-leveldown "^6.2.1"
     inherits "^2.0.3"
     level-codec "^9.0.0"
     level-errors "^2.0.0"
 
-enhanced-resolve@^5.13.0:
-  version "5.13.0"
-  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz#26d1ecc448c02de997133217b5c1053f34a0a275"
-  integrity sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==
+enhanced-resolve@^5.10.0:
+  version "5.12.0"
+  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz#300e1c90228f5b570c4d35babf263f6da7155634"
+  integrity sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 enquirer@^2.3.5:
   version "2.3.6"
   resolved "https://registry.yarnpkg.com/enquirer/-/enquirer-2.3.6.tgz#2a7fe5dd634a1e4125a975ec994ff5456dc3734d"
@@ -2917,18 +2917,18 @@
   version "0.4.1"
   resolved "https://registry.yarnpkg.com/levn/-/levn-0.4.1.tgz#ae4562c007473b932a6200d403268dd2fffc6ade"
   integrity sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==
   dependencies:
     prelude-ls "^1.2.1"
     type-check "~0.4.0"
 
-lib0@^0.2.31, lib0@^0.2.42, lib0@^0.2.52, lib0@^0.2.74:
-  version "0.2.74"
-  resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.74.tgz#7a4cc816a0420e76de85009423c8ab63655ff817"
-  integrity sha512-roj9i46/JwG5ik5KNTkxP2IytlnrssAkD/OhlAVtE+GqectrdkfR+pttszVLrOzMDeXNs1MPt6yo66MUolWSiA==
+lib0@^0.2.31, lib0@^0.2.42, lib0@^0.2.52, lib0@^0.2.72:
+  version "0.2.73"
+  resolved "https://registry.yarnpkg.com/lib0/-/lib0-0.2.73.tgz#af7d7ce9ad523fa3e241d437cc3ab1862f9a1f29"
+  integrity sha512-aJJIElCLWnHMcYZPtsM07QoSfHwpxCy4VUzBYGXFYEmh/h2QS5uZNbCCfL0CqnkOE30b7Tp9DVfjXag+3qzZjQ==
   dependencies:
     isomorphic.js "^0.2.4"
 
 license-webpack-plugin@^2.3.14:
   version "2.3.21"
   resolved "https://registry.yarnpkg.com/license-webpack-plugin/-/license-webpack-plugin-2.3.21.tgz#152f5e82d5f51f8bab78905731f2b8042aa5691b"
   integrity sha512-rVaYU9TddZN3ao8M/0PrRSCdTp2EW6VQymlgsuScld1vef0Ou7fALx3ePe83KLP3xAEDcPK5fkqUVqGBnbz1zQ==
@@ -3512,30 +3512,30 @@
 
 postcss-safe-parser@^6.0.0:
   version "6.0.0"
   resolved "https://registry.yarnpkg.com/postcss-safe-parser/-/postcss-safe-parser-6.0.0.tgz#bb4c29894171a94bc5c996b9a30317ef402adaa1"
   integrity sha512-FARHN8pwH+WiS2OPCxJI8FuRJpTVnn6ZNFiqAM2aeW2LwTHWWmWgIyKC6cUo0L8aeKiF/14MNvnpls6R2PBeMQ==
 
 postcss-selector-parser@^6.0.11, postcss-selector-parser@^6.0.2, postcss-selector-parser@^6.0.4:
-  version "6.0.12"
-  resolved "https://registry.yarnpkg.com/postcss-selector-parser/-/postcss-selector-parser-6.0.12.tgz#2efae5ffab3c8bfb2b7fbf0c426e3bca616c4abb"
-  integrity sha512-NdxGCAZdRrwVI1sy59+Wzrh+pMMHxapGnpfenDVlMEXoOcvt4pGE0JLK9YY2F5dLxcFYA/YbVQKhcGU+FtSYQg==
+  version "6.0.11"
+  resolved "https://registry.yarnpkg.com/postcss-selector-parser/-/postcss-selector-parser-6.0.11.tgz#2e41dc39b7ad74046e1615185185cd0b17d0c8dc"
+  integrity sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==
   dependencies:
     cssesc "^3.0.0"
     util-deprecate "^1.0.2"
 
 postcss-value-parser@^4.1.0, postcss-value-parser@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.2.15, postcss@^8.3.11, postcss@^8.4.19:
-  version "8.4.23"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.23.tgz#df0aee9ac7c5e53e1075c24a3613496f9e6552ab"
-  integrity sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==
+  version "8.4.22"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.22.tgz#c29e6776b60ab3af602d4b513d5bd2ff9aa85dc1"
+  integrity sha512-XseknLAfRHzVWjCEtdviapiBtfLdgyzExD50Rg2ePaucEesyh8Wv4VPdW0nbyDa1ydbrAxV19jvMT4+LFmcNUA==
   dependencies:
     nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
@@ -3546,17 +3546,17 @@
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/prettier-linter-helpers/-/prettier-linter-helpers-1.0.0.tgz#d23d41fe1375646de2d0104d3454a3008802cf7b"
   integrity sha512-GbK2cP9nraSSUF9N2XwUwqfzlAFlMNYYl+ShE/V+H8a9uNl/oUqB1w2EL54Jh0OlyRSd8RfWYJ3coVS4TROP2w==
   dependencies:
     fast-diff "^1.1.2"
 
 prettier@^2.1.1:
-  version "2.8.8"
-  resolved "https://registry.yarnpkg.com/prettier/-/prettier-2.8.8.tgz#e8c5d7e98a4305ffe3de2e1fc4aca1a71c28b1da"
-  integrity sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==
+  version "2.8.7"
+  resolved "https://registry.yarnpkg.com/prettier/-/prettier-2.8.7.tgz#bb79fc8729308549d28fe3a98fce73d2c0656450"
+  integrity sha512-yPngTo3aXUUmyuTjeTUT75txrf+aMh9FiD7q9ZE/i6r0bPb22g4FsE6Y338PQX1bmfy08i9QQCB7/rcUAVntfw==
 
 process@^0.11.10:
   version "0.11.10"
   resolved "https://registry.yarnpkg.com/process/-/process-0.11.10.tgz#7332300e840161bda3e69a1d1d91a7d4bc16f182"
   integrity sha512-cdGef/drWFoydD1JsMzuFf8100nZl+GT+yacc2bEced5f9Rjk4z+WtFUTBu9PhOi9j/jfmBPu0mMEY4wIdAF8A==
 
 progress@^2.0.0:
@@ -3853,15 +3853,15 @@
   resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-2.7.1.tgz#1ca4f32d1b24c590c203b8e7a50bf0ea4cd394d7"
   integrity sha512-SHiNtMOUGWBQJwzISiVYKu82GiV4QYGePp3odlY1tuKO7gPtphAT5R/py0fA6xtbgLL/RvtJZnU9b8s0F1q0Xg==
   dependencies:
     "@types/json-schema" "^7.0.5"
     ajv "^6.12.4"
     ajv-keywords "^3.5.2"
 
-schema-utils@^3.0.0, schema-utils@^3.1.1, schema-utils@^3.1.2:
+schema-utils@^3.0.0, schema-utils@^3.1.0, schema-utils@^3.1.1:
   version "3.1.2"
   resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.1.2.tgz#36c10abca6f7577aeae136c804b0c741edeadc99"
   integrity sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==
   dependencies:
     "@types/json-schema" "^7.0.8"
     ajv "^6.12.5"
     ajv-keywords "^3.5.2"
@@ -4586,38 +4586,38 @@
 
 webpack-sources@^3.2.3:
   version "3.2.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
 webpack@^5.41.1:
-  version "5.81.0"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.81.0.tgz#27a2e8466c8b4820d800a8d90f06ef98294f9956"
-  integrity sha512-AAjaJ9S4hYCVODKLQTgG5p5e11hiMawBwV2v8MYLE0C/6UAGLuAF4n1qa9GOwdxnicaP+5k6M5HrLmD4+gIB8Q==
+  version "5.79.0"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.79.0.tgz#8552b5da5a26e4e25842c08a883e08fc7740547a"
+  integrity sha512-3mN4rR2Xq+INd6NnYuL9RC9GAmc1ROPKJoHhrZ4pAjdMFEkJJWrsPw8o2JjCIyQyTu7rTXYn4VG6OpyB3CobZg==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
     "@types/estree" "^1.0.0"
-    "@webassemblyjs/ast" "^1.11.5"
-    "@webassemblyjs/wasm-edit" "^1.11.5"
-    "@webassemblyjs/wasm-parser" "^1.11.5"
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/wasm-edit" "1.11.1"
+    "@webassemblyjs/wasm-parser" "1.11.1"
     acorn "^8.7.1"
     acorn-import-assertions "^1.7.6"
     browserslist "^4.14.5"
     chrome-trace-event "^1.0.2"
-    enhanced-resolve "^5.13.0"
+    enhanced-resolve "^5.10.0"
     es-module-lexer "^1.2.1"
     eslint-scope "5.1.1"
     events "^3.2.0"
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.2.9"
     json-parse-even-better-errors "^2.3.1"
     loader-runner "^4.2.0"
     mime-types "^2.1.27"
     neo-async "^2.6.2"
-    schema-utils "^3.1.2"
+    schema-utils "^3.1.0"
     tapable "^2.1.1"
     terser-webpack-plugin "^5.3.7"
     watchpack "^2.4.0"
     webpack-sources "^3.2.3"
 
 whatwg-mimetype@^2.3.0:
   version "2.3.0"
@@ -4675,17 +4675,17 @@
   version "2.0.2"
   resolved "https://registry.yarnpkg.com/which/-/which-2.0.2.tgz#7c6a8dd0a636a0327e10b59c9286eee93f3f51b1"
   integrity sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==
   dependencies:
     isexe "^2.0.0"
 
 wildcard@^2.0.0:
-  version "2.0.1"
-  resolved "https://registry.yarnpkg.com/wildcard/-/wildcard-2.0.1.tgz#5ab10d02487198954836b6349f74fff961e10f67"
-  integrity sha512-CC1bOL87PIWSBhDcTrdeLo6eGT7mCFtrg0uIJtqJUFyK+eJnzl8A1niH56uu7KMa5XFrtiV+AQuHO3n7DsHnLQ==
+  version "2.0.0"
+  resolved "https://registry.yarnpkg.com/wildcard/-/wildcard-2.0.0.tgz#a77d20e5200c6faaac979e4b3aadc7b3dd7f8fec"
+  integrity sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==
 
 word-wrap@^1.2.3:
   version "1.2.3"
   resolved "https://registry.yarnpkg.com/word-wrap/-/word-wrap-1.2.3.tgz#610636f6b1f703891bd34771ccb17fb93b47079c"
   integrity sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==
 
 worker-loader@^3.0.2:
@@ -4772,17 +4772,17 @@
 
 yargs-parser@^20.2.3:
   version "20.2.9"
   resolved "https://registry.yarnpkg.com/yargs-parser/-/yargs-parser-20.2.9.tgz#2eb7dc3b0289718fc295f362753845c41a0c94ee"
   integrity sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==
 
 yjs@^13.5.40:
-  version "13.6.0"
-  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.6.0.tgz#3ede38b3c57653c302fd63d7294e63892514fb0a"
-  integrity sha512-tFZtuQV6XamtDa9SfZhUsxchUcTBWe7fzpo1UWZDLXGejTZ5t9MCswGYzyvq7+BDzfEc9oX54QEbzI/4NyS6+g==
+  version "13.5.53"
+  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.5.53.tgz#6531378981b89cfadd107145f7fb9f65f708a01f"
+  integrity sha512-B4UUycEK8BcYf195HL4LN4Az4Sg2+QzTHnabFHjQwLvGn96v/G+4CS52xNZk/0QWNXhLRCb+2GK3JmcX5fiCEQ==
   dependencies:
-    lib0 "^0.2.74"
+    lib0 "^0.2.72"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
```

