# Comparing `tmp/matfree-0.0.2.tar.gz` & `tmp/matfree-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matfree-0.0.2.tar", last modified: Fri Apr 28 12:15:50 2023, max compression
+gzip compressed data, was "matfree-0.0.3.tar", last modified: Mon May  1 07:51:31 2023, max compression
```

## Comparing `matfree-0.0.2.tar` & `matfree-0.0.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.030550 matfree-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-28 12:15:34.000000 matfree-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-28 12:15:34.000000 matfree-0.0.2/.github/workflows/doc-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 12:15:34.000000 matfree-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 12:15:34.000000 matfree-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 12:15:34.000000 matfree-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 12:15:34.000000 matfree-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 12:15:34.000000 matfree-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 12:15:50.038550 matfree-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-28 12:15:34.000000 matfree-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/decomp.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/hutch.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/montecarlo.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/api/slq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/benchmarks/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/benchmarks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/dev/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.034550 matfree-0.0.2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 12:15:34.000000 matfree-0.0.2/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/matfree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 12:15:49.000000 matfree-0.0.2/matfree/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/matfree/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/np.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/prng.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/backend/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/slq.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 12:15:34.000000 matfree-0.0.2/matfree/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/matfree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 12:15:50.000000 matfree-0.0.2/matfree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-28 12:15:34.000000 matfree-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-28 12:15:34.000000 matfree-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 12:15:50.042550 matfree-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 12:15:34.000000 matfree-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:50.038550 matfree-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_autodiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 12:15:34.000000 matfree-0.0.2/tests/test_slq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.367911 matfree-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.355911 matfree-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.355911 matfree-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-01 07:51:11.000000 matfree-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 07:51:11.000000 matfree-0.0.3/.github/workflows/doc-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-01 07:51:11.000000 matfree-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-01 07:51:11.000000 matfree-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-01 07:51:11.000000 matfree-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 07:51:11.000000 matfree-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 07:51:11.000000 matfree-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-01 07:51:31.367911 matfree-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-01 07:51:11.000000 matfree-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.355911 matfree-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/decomp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/hutch.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/montecarlo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/slq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/benchmarks/control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/benchmarks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/dev/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/matfree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.363911 matfree-0.0.3/matfree/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/hutch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/slq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.363911 matfree-0.0.3/matfree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 07:51:11.000000 matfree-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-01 07:51:11.000000 matfree-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-01 07:51:31.367911 matfree-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 07:51:11.000000 matfree-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.367911 matfree-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_autodiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_hutch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_slq.py
```

### Comparing `matfree-0.0.2/.github/workflows/ci.yaml` & `matfree-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/.github/workflows/doc-publish.yml` & `matfree-0.0.3/.github/workflows/doc-publish.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/.github/workflows/release.yml` & `matfree-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/.gitignore` & `matfree-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/.pre-commit-config.yaml` & `matfree-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/LICENSE` & `matfree-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/PKG-INFO` & `matfree-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.2
+Version: 0.0.3
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
@@ -82,42 +82,62 @@
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
->>> keys = jax.random.split(key, num=10_000)
->>> trace, diagonal = hutch.trace_and_diagonal(matvec, keys=keys, sample_fun=sample_fun)
+>>> trace, diagonal = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-509.0
+507.0
 
 >>> print(jnp.round(diagonal))
-[222. 287.]
+[221. 287.]
 
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
 
 
 ```
 
+Why is the argument called `num_levels`? Because under the hood,
+`trace_and_diagonal` implements a multilevel diagonal-estimation scheme:
+```python
+>>> _, diagonal_1 = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
+>>> init = jnp.zeros(shape=(2,), dtype=float)
+>>> diagonal_2 = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10_000, sample_fun=sample_fun)
+
+>>> print(jnp.round(diagonal_1, 4))
+[220.54979 286.7476 ]
+
+>>> print(jnp.round(diagonal_2, 4))
+[220.54979 286.7476 ]
+
+>>> diagonal = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10, num_samples_per_batch=1000, num_batches_per_level=10, sample_fun=sample_fun)
+>>> print(jnp.round(diagonal))
+[219. 285.]
+
+```
+
+Does the multilevel scheme help? That is not always clear; but [here](https://github.com/pnkraemer/matfree/blob/main/docs/benchmarks/control_variates.py) is a benchmark.
+
 ### Determinants
 
 
 Estimate log-determinants as such:
 ```python
 >>> a = jnp.reshape(jnp.arange(36.), (6, 6)) / 36
 >>> sample_fun = montecarlo.normal(shape=(6,))
 >>> matvec = lambda x: a.T @ (a @ x) + x
 >>> order = 3
