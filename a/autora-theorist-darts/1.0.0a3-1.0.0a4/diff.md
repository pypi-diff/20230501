# Comparing `tmp/autora-theorist-darts-1.0.0a3.tar.gz` & `tmp/autora-theorist-darts-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-darts-1.0.0a3.tar", last modified: Thu Apr 27 20:19:13 2023, max compression
+gzip compressed data, was "autora-theorist-darts-1.0.0a4.tar", last modified: Mon May  1 16:04:21 2023, max compression
```

## Comparing `autora-theorist-darts-1.0.0a3.tar` & `autora-theorist-darts-1.0.0a4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/autora-darts.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/how_it_works.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   681971 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/img/darts_computation_graph.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/meta_parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/search_space.md
--rw-r--r--   0 runner    (1001) docker     (123)   796099 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/architect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/fan_out.py
--rw-r--r--   0 runner    (1001) docker     (123)    30660 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/model_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/tests/test_sklearn_darts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.365971 autora-theorist-darts-1.0.0a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.337969 autora-theorist-darts-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.345970 autora-theorist-darts-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.349970 autora-theorist-darts-1.0.0a4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.idea/autora-darts.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.349970 autora-theorist-darts-1.0.0a4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-01 16:04:21.365971 autora-theorist-darts-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.353970 autora-theorist-darts-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/how_it_works.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.353970 autora-theorist-darts-1.0.0a4/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   681971 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/img/darts_computation_graph.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.357970 autora-theorist-darts-1.0.0a4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/meta_parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/search_space.md
+-rw-r--r--   0 runner    (1001) docker     (123)   796098 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/docs/weber.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.357970 autora-theorist-darts-1.0.0a4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:04:21.365971 autora-theorist-darts-1.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.341970 autora-theorist-darts-1.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.341970 autora-theorist-darts-1.0.0a4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.341970 autora-theorist-darts-1.0.0a4/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.361971 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/architect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/fan_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30660 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/model_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.365971 autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-01 16:04:21.000000 autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-01 16:04:21.000000 autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:04:21.000000 autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-01 16:04:21.000000 autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 16:04:21.000000 autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:21.365971 autora-theorist-darts-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-05-01 16:03:44.000000 autora-theorist-darts-1.0.0a4/tests/test_sklearn_darts.py
```

### Comparing `autora-theorist-darts-1.0.0a3/.github/workflows/python-publish.yml` & `autora-theorist-darts-1.0.0a4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/.gitignore` & `autora-theorist-darts-1.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/.idea/autora-darts.iml` & `autora-theorist-darts-1.0.0a4/.idea/autora-darts.iml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-darts-1.0.0a4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/.pre-commit-config.yaml` & `autora-theorist-darts-1.0.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/PKG-INFO` & `autora-theorist-darts-1.0.0a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: autora-theorist-darts
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Differentiable Architecture Search theorist for AutoRA
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
-Project-URL: homepage, https://www.empiricalresearch.ai
+Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-darts
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA DARTS Theorist
 
@@ -24,15 +24,15 @@
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
   [https://graphviz.org/download/](https://graphviz.org/download/)
 
 Install DARTS as part of the `autora` package:
 
 ```shell
-pip install -U "autora[theorist-darts]"
+pip install -U "autora-theorist-darts"
 ```
 
 > It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
 python -c "from autora.theorist.darts import DARTSRegressor; DARTSRegressor()"
```

### Comparing `autora-theorist-darts-1.0.0a3/README.md` & `autora-theorist-darts-1.0.0a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
   [https://graphviz.org/download/](https://graphviz.org/download/)
 
 Install DARTS as part of the `autora` package:
 
 ```shell
-pip install -U "autora[theorist-darts]"
+pip install -U "autora-theorist-darts"
 ```
 
 > It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
 python -c "from autora.theorist.darts import DARTSRegressor; DARTSRegressor()"
```

### Comparing `autora-theorist-darts-1.0.0a3/docs/example.ipynb` & `autora-theorist-darts-1.0.0a4/docs/example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995098039215686%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '# !pip install autora-theorist-darts')], delete: [1]}}}"}*

