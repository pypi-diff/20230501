# Comparing `tmp/quartodoc-0.2.2.tar.gz` & `tmp/quartodoc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.2.2.tar", last modified: Thu Apr  6 19:24:24 2023, max compression
+gzip compressed data, was "quartodoc-0.3.0.tar", last modified: Mon May  1 17:56:58 2023, max compression
```

## Comparing `quartodoc-0.2.2.tar` & `quartodoc-0.3.0.tar`

### file list

```diff
@@ -1,101 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.879831 quartodoc-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.867831 quartodoc-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.871831 quartodoc-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-06 19:24:15.000000 quartodoc-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-06 19:24:15.000000 quartodoc-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-06 19:24:15.000000 quartodoc-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-06 19:24:15.000000 quartodoc-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-06 19:24:15.000000 quartodoc-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-06 19:24:24.879831 quartodoc-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-06 19:24:15.000000 quartodoc-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-06 19:24:15.000000 quartodoc-0.2.2/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.867831 quartodoc-0.2.2/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.871831 quartodoc-0.2.2/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/example.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/objects_siuba.json
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/objects_vetiver.inv
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-06 19:24:15.000000 quartodoc-0.2.2/_extensions/interlinks/objects_vetiver.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.871831 quartodoc-0.2.2/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-04-06 19:24:15.000000 quartodoc-0.2.2/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-06 19:24:15.000000 quartodoc-0.2.2/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-06 19:24:15.000000 quartodoc-0.2.2/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-06 19:24:15.000000 quartodoc-0.2.2/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-06 19:24:15.000000 quartodoc-0.2.2/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.871831 quartodoc-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.871831 quartodoc-0.2.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.871831 quartodoc-0.2.2/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 19:24:15.000000 quartodoc-0.2.2/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.871831 quartodoc-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/examples/shiny/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/shiny/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/shiny/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/shiny/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/shiny/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/examples/shiny/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/shiny/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/shiny/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-06 19:24:15.000000 quartodoc-0.2.2/examples/single-page/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-06 19:24:15.000000 quartodoc-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/autosummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.879831 quartodoc-0.2.2/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/tests/example_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-06 19:24:15.000000 quartodoc-0.2.2/quartodoc/tests/test_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:24:24.875831 quartodoc-0.2.2/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-06 19:24:24.000000 quartodoc-0.2.2/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-06 19:24:24.000000 quartodoc-0.2.2/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:24:24.000000 quartodoc-0.2.2/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-06 19:24:24.000000 quartodoc-0.2.2/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 19:24:24.000000 quartodoc-0.2.2/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-06 19:24:15.000000 quartodoc-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-06 19:24:24.879831 quartodoc-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.213488 quartodoc-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.217488 quartodoc-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-01 17:56:44.000000 quartodoc-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-01 17:56:44.000000 quartodoc-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 17:56:44.000000 quartodoc-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 17:56:44.000000 quartodoc-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-01 17:56:44.000000 quartodoc-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-01 17:56:58.229488 quartodoc-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-01 17:56:44.000000 quartodoc-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-01 17:56:44.000000 quartodoc-0.3.0/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.213488 quartodoc-0.3.0/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.217488 quartodoc-0.3.0/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/example.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/objects_siuba.json
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-05-01 17:56:44.000000 quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.217488 quartodoc-0.3.0/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-01 17:56:44.000000 quartodoc-0.3.0/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-01 17:56:44.000000 quartodoc-0.3.0/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.221488 quartodoc-0.3.0/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-01 17:56:44.000000 quartodoc-0.3.0/examples/single-page/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-01 17:56:44.000000 quartodoc-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.229488 quartodoc-0.3.0/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-01 17:56:44.000000 quartodoc-0.3.0/quartodoc/tests/test_renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:56:58.225488 quartodoc-0.3.0/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 17:56:58.000000 quartodoc-0.3.0/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-01 17:56:44.000000 quartodoc-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-01 17:56:58.229488 quartodoc-0.3.0/setup.cfg
```

### Comparing `quartodoc-0.2.2/.github/workflows/ci.yml` & `quartodoc-0.3.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name: "Test"
     needs: ["run-if"]
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         # Checks based on python versions ---
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.9', '3.10']
         requirements: [""]
 
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
           python-version: "${{ matrix.python-version }}"
@@ -69,24 +69,26 @@
 
   build-docs:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
-          python-version: "3.9"
+          python-version: "3.10"
       - name: Install dependencies
         run: |
           python -m pip install -r requirements-dev.txt
           python -m pip install .
           # TODO: temporary installs for examples
           # once quartodoc is stable we should move into their own libraries
           python -m pip install shiny shinylive
           python -m pip install --no-deps dascore==0.0.8
       - uses: quarto-dev/quarto-actions/setup@v2
+        with:
+          version: "1.2.475"
       - name: Build docs
         run: |
           make docs-build
       # push to netlify -------------------------------------------------------
 
       # set release name ----
 
@@ -135,10 +137,11 @@
           step: finish
           token: ${{ secrets.GITHUB_TOKEN }}
           status: ${{ job.status }}
           deployment_id: ${{ steps.deployment.outputs.deployment_id }}
           env_url: 'https://${{ steps.deployment.outputs.env }}--quartodoc.netlify.app'
           logs: 'https://github.com/${{ github.repository }}/actions/runs/${{ github.run_id }}'
       - uses: peaceiris/actions-gh-pages@v3
+        if: github.event_name == 'release'
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: docs/_build
```

### Comparing `quartodoc-0.2.2/.gitignore` & `quartodoc-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/LICENSE` & `quartodoc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/Makefile` & `quartodoc-0.3.0/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 README.md: README.qmd
 	quarto render $<
 
 examples/%/_site: examples/%/_quarto.yml
 	cd examples/$* \
 		&& quarto add --no-prompt ../.. \
 		&& quarto add --no-prompt quarto-ext/shinylive
-	cd examples/$* && python -m quartodoc build _quarto.yml --verbose
-	cd examples/$* && python -m quartodoc interlinks
+	cd examples/$* && quartodoc build _quarto.yml --verbose
+	cd examples/$* && quartodoc interlinks
 	quarto render $(dir $<)
 
 docs/examples/%: examples/%/_site
 	rm -rf docs/examples/$*
 	cp -rv $< $@
 
-docs-build-examples: docs/examples/single-page docs/examples/pkgdown docs/examples/shiny
+docs-build-examples: docs/examples/single-page docs/examples/pkgdown
 
 docs-build: docs-build-examples
 	cd docs && quarto add --no-prompt ..
-	cd docs && python -m quartodoc build
-	cd docs && python -m quartodoc interlinks
+	cd docs && quartodoc build
+	cd docs && quartodoc interlinks
 	quarto render docs
 
 requirements-dev.txt:
 	pip-compile setup.cfg --extra dev -o $@