->>> logdet, _ = slq.trace_of_matfun(jnp.log, matvec, order, key=key, sample_fun=sample_fun)
+>>> logdet = slq.logdet(matvec, order, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(logdet))
 3.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.linalg.slogdet(a.T @ a + jnp.eye(6))[1]))
 3.0
 
 ```
```

### Comparing `matfree-0.0.2/README.md` & `matfree-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -65,42 +65,62 @@
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
->>> keys = jax.random.split(key, num=10_000)
->>> trace, diagonal = hutch.trace_and_diagonal(matvec, keys=keys, sample_fun=sample_fun)
+>>> trace, diagonal = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-509.0
+507.0
 
 >>> print(jnp.round(diagonal))
-[222. 287.]
+[221. 287.]
 
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
 
 
 ```
 
+Why is the argument called `num_levels`? Because under the hood,
+`trace_and_diagonal` implements a multilevel diagonal-estimation scheme:
+```python
+>>> _, diagonal_1 = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
+>>> init = jnp.zeros(shape=(2,), dtype=float)
+>>> diagonal_2 = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10_000, sample_fun=sample_fun)
+
+>>> print(jnp.round(diagonal_1, 4))
+[220.54979 286.7476 ]
+
+>>> print(jnp.round(diagonal_2, 4))
+[220.54979 286.7476 ]
+
+>>> diagonal = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10, num_samples_per_batch=1000, num_batches_per_level=10, sample_fun=sample_fun)
+>>> print(jnp.round(diagonal))
+[219. 285.]
+
+```
+
+Does the multilevel scheme help? That is not always clear; but [here](https://github.com/pnkraemer/matfree/blob/main/docs/benchmarks/control_variates.py) is a benchmark.
+
 ### Determinants
 
 
 Estimate log-determinants as such:
 ```python
 >>> a = jnp.reshape(jnp.arange(36.), (6, 6)) / 36
 >>> sample_fun = montecarlo.normal(shape=(6,))
 >>> matvec = lambda x: a.T @ (a @ x) + x
 >>> order = 3
->>> logdet, _ = slq.trace_of_matfun(jnp.log, matvec, order, key=key, sample_fun=sample_fun)
+>>> logdet = slq.logdet(matvec, order, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(logdet))
 3.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.linalg.slogdet(a.T @ a + jnp.eye(6))[1]))
 3.0
 
 ```
```

### Comparing `matfree-0.0.2/docs/benchmarks/control_variates.py` & `matfree-0.0.3/docs/benchmarks/control_variates.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 
 from matfree import hutch, montecarlo
 from matfree.backend import func, linalg, np, plt, prng, progressbar, time
 
 
 def rmse_relative(received, *, expected):
     """Compute the relative root-mean-square error."""
-    return linalg.norm((received - expected) / expected) / np.sqrt(expected.size)
+    return linalg.vector_norm((received - expected) / expected) / np.sqrt(expected.size)
 
 
 def error_and_time(fun, error_fun):
     """Compute error and runtime of a function with a single outputs."""
 
     def fun_wrapped(*args, **kwargs):
         # Execute once for compilation
         _ = fun(*args, **kwargs)
 
         # Execute and time
-        t0 = time.clock()
+        t0 = time.perf_counter()
         result = fun(*args, **kwargs)
         result.block_until_ready()
-        t1 = time.clock()
+        t1 = time.perf_counter()
         return error_fun(result), (t1 - t0)
 
     return fun_wrapped
 
 
 def problem(n):
     """Create an example problem."""
 
     # This function has a Jacobian with x-shaped sparsity pattern
     # We expect control variates to do pretty well
     # (But I don't know why)
     def f(x):
         return np.sin(np.roll(np.sin(np.flip(np.cos(x)) + 1) ** 2, 1)) * np.sin(x**2)
 
-    key = prng.PRNGKey(seed=2)
+    key = prng.prng_key(seed=2)
     x0 = prng.uniform(key, shape=(n,))
 
     _, jvp = func.linearize(f, x0)
     J = func.jacfwd(f)(x0)
-    trace = np.trace(J)
+    trace = linalg.trace(J)
     sample_fun = montecarlo.normal(shape=(n,), dtype=float)
 
     return (jvp, trace, J), (key, sample_fun)
 
 
 if __name__ == "__main__":
     dim = 100
