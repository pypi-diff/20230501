# Comparing `tmp/augmenty-1.3.3.tar.gz` & `tmp/augmenty-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmenty-1.3.3.tar", last modified: Thu Apr 27 19:19:23 2023, max compression
+gzip compressed data, was "augmenty-1.3.4.tar", last modified: Mon May  1 20:02:23 2023, max compression
```

## Comparing `augmenty-1.3.3.tar` & `augmenty-1.3.4.tar`

### file list

```diff
@@ -1,157 +1,158 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.207014 augmenty-1.3.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      283 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/04_augmenter-request.md
--rw-r--r--   0 root         (0) root         (0)      625 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1013 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1280 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2697 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-27 19:19:12.000000 augmenty-1.3.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)      797 2023-04-27 19:19:12.000000 augmenty-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     2038 2023-04-27 19:19:13.000000 augmenty-1.3.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-04-27 19:19:12.000000 augmenty-1.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7212 2023-04-27 19:19:23.207014 augmenty-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2023-04-27 19:19:12.000000 augmenty-1.3.3/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.191014 augmenty-1.3.3/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.191014 augmenty-1.3.3/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   385037 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   395381 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)     2308 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/adding_an_augmenter.rst
--rw-r--r--   0 root         (0) root         (0)     6366 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenters_overview.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.augment_utilities.rst
--rw-r--r--   0 root         (0) root         (0)     1009 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.character.rst
--rw-r--r--   0 root         (0) root         (0)      733 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.doc.rst
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.keyboard.rst
--rw-r--r--   0 root         (0) root         (0)      500 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.lang.rst
--rw-r--r--   0 root         (0) root         (0)      334 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.span.rst
--rw-r--r--   0 root         (0) root         (0)     1089 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.token.rst
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.util.rst
--rw-r--r--   0 root         (0) root         (0)     4190 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/create_augmenters_table.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2578 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1055 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1149 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.191014 augmenty-1.3.3/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    15539 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/tutorials/introduction.ipynb
--rw-r--r--   0 root         (0) root         (0)      210 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/tutorials/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/img/
--rw-r--r--   0 root         (0) root         (0)   385037 2023-04-27 19:19:12.000000 augmenty-1.3.3/img/icon.png
--rw-r--r--   0 root         (0) root         (0)     3152 2023-04-27 19:19:13.000000 augmenty-1.3.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     4521 2023-04-27 19:19:12.000000 augmenty-1.3.3/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 19:19:23.207014 augmenty-1.3.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/
--rw-r--r--   0 root         (0) root         (0)     2053 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/__init__.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/about.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/augment_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/character/
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/casing.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/replace.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/spacing.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/swap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/doc/
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/doc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/doc/casing.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/doc/subset.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/lang/
--rw-r--r--   0 root         (0) root         (0)      784 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/lang/da/
--rw-r--r--   0 root         (0) root         (0)      195 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1878 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/da/augmenters.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/da/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/lang/de/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/de/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/de/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/el/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/el/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/el/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/en/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/en/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/es/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/es/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/es/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/fr/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/fr/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/hu/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/hu/__init__.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/hu/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/it/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/it/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/it/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/lt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/lt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      794 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/lt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/mk/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/mk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/mk/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/nb/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nb/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/nl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/pl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/pt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/lang/ro/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ro/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ro/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/lang/ru/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ru/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ru/keyboard.py
--rw-r--r--   0 root         (0) root         (0)     8801 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/span/
--rw-r--r--   0 root         (0) root         (0)      177 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/span/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11636 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/span/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/token/
--rw-r--r--   0 root         (0) root         (0)      680 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/casing.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/insert.py
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/replace.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/spacing.py
--rw-r--r--   0 root         (0) root         (0)     2325 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/static_embedding_util.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/swap.py
--rw-r--r--   0 root         (0) root         (0)      814 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/wordnet_util.py
--rw-r--r--   0 root         (0) root         (0)     3798 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7212 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3399 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.207014 augmenty-1.3.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20399 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.207014 augmenty-1.3.3/tests/lang/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/lang/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/lang/test_da.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2960 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_all_augmenters.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_augmentation_utilities.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_character.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_doc.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_general.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_spans.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_static_embedding.py
--rw-r--r--   0 root         (0) root         (0)     7445 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.196367 augmenty-1.3.4/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.196367 augmenty-1.3.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      283 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/04_augmenter-request.md
+-rw-r--r--   0 root         (0) root         (0)      625 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.196367 augmenty-1.3.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-01 20:02:12.000000 augmenty-1.3.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-01 20:02:12.000000 augmenty-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-05-01 20:02:13.000000 augmenty-1.3.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-01 20:02:12.000000 augmenty-1.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:02:23.212367 augmenty-1.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2023-05-01 20:02:12.000000 augmenty-1.3.4/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   395381 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/adding_an_augmenter.rst
+-rw-r--r--   0 root         (0) root         (0)     6366 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenters_overview.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.augment_utilities.rst
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.character.rst
+-rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.doc.rst
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.keyboard.rst
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.lang.rst
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.span.rst
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.token.rst
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.util.rst
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/create_augmenters_table.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    15539 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/tutorials/introduction.ipynb
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/tutorials/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/img/
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:02:12.000000 augmenty-1.3.4/img/icon.png
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-05-01 20:02:13.000000 augmenty-1.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-05-01 20:02:12.000000 augmenty-1.3.4/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 20:02:23.212367 augmenty-1.3.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.192367 augmenty-1.3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/about.py
+-rw-r--r--   0 root         (0) root         (0)     3336 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/augment_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/character/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/casing.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/replace.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/swap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/doc/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/doc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/doc/casing.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/doc/subset.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/da/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/da/augmenters.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/da/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/de/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/de/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/de/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/el/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/el/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/el/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/en/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/en/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/es/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/es/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/fr/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/fr/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/hu/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/hu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/hu/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/it/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/it/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/it/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/lt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/lt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/lt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/mk/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/mk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/mk/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/nb/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nb/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/nl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/pl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/pt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/ro/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ro/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/ru/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ru/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ru/keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/span/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/span/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/span/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/src/augmenty/token/
+-rw-r--r--   0 root         (0) root         (0)      680 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/casing.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/insert.py
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/replace.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/static_embedding_util.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/swap.py
+-rw-r--r--   0 root         (0) root         (0)      814 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/wordnet_util.py
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20399 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/tests/lang/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/lang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/lang/test_da.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_all_augmenters.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_augmentation_utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_doc.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_general.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_issue_170.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_spans.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_static_embedding.py
+-rw-r--r--   0 root         (0) root         (0)     7445 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_util.py
```

### Comparing `augmenty-1.3.3/.github/ISSUE_TEMPLATE/01_bugs.md` & `augmenty-1.3.4/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/.github/ISSUE_TEMPLATE/config.yml` & `augmenty-1.3.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/.github/dependabot.yml` & `augmenty-1.3.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/.github/workflows/dependabot_automerge.yml` & `augmenty-1.3.4/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/.github/workflows/documentation.yml` & `augmenty-1.3.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/.github/workflows/release.yml` & `augmenty-1.3.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/.github/workflows/tests.yml` & `augmenty-1.3.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/.pre-commit-config.yaml` & `augmenty-1.3.4/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

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
-    rev: v1.6.3
+    rev: v1.6.4
     hooks:
       - id: docformatter
         args: [--in-place]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         args: [--line-length, "88"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.262
+    rev: v0.0.263
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
```

### Comparing `augmenty-1.3.3/CHANGELOG.md` & `augmenty-1.3.4/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.4 (2023-05-01)
+### Fix
+* Handle offset outside "head" annotation scope ([`c02f076`](https://github.com/KennethEnevoldsen/augmenty/commit/c02f076d64ff7e18b5d6a239d2f02a7be966326d))
+* Added fix for issues 170 ([`74aa006`](https://github.com/KennethEnevoldsen/augmenty/commit/74aa00613b6dad7ef004a8f30ab0e8ec3838be94))
+
+### Documentation
+* Updated docstrings on repeat augmenter ([`f4cf48c`](https://github.com/KennethEnevoldsen/augmenty/commit/f4cf48c1585a592e7e798738f46b02bd5d816878))
+
 ## v1.3.3 (2023-04-27)
 ### Fix
 * Adjust dep. annotations for ent augmenter ([`00bbc56`](https://github.com/KennethEnevoldsen/augmenty/commit/00bbc561211ca5bde68f030c191ea20caad6dbfc))
 
 ### Documentation
 * Fix formatting such that is rendered as intended in the docs ([`a77c362`](https://github.com/KennethEnevoldsen/augmenty/commit/a77c362a09762bf4473d0e4afd1289cbbb15e526))
```

### Comparing `augmenty-1.3.3/LICENSE` & `augmenty-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/PKG-INFO` & `augmenty-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.3
+Version: 1.3.4
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.3 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.4 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.3/docs/Makefile` & `augmenty-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/_static/favicon.ico` & `augmenty-1.3.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/_static/icon.png` & `augmenty-1.3.4/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/_static/icon_dark.png` & `augmenty-1.3.4/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/adding_an_augmenter.rst` & `augmenty-1.3.4/docs/adding_an_augmenter.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/augmenters_overview.md` & `augmenty-1.3.4/docs/augmenters_overview.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/augmenty.character.rst` & `augmenty-1.3.4/docs/augmenty.character.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/augmenty.doc.rst` & `augmenty-1.3.4/docs/augmenty.doc.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/augmenty.token.rst` & `augmenty-1.3.4/docs/augmenty.token.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/conf.py` & `augmenty-1.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/create_augmenters_table.py` & `augmenty-1.3.4/docs/create_augmenters_table.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/faq.rst` & `augmenty-1.3.4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/index.rst` & `augmenty-1.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/installation.rst` & `augmenty-1.3.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/make.bat` & `augmenty-1.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/news.rst` & `augmenty-1.3.4/docs/news.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/docs/tutorials/introduction.ipynb` & `augmenty-1.3.4/docs/tutorials/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/img/icon.png` & `augmenty-1.3.4/img/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/pyproject.toml` & `augmenty-1.3.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "augmenty"
-version = "1.3.3"
+version = "1.3.4"
 description = "An augmentation library based on SpaCy for joint augmentation of text and labels."
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -126,7 +126,20 @@
 [tool.ruff]
 exclude = [
     ".venv",
     ".env",
     ".git",
     "__pycache__",
 ]
+ignore = [
+  "ANN101",
+  "ANN401",
+  "E402",
+  "E501",
+  "F401",
+  "F841",
+  "RET504",
+  "ANN202",
+]
+ignore-init-module-imports = true
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+unfixable = ["ERA"]
```

### Comparing `augmenty-1.3.3/readme.md` & `augmenty-1.3.4/readme.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/__init__.py` & `augmenty-1.3.4/src/augmenty/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/augment_utilities.py` & `augmenty-1.3.4/src/augmenty/augment_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 
 def combine(
     augmenters: Iterable[Callable[[Language, Example], Iterator[Example]]],
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Combines a series of spaCy style augmenters.
 
     Args:
-        augmenters (Iterable[Callable[[Language, Example], Iterator[Example]]]): An
-            list of spaCy augmenters.
+        augmenters: An list of spaCy augmenters.
 
     Returns:
-        Callable[[Language, Example], Iterator[Example]]: The combined augmenter
+        The combined augmenter
     """
 
     def apply_multiple_augmenters(nlp: Language, example: Example):
         examples = [example]
         for aug in augmenters:
             examples = [e for example in examples for e in aug(nlp, example)]
         yield from examples
@@ -33,20 +32,20 @@
 def set_doc_level(
     augmenter: Callable[[Language, Example], Iterator[Example]],
     level: float,
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Set the percantage of examples that the augmenter should be applied to.
 
     Args:
-        augmenter (Callable[[Language, Example], Iterator[Example]]): A spaCy
-            augmenters which you only want to apply to a certain percentage of docs
-        level (float): The percentage of docs the which should be augmented.
+        augmenter: A spaCy augmenters which you only want to apply to a
+            certain percentage of docs
+        level: The percentage of docs the which should be augmented.
 
     Returns:
-        Callable[[Language, Example], Iterator[Example]]: The combined augmenter
+        The combined augmenter
     """
 
     def __augment(nlp: Language, example: Example):
         if random.random() > level:
             yield example
         else:
             yield from augmenter(nlp, example)
@@ -54,22 +53,23 @@
     return __augment
 
 
 def repeat(
     augmenter: Callable[[Language, Example], Iterator[Example]],
     n: int,
 ) -> Callable[[Language, Example], Iterator[Example]]:
-    """Set the document level at which the tokenizer should be.
+    """Repeats an augmenter n times over the same example thus increasing the
+    sample size.
 
     Args:
-        augmenter (Callable[[Language, Example], Iterator[Example]]): An augmenter.
-        n (int): Number of times the augmenter should be repeated
+        augmenter: An augmenter.
+        n: Number of times the augmenter should be repeated
 
     Returns:
-        Callable[[Language, Example], Iterator[Example]]: The repeated augmenter
+        The repeated augmenter
 
     Example:
         >>> augmenter = augmenty.load("char_swap_v1", level=.02)
         >>> repeated_augmenter = augmenty.repeat(augmenter=aug, n=3)
     """
 
     def __augment(nlp: Language, example: Example):
@@ -83,22 +83,20 @@
     augmenter: Callable[[Language, Example], Iterator[Example]],
     doc_level: float = 1.0,
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Wraps and augmented such that it yields both the original and augmented
     example.
 
     Args:
-        augmenter (Callable[[Language, Example], Iterator[Example]]): A spaCy
-            augmenters.
-        doc_level (float, optional): The percentage of documents the augmenter should
-            be applied to. Only yield the original when the original doc is augmented.
+        augmenter: A spaCy augmenters.
+        doc_level: The percentage of documents the augmenter should be applied to.
+            Only yield the original when the original doc is augmented.
 
     Returns:
-        Callable[[Language, Example], Iterator[Example]]: The augmenter, which now
-            yields both the original and augmented example.
+        The augmenter, which now yields both the original and augmented example.
     """
 
     def __augment(nlp: Language, example: Example, level: float):
         if random.random() < level:
             yield from augmenter(nlp, example)
         yield example
```

### Comparing `augmenty-1.3.3/src/augmenty/character/casing.py` & `augmenty-1.3.4/src/augmenty/character/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/character/replace.py` & `augmenty-1.3.4/src/augmenty/character/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/character/spacing.py` & `augmenty-1.3.4/src/augmenty/character/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/character/swap.py` & `augmenty-1.3.4/src/augmenty/character/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/doc/casing.py` & `augmenty-1.3.4/src/augmenty/doc/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/doc/subset.py` & `augmenty-1.3.4/src/augmenty/doc/subset.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/keyboard.py` & `augmenty-1.3.4/src/augmenty/keyboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 for y, k in enumerate(row):
                     if key == k:
                         return (x, y)
 
         raise ValueError(f"key {key} was not found in keyboard array")
 
     def is_shifted(self, key: str) -> bool:
-        """is the key shifted?
+        """Is the key shifted?
 
         Args:
             key (str): keyboard key
 
         Returns:
             bool: a boolean indicating whether key is shifted.
         """
@@ -71,25 +71,25 @@
             if self.is_shifted(key_a) == self.is_shifted(key_b)
             else self.shift_distance
         )
 
         return ((x1 - x2) ** 2 + (y1 - y2) ** 2) ** 0.5 + shift_cost
 
     def all_keys(self):
-        """yields all keys in keyboard.
+        """Yields all keys in keyboard.
 
         Yields:
             all keys in keyboard.
         """
         for arr in self.keyboard_array:
             for x, _ in enumerate(self.keyboard_array[arr]):
                 yield from self.keyboard_array[arr][x]
 
     def get_neighbours(self, key: str, distance: int = 1) -> List[int]:
-        """gets the neighbours of a key with a specified distance.
+        """Gets the neighbours of a key with a specified distance.
 
         Args:
             key (str): A keyboard key
             distance (int, optional): The euclidian distance of neightbours.
                 Defaults to 1.
 
         Returns:
```

### Comparing `augmenty-1.3.3/src/augmenty/lang/__init__.py` & `augmenty-1.3.4/src/augmenty/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/da/augmenters.py` & `augmenty-1.3.4/src/augmenty/lang/da/augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/da/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/da/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/de/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/de/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/el/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/el/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/en/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/en/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/es/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/es/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/fr/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/fr/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/hu/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/hu/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/it/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/it/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/lt/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/lt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/mk/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/mk/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/nb/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/nb/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/nl/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/nl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/pl/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/pl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/pt/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/pt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/ro/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/ro/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/lang/ru/keyboard.py` & `augmenty-1.3.4/src/augmenty/lang/ru/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/meta.json` & `augmenty-1.3.4/src/augmenty/meta.json`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/span/entities.py` & `augmenty-1.3.4/src/augmenty/span/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,39 +51,39 @@
 
             tok_anno["TAG"][i] = ["PROPN"] * len_ent
             tok_anno["POS"][i] = ["PROPN"] * len_ent
 
             tok_anno["MORPH"][i] = [""] * len_ent
             tok_anno["DEP"][i] = [ent[0].dep_] + ["flat"] * (len_ent - 1)
 
-            tok_anno["SENT_START"][i] = [tok_anno["SENT_START"][i][0]] + [0] * (
-                len_ent - 1
-            )
-            tok_anno["SPACY"][i] = [True] * (len_ent - 1) + (
-                tok_anno["SPACY"][i][-1:]  # set last spacing
-            )
+            # Set sentence start based on first token in previous entity
+            tok_anno["SENT_START"][i] = [ent[0].sent_start] + [0] * (len_ent - 1)
 
+            # set spacing to be whitespace for all tokens except the last one
+            # which is set based on the original entity
+            tok_anno["SPACY"][i] = [True] * (len_ent - 1) + [bool(ent[-1].whitespace_)]
+
+            offset_ = len_ent - (ent.end - ent.start)
             if example.y.has_annotation("HEAD") and resolve_dependencies:
                 # Handle HEAD
-                offset_ = len_ent - (ent.end - ent.start)
 
                 head[head > ent.start + offset] += offset_
                 # keep first head correcting for changing entity size, set rest to
                 # refer to index of first name
                 head = np.concatenate(
                     [
                         np.array(head[: ent.start + offset]),  # before
                         np.array(
                             [head[ent.root.i + offset]]
                             + [ent.start + offset] * (len_ent - 1),
                         ),  # the entity
                         np.array(head[ent.end + offset :]),  # after
                     ],
                 )
-                offset += offset_
+            offset += offset_
 
             # Handle entities IOB tags
             if len_ent == 1:
                 ents[i] = ["U-" + ent.label_]
             else:
                 ents[i] = (
                     ["B-" + ent.label_]
```

### Comparing `augmenty-1.3.3/src/augmenty/token/__init__.py` & `augmenty-1.3.4/src/augmenty/token/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/token/casing.py` & `augmenty-1.3.4/src/augmenty/token/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/token/insert.py` & `augmenty-1.3.4/src/augmenty/token/insert.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/token/replace.py` & `augmenty-1.3.4/src/augmenty/token/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/token/spacing.py` & `augmenty-1.3.4/src/augmenty/token/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/token/static_embedding_util.py` & `augmenty-1.3.4/src/augmenty/token/static_embedding_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/token/swap.py` & `augmenty-1.3.4/src/augmenty/token/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/token/wordnet_util.py` & `augmenty-1.3.4/src/augmenty/token/wordnet_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty/util.py` & `augmenty-1.3.4/src/augmenty/util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/src/augmenty.egg-info/PKG-INFO` & `augmenty-1.3.4/src/augmenty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.3
+Version: 1.3.4
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.3 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.4 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.3/src/augmenty.egg-info/SOURCES.txt` & `augmenty-1.3.4/src/augmenty.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 tests/fixtures.py
 tests/requirements.txt
 tests/test_all_augmenters.py
 tests/test_augmentation_utilities.py
 tests/test_character.py
 tests/test_doc.py
 tests/test_general.py
+tests/test_issue_170.py
 tests/test_keyboard.py
 tests/test_spans.py
 tests/test_static_embedding.py
 tests/test_token.py
 tests/test_util.py
 tests/lang/__init__.py
 tests/lang/test_da.py
```

### Comparing `augmenty-1.3.3/src/augmenty.egg-info/requires.txt` & `augmenty-1.3.4/src/augmenty.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/books.py` & `augmenty-1.3.4/tests/books.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/fixtures.py` & `augmenty-1.3.4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/lang/test_da.py` & `augmenty-1.3.4/tests/lang/test_da.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/test_all_augmenters.py` & `augmenty-1.3.4/tests/test_all_augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/test_augmentation_utilities.py` & `augmenty-1.3.4/tests/test_augmentation_utilities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/test_character.py` & `augmenty-1.3.4/tests/test_character.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/test_doc.py` & `augmenty-1.3.4/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/test_spans.py` & `augmenty-1.3.4/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.3/tests/test_token.py` & `augmenty-1.3.4/tests/test_token.py`

 * *Files identical despite different names*