```

### Comparing `quartodoc-0.2.2/PKG-INFO` & `quartodoc-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.2.2
+Version: 0.3.0
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: mc_al_github@fastmail.com
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # quartodoc
```

### Comparing `quartodoc-0.2.2/README.md` & `quartodoc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/README.qmd` & `quartodoc-0.3.0/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/_extensions/interlinks/README.md` & `quartodoc-0.3.0/_extensions/interlinks/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/_extensions/interlinks/example.qmd` & `quartodoc-0.3.0/_extensions/interlinks/example.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/_extensions/interlinks/interlinks.py` & `quartodoc-0.3.0/_extensions/interlinks/interlinks.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,20 @@
     url = el.url
     if (url.startswith("%60") or url.startswith(":")) and url.endswith("%60"):
         # Get URL ----
         try:
             return ref_to_anchor(url.replace("%60", "`"), el.content)
         except InvLookupError as e:
             pf.debug("WARNING: " + str(e))
+            if el.content:
+                # Assuming content is a ListContainer(Str(...))
+                body = el.content[0].text
+            else:
+                body = url.replace("%60", "")
+            return pf.Code(body)
 
     return el
 
 
 def main(doc=None):
     return pf.run_filter(visit, prepare=prepare, doc=None)
```

### Comparing `quartodoc-0.2.2/_extensions/interlinks/objects_vetiver.inv` & `quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/_extensions/interlinks/objects_vetiver.json` & `quartodoc-0.3.0/_extensions/interlinks/objects_vetiver.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/case_studies/objects_sqla.inv` & `quartodoc-0.3.0/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/case_studies/parsing.qmd` & `quartodoc-0.3.0/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/case_studies/some_package.py` & `quartodoc-0.3.0/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/case_studies/sphinx-inventory.md` & `quartodoc-0.3.0/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/case_studies/sphinx-inventory.qmd` & `quartodoc-0.3.0/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/docs/examples/index.qmd` & `quartodoc-0.3.0/docs/examples/index.qmd`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+### Demo sites
+
 | style | source | layout |
 | ----- | ------ | ------ |
 | [pkgdown] | [github][pkgdown-code] | Index page with a title and short description for functions listed in each section. Each function gets its own documentation page. |
 | [single-page] | [github][sp-code] | Index page has function documentation embedded on it. |
-| [shiny] | [github][shiny-code] | The shiny docs translated to quartodoc, using a custom renderer. |
+
+### Packages using quartodoc
+
+
+| package | source | about |
+| ----- | ------ | ------ |
+| [siuba] | [github][sb-code] | Data analysis library. |
+| [shiny][shiny] |  | Dashboarding framework. |
+| [vetiver][vetiver] | [github][vt-code] | A tool to version, share, deploy and monitor ML models. |
 
 : {tbl-colwidths="[20, 20, 60]"}
 
 [pkgdown]: /examples/pkgdown/reference
 [pkgdown-code]: https://github.com/machow/quartodoc/tree/main/examples/pkgdown
 [single-page]: /examples/single-page/reference
 [sp-code]: https://github.com/machow/quartodoc/tree/main/examples/single-page
-[shiny]: /examples/shiny/reference
-[shiny-code]: https://github.com/machow/quartodoc/tree/main/examples/shiny
+[shiny]: https://shiny.rstudio.com/py/api/
+[vetiver]: https://rstudio.github.io/vetiver-python/stable/reference/
+[vt-code]: https://github.com/rstudio/vetiver-python
+[siuba]: https://siuba.org/api/
+[sb-code]: https://github.com/machow/siuba.org
```

### Comparing `quartodoc-0.2.2/docs/get-started/architecture.qmd` & `quartodoc-0.3.0/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/docs/get-started/crossrefs.qmd` & `quartodoc-0.3.0/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/docs/get-started/docstrings.qmd` & `quartodoc-0.3.0/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/docs/get-started/extending.qmd` & `quartodoc-0.3.0/docs/get-started/extending.qmd`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-title: More Customization
+title: More customization
 ---
 
 This page details 3 common aspects of quartodoc you can extend:
 
 * The reference index page generated (which lists all your functions).
 * The way docstrings are renderered.
 * The overall building process.
@@ -60,16 +60,16 @@
 
 ```yaml
 quartodoc:
   renderer:
     style: _renderer.py
 ```
 