@@ -66,16 +66,17 @@
             Av, key=key, sample_fun=sample_fun, num_batches=num, num_samples_per_batch=1
         )
 
     @func.partial(error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def fun2(num, key):
         """Estimate trace and diagonal jointly and discard the diagonal."""
-        keys = prng.split(key, num=num)
-        trace2, _ = hutch.trace_and_diagonal(Av, keys=keys, sample_fun=sample_fun)
+        trace2, _ = hutch.trace_and_diagonal(
+            Av, key=key, num_levels=num, sample_fun=sample_fun
+        )
         return trace2
 
     errors1, stds1, times1 = [], [], []
     errors2, stds2, times2 = [], [], []
 
     for n in progressbar.progressbar(num_samples):
         test_keys = prng.split(k, num=num_restarts)
```

### Comparing `matfree-0.0.2/matfree/backend/func.py` & `matfree-0.0.3/matfree/backend/func.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/matfree/backend/np.py` & `matfree-0.0.3/matfree/backend/np.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # But deviate in a few points:
 # * The functions here do not have all the arguments specified in the API
 #   (we only wrap the arguments we need)
 # * Our current version of diag/diagonal is slightly different
 # * We do not use methods on Array types, e.g. shape(), dtype(). Instead
 #   these are functions. (Not all backends might always follow this method interface.)
 # * We do not implement any constants (e.g. NaN, Pi). Instead, these are methods.
-# * We implement some linear algebra content (e.g. trace()) here (todo!) instead of in
-#   backend.linalg.
 
 
 import jax.numpy as jnp
 
 # Creation functions:
 
 
@@ -63,30 +61,14 @@
     return jnp.cos(x)
 
 
 def sqrt(x, /):
     return jnp.sqrt(x)
 
 
-# Linear algebra functions
-# Todo: move to backend.linalg?
-
-
-def vecdot(x1, x2, /):
-    return jnp.dot(x1, x2)
-
-
-def diagonal(x, /, offset=0):
-    return jnp.diag(x, offset)
-
-
-def trace(x, /):
-    return jnp.trace(x)
-
-
 # Utility functions
 
 
 def any(x, /):  # noqa: A001
     return jnp.any(x)
 
 
@@ -135,15 +117,15 @@
     return jnp.flip(x)
 
 
 def roll(x, /, shift):
     return jnp.roll(x, shift)
 
 
-# Functional implementation of methods
+# Functional implementation of what are usually array-methods
 
 
 def shape(x, /):
     return jnp.shape(x)
 
 
 def dtype(x, /):
```

### Comparing `matfree-0.0.2/matfree/decomp.py` & `matfree-0.0.3/matfree/decomp.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,20 +115,20 @@
 
 def _lanczos_extract(state: _LanczosState, /):
     _, basis, (diag, offdiag), _ = state
     return basis, (diag, offdiag)
 
 
 def _normalise(vec):
-    length = linalg.norm(vec)
+    length = linalg.vector_norm(vec)
     return vec / length, length
 
 
 def _gram_schmidt_orthogonalise_set(vec, vectors):  # Gram-Schmidt
-    vec, coeffs = control_flow.scan(_gram_schmidt_orthogonalise, init=vec, xs=vectors)
+    vec, coeffs = control_flow.scan(_gram_schmidt_orthogonalise, vec, xs=vectors)
     return vec, coeffs
 
 
 def _gram_schmidt_orthogonalise(vec1, vec2):
-    coeff = np.vecdot(vec1, vec2)
+    coeff = linalg.vecdot(vec1, vec2)
     vec_ortho = vec1 - coeff * vec2
     return vec_ortho, coeff
```

### Comparing `matfree-0.0.2/matfree/montecarlo.py` & `matfree-0.0.3/matfree/montecarlo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,123 @@
-"""A million ways of computing arithmetic means."""
+"""Monte-Carlo estimation."""
 
 from matfree.backend import containers, control_flow, func, np, prng
-from matfree.backend.typing import Any
+from matfree.backend.typing import Any, Array, Callable
 
 
-def montecarlo(f, /, *, sample_fun):
+def estimate(
+    fun: Callable,
+    /,
+    *,
+    key: Array,
+    sample_fun: Callable,
+    num_batches: int = 1,
+    num_samples_per_batch: int = 10_000,
+) -> Array:
+    """Monte-Carlo estimation: Compute the expected value of a function.
+
+    Parameters
+    ----------
+    fun:
+        Function whose expected value shall be estimated.
+    key:
+        Pseudo-random number generator key.
+    sample_fun:
+        Sampling function.
+        For trace-estimation, use
+        either [montecarlo.normal(...)][matfree.montecarlo.normal]
+        or [montecarlo.rademacher(...)][matfree.montecarlo.normal].
+    num_batches:
+        Number of batches when computing arithmetic means.
+    num_samples_per_batch:
+        Number of samples per batch.
+    """
+    fun_mc = _montecarlo(fun, sample_fun=sample_fun)
+    fun_single_batch = _mean_vmap(fun_mc, num_samples_per_batch)
+    fun_batched = _mean_loop(fun_single_batch, num_batches)
+    return fun_batched(key)
+
+
+def _montecarlo(f, /, *, sample_fun):
     """Turn a function into a Monte-Carlo problem.
 
     More specifically, f(x) becomes g(key) = f(h(key)),
     using a sample function h: key -> x.
     This can then be evaluated and averaged in batches, loops, and compositions thereof.
     """
     # todo: what about randomised QMC? How do we best implement this?
 
     def f_mc(key, /):
         sample = sample_fun(key)
-        return f(sample), 0
+        return f(sample)
 
     return f_mc
 
 
-def mean_vmap(f, num, /):
+def _mean_vmap(f, num, /):
     """Compute a batch-mean via jax.vmap."""
 
     def f_mean(key, /):
         subkeys = prng.split(key, num)
-        fx_values, how_many_previously = func.vmap(f)(subkeys)
-        return _filter_nan_and_mean(fx_values, how_many_previously)
+        fx_values = func.vmap(f)(subkeys)
+        return np.nanmean(fx_values, axis=0)
 
     return f_mean
 
 
-def mean_map(f, num, /):
-    """Compute a batch-mean via jax.lax.map."""
-
-    def f_mean(key, /):
-        subkeys = prng.split(key, num)
-        fx_values, how_many_previously = control_flow.map(f, subkeys)
-        return _filter_nan_and_mean(fx_values, how_many_previously)
-
-    return f_mean
-
-
-def _filter_nan_and_mean(fx_values, how_many_previously):
-    is_nan = np.any(np.isnan(fx_values))
-    how_many = np.sum(np.where(is_nan, np.maximum(1, how_many_previously), 0))
-    mean = np.nanmean(fx_values, axis=0)
-    return mean, how_many
-
-
 class _MState(containers.NamedTuple):
     mean: Any
     key: Any
-    num_nans: Any
 
 
-def mean_loop(f, num, /):
+def _mean_loop(f, num, /):
     """Compute an on-the-fly mean via a for-loop."""
 
     def f_mean(key, /):
         # Initialise
-        fx_shape = func.eval_shape(f, key)[0].shape
+        fx_shape = func.eval_shape(f, key).shape
         mean = np.zeros(fx_shape, dtype=float)
-        mstate = _MState(mean=mean, key=key, num_nans=0)
+        mstate = _MState(mean=mean, key=key)
 
         # Run for-loop
         increment = func.partial(_mean_increment, fun=f)
         mstate = control_flow.fori_loop(0, num, body_fun=increment, init_val=mstate)
-        mean, _key, num_nans = mstate  # todo: why not return key?
+        mean, _key = mstate  # todo: why not return key?
 
         # Return results
-        return mean, num_nans
+        return mean
 
     return f_mean
 
 
 def _mean_increment(i, mstate: _MState, fun) -> _MState:
     """Increment the current mean-estimate."""
     # Read and split key
-    mean, key, num_nans = mstate
+    mean, key = mstate
     _, subkey = prng.split(key)
 
     # Evaluate function
-    fx_values, how_many_previously = fun(subkey)
-
-    # Update NaN-count
-    how_many_max = np.maximum(1, np.sum(how_many_previously))
-    fx_is_nan = np.any(np.isnan(fx_values))
-    num_nans_new = num_nans + fx_is_nan * how_many_max
+    fx_values = fun(subkey)
 
     # Update mean estimate
     mean_new = np.sum(np.asarray([mean * i, fx_values]), axis=0) / (i + 1)
-    return _MState(mean=mean_new, key=subkey, num_nans=num_nans_new)
+    return _MState(mean=mean_new, key=subkey)
 
 
 def normal(*, shape, dtype=float):
     """Construct a function that samples from a standard normal distribution."""
 
     def fun(key):
         return prng.normal(key, shape=shape, dtype=dtype)
 
     return fun
 
 
 def rademacher(*, shape, dtype=float):
-    """Normalised Rademacher distributions."""
+    """Construct a function that samples from a Rademacher distribution."""
 
     def fun(key):
         return prng.rademacher(key, shape=shape, dtype=dtype)
 
     return fun
```

### Comparing `matfree-0.0.2/matfree/test_util.py` & `matfree-0.0.3/matfree/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def generate_symmetric_matrix_from_eigvals(eigvals, /):
     """Generate a symmetric matrix with prescribed eigenvalues."""
     (n,) = eigvals.shape
 
     # Need _some_ matrix to start with
     A = np.reshape(np.arange(1.0, n**2 + 1.0), (n, n))
-    A = A / linalg.norm(A)
+    A = A / linalg.matrix_norm(A)
     X = A.T @ A + np.eye(n)
 
     # QR decompose. We need the orthogonal matrix.
     # Treat Q as a stack of eigenvectors.
     Q, R = linalg.qr(X)
 
     # Treat Q as eigenvectors, and 'D' as eigenvalues.
```

### Comparing `matfree-0.0.2/matfree.egg-info/PKG-INFO` & `matfree-0.0.3/matfree.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.2
+Version: 0.0.3
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
@@ -82,42 +82,62 @@
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
->>> keys = jax.random.split(key, num=10_000)
->>> trace, diagonal = hutch.trace_and_diagonal(matvec, keys=keys, sample_fun=sample_fun)
+>>> trace, diagonal = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-509.0
+507.0
 
 >>> print(jnp.round(diagonal))
-[222. 287.]
+[221. 287.]
 
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
 
 
 ```
 
+Why is the argument called `num_levels`? Because under the hood,
+`trace_and_diagonal` implements a multilevel diagonal-estimation scheme:
+```python
+>>> _, diagonal_1 = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
+>>> init = jnp.zeros(shape=(2,), dtype=float)
+>>> diagonal_2 = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10_000, sample_fun=sample_fun)
+
+>>> print(jnp.round(diagonal_1, 4))
+[220.54979 286.7476 ]
+
+>>> print(jnp.round(diagonal_2, 4))
+[220.54979 286.7476 ]
+
+>>> diagonal = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10, num_samples_per_batch=1000, num_batches_per_level=10, sample_fun=sample_fun)
+>>> print(jnp.round(diagonal))
+[219. 285.]
+
+```
+
+Does the multilevel scheme help? That is not always clear; but [here](https://github.com/pnkraemer/matfree/blob/main/docs/benchmarks/control_variates.py) is a benchmark.
+
 ### Determinants
 
 
 Estimate log-determinants as such:
 ```python
 >>> a = jnp.reshape(jnp.arange(36.), (6, 6)) / 36
 >>> sample_fun = montecarlo.normal(shape=(6,))
 >>> matvec = lambda x: a.T @ (a @ x) + x
 >>> order = 3
