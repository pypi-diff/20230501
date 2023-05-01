# Comparing `tmp/spacy_wrap-1.4.1.tar.gz` & `tmp/spacy_wrap-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_wrap-1.4.1.tar", last modified: Tue Feb 14 20:51:43 2023, max compression
+gzip compressed data, was "spacy_wrap-1.4.2.tar", last modified: Mon May  1 20:30:26 2023, max compression
```

## Comparing `spacy_wrap-1.4.1.tar` & `spacy_wrap-1.4.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.713708 spacy_wrap-1.4.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.709708 spacy_wrap-1.4.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.709708 spacy_wrap-1.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      731 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      617 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.709708 spacy_wrap-1.4.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1141 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2842 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      213 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      801 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     2526 2023-02-14 20:51:34.000000 spacy_wrap-1.4.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2760 2023-02-14 20:51:43.713708 spacy_wrap-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      393 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.709708 spacy_wrap-1.4.1/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.709708 spacy_wrap-1.4.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     4286 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   289957 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   289957 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)     4325 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2504 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      584 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)     1768 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)      930 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/docs/wrap.pipeline_component.rst
--rw-r--r--   0 root         (0) root         (0)     3648 2023-02-14 20:51:34.000000 spacy_wrap-1.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     7152 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-14 20:51:43.713708 spacy_wrap-1.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.705708 spacy_wrap-1.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.709708 spacy_wrap-1.4.1/src/spacy_wrap/
--rw-r--r--   0 root         (0) root         (0)      486 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      239 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/about.py
--rw-r--r--   0 root         (0) root         (0)     5999 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/architectures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.713708 spacy_wrap-1.4.1/src/spacy_wrap/layers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/layers/clf_transformer_model.py
--rw-r--r--   0 root         (0) root         (0)    15473 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/pipeline_component_seq_clf.py
--rw-r--r--   0 root         (0) root         (0)    20386 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/pipeline_component_tok_clf.py
--rw-r--r--   0 root         (0) root         (0)     5022 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/src/spacy_wrap/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.713708 spacy_wrap-1.4.1/src/spacy_wrap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2760 2023-02-14 20:51:43.000000 spacy_wrap-1.4.1/src/spacy_wrap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2023-02-14 20:51:43.000000 spacy_wrap-1.4.1/src/spacy_wrap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 20:51:43.000000 spacy_wrap-1.4.1/src/spacy_wrap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      499 2023-02-14 20:51:43.000000 spacy_wrap-1.4.1/src/spacy_wrap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      689 2023-02-14 20:51:43.000000 spacy_wrap-1.4.1/src/spacy_wrap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-14 20:51:43.000000 spacy_wrap-1.4.1/src/spacy_wrap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 20:51:43.713708 spacy_wrap-1.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3480 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/tests/test_seq_clf_transformer.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-02-14 20:51:33.000000 spacy_wrap-1.4.1/tests/test_tok_clf_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      617 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      213 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-05-01 20:30:15.000000 spacy_wrap-1.4.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      393 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   289957 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   289957 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)     4325 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      584 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)      930 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/wrap.pipeline_component.rst
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-01 20:30:15.000000 spacy_wrap-1.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     7395 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.610149 spacy_wrap-1.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/src/spacy_wrap/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/about.py
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/architectures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/src/spacy_wrap/layers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/layers/clf_transformer_model.py
+-rw-r--r--   0 root         (0) root         (0)    15473 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_seq_clf.py
+-rw-r--r--   0 root         (0) root         (0)    20386 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_tok_clf.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/tests/test_seq_clf_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/tests/test_tok_clf_transformer.py
```

### Comparing `spacy_wrap-1.4.1/.github/ISSUE_TEMPLATE/01_bugs.md` & `spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.github/ISSUE_TEMPLATE/config.yml` & `spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.github/dependabot.yml` & `spacy_wrap-1.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.github/workflows/dependabot_automerge.yml` & `spacy_wrap-1.4.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.github/workflows/documentation.yml` & `spacy_wrap-1.4.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.github/workflows/release.yml` & `spacy_wrap-1.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.github/workflows/stale.yml` & `spacy_wrap-1.4.2/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.github/workflows/tests.yml` & `spacy_wrap-1.4.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/.pre-commit-config.yaml` & `spacy_wrap-1.4.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 default_stages: [commit, push]
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
 
   - repo: https://github.com/bwhmather/ssort
     rev: v0.11.6
     hooks:
       - id: ssort
 
   - repo: https://github.com/asottile/add-trailing-comma
     rev: v2.4.0
     hooks:
       - id: add-trailing-comma
 
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.6.0.rc1
+    rev: v1.6.4
     hooks:
       - id: docformatter
         args: [--in-place]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: [--line-length, "88"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.246
+    rev: v0.0.263
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.0
+    rev: v1.2.0
     hooks:
       - id: mypy
```

### Comparing `spacy_wrap-1.4.1/CHANGELOG.md` & `spacy_wrap-1.4.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.2 (2023-05-01)
+### Fix
+* Relaxed upper bound of dev. dependencies ([`f9c8a87`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/f9c8a878ef0d4a03019925bb97af658a4a2bf658))
+
+### Documentation
+* Update errors in example in readme ([`25063be`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/25063bee591c70ce6b335e46acbef4ea8dea103b))
+
 ## v1.4.1 (2023-02-14)
 ### Fix
 * Now properly handles sequences longer than window size ([`338117e`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/338117ef265876410b10914b6438815b524a3f9a))
 
 ## v1.4.0 (2023-01-30)
 ### Feature
 * Fixed indexerror for emojis in tokens models ([`4c6a64a`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/4c6a64ab445bb4f8d59359ee2add64d83fd4fb70))
```

### Comparing `spacy_wrap-1.4.1/LICENSE` & `spacy_wrap-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/PKG-INFO` & `spacy_wrap-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy_wrap
-Version: 1.4.1
+Version: 1.4.2
 Summary: Wrappers for including pre-trained transformers in spaCy pipelines
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spacy_wrap-1.4.1/docs/Makefile` & `spacy_wrap-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/_static/favicon.ico` & `spacy_wrap-1.4.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/_static/icon.png` & `spacy_wrap-1.4.2/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/_static/icon_dark.png` & `spacy_wrap-1.4.2/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/conf.py` & `spacy_wrap-1.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/faq.rst` & `spacy_wrap-1.4.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/index.rst` & `spacy_wrap-1.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/installation.rst` & `spacy_wrap-1.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/news.rst` & `spacy_wrap-1.4.2/docs/news.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/docs/wrap.pipeline_component.rst` & `spacy_wrap-1.4.2/docs/wrap.pipeline_component.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/pyproject.toml` & `spacy_wrap-1.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spacy_wrap"
-version = "1.4.1"
+version = "1.4.2"
 description = "Wrappers for including pre-trained transformers in spaCy pipelines"
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -40,27 +40,27 @@
 repository = "https://github.com/KennethEnevoldsen/spacy-wrap"
 documentation = "https://kennethenevoldsen.github.io/spacy-wrap/"
 
 [project.optional-dependencies]
 style = [
     "black==22.12.0",
     "pre-commit>=2.20.0,<2.21.0",
-    "ruff==0.0.191",
+    "ruff==0.0.263",
     "mypy==0.991"
 ]
 tests = [
     "pytest>=7.1.3,<7.3.0",
     "pytest-cov>=3.0.0,<3.0.1",
 ]
 docs = [
-    "sphinx>=5.3.0,<5.4.0",
-    "furo==2022.12.7",
-    "sphinx-copybutton>=0.5.1,<0.5.2",
-    "sphinxext-opengraph>=0.7.3,<0.7.4",
-    "sphinx_design>=0.3.0,<0.3.1",
+    "sphinx>=5.3.0",
+    "furo>=2022.12.7",
+    "sphinx-copybutton>=0.5.1",
+    "sphinxext-opengraph>=0.7.3",
+    "sphinx_design>=0.3.0",
 ]
 cuda = ["cupy>=5.0.0b4"]
 cuda80 = ["cupy-cuda80>=5.0.0b4"]
 cuda90 = ["cupy-cuda90>=5.0.0b4"]
 cuda91 = ["cupy-cuda91>=5.0.0b4"]
 cuda92 = ["cupy-cuda92>=5.0.0b4"]
 cuda100 = ["cupy-cuda100>=5.0.0b4"]
```

### Comparing `spacy_wrap-1.4.1/readme.md` & `spacy_wrap-1.4.2/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -117,42 +117,45 @@
 We can also use the model for token classification: 
 
 ```python
 import spacy
 import spacy_wrap
 nlp = spacy.blank("en")
 
-config = {"model": {"name": "vblagoje/bert-english-uncased-finetuned-pos"}}
+config = {"model": {"name": "vblagoje/bert-english-uncased-finetuned-pos"}, 
+          # "predictions_to": ["pos"]  # optional, can be "pos", "tag" or "ents"
+}
 
-nlp.add_pipe("token_classification_transformer", config=config)
+snlp.add_pipe("token_classification_transformer", config=config)
 
 text = "My name is Wolfgang and I live in Berlin"
 
 doc = nlp(text)
-doc._.tok_clf_predictions
-# ['O', 'O', 'O', 'B-PER', 'O', 'O', 'O', 'O', 'B-LOC', 'O']
+print(doc._.tok_clf_predictions)
+# ['PRON', 'NOUN', 'AUX', 'PROPN', 'CCONJ', 'PRON', 'VERB', 'ADP', 'PROPN']
 ```
 
 By default, spacy-wrap will automatically detect it the labels follow the universal POS tags as well. If so it will also assign it to the `token.pos`, similar regular spacy pipelines:
 
 ```python
-doc[0].pos_
+print(doc[0].pos_)
 # 'PRON'
 ```
 
 ### Named Entity Recognition
 In this example, we use a model fine-tuned for named entity recognition. spacy-wrap will in this case infer from the IOB tags that the model is intended for named entity recognition and assign it to `doc.ents`.
 
 ```python
 import spacy
 import spacy_wrap
 nlp = spacy.blank("en")
 
 # specify model from the hub
-config = {"model": {"name": "dslim/bert-base-NER"}}
+config = {"model": {"name": "dslim/bert-base-NER"}, 
+          "predictions_to": ["ents"]} # forced to be named entity recognition, if left out it will be estimated from the labels
 
 # add it to the pipe
 nlp.add_pipe("token_classification_transformer", config=config)
 
 doc = nlp("My name is Wolfgang and I live in Berlin.")
 
 print(doc.ents)
```

#### html2text {}

```diff
@@ -54,36 +54,40 @@
 nlp.add_pipe("classification_transformer", config=config) doc = nlp("Senile
 gamle idiot") # old senile idiot doc._.clf_trf_data # TransformerData
 (wordpieces=... doc._.hate_speech # "Hate speech" doc._.hate_speech_prob #
 {'prob': array([0.013, 0.987], dtype=float32), 'labels': ['Not hate Speech',
 'Hate speech']} ```
 ### Token Classification We can also use the model for token classification:
 ```python import spacy import spacy_wrap nlp = spacy.blank("en") config =
-{"model": {"name": "vblagoje/bert-english-uncased-finetuned-pos"}} nlp.add_pipe
-("token_classification_transformer", config=config) text = "My name is Wolfgang
-and I live in Berlin" doc = nlp(text) doc._.tok_clf_predictions # ['O', 'O',
-'O', 'B-PER', 'O', 'O', 'O', 'O', 'B-LOC', 'O'] ``` By default, spacy-wrap will
-automatically detect it the labels follow the universal POS tags as well. If so
-it will also assign it to the `token.pos`, similar regular spacy pipelines:
-```python doc[0].pos_ # 'PRON' ``` ### Named Entity Recognition In this
-example, we use a model fine-tuned for named entity recognition. spacy-wrap
-will in this case infer from the IOB tags that the model is intended for named
-entity recognition and assign it to `doc.ents`. ```python import spacy import
-spacy_wrap nlp = spacy.blank("en") # specify model from the hub config =
-{"model": {"name": "dslim/bert-base-NER"}} # add it to the pipe nlp.add_pipe
-("token_classification_transformer", config=config) doc = nlp("My name is
-Wolfgang and I live in Berlin.") print(doc.ents) # (Wolfgang, Berlin) ``` #
-ð Documentation | Documentation | | | -------------------------- | ---------
----------------------------------- | | ð§ **[Installation]** | Installation
-instructions for spacy-wrap. | | ð° **[News and changelog]** | New additions,
-changes and version history. | | ð **[Documentation]** | The reference for
-spacy-wrap's API. | [Documentation]: https://kennethenevoldsen.github.io/spacy-
-wrap/index.html [Installation]: https://kennethenevoldsen.github.io/spacy-wrap/
-installation.html [News and changelog]: https://kennethenevoldsen.github.io/
-spacy-wrap/news.html # ð¬ Where to ask questions | Type | | | ---------------
---------------- | ---------------------- | | ð¨ **FAQ** | [FAQ] | | ð¨
-**Bug Reports** | [GitHub Issue Tracker] | | ð **Feature Requests & Ideas**
-| [GitHub Issue Tracker] | | ð©âð» **Usage Questions** | [GitHub
-Discussions] | | ð¯ **General Discussion** | [GitHub Discussions] | [FAQ]:
-https://kennethenevoldsen.github.io/spacy-wrap/faq.html [github issue tracker]:
-https://github.com/kennethenevoldsen/spacy-wrap/issues [github discussions]:
-https://github.com/kennethenevoldsen/spacy-wrap/discussions
+{"model": {"name": "vblagoje/bert-english-uncased-finetuned-pos"}, #
+"predictions_to": ["pos"] # optional, can be "pos", "tag" or "ents" }
+snlp.add_pipe("token_classification_transformer", config=config) text = "My
+name is Wolfgang and I live in Berlin" doc = nlp(text) print
+(doc._.tok_clf_predictions) # ['PRON', 'NOUN', 'AUX', 'PROPN', 'CCONJ', 'PRON',
+'VERB', 'ADP', 'PROPN'] ``` By default, spacy-wrap will automatically detect it
+the labels follow the universal POS tags as well. If so it will also assign it
+to the `token.pos`, similar regular spacy pipelines: ```python print(doc
+[0].pos_) # 'PRON' ``` ### Named Entity Recognition In this example, we use a
+model fine-tuned for named entity recognition. spacy-wrap will in this case
+infer from the IOB tags that the model is intended for named entity recognition
+and assign it to `doc.ents`. ```python import spacy import spacy_wrap nlp =
+spacy.blank("en") # specify model from the hub config = {"model": {"name":
+"dslim/bert-base-NER"}, "predictions_to": ["ents"]} # forced to be named entity
+recognition, if left out it will be estimated from the labels # add it to the
+pipe nlp.add_pipe("token_classification_transformer", config=config) doc = nlp
+("My name is Wolfgang and I live in Berlin.") print(doc.ents) # (Wolfgang,
+Berlin) ``` # ð Documentation | Documentation | | | ------------------------
+-- | ------------------------------------------- | | ð§ **[Installation]** |
+Installation instructions for spacy-wrap. | | ð° **[News and changelog]** |
+New additions, changes and version history. | | ð **[Documentation]** | The
+reference for spacy-wrap's API. | [Documentation]: https://
+kennethenevoldsen.github.io/spacy-wrap/index.html [Installation]: https://
+kennethenevoldsen.github.io/spacy-wrap/installation.html [News and changelog]:
+https://kennethenevoldsen.github.io/spacy-wrap/news.html # ð¬ Where to ask
+questions | Type | | | ------------------------------ | ---------------------
+- | | ð¨ **FAQ** | [FAQ] | | ð¨ **Bug Reports** | [GitHub Issue Tracker] |
+| ð **Feature Requests & Ideas** | [GitHub Issue Tracker] | | ð©âð»
+**Usage Questions** | [GitHub Discussions] | | ð¯ **General Discussion** |
+[GitHub Discussions] | [FAQ]: https://kennethenevoldsen.github.io/spacy-wrap/
+faq.html [github issue tracker]: https://github.com/kennethenevoldsen/spacy-
+wrap/issues [github discussions]: https://github.com/kennethenevoldsen/spacy-
+wrap/discussions
```

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap/architectures.py` & `spacy_wrap-1.4.2/src/spacy_wrap/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap/layers/clf_transformer_model.py` & `spacy_wrap-1.4.2/src/spacy_wrap/layers/clf_transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap/pipeline_component_seq_clf.py` & `spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_seq_clf.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 stride = 96
 """
 
 DEFAULT_CONFIG = Config().from_str(DEFAULT_CONFIG_STR)
 
 
 class SequenceClassificationTransformer(TrainablePipe):
-    """spaCy pipeline component that provides access to a transformer model
+    """SpaCy pipeline component that provides access to a transformer model
     from the Huggingface transformers library. Usually you will connect
     subsequent components to the shared transformer using the
     TransformerListener layer. This works similarly to spaCy's Tok2Vec
     component and Tok2VecListener sublayer. The activations from the
     transformer are saved in the doc._.{doc_extension_trf_data} extension
     attribute. You can also provide a callback to set additional annotations.
```

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap/pipeline_component_tok_clf.py` & `spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_tok_clf.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         (bool): True if the label is an IOB tag.
     """
     label_ = label.lower()
     return label_.startswith("i-") or label_.startswith("b-") or label_ == "o"
 
 
 class TokenClassificationTransformer(TrainablePipe):
-    """spaCy pipeline component that provides access to a transformer model
+    """SpaCy pipeline component that provides access to a transformer model
     from the Huggingface transformers library.
 
     Usually you will connect subsequent components to the shared
     transformer using the TransformerListener layer. This works
     similarly to spaCy's Tok2Vec component and Tok2VecListener sublayer.
     The activations from the transformer are saved in the doc._.trf_data
     extension attribute. You can also provide a callback to set
```

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap/util.py` & `spacy_wrap-1.4.2/src/spacy_wrap/util.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap.egg-info/PKG-INFO` & `spacy_wrap-1.4.2/src/spacy_wrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-wrap
-Version: 1.4.1
+Version: 1.4.2
 Summary: Wrappers for including pre-trained transformers in spaCy pipelines
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap.egg-info/SOURCES.txt` & `spacy_wrap-1.4.2/src/spacy_wrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.1/src/spacy_wrap.egg-info/requires.txt` & `spacy_wrap-1.4.2/src/spacy_wrap.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -32,22 +32,22 @@
 [cuda91]
 cupy-cuda91>=5.0.0b4
 
 [cuda92]
 cupy-cuda92>=5.0.0b4
 
 [docs]
-sphinx<5.4.0,>=5.3.0
-furo==2022.12.7
-sphinx-copybutton<0.5.2,>=0.5.1
-sphinxext-opengraph<0.7.4,>=0.7.3
-sphinx_design<0.3.1,>=0.3.0
+sphinx>=5.3.0
+furo>=2022.12.7
+sphinx-copybutton>=0.5.1
+sphinxext-opengraph>=0.7.3
+sphinx_design>=0.3.0
 
 [style]
 black==22.12.0
 pre-commit<2.21.0,>=2.20.0
-ruff==0.0.191
+ruff==0.0.263
 mypy==0.991
 
 [tests]
 pytest<7.3.0,>=7.1.3
 pytest-cov<3.0.1,>=3.0.0
```

### Comparing `spacy_wrap-1.4.1/tests/test_seq_clf_transformer.py` & `spacy_wrap-1.4.2/tests/test_seq_clf_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ),
 )
 
 
 class TestSequenceClassificationTransformer:
     @pytest.mark.parametrize("config, examples", EXAMPLES)
     def test_forward(self, config: dict, examples: list):
-        """tests if that the forward pass work as intended."""
+        """Tests if that the forward pass work as intended."""
         nlp = spacy.blank("en")
         nlp.add_pipe("sequence_classification_transformer", config=config)
 
         for text, label in examples:
             doc = nlp(text)
 
             trf_data_ext = (
@@ -83,15 +83,15 @@
             if "assign_to_cats" not in config or config["assign_to_cats"]:
                 if label:
                     assert max(doc.cats, key=doc.cats.get) == label
             else:
                 assert doc.cats == {}
 
     def test_to_and_from_disk(self):
-        """tests if the pipeline can be serialized to disk."""
+        """Tests if the pipeline can be serialized to disk."""
         nlp = spacy.blank("da")
         config = {
             "doc_extension_trf_data": "clf_trf_data",
             "doc_extension_prediction": "hate_speech",
             "labels": ["Not hate Speech", "Hate speech"],
             "model": {
                 "name": "alexandrainst/da-hatespeech-detection-base",
```

### Comparing `spacy_wrap-1.4.1/tests/test_tok_clf_transformer.py` & `spacy_wrap-1.4.2/tests/test_tok_clf_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     ),
 )
 
 
 class TestTokenClassificationTransformer:
     @pytest.mark.parametrize("config, example", EXAMPLES_NER)
     def test_forward_ner(self, config: dict, example: tuple):
-        """tests if that the forward pass work as intended for NER models."""
+        """Tests if that the forward pass work as intended for NER models."""
         nlp = spacy.blank("es")
         nlp.add_pipe("token_classification_transformer", config=config)
 
         text, expected = example
         doc = nlp(text)
 
         trf_data_ext = (
@@ -147,25 +147,25 @@
             assert ent.text == text
             assert ent.start == start
             assert ent.end == end
             assert ent.label_ == label
 
     @pytest.mark.parametrize("config, example", EXAMPLES_POS)
     def test_forward_pos(self, config: dict, example: tuple):
-        """tests if that the forward pass work as intended for POS models."""
+        """Tests if that the forward pass work as intended for POS models."""
         nlp = spacy.blank("en")
         nlp.add_pipe("token_classification_transformer", config=config)
         text, expected = example
         doc = nlp(text)
 
         for token, label in zip(doc, expected):
             assert token.pos_ == label
 
     def test_to_and_from_disk(self):
-        """tests if the pipeline can be serialized to disk."""
+        """Tests if the pipeline can be serialized to disk."""
         nlp = spacy.blank("en")
         nlp.add_pipe("token_classification_transformer", config=EXAMPLES_NER[0][0])
 
         transformer = nlp.get_pipe("token_classification_transformer")
 
         transformer.to_disk("spacy_wrap_serialization_test")
         transformer.from_disk("spacy_wrap_serialization_test")
```