-See the [shiny example docs](https://github.com/machow/quartodoc/tree/main/examples/shiny), which contains a custom renderer.
-
+See the [Rendering docstrings](/get-started/renderers.qmd) page for instructions on
+creating a custom renderer, and the [](`quartodoc.MdRenderer`) docs for more information.
 
 ## Using a custom Builder
 
 Since the Builder controls the full quartodoc build process, using a custom builder
 provides total flexibility. This option currently isn't available, but would be easy
 to enable.
```

### Comparing `quartodoc-0.2.2/docs/get-started/interlinks.qmd` & `quartodoc-0.3.0/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/docs/get-started/overview.qmd` & `quartodoc-0.3.0/docs/get-started/overview.qmd`

 * *Files 27% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 jupyter:
   kernelspec:
     display_name: Python 3 (ipykernel)
     language: python
     name: python3
 ---
 
-::: {.callout-warning} 
-quartodoc is work in progress!
+::: {.callout-note} 
+quartodoc is used to create the API documentation for [shiny], [siuba], and [vetiver].
+
+It's full-featured and relatively stable, but may see some small changes in the the name of making API documentation a real delight.
+
+If you're interested in using quartodoc for your package's documentation, please open an issue, so we can make sure it does exactly what you want.
 :::
 
-quartodoc let's you quickly generate python package documentation,
+quartodoc lets you quickly generate python package documentation,
 using markdown and [quarto](https://quarto.org).
 It is designed as an alternative to Sphinx.
 
 ## Installation
 
 ```bash
 python -m pip install quartodoc
@@ -32,25 +36,24 @@
 and generating documentation pages for your library.
 
 First, create a `_quarto.yml` file with the following:
 
 ```yaml
 project:
   type: website
-  resources:
-    - objects.json
 
 quartodoc:
-  style: single-page
-  dir: reference
+  # the name used to import the package
   package: quartodoc
   sections:
     - title: Some functions
       desc: Functions to inspect docstrings.
       contents:
+        # the functions being documented in the package.
+        # you can refer to anything: class methods, modules, etc..
         - get_object
         - preview
 ```
 
 Next, run this command to generate your API pages:
 
 ```bash
@@ -62,33 +65,80 @@
 
 Finally, preview your website with quarto:
 
 ```bash
 quarto preview
 ```
 
-## Key Features
+## Rebuilding site
+
+As mentioned in the previous section, you can preview your quartodoc site using these commands:
+
+```bash
+python -m quartodoc build
+quarto preview
+```
+
+In order to rebuild your API documentation pages during a quarto preview, re-run
+the quartodoc build command:
+
+```bash
+# with quarto preview running, you only need to re-run quartodoc build,
+# which will re-create the pages of your API documentation.
+python -m quartodoc build
+```
+
+## Looking up objects
+
+Finding python objects to document involves two pieces of configuration:
+
+* the package name.
+* a list of objects for content.
+
+Note that quartodoc can look up anything---whether functions, modules, classes, attributes, or methods.
+
+```yaml
+quartodoc:
+  package: quartodoc
+  sections:
+    - title: Some section
+      desc: ""
+      contents:
+        - get_object        # function: quartodoc.get_object
+        - ast.preview       # submodule func: quartodoc.ast.preview
+        - MdRenderer        # class: quartodoc.MdRenderer
+        - MdRenderer.render # method: quartodoc.MDRenderer.render
+        - renderers         # module: quartodoc.renderers
+```
+
+The functions listed in `contents` are assumed to be imported from the package.
 
-* Load docstrings (with [griffe](https://github.com/mkdocstrings/griffe))
-* Render docstrings (e.g. with [MdRenderer](/api/#sec-MdRenderer))
-* Enable cross references to function documentation (with interlinks filter).
-  - Link to functions within a doc.
-  - Link to functions in other docs.
-  - Generate an inventory file for other docs to link to yours.
-* Generate high-level summaries (with [Builder](/api/#api-builders)).
-  - First line of docstring used as description.
-  - Class doc pages have table of class attributes.
-  - Index pages list function names and descriptions.
 
 ## Example sites
 
+### Demo sites
+
 | style | source | layout |
 | ----- | ------ | ------ |
 | [pkgdown] | [github][pkgdown-code] | Index page with a title and short description for functions listed in each section. Each function gets its own documentation page. |
 | [single-page] | [github][sp-code] | Index page has function documentation embedded on it. |
 
+### Packages using quartodoc
+
+
+| package | source | about |
+| ----- | ------ | ------ |
+| [siuba] | [github][sb-code] | Data analysis library. |
+| [shiny][shiny] |  | Dashboarding framework. |
+| [vetiver][vetiver] | [github][vt-code] | A tool to version, share, deploy and monitor ML models. |
+
 : {tbl-colwidths="[20, 20, 60]"}
 
 [pkgdown]: /examples/pkgdown/reference
 [pkgdown-code]: https://github.com/machow/quartodoc/tree/main/examples/pkgdown
 [single-page]: /examples/single-page/reference
 [sp-code]: https://github.com/machow/quartodoc/tree/main/examples/single-page
+[shiny]: https://shiny.rstudio.com/py/api/
+[vetiver]: https://rstudio.github.io/vetiver-python/stable/reference/
+[vt-code]: https://github.com/rstudio/vetiver-python
+[siuba]: https://siuba.org/api/
+[sb-code]: https://github.com/machow/siuba.org
```

### Comparing `quartodoc-0.2.2/docs/get-started/renderers.qmd` & `quartodoc-0.3.0/docs/get-started/dev-renderers.qmd`

 * *Files 9% similar despite different names*

```diff
@@ -125,7 +125,33 @@
 
 * **Generic dispatch**: The plum `dispatch` function decorates each `render` method. The type annotations
   specify the types of data each version of render should dispatch on.
 * **Default behavior**: The first `render` method ensures a `NotImplementedError` is raised by default.
 * **Tree walking**: `render` methods often call `render` again on sub elements.
 
 
+## Completing the Renderer
+
+While the above example showed a simple example with a `.render` method, a complete renderer will often do two more things:
+
+* Subclass an existing renderer.
+* Also override other methods like `.summarize()`
+
+```{python}
+from quartodoc import MdRenderer
+
+class NewRenderer(MdRenderer):
+    style = "new_renderer"
+
+    @dispatch
+    def render(self, el):
+        print("calling parent method for render")
+        return super().render(el)
+    
+    @dispatch
+    def summarize(self, el):
+        print("calling parent method for summarize")
+        return super().summarize(el)
+```
+
+For a list of methods, see the [](`~quartodoc.MdRenderer`) docs.
+
```

### Comparing `quartodoc-0.2.2/docs/get-started/sidebar.qmd` & `quartodoc-0.3.0/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/examples/dascore/_quarto.yml` & `quartodoc-0.3.0/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/examples/dascore/generate_api.py` & `quartodoc-0.3.0/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/examples/pkgdown/_quarto.yml` & `quartodoc-0.3.0/examples/pkgdown/_quarto.yml`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     theme:
       light: minty
     toc: true
 
 quartodoc:
   style: pkgdown
   dir: reference
-  display_name: relative
   package: quartodoc
   sections:
     - title: Some functions
       desc: These functions inspect and parse docstrings.
       contents:
         - get_object
         - preview
```

### Comparing `quartodoc-0.2.2/examples/pkgdown/objects.json` & `quartodoc-0.3.0/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.3.0/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.3.0/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/examples/single-page/_quarto.yml` & `quartodoc-0.3.0/examples/single-page/_quarto.yml`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,14 @@
   html:
     theme: minty
     toc: true
 
 quartodoc:
   style: single-page
   dir: reference
-  display_name: relative
   package: quartodoc
   sections:
     - title: Some functions
       desc: These functions inspect and parse docstrings.
       contents:
         - get_object
         - preview
```

### Comparing `quartodoc-0.2.2/examples/single-page/objects.json` & `quartodoc-0.3.0/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/examples/single-page/reference/index.qmd` & `quartodoc-0.3.0/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/quartodoc/__main__.py` & `quartodoc-0.3.0/quartodoc/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,27 +38,29 @@
 @click.group()
 def cli():
     pass
 
 
 @click.command()
 @click.argument("config", default="_quarto.yml")
+@click.option("--filter", nargs=1, default="*")
 @click.option("--dry-run", is_flag=True, default=False)
 @click.option("--verbose", is_flag=True, default=False)
-def build(config, dry_run, verbose):
+def build(config, filter, dry_run, verbose):
     if verbose:
         _enable_logs()
 
     builder = Builder.from_quarto_config(config)
 
     if dry_run:
-        click.echo(builder.render_index())
+        # click.echo(builder.render_index())
+        pass
     else:
         with chdir(Path(config).parent):
-            builder.build()
+            builder.build(filter=filter)
 
 
 @click.command()
 @click.argument("config", default="_quarto.yml")
 @click.option("--dry-run", is_flag=True, default=False)
 def interlinks(config, dry_run):
     cfg = yaml.safe_load(open(config))
```

### Comparing `quartodoc-0.2.2/quartodoc/ast.py` & `quartodoc-0.3.0/quartodoc/ast.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from __future__ import annotations
+
+import warnings
+
 from enum import Enum
 from dataclasses import dataclass
 from griffe.docstrings import dataclasses as ds
 from griffe import dataclasses as dc
 from plum import dispatch
 from typing import Union
+from pydantic import BaseModel  # for previewing
 
 
 # Transform and patched-in classes ============================================
 # TODO: annotate transform return types. make sure subtypes inherit from correct
 # griffe base objects.
 # TODO: it seems like transform should happen on the root, not individual elements.
 
@@ -16,16 +21,19 @@
     """Return a more specific docstring element, or simply return the original one."""
 
     if isinstance(el, tuple):
         try:
             return tuple_to_data(el)
         except ValueError:
             pass
-    elif isinstance(el, ds.DocstringSection):
-        return _DocstringSectionPatched.transform(el)
+
+    # patch a list of docstring sections. note that this has to happen on the
+    # list, since we replace single nodes on the tree (the list is the node).
+    elif isinstance(el, list) and len(el) and isinstance(el[0], dc.DocstringSection):
+        return _DocstringSectionPatched.transform_all(el)
 
     return el
 
 
 # Patch DocstringSection ------------------------------------------------------
 
 
@@ -35,41 +43,82 @@
     warnings = "warnings"
 
 
 class _DocstringSectionPatched(ds.DocstringSection):
     _registry: "dict[Enum, _DocstringSectionPatched]" = {}
 
     def __init__(self, value: str, title: "str | None" = None):
-        super().__init__(title)
         self.value = value
+        super().__init__(title)
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
         if cls.kind.value in cls._registry:
             raise KeyError(f"A section for kind {cls.kind} already exists")
 
-        cls._registry[cls.kind] = cls
+        cls._registry[cls.kind.value] = cls
+
+    @staticmethod
+    def split_sections(text) -> list[tuple[str, str]]:
+        """Return tuples of (title, body) for all numpydoc style sections in the text.
+
+        Note that this function does not check the value of the section header,
+        only that it is a header on one line, with dashed on the next.
+        """
+        import re
+
+        comp = re.compile(r"^([\S \t]+)\n-+$\n?", re.MULTILINE)
+
+        crnt_match = comp.search(text)
+        crnt_pos = 0
+
+        # This loop takes a match, then attempts to look ahead at the next one,
+        # in order to find the body of text between multiple sections.
+        results = []
+        while crnt_match is not None:
+            next_pos = crnt_pos + crnt_match.end()
+            substr = text[next_pos:]
+            next_match = comp.search(substr)
+
+            title = crnt_match.groups()[0]
+            body = substr if next_match is None else substr[: next_match.start()]
+
+            results.append((title, body))
+
+            crnt_match, crnt_pos = next_match, next_pos
+
+        return results
 
     @classmethod
-    def transform(cls, el: ds.DocstringSection) -> ds.DocstringSection:
+    def transform(cls, el: ds.DocstringSection) -> list[ds.DocstringSection]:
         """Attempt to cast DocstringSection element to more specific section type.
 
         Note that this is meant to patch cases where the general DocstringSectionText
         class represents a section like See Also, etc..
         """
 
-        if isinstance(el, ds.DocstringSectionText):
-            for kind, sub_cls in cls._registry.items():
-                prefix = kind.value.title() + "\n---"
-                if el.value.lstrip("\n").startswith(prefix):
-                    stripped = el.value.replace(prefix, "", 1).lstrip("-\n")
-                    return sub_cls(stripped, el.title)
+        if not isinstance(el, ds.DocstringSectionText):
+            return [el]
+
+        splits = cls.split_sections(el.value)
+        results = []
+        for title, body in splits:
+            sub_cls = cls._registry.get(title.lower(), ds.DocstringSectionText)
+
+            # note that griffe currently doesn't store the title anywhere,
+            # but we add the exact title here, so we can be flexible about the
+            # sections we parse (e.g. Note instead of Notes) in the future.
+            results.append(sub_cls(body, title))
 
-        return el
+        return results or [el]
+
+    @classmethod
+    def transform_all(cls, el: list[ds.DocstringSection]) -> list[ds.DocstringSection]:
+        return sum(map(cls.transform, el), [])
 
 
 class DocstringSectionSeeAlso(_DocstringSectionPatched):
     kind = DocstringSectionKindPatched.see_also
 
 
 class DocstringSectionNotes(_DocstringSectionPatched):
@@ -106,14 +155,21 @@
     raise ValueError(f"Unsupported first element in tuple: {kind}")
 
 
 # Tree previewer ==============================================================
 
 
 @dispatch
+def fields(el: BaseModel):
+    # return fields whose values were not set to the default
+    field_defaults = {mf.name: mf.default for mf in el.__fields__.values()}
+    return [k for k, v in el if field_defaults[k] is not v]
+
+
+@dispatch
 def fields(el: dc.Object):
     options = [
         "name",
         "canonical_path",
         "classes",
         "parameters",
         "members",
@@ -121,15 +177,23 @@
         "docstring",
     ]
     return [opt for opt in options if hasattr(el, opt)]
 
 
 @dispatch
 def fields(el: dc.ObjectAliasMixin):
-    return fields(el.target)
+    try:
+        return fields(el.target)
+    except dc.AliasResolutionError:
+        warnings.warn(
+            f"Could not resolve Alias target `{el.target_path}`."
+            " This often occurs because the module was not loaded (e.g. it is a"
+            " package outside of your package)."
+        )
+        return ["name", "target_path"]
 
 
 @dispatch
 def fields(el: dc.Function):
     return ["name", "annotation", "parameters", "docstring"]
 
 
@@ -192,17 +256,18 @@
     n_spaces = 3
     icon_block = "█─"
     icon_pipe = "├─"
     icon_endpipe = "└─"
     icon_connector = "│ "
     string_truncate_mark = " ..."
 
-    def __init__(self, string_max_length: int = 50, max_depth=999):
+    def __init__(self, string_max_length: int = 50, max_depth=999, compact=False):
         self.string_max_length = string_max_length
         self.max_depth = max_depth
+        self.compact = compact
 
     def format(self, call, depth=0, pad=0):
         """Return a Symbolic or Call back as a nice tree, with boxes for nodes."""
 
         call = transform(call)
 
         crnt_fields = fields(call)
@@ -220,18 +285,27 @@
         if depth >= self.max_depth:
             return call_str + self.string_truncate_mark
 
         # format arguments ----
         fields_str = []
         for name in crnt_fields:
             val = self.get_field(call, name)
-            formatted_val = self.format(
-                val, depth + 1, pad=len(str(name)) + self.n_spaces
-            )
-            fields_str.append(f"{name} = {formatted_val}")
+
+            # either align subfields with the end of the name, or put the node
+            # on a newline, so it doesn't have to be so indented.
+            if self.compact:
+                sub_pad = pad
+                linebreak = "\n" if fields(val) else ""
+            else:
+                sub_pad = len(str(name)) + self.n_spaces
+                linebreak = ""
+
+            # do formatting
+            formatted_val = self.format(val, depth + 1, pad=sub_pad)
+            fields_str.append(f"{name} = {linebreak}{formatted_val}")
 
         padded = []
         for ii, entry in enumerate(fields_str):
             is_final = ii == len(fields_str) - 1
 
             chunk = self.fmt_pipe(entry, is_final=is_final, pad=pad)
             padded.append(chunk)
@@ -255,15 +329,15 @@
         connector = "\n" + " " * pad + connector
         prefix = "\n" + " " * pad + prefix
         # NOTE: because visiting is depth first, this is essentially prepending
         # the text to the left.
         return prefix + connector.join(x.splitlines())
 
 
-def preview(ast: "dc.Object | ds.Docstring | object", max_depth=999):
+def preview(ast: "dc.Object | ds.Docstring | object", max_depth=999, compact=False):
     """Print a friendly representation of a griffe object (e.g. function, docstring)
 
     Examples
     --------
 
     >>> from quartodoc import get_object
     >>> obj = get_object("quartodoc", "get_object")
@@ -271,8 +345,8 @@
     >>> preview(obj.docstring.parsed)
      ...
 
     >>> preview(obj)
      ...
 
     """
-    print(Formatter(max_depth=max_depth).format(ast))
+    print(Formatter(max_depth=max_depth, compact=compact).format(ast))
```

### Comparing `quartodoc-0.2.2/quartodoc/autosummary.py` & `quartodoc-0.3.0/quartodoc/autosummary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from __future__ import annotations
 
 import logging
+import warnings
 import yaml
 
-from functools import partial
+from fnmatch import fnmatchcase
 from griffe.loader import GriffeLoader
-from griffe.collections import ModulesCollection
+from griffe.collections import ModulesCollection, LinesCollection
 from griffe.dataclasses import Alias
 from griffe.docstrings.parsers import Parser, parse
 from griffe.docstrings import dataclasses as ds  # noqa
 from griffe import dataclasses as dc
 from plum import dispatch  # noqa
 from pathlib import Path
+from types import ModuleType
 
 from .inventory import create_inventory, convert_inventory
+from . import layout
 from .renderers import Renderer
 
-from typing import Any, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    import sphobjinv as soi
-
-    from griffe import dataclasses as dc
-    from griffe.collections import ModulesCollection
+from typing import Any
 
 
 _log = logging.getLogger(__name__)
 
 
 # Docstring loading / parsing =================================================
 
@@ -64,106 +61,256 @@
 
     f_data = mod.functions[func_name]
 
     return f_data
 
 
 def get_object(
-    module: str,
-    object_name: str,
+    path: str,
+    object_name: "str | None" = None,
     parser: str = "numpy",
     load_aliases=True,
     dynamic=False,
-    modules_collection: "None | ModulesCollection" = None,
+    loader: None | GriffeLoader = None,
 ) -> dc.Object:
     """Fetch a griffe object.
 
     Parameters
     ----------
-    module: str
-        A module name.
+    path: str
+        An import path to the object. This should have the form `path.to.module:object`.
+        For example, `quartodoc:get_object` or `quartodoc:MdRenderer.render`.
     object_name: str
-        A function name.
+        (Deprecated). A function name.
     parser: str
         A docstring parser to use.
     load_aliases: bool
         For aliases that were imported from other modules, should we load that module?
     dynamic: bool
         Whether to dynamically import object. Useful if docstring is not hard-coded,
         but was set on object by running python code.
-    modules_collection: optional
-        A griffe [](`~griffe.collections.ModulesCollection`), used to hold loaded modules.
 
     See Also
     --------
-    get_function: a deprecated function.
+    preview: print a user-friendly preview of a griffe object.
 
     Examples
     --------
 
     >>> get_function("quartodoc", "get_function")
     <Function('get_function', ...
 
     """
-    griffe = GriffeLoader(
-        docstring_parser=Parser(parser), modules_collection=modules_collection
-    )
-    mod = griffe.load_module(module)
 
-    parts = object_name.split(".")
-    f_data = mod._modules_collection[f"{module}.{object_name}"]
+    if object_name is not None:
+        warnings.warn(
+            "object_name argument is deprecated in get_object", DeprecationWarning
+        )
+
+        path = f"{path}:{object_name}"
+
+    if loader is None:
+        loader = GriffeLoader(
+            docstring_parser=Parser(parser),
+            modules_collection=ModulesCollection(),
+            lines_collection=LinesCollection(),
+        )
+
+    try:
+        module, object_path = path.split(":", 1)
+    except ValueError:
+        module, object_path = path, None
+
+    # load the module if it hasn't been already.
+    # note that it is critical for performance that we only do this when necessary.
+    root_mod = module.split(".", 1)[0]
+    if root_mod not in loader.modules_collection:
+        loader.load_module(module)
+
+    # griffe uses only periods for the path
+    griffe_path = f"{module}.{object_path}" if object_path else module
+
+    # Case 1: dynamic loading ----
+    if dynamic:
+        if isinstance(dynamic, str):
+            return dynamic_alias(path, target=dynamic, loader=loader)
+
+        return dynamic_alias(path, loader=loader)
+
+    # Case 2: static loading an object ----
+    f_parent = loader.modules_collection[griffe_path.rsplit(".", 1)[0]]
+    f_data = loader.modules_collection[griffe_path]
 
     # ensure that function methods fetched off of an Alias of a class, have that
     # class Alias as their parent, not the Class itself.
-    if isinstance(f_data, dc.Function):
-        try:
-            parent_path = ".".join(parts[:-1])
-            parent_alias = mod._modules_collection[f"{module}.{parent_path}"]
-        except KeyError:
-            pass
-        else:
-            f_data = dc.Alias(f_data.name, f_data, parent=parent_alias)
+    if isinstance(f_parent, dc.Alias) and isinstance(
+        f_data, (dc.Function, dc.Attribute)
+    ):
+        f_data = dc.Alias(f_data.name, f_data, parent=f_parent)
 
     # Alias objects can refer to objects imported from other modules.
     # in this case, we need to import the target's module in order to resolve
     # the alias
     if isinstance(f_data, Alias) and load_aliases:
         target_mod = f_data.target_path.split(".")[0]
         if target_mod != module:
-            griffe.load_module(target_mod)
-
-    if dynamic:
-        obj = f_data.target if isinstance(f_data, Alias) else f_data
-        replace_docstring(obj)
+            loader.load_module(target_mod)
 
     return f_data
 
 
-def replace_docstring(obj: dc.Object | dc.Alias, f):
+def _resolve_target(obj: dc.Alias):
+    target = obj.target
+
+    count = 0
+    while isinstance(target, dc.Alias):
+        count += 1
+        if count > 100:
+            raise ValueError(
+                "Attempted to resolve target, but may be infinitely recursing?"
+            )
+
+        target = target.target
+
+    return target
+
+
+def replace_docstring(obj: dc.Object | dc.Alias, f=None):
+    """Replace (in place) a docstring for a griffe object.
+
+    Parameters
+    ----------
+    obj:
+        Object to replace the docstring of.
+    f:
+        The python object whose docstring to use in the replacement. If not
+        specified, then attempt to import obj and use its docstring.
+
+    """
     import importlib
 
-    mod = importlib.import_module(obj.module.canonical_path)
+    if isinstance(obj, dc.Alias):
+        obj = _resolve_target(obj)
 
-    # TODO: handle top-level modules. this assumes it's the child of a module.
-    f = getattr(mod, obj.name)
+    # for classes, we dynamically load the docstrings for all their methods.
+    # since griffe reads class docstrings from the .__init__ method, this should
+    # also have the effect of updating the class docstring.
+    if isinstance(obj, dc.Class):
+        for child_obj in obj.members.values():
+            replace_docstring(child_obj)
+
+    if f is None:
+        mod = importlib.import_module(obj.module.canonical_path)
+
+        if isinstance(obj.parent, dc.Class):
+            f = getattr(getattr(mod, obj.parent.name), obj.name)
+        else:
+            f = getattr(mod, obj.name)
+
+    # if no docstring on the dynamically loaded function, then stop
+    # since there's nothing to update.
+    # TODO: A static docstring could have been detected erroneously
+    if f.__doc__ is None:
+        return
 
     old = obj.docstring
     new = dc.Docstring(
         value=f.__doc__,
-        lineno=old.lineno,
-        endlineno=old.endlineno,
-        parent=old.parent,
-        parser=old.parser,
-        parser_options=old.parser_options,
+        lineno=getattr(old, "lineno", None),
+        endlineno=getattr(old, "endlineno", None),
+        parent=getattr(old, "parent", None),
+        parser=getattr(old, "parser", None),
+        parser_options=getattr(old, "parser_options", None),
     )
 
-    if isinstance(obj, dc.Alias):
-        obj.target.docstring = new
+    obj.docstring = new
+
+
+def dynamic_alias(
+    path: str, target: "str | None" = None, loader=None
+) -> dc.Object | dc.Alias:
+    """Return and Alias, using a dynamic import to find the target.
+
+    Parameters
+    ----------
+    path:
+        Full path to the object. E.g. `quartodoc.get_object`.
+    get_object_:
+        Function used to fetch the alias target.
+    target:
+        Optional path to ultimate Alias target. By default, this is inferred
+        using the __module__ attribute of the imported object.
+
+    """
+    import importlib
+
+    # TODO: raise an informative error if no period
+    try:
+        mod_name, object_path = path.split(":", 1)
+    except ValueError:
+        mod_name, object_path = path, None
+
+    # get underlying object dynamically ----
+
+    mod = importlib.import_module(mod_name)
+
+    # Case 1: path is just to a module
+    if object_path is None:
+        attr = mod
+        canonical_path = mod.__name__
+
+    # Case 2: path is to a member of a module
     else:
-        obj.docstring = new
+        splits = object_path.split(".")
+
+        canonical_path = None
+        parts = []
+        crnt_part = mod
+        for ii, attr_name in enumerate(splits):
+            try:
+                crnt_part = getattr(crnt_part, attr_name)
+                if not isinstance(crnt_part, ModuleType) and not canonical_path:
+                    canonical_path = crnt_part.__module__ + ":" + ".".join(splits[ii:])
+
+                parts.append(crnt_part)
+            except AttributeError:
+                raise AttributeError(
+                    f"No attribute named `{attr_name}` in the path `{path}`."
+                )
+
+        if canonical_path is None:
+            raise ValueError("Cannot find canonical path for `{path}`")
+
+        attr = crnt_part
+
+    # start loading object with griffe ----
+
+    if target:
+        obj = get_object(target, loader=loader)
+    else:
+        obj = get_object(canonical_path, loader=loader)
+
+    # use dynamically imported object's docstring
+    replace_docstring(obj, attr)
+
+    if obj.canonical_path == path.replace(":", "."):
+        return obj
+    else:
+        # TODO: this logic should live in a MemberPath dataclass or something
+        if object_path:
+            if "." in object_path:
+                prev_member = object_path.rsplit(".", 1)[0]
+                parent_path = f"{mod_name}:{prev_member}"
+            else:
+                parent_path = mod_name
+        else:
+            parent_path = mod_name.rsplit(".", 1)[0]
+
+        parent = get_object(parent_path, loader=loader)
+        return dc.Alias(attr_name, obj, parent=parent)
 
 
 # pkgdown =====================================================================
 
 # TODO: styles -- pkgdown, single-page, many-pages
 class Builder:
     """Base class for building API docs.
@@ -183,19 +330,16 @@
         Title of the API index page.
     renderer: Renderer
         The renderer used to convert docstrings (e.g. to markdown).
     out_index:
         The output path of the index file, used to list all API functions.
     sidebar:
         The output path for a sidebar yaml config (by default no config generated).
-    display_name: str
-        The default name shown for documented functions. Either "name", "relative",
-        "full", or "canonical". These options range from just the function name, to its
-        full path relative to its package, to including the package name, to its
-        the its full path relative to its .__module__.
+    rewrite_all_pages:
+        Whether to rewrite all rendered doc pages, or only those with changes.
 
     """
 
     # builder dispatching ----
     style: str
     _registry: "dict[str, Builder]" = {}
 
@@ -203,15 +347,14 @@
     out_inventory: str = "objects.json"
     out_index: str = "index.qmd"
     out_page_suffix = ".qmd"
 
     # quarto yaml config -----
     # TODO: add model for section with the fields:
     # title, desc, contents: list[str]
-    sections: "list[Any]"
     package: str
     version: "str | None"
     dir: str
     title: str
 
     renderer: Renderer
 
@@ -229,245 +372,207 @@
         sections: "list[Any]",
         version: "str | None" = None,
         dir: str = "reference",
         title: str = "Function reference",
         renderer: "dict | Renderer | str" = "markdown",
         out_index: str = None,
         sidebar: "str | None" = None,
-        use_interlinks: bool = False,
-        display_name: str = "name",
+        rewrite_all_pages=False,
     ):