->>> logdet, _ = slq.trace_of_matfun(jnp.log, matvec, order, key=key, sample_fun=sample_fun)
+>>> logdet = slq.logdet(matvec, order, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(logdet))
 3.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.linalg.slogdet(a.T @ a + jnp.eye(6))[1]))
 3.0
 
 ```
```

### Comparing `matfree-0.0.2/matfree.egg-info/SOURCES.txt` & `matfree-0.0.3/matfree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/mkdocs.yml` & `matfree-0.0.3/mkdocs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         python:
           options:
             show_root_members_full_path: false
             show_category_heading: false
             docstring_style: numpy
             show_if_no_docstring: true
             show_signature_annotations: true
-            members_order: source
+            members_order: alphabetical
+            docstring_section_style: list
 watch: [matfree]
 extra:
   social:
     - icon: fontawesome/brands/twitter
       link: https://twitter.com/@pnkraemer
       name: Nico
   generator: false
```

### Comparing `matfree-0.0.2/pyproject.toml` & `matfree-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -26,9 +26,16 @@
     "D213",
     # zip(..., strict=True/False) is not supported on Python < 3.10
     "B905",
 ]
 
 [tool.ruff.per-file-ignores]
 # We don't write docstrings for the backend
-"matfree/backend/np.py" = ["D103"]
+"matfree/backend/control_flow.py" = ["D103"]
 "matfree/backend/func.py" = ["D103"]