```diff
@@ -16,15 +16,15 @@
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Uncomment the following line when running on Google Colab\n",
-                "# !pip install autora[theorist-darts]"
+                "# !pip install autora-theorist-darts"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
```

### Comparing `autora-theorist-darts-1.0.0a3/docs/how_it_works.md` & `autora-theorist-darts-1.0.0a4/docs/how_it_works.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/docs/img/darts_computation_graph.jpg` & `autora-theorist-darts-1.0.0a4/docs/img/darts_computation_graph.jpg`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/docs/index.md` & `autora-theorist-darts-1.0.0a4/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/docs/meta_parameters.md` & `autora-theorist-darts-1.0.0a4/docs/meta_parameters.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/docs/quickstart.md` & `autora-theorist-darts-1.0.0a4/docs/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
   [https://graphviz.org/download/](https://graphviz.org/download/)
 
 Install DARTS as part of the `autora` package:
 
 ```shell
-pip install -U "autora[theorist-darts]"
+pip install -U "autora-theorist-darts"
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
```

### Comparing `autora-theorist-darts-1.0.0a3/docs/search_space.md` & `autora-theorist-darts-1.0.0a4/docs/search_space.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/docs/weber.ipynb` & `autora-theorist-darts-1.0.0a4/docs/weber.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '# !pip install autora-theorist-darts')], delete: [1]}}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Uncomment the following line when running on Google Colab\n",
-                "# !pip install autora[theorist-darts]"
+                "# !pip install autora-theorist-darts"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
```

### Comparing `autora-theorist-darts-1.0.0a3/mkdocs/base.yml` & `autora-theorist-darts-1.0.0a4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/mkdocs/gen_ref_pages.py` & `autora-theorist-darts-1.0.0a4/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/mkdocs.yml` & `autora-theorist-darts-1.0.0a4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/pyproject.toml` & `autora-theorist-darts-1.0.0a4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [project]
-# UPDATE THIS BEFORE PUBLISHING
 name = "autora-theorist-darts"
 description = "Differentiable Architecture Search theorist for AutoRA"
 authors = [
   { name = "Sebastian Musslick", email = "sebastian_musslick@brown.edu" },
   { name = "John Gerrard Holland", email = "john_holland1@brown.edu" },
 ]
 dynamic = ["version"]
@@ -18,19 +17,20 @@
     "matplotlib",
     "graphviz",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "autora-core[dev]"
+    "autora-core[dev]",
+    "autora-synthetic-data"
 ]
 
 [project.urls]
-homepage = "https://www.empiricalresearch.ai"
+homepage = "http://www.empiricalresearch.ai"
 repository = "https://github.com/AutoResearch/autora-theorist-darts"
 documentation = "https://autoresearch.github.io/autora/"
 
 [build-system]
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/architect.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/architect.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/dataset.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/dataset.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/fan_out.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/fan_out.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/model_search.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/model_search.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/operations.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/operations.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/regressor.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/utils.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/visualize.py` & `autora-theorist-darts-1.0.0a4/src/autora/theorist/darts/visualize.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/PKG-INFO` & `autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: autora-theorist-darts
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Differentiable Architecture Search theorist for AutoRA
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
-Project-URL: homepage, https://www.empiricalresearch.ai
+Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-darts
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA DARTS Theorist
 
@@ -24,15 +24,15 @@
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
   [https://graphviz.org/download/](https://graphviz.org/download/)
 
 Install DARTS as part of the `autora` package:
 
 ```shell
-pip install -U "autora[theorist-darts]"
+pip install -U "autora-theorist-darts"
 ```
 
 > It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
 python -c "from autora.theorist.darts import DARTSRegressor; DARTSRegressor()"
```

### Comparing `autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/SOURCES.txt` & `autora-theorist-darts-1.0.0a4/src/autora_theorist_darts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/tests/README.md` & `autora-theorist-darts-1.0.0a4/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a3/tests/test_sklearn_darts.py` & `autora-theorist-darts-1.0.0a4/tests/test_sklearn_darts.py`

 * *Files identical despite different names*