-        self.validate(sections)
+        self.layout = self.load_layout(sections=sections, package=package)
 
-        self.sections = sections
         self.package = package
         self.version = None
         self.dir = dir
         self.title = title
-        self.display_name = display_name
-
-        self.items: "dict[str, dc.Object | dc.Alias]" = {}
-        self.create_items()
-
-        self.inventory: "None | soi.Inventory"
-        self.create_inventory()
+        self.sidebar = sidebar
 
         self.renderer = Renderer.from_config(renderer)
 
-        self.sidebar = sidebar
-
         if out_index is not None:
             self.out_index = out_index
 
-        self.use_interlinks = use_interlinks
+        self.rewrite_all_pages = rewrite_all_pages
 
-    def build(self):
-        """Build index page, sphinx inventory, and individual doc pages."""
+    def load_layout(self, sections: dict, package: str):
+        # TODO: currently returning the list of sections, to make work with
+        # previous code. We should make Layout a first-class citizen of the
+        # process.
+        return layout.Layout(sections=sections, package=package)
 
-        _log.info("Rendering index")
-        content = self.render_index()
+    # building ----------------------------------------------------------------
 
-        _log.info(f"Writing index to directory: {self.dir}")
-        p_index = Path(self.dir) / self.out_index
-        p_index.parent.mkdir(exist_ok=True, parents=True)
-        p_index.write_text(content)
-
-        _log.info(f"Saving inventory to {self.out_inventory}")
-        convert_inventory(self.inventory, self.out_inventory)
+    def build(self, filter: str = "*"):
+        """Build index page, sphinx inventory, and individual doc pages.
 
-        _log.info("Writing doc pages")
-        self.write_doc_pages()
-
-        if self.sidebar:
-            _log.info(f"Writing sidebar yaml to {self.sidebar}")
-            d_sidebar = self.generate_sidebar()
-            yaml.dump(d_sidebar, open(self.sidebar, "w"))
+        Parameters
+        ----------
+        filter:
+            A simple pattern, that may include * as a wildcard. If specified,
+            only doc paths for objects with matching names will be written.
+            Path is the file's base name in the API dir (e.g. MdRenderer.render)
+        """
 