+"matfree/backend/linalg.py" = ["D103"]
+"matfree/backend/np.py" = ["D103"]
+"matfree/backend/plt.py" = ["D103"]
+"matfree/backend/prng.py" = ["D103"]
+"matfree/backend/progressbar.py" = ["D103"]
+"matfree/backend/testing.py" = ["D103"]
+"matfree/backend/time.py" = ["D103"]
```

### Comparing `matfree-0.0.2/setup.cfg` & `matfree-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `matfree-0.0.2/tests/test_autodiff.py` & `matfree-0.0.3/tests/test_slq.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-"""Tests for (selected) autodiff functionality."""
-
+"""Tests for Lanczos functionality."""
 
 from matfree import montecarlo, slq, test_util
-from matfree.backend import np, prng, testing
+from matfree.backend import linalg, np, prng, testing
 
 
-@testing.fixture
+@testing.fixture()
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
-    d = np.arange(n) + 10.0
+    d = np.arange(n) / n + 1.0
     d = d.at[num_significant_eigvals:].set(0.001)
 
     return test_util.generate_symmetric_matrix_from_eigvals(d)
 
 
 @testing.parametrize("n", [200])
 @testing.parametrize("num_significant_eigvals", [30])
 @testing.parametrize("order", [10])
 # usually: ~1.5 * num_significant_eigvals.
 # But logdet seems to converge sooo much faster.
 def test_logdet(A, order):
-    """Assert that log-determinant computation admits valid VJPs and JVPs."""
-    key = prng.PRNGKey(1)
-
-    def fun(s):
-        return _logdet(s, order, key)
-
-    testing.check_grads(fun, (A,), order=1, atol=1e-1, rtol=1e-1)
-
-
-def _logdet(A, order, key):
+    """Assert that the log-determinant estimation matches the true log-determinant."""
     n, _ = np.shape(A)
+    key = prng.prng_key(1)
     fun = montecarlo.normal(shape=(n,))
-    received, num_nans = slq.trace_of_matfun(
-        np.log,
+    received = slq.logdet(
         lambda v: A @ v,
         order,
         key=key,
         num_samples_per_batch=10,
         num_batches=1,
         sample_fun=fun,
     )
-    return received
+    expected = linalg.slogdet(A)[1]
+    print_if_assert_fails = ("error", np.abs(received - expected), "target:", expected)
+    assert np.allclose(received, expected, atol=1e-2, rtol=1e-2), print_if_assert_fails
```