-    def validate(self, d):
-        # TODO: validate sections (or config values generally)
-        return True
-
-    # introspection ----
-
-    def create_items(self):
-        """Collect items for all docstrings."""
-
-        collection = ModulesCollection()
-        f_get_object = partial(get_object, modules_collection=collection)
-
-        _log.info("Creating items")
-        for section in self.sections:
-            for func_name in section["contents"]:
-                _log.info(f"Getting object for `{self.package}.{func_name}`")
-                obj = f_get_object(self.package, func_name)
-                self.items[func_name] = obj
+        from quartodoc import blueprint, collect
 
-    # inventory ----
+        # shaping and collection ----
 
-    def create_inventory(self):
-        """Generate sphinx inventory object."""
+        _log.info("Generating blueprint.")
+        blueprint = blueprint(self.layout)
 
-        # TODO: get package version
-        _log.info("Creating inventory")
-        version = "0.0.9999" if self.version is None else self.version
-        self.inventory = create_inventory(
-            self.package,
-            version,
-            list(self.items.values()),
-            self.fetch_object_uri,
-            self.fetch_object_dispname,
-        )
+        _log.info("Collecting pages and inventory items.")
+        pages, items = collect(blueprint, base_dir=self.dir)
 
-    def fetch_object_uri(self, obj, suffix=".html"):
-        """Define the final url that will point to individual doc pages."""
+        # writing pages ----
 
-        dispname = self.fetch_object_dispname(obj)
-        return f"{self.dir}/{dispname}{suffix}"
+        _log.info("Writing index")
+        self.write_index(blueprint)
 
-    def fetch_object_dispname(self, obj):
-        """Define the name that will be displayed for individual api functions."""
+        _log.info("Writing docs pages")
+        self.write_doc_pages(pages, filter)
 
-        if self.display_name == "name":
-            return obj.name
-        elif self.display_name == "relative":
-            return ".".join(obj.path.split(".")[1:])
+        # inventory ----
 
-        elif self.display_name == "full":
-            return obj.path
+        _log.info("Creating inventory file")
+        inv = self.create_inventory(items)
+        convert_inventory(inv, self.out_inventory)
 
-        elif self.display_name == "canonical":
-            return obj.canonical_path
+        # sidebar ----
 
-        raise ValueError(f"Unsupported display_name: `{self.display_name}`")
+        if self.sidebar:
+            _log.info(f"Writing sidebar yaml to {self.sidebar}")
+            self.write_sidebar(blueprint)
 
-    # rendering ----
+    def write_index(self, blueprint: layout.Layout):
+        """Write API index page."""
 
-    def render_index(self):
-        """Generate API index page."""
+        _log.info("Summarizing docs for index page.")
+        content = self.renderer.summarize(blueprint)
+        _log.info(f"Writing index to directory: {self.dir}")
 