### Comparing `matfree-0.0.2/tests/test_decomp.py` & `matfree-0.0.3/tests/test_decomp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Tests for Lanczos functionality."""
 
 from matfree import decomp, test_util
-from matfree.backend import np, prng, testing
+from matfree.backend import linalg, np, prng, testing
 
 
-@testing.fixture
+@testing.fixture()
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
     d = np.arange(n) + 10.0
     d = d.at[num_significant_eigvals:].set(0.001)
 
     return test_util.generate_symmetric_matrix_from_eigvals(d)
 
 
 @testing.parametrize("n", [6])
 @testing.parametrize("num_significant_eigvals", [4])
 def test_tridiagonal_error_for_too_high_order(A):
     """Assert graceful failure if the depth matches or exceeds the number of columns."""
     n, _ = np.shape(A)
-    key = prng.PRNGKey(1)
+    key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
     with testing.raises(ValueError):
         alg = decomp.lanczos(n + 10)
         _ = decomp.decompose_fori_loop(0, n + 10, lambda v: A @ v, v0, alg=alg)
     with testing.raises(ValueError):
         alg = decomp.lanczos(n)
         _ = decomp.decompose_fori_loop(0, n + 1, lambda v: A @ v, v0, alg=alg)
@@ -31,15 +31,15 @@
 
 @testing.parametrize("n", [6])
 @testing.parametrize("num_significant_eigvals", [6])
 def test_tridiagonal_max_order(A):
     """If m == n, the matrix should be equal to the full tridiagonal."""
     n, _ = np.shape(A)
     order = n - 1
-    key = prng.PRNGKey(1)
+    key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
     alg = decomp.lanczos(order)
     Q, (d_m, e_m) = decomp.decompose_fori_loop(
         0, order + 1, lambda v: A @ v, v0, alg=alg
     )
 
     # Lanczos is not stable.
@@ -47,22 +47,22 @@
 
     # Since full-order mode: Q must be unitary
     assert np.shape(Q) == (order + 1, n)
     assert np.allclose(Q @ Q.T, np.eye(n), **tols_decomp), Q @ Q.T
     assert np.allclose(Q.T @ Q, np.eye(n), **tols_decomp), Q.T @ Q
 
     # T = Q A Qt