-        raise NotImplementedError()
+        final = f"# {self.title}\n\n{content}"
 
-    def render_item_link(self, obj):
-        if self.use_interlinks:
-            return f"[](`{obj.path}`)"
+        p_index = Path(self.dir) / self.out_index
+        p_index.parent.mkdir(exist_ok=True, parents=True)
+        p_index.write_text(final)
 
-        link = "/" + self.fetch_object_uri(obj, suffix=self.out_page_suffix)
-        name = self.fetch_object_dispname(obj)
-        return f"[{name}]({link})"
+        return str(p_index)
 
-    def write_doc_pages(self):
+    def write_doc_pages(self, pages, filter: str):
         """Write individual function documentation pages."""
 
-        for item in self.items.values():
-            _log.info(f"Rendering `{item.canonical_path}`")
-            rendered = self.renderer.render(item)
-            html_path = Path(self.fetch_object_uri(item))
+        for page in pages:
+            _log.info(f"Rendering {page.path}")
+            rendered = self.renderer.render(page)
+            html_path = Path(self.dir) / (page.path + self.out_page_suffix)
             html_path.parent.mkdir(exist_ok=True, parents=True)
 
-            html_path.with_suffix(self.out_page_suffix).write_text(rendered)
+            # Only write out page if it has changed, or we've set the
+            # rewrite_all_pages option. This ensures that quarto won't have
+            # to re-render every page of the API all the time.
+            if filter != "*":
+                is_match = fnmatchcase(page.path, filter)
+
+                if is_match:
+                    _log.info("Matched filter")
+                else:
+                    _log.info("Skipping write (no filter match)")
+                    continue
+
+            if (
+                self.rewrite_all_pages
+                or (not html_path.exists())
+                or (html_path.read_text() != rendered)
+            ):
+                _log.info(f"Writing: {page.path}")
+                html_path.write_text(rendered)
+            else:
+                _log.info("Skipping write (content unchanged)")
+
+    # inventory ----
+
+    def create_inventory(self, items):
+        """Generate sphinx inventory object."""
+
+        # TODO: get package version
+        _log.info("Creating inventory")
+        version = "0.0.9999" if self.version is None else self.version
+        inventory = create_inventory(self.package, version, items)
+
+        return inventory
 
     # sidebar ----
 
-    def generate_sidebar(self):
-        contents = [f"{self.dir}/{self.out_index}"]
-        for section in self.sections:
-            links = [
-                self.fetch_object_uri(self.items[k], suffix=self.out_page_suffix)
-                for k in section["contents"]
-            ]
+    def _generate_sidebar(self, blueprint: layout.Layout):
+        contents = [f"{self.dir}/index{self.out_page_suffix}"]
+        for section in blueprint.sections:
+            links = []
+            for entry in section.contents:
+                links.extend(self._page_to_links(entry))
 
-            contents.append({"section": section["title"], "contents": links})
+            contents.append({"section": section.title, "contents": links})
 
         return {"website": {"sidebar": {"id": self.dir, "contents": contents}}}
 
+    def write_sidebar(self, blueprint: layout.Layout):
+        """Write a yaml config file for API sidebar."""
+
+        d_sidebar = self._generate_sidebar(blueprint)
+        yaml.dump(d_sidebar, open(self.sidebar, "w"))
+
+    def _page_to_links(self, el: layout.Page) -> list[str]:
+        # if el.flatten:
+        #     links = []
+        #     for entry in el.contents:
+        #         links.append(f"{self.dir}/{entry.path}{self.out_page_suffix}")
+        #     return links
+
+        return [f"{self.dir}/{el.path}{self.out_page_suffix}"]
+
     # constructors ----
 
     @classmethod
     def from_quarto_config(cls, quarto_cfg: "str | dict"):
         """Construct a Builder from a configuration object (or yaml file)."""
 
         # TODO: validation / config model loading
         if isinstance(quarto_cfg, str):
             import yaml
 
             quarto_cfg = yaml.safe_load(open(quarto_cfg))
 
         cfg = quarto_cfg["quartodoc"]
-        style = cfg["style"]
+        style = cfg.get("style", "pkgdown")
 
         cls_builder = cls._registry[style]
 
         return cls_builder(**{k: v for k, v in cfg.items() if k != "style"})
 
 
 class BuilderPkgdown(Builder):
     """Build an API in R pkgdown style.
 
     """
 
     style = "pkgdown"
 