-    T = np.diagonal(d_m) + np.diagonal(e_m, -1) + np.diagonal(e_m, 1)
+    T = _sym_tridiagonal_dense(d_m, e_m)
     QAQt = Q @ A @ Q.T
     assert np.shape(T) == (order + 1, order + 1)
 
     # Fail early if the (off)diagonals don't coincide
-    assert np.allclose(np.diagonal(QAQt), d_m, **tols_decomp)
-    assert np.allclose(np.diagonal(QAQt, 1), e_m, **tols_decomp)
-    assert np.allclose(np.diagonal(QAQt, -1), e_m, **tols_decomp)
+    assert np.allclose(linalg.diagonal(QAQt), d_m, **tols_decomp)
+    assert np.allclose(linalg.diagonal(QAQt, 1), e_m, **tols_decomp)
+    assert np.allclose(linalg.diagonal(QAQt, -1), e_m, **tols_decomp)
 
     # Test the full decomposition
     # (i.e. assert that the off-tridiagonal elements are actually small)
     # be loose with this test. off-diagonal elements accumulate quickly.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
     assert np.allclose(QAQt, T, **tols_decomp)
 
@@ -74,31 +74,38 @@
 
 @testing.parametrize("n", [50])
 @testing.parametrize("num_significant_eigvals", [4])
 @testing.parametrize("order", [6])  # ~1.5 * num_significant_eigvals
 def test_tridiagonal(A, order):
     """Test that Lanczos tridiagonalisation yields an orthogonal-tridiagonal decomp."""
     n, _ = np.shape(A)
-    key = prng.PRNGKey(1)
+    key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
     alg = decomp.lanczos(order)
     Q, tridiag = decomp.decompose_fori_loop(0, order + 1, lambda v: A @ v, v0, alg=alg)
     (d_m, e_m) = tridiag
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     assert np.shape(Q) == (order + 1, n)
     assert np.allclose(Q @ Q.T, np.eye(order + 1), **tols_decomp), Q @ Q.T
 
     # T = Q A Qt
-    T = np.diagonal(d_m) + np.diagonal(e_m, -1) + np.diagonal(e_m, 1)
+    T = _sym_tridiagonal_dense(d_m, e_m)
     QAQt = Q @ A @ Q.T
     assert np.shape(T) == (order + 1, order + 1)
 
     # Fail early if the (off)diagonals don't coincide
-    assert np.allclose(np.diagonal(QAQt), d_m, **tols_decomp)
-    assert np.allclose(np.diagonal(QAQt, 1), e_m, **tols_decomp)
-    assert np.allclose(np.diagonal(QAQt, -1), e_m, **tols_decomp)
+    assert np.allclose(linalg.diagonal(QAQt), d_m, **tols_decomp)
+    assert np.allclose(linalg.diagonal(QAQt, 1), e_m, **tols_decomp)
+    assert np.allclose(linalg.diagonal(QAQt, -1), e_m, **tols_decomp)
 
     # Test the full decompoisition
     assert np.allclose(QAQt, T, **tols_decomp)
+
+
+def _sym_tridiagonal_dense(d, e):
+    diag = linalg.diagonal_matrix(d)
+    offdiag1 = linalg.diagonal_matrix(e, 1)
+    offdiag2 = linalg.diagonal_matrix(e, -1)
+    return diag + offdiag1 + offdiag2
```

### Comparing `matfree-0.0.2/tests/test_hutch.py` & `matfree-0.0.3/tests/test_hutch.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     return f
 
 
 @testing.fixture(name="key")
 def fixture_key():
     """Fix a pseudo-random number generator."""
-    return prng.PRNGKey(seed=1)
+    return prng.prng_key(seed=1)
 
 
 @testing.parametrize("num_batches", [1_000])
 @testing.parametrize("num_samples_per_batch", [1_000])
 @testing.parametrize("dim", [1, 10])
 @testing.parametrize("sample_fun", [montecarlo.normal, montecarlo.rademacher])
 def test_frobeniusnorm_squared(
@@ -38,15 +38,15 @@
     estimate = hutch.frobeniusnorm_squared(
         jvp,
         num_batches=num_batches,
         key=key,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
     )
-    truth = np.trace(J.T @ J)
+    truth = linalg.trace(J.T @ J)
     assert np.allclose(estimate, truth, rtol=1e-2)
 
 
 @testing.parametrize("num_batches", [1_000])
 @testing.parametrize("num_samples_per_batch", [1_000])
 @testing.parametrize("dim", [1, 10])
 @testing.parametrize("sample_fun", [montecarlo.normal, montecarlo.rademacher])
@@ -62,15 +62,15 @@
     estimate = hutch.trace(
         jvp,
         num_batches=num_batches,
         key=key,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
     )
-    truth = np.trace(J)
+    truth = linalg.trace(J)
     assert np.allclose(estimate, truth, rtol=1e-2)
 
 
 @testing.parametrize("num_batches", [1_000])
 @testing.parametrize("num_samples_per_batch", [1_000])
 @testing.parametrize("dim", [1, 10])
 @testing.parametrize("sample_fun", [montecarlo.normal, montecarlo.rademacher])
@@ -86,31 +86,32 @@
     estimate = hutch.diagonal(
         jvp,
         num_batches=num_batches,
         key=key,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
     )
-    truth = np.diagonal(J)
+    truth = linalg.diagonal(J)
     assert np.allclose(estimate, truth, rtol=1e-2)
 
 
 @testing.parametrize("num_samples", [10_000])
 @testing.parametrize("dim", [5])
 @testing.parametrize("sample_fun", [montecarlo.normal, montecarlo.rademacher])
 def test_trace_and_diagonal(fun, key, num_samples, dim, sample_fun):
     """Assert that the estimated trace and diagonal approximations are accurate."""
     # Linearise function
     x0 = prng.uniform(key, shape=(dim,))
     _, jvp = func.linearize(fun, x0)
     J = func.jacfwd(fun)(x0)
 
-    # Sequential batches
-    keys = prng.split(key, num=num_samples)
-
     # Estimate the trace
     fun = sample_fun(shape=np.shape(x0), dtype=np.dtype(x0))
-    trace, diag = hutch.trace_and_diagonal(jvp, keys=keys, sample_fun=fun)
-    assert np.allclose(diag, np.diagonal(J), rtol=1e-2), linalg.norm(
-        diag - np.diagonal(J)
+    trace, diag = hutch.trace_and_diagonal(
+        jvp, key=key, num_levels=num_samples, sample_fun=fun
     )
-    assert np.allclose(trace, np.trace(J), rtol=1e-2), linalg.norm(trace - np.trace(J))
+
+    # Print errors if test fails
+    error_diag = linalg.vector_norm(diag - linalg.diagonal(J))
+    error_trace = linalg.vector_norm(trace - linalg.trace(J))
+    assert np.allclose(diag, linalg.diagonal(J), rtol=1e-2), error_diag
+    assert np.allclose(trace, linalg.trace(J), rtol=1e-2), error_trace
```

### Comparing `matfree-0.0.2/tests/test_slq.py` & `matfree-0.0.3/tests/test_autodiff.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""Tests for Lanczos functionality."""
+"""Tests for (selected) autodiff functionality."""
+
 
 from matfree import montecarlo, slq, test_util
-from matfree.backend import linalg, np, prng, testing
+from matfree.backend import np, prng, testing
 
 
-@testing.fixture
+@testing.fixture()
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
     d = np.arange(n) + 10.0
     d = d.at[num_significant_eigvals:].set(0.001)
 
     return test_util.generate_symmetric_matrix_from_eigvals(d)
@@ -16,23 +17,27 @@
 
 @testing.parametrize("n", [200])
 @testing.parametrize("num_significant_eigvals", [30])
 @testing.parametrize("order", [10])
 # usually: ~1.5 * num_significant_eigvals.
 # But logdet seems to converge sooo much faster.
 def test_logdet(A, order):
-    """Assert that the log-determinant estimation matches the true log-determinant."""
+    """Assert that log-determinant computation admits valid VJPs and JVPs."""
+    key = prng.prng_key(1)
+
+    def fun(s):
+        return _logdet(s, order, key)
+
+    testing.check_grads(fun, (A,), order=1, atol=1e-1, rtol=1e-1)
+
+
+def _logdet(A, order, key):
     n, _ = np.shape(A)
-    key = prng.PRNGKey(1)
     fun = montecarlo.normal(shape=(n,))
-    received, num_nans = slq.trace_of_matfun(
-        np.log,
+    return slq.logdet(
         lambda v: A @ v,
         order,
         key=key,
         num_samples_per_batch=10,
         num_batches=1,
         sample_fun=fun,
     )
-    expected = linalg.slogdet(A)[1]
-    print_if_assert_fails = ("error", np.abs(received - expected), "target:", expected)
-    assert np.allclose(received, expected, atol=1e-2, rtol=1e-2), print_if_assert_fails
```