-    def render_index(self):
-        rendered_sections = list(map(self._render_section, self.sections))
-        str_sections = "\n\n".join(rendered_sections)
-
-        return f"# {self.title}\n\n{str_sections}"
-
-    def _render_section(self, section):
-        header = f"## {section['title']}\n\n{section['desc']}"
-
-        thead = "| | |\n| --- | --- |"
-
-        rendered = []
-        for func_name in section["contents"]:
-            # TODO: shouldn't need to collect object again after .create_items()
-            obj = get_object(self.package, func_name)
-            rendered.append(self._render_object(obj))
-
-        str_func_table = "\n".join([thead, *rendered])
-        return f"{header}\n\n{str_func_table}"
-
-    def _render_object(self, obj):
-        # get high-level description
-        doc = obj.docstring
-        if doc is None:
-            # TODO: add a single empty
-            docstring_parts = []
-        else:
-            docstring_parts = doc.parsed
-
-        # TODO: look up from inventory?
-        link = self.render_item_link(obj)
-        if len(docstring_parts) and isinstance(
-            docstring_parts[0], ds.DocstringSectionText
-        ):
-            # TODO: or canonical_path
-            description = docstring_parts[0].value
-            short = description.split("\n")[0]
-            return f"| {link} | {short} |"
-        else:
-            return f"| {link} | |"
-
-    # def fetch_object_dispname(self, obj):
-    #    return obj.name
-
 
 class BuilderSinglePage(Builder):
     """Build an API with all docs embedded on a single page."""
 
     style = "single-page"
 
-    def render_index(self):
-        return "\n\n".join([self.renderer.render(item) for item in self.items.values()])
+    def load_layout(self, *args, **kwargs):
+        el = super().load_layout(*args, **kwargs)
+
+        el.sections = [layout.Page(path=self.out_index, contents=el.sections)]
 
-    def fetch_object_uri(self, obj):
-        index_name = Path(self.out_index).with_suffix(".html")
-        return f"{self.dir}/{index_name}#{obj.path}"
+        return el
 
-    def write_doc_pages(self):
+    def write_index(self, *args, **kwargs):
         pass
 
 
 # Builders ====================================================================
 
 # renderer
 # package name
```

### Comparing `quartodoc-0.2.2/quartodoc/inventory.py` & `quartodoc-0.3.0/quartodoc/inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from __future__ import annotations
+
 import sphobjinv as soi
 
 from dataclasses import dataclass
 from griffe import dataclasses as dc
+from plum import dispatch
+from quartodoc import layout
 
 from typing import Union, Callable
 
 
 # Inventory files =============================================================
 #
 # inventories have this form:
@@ -125,32 +129,44 @@
 
     out = dict(meta)
     out["items"] = entries
 
     return out
 
 
+@dispatch
 def _create_inventory_item(
-    item: "dc.Object | dc.Alias",
-    uri: "str | Callable[dc.Object, str]",
-    dispname: "str | Callable[dc.Object, str]" = "-",
-    priority="1",
+    item: Union[dc.Object, dc.Alias], uri, dispname="-", priority="1",
 ) -> soi.DataObjStr:
     target = item
 
     return soi.DataObjStr(
         name=target.path,
         domain="py",
         role=target.kind.value,
         priority=priority,
         uri=_maybe_call(uri, target),
         dispname=_maybe_call(dispname, target),
     )
 
 
+@dispatch
+def _create_inventory_item(
+    item: layout.Item, *args, priority="1", **kwargs
+) -> soi.DataObjStr:
+    return soi.DataObjStr(
+        name=item.name,
+        domain="py",
+        role=item.obj.kind.value,
+        priority=priority,
+        uri=item.uri,
+        dispname=item.dispname or "-",
+    )
+
+
 def _maybe_call(s: "str | Callable", obj):
     if callable(s):
         return s(obj)
     elif isinstance(s, str):
         return s
 
     raise TypeError(f"Expected string or callable, received: {type(s)}")
```

### Comparing `quartodoc-0.2.2/quartodoc/renderers/base.py` & `quartodoc-0.3.0/quartodoc/renderers/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,45 +7,31 @@
 
 
 def escape(val: str):
     return f"`{val}`"
 
 
 def sanitize(val: str):
-    return val.replace("\n", " ")
+    return (
+        val.replace("\n", " ")
+        .replace("|", "\\|")
+        .replace("[", "\\[")
+        .replace("]", "\\]")
+    )
 
 
 def convert_rst_link_to_md(rst):
     expr = (
         r"((:external(\+[a-zA-Z\._]+))?(:[a-zA-Z\._]+)?:[a-zA-Z\._]+:`~?[a-zA-Z\._]+`)"
     )
 
     return re.sub(expr, r"[](\1)", rst, flags=re.MULTILINE)
 
 
 # render -----------------------------------------------------------------------
-# griffe function dataclass structure:
-#   Object:
-#     kind: Kind {"module", "class", "function", "attribute"}
-#     name: str
-#     docstring: Docstring
-#     parent
-#     path, canonical_path: str
-#
-#   Alias: wraps Object (_target) to lookup properties
-#
-#   Module, Class, Function, Attribute
-#
-# griffe docstring dataclass structure:
-#   DocstringSection -> DocstringSection*
-#   DocstringElement -> DocstringNamedElement -> Docstring*
-#
-#
-# example templates:
-#   https://github.com/mkdocstrings/python/tree/master/src/mkdocstrings_handlers/python/templates
 
 
 class Renderer:
     style: str
     _registry: "dict[str, Renderer]" = {}
 
     def __init_subclass__(cls, **kwargs):
@@ -65,18 +51,30 @@
         elif isinstance(cfg, dict):
             style = cfg["style"]
             cfg = {k: v for k, v in cfg.items() if k != "style"}
         else:
             raise TypeError(type(cfg))
 
         if style.endswith(".py"):
+            import os
+            import sys
             import importlib
 
-            mod = importlib.import_module(style.rsplit(".", 1)[0])
-            return mod.Renderer(**cfg)
+            # temporarily add the current directory to sys path and import
+            # this ensures that even if we're executing the quartodoc cli,
+            # we can import a custom _renderer.py file.
+            # it probably isn't ideal, but seems like a more convenient
+            # option than requiring users to register entrypoints.
+            sys.path.append(os.getcwd())
+
+            try:
+                mod = importlib.import_module(style.rsplit(".", 1)[0])
+                return mod.Renderer(**cfg)
+            finally:
+                sys.path.pop()
 
         subclass = cls._registry[style]
         return subclass(**cfg)
 
     @dispatch
     def render(self, el):
         raise NotImplementedError(f"render method does not support type: {type(el)}")
```

### Comparing `quartodoc-0.2.2/quartodoc/tests/test_inventory.py` & `quartodoc-0.3.0/quartodoc/tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.3.0/quartodoc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.2.2
+Version: 0.3.0
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: mc_al_github@fastmail.com
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # quartodoc
```

### Comparing `quartodoc-0.2.2/requirements-dev.txt` & `quartodoc-0.3.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.2.2/setup.cfg` & `quartodoc-0.3.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -14,29 +14,36 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 packages = find:
 include_package_data = True
 zipsafe = False
-python_requires = >3.8
+python_requires = >=3.9
 install_requires = 
-	griffe>=0.25
-	plum-dispatch
+	griffe==0.25
+	plum-dispatch<2.0.0;python_version<'3.10'
+	plum-dispatch;python_version>='3.10'
 	sphobjinv
 	tabulate
 	importlib-metadata
 	panflute
+	pydantic
+	typing-extensions
 
 [options.extras_require]
 dev = 
 	pytest
 	jupyterlab
 	jupytext
 
+[options.entry_points]
+console_scripts = 
+	quartodoc = quartodoc.__main__:cli
+
 [project.scripts]
 quartodoc = "quartodoc.cli:main"
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
```

