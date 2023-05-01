# Comparing `tmp/augmenty-1.3.4.tar.gz` & `tmp/augmenty-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmenty-1.3.4.tar", last modified: Mon May  1 20:02:23 2023, max compression
+gzip compressed data, was "augmenty-1.3.5.tar", last modified: Mon May  1 20:20:19 2023, max compression
```

## Comparing `augmenty-1.3.4.tar` & `augmenty-1.3.5.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.196367 augmenty-1.3.4/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.196367 augmenty-1.3.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      283 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/04_augmenter-request.md
--rw-r--r--   0 root         (0) root         (0)      625 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.196367 augmenty-1.3.4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1013 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1280 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-01 20:02:12.000000 augmenty-1.3.4/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-01 20:02:12.000000 augmenty-1.3.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-01 20:02:12.000000 augmenty-1.3.4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     2532 2023-05-01 20:02:13.000000 augmenty-1.3.4/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-01 20:02:12.000000 augmenty-1.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:02:23.212367 augmenty-1.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2023-05-01 20:02:12.000000 augmenty-1.3.4/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   395381 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)     2308 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/adding_an_augmenter.rst
--rw-r--r--   0 root         (0) root         (0)     6366 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenters_overview.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.augment_utilities.rst
--rw-r--r--   0 root         (0) root         (0)     1009 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.character.rst
--rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.doc.rst
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.keyboard.rst
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.lang.rst
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.span.rst
--rw-r--r--   0 root         (0) root         (0)     1089 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.token.rst
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/augmenty.util.rst
--rw-r--r--   0 root         (0) root         (0)     4190 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/create_augmenters_table.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2578 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1055 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1149 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    15539 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/tutorials/introduction.ipynb
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-01 20:02:12.000000 augmenty-1.3.4/docs/tutorials/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.200367 augmenty-1.3.4/img/
--rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:02:12.000000 augmenty-1.3.4/img/icon.png
--rw-r--r--   0 root         (0) root         (0)     3372 2023-05-01 20:02:13.000000 augmenty-1.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     4521 2023-05-01 20:02:12.000000 augmenty-1.3.4/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 20:02:23.212367 augmenty-1.3.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.192367 augmenty-1.3.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/
--rw-r--r--   0 root         (0) root         (0)     2053 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/__init__.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/about.py
--rw-r--r--   0 root         (0) root         (0)     3336 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/augment_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/character/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/casing.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/replace.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/spacing.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/character/swap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/doc/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/doc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/doc/casing.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/doc/subset.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/da/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1878 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/da/augmenters.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/da/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/de/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/de/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/de/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/el/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/el/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/el/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/en/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/en/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/es/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/es/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/es/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty/lang/fr/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/fr/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/hu/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/hu/__init__.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/hu/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/it/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/it/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/it/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/lt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/lt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/lt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/mk/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/mk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/mk/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/nb/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nb/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/nl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/nl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/pl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/pt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/pt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/ro/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ro/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ro/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/lang/ru/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ru/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/lang/ru/keyboard.py
--rw-r--r--   0 root         (0) root         (0)     8801 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.208367 augmenty-1.3.4/src/augmenty/span/
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/span/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/span/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/src/augmenty/token/
--rw-r--r--   0 root         (0) root         (0)      680 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/casing.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/insert.py
--rw-r--r--   0 root         (0) root         (0)    11343 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/replace.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/spacing.py
--rw-r--r--   0 root         (0) root         (0)     2325 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/static_embedding_util.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/swap.py
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/token/wordnet_util.py
--rw-r--r--   0 root         (0) root         (0)     3798 2023-05-01 20:02:12.000000 augmenty-1.3.4/src/augmenty/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.204367 augmenty-1.3.4/src/augmenty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3423 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 20:02:23.000000 augmenty-1.3.4/src/augmenty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20399 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:02:23.212367 augmenty-1.3.4/tests/lang/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/lang/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/lang/test_da.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2960 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_all_augmenters.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_augmentation_utilities.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_character.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_doc.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_general.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_issue_170.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_spans.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_static_embedding.py
--rw-r--r--   0 root         (0) root         (0)     7445 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-01 20:02:12.000000 augmenty-1.3.4/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.755472 augmenty-1.3.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      283 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/04_augmenter-request.md
+-rw-r--r--   0 root         (0) root         (0)      625 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-01 20:20:08.000000 augmenty-1.3.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-01 20:20:08.000000 augmenty-1.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-05-01 20:20:09.000000 augmenty-1.3.5/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-01 20:20:08.000000 augmenty-1.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:20:19.755472 augmenty-1.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2023-05-01 20:20:08.000000 augmenty-1.3.5/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.739472 augmenty-1.3.5/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.739472 augmenty-1.3.5/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   395381 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/adding_an_augmenter.rst
+-rw-r--r--   0 root         (0) root         (0)     6366 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenters_overview.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.augment_utilities.rst
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.character.rst
+-rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.doc.rst
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.keyboard.rst
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.lang.rst
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.span.rst
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.token.rst
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.util.rst
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/create_augmenters_table.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.739472 augmenty-1.3.5/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    15539 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/tutorials/introduction.ipynb
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/tutorials/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/img/
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:20:08.000000 augmenty-1.3.5/img/icon.png
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-05-01 20:20:09.000000 augmenty-1.3.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-05-01 20:20:08.000000 augmenty-1.3.5/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 20:20:19.755472 augmenty-1.3.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/about.py
+-rw-r--r--   0 root         (0) root         (0)     3336 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/augment_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/character/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/casing.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/replace.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/swap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/doc/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/doc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/doc/casing.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/doc/subset.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/lang/
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/lang/da/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/da/augmenters.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/da/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/de/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/de/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/de/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/el/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/el/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/el/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/en/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/en/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/es/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/es/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/fr/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/fr/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/hu/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/hu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/hu/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/it/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/it/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/it/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/lt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/lt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/lt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/mk/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/mk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/mk/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/nb/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nb/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/nl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/pl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/lang/pt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/lang/ro/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ro/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/lang/ru/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ru/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ru/keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/span/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/span/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/span/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/token/
+-rw-r--r--   0 root         (0) root         (0)      680 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/casing.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/insert.py
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/replace.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/static_embedding_util.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/swap.py
+-rw-r--r--   0 root         (0) root         (0)      814 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/wordnet_util.py
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      438 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.755472 augmenty-1.3.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20399 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.755472 augmenty-1.3.5/tests/lang/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/lang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/lang/test_da.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_all_augmenters.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_augmentation_utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_doc.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_general.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_issue_170.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_spans.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_static_embedding.py
+-rw-r--r--   0 root         (0) root         (0)     7445 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_util.py
```

### Comparing `augmenty-1.3.4/.github/ISSUE_TEMPLATE/01_bugs.md` & `augmenty-1.3.5/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/.github/ISSUE_TEMPLATE/config.yml` & `augmenty-1.3.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/.github/dependabot.yml` & `augmenty-1.3.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/.github/workflows/dependabot_automerge.yml` & `augmenty-1.3.5/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/.github/workflows/documentation.yml` & `augmenty-1.3.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/.github/workflows/release.yml` & `augmenty-1.3.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/.github/workflows/tests.yml` & `augmenty-1.3.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/.pre-commit-config.yaml` & `augmenty-1.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/CHANGELOG.md` & `augmenty-1.3.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.5 (2023-05-01)
+### Fix
+* Removed upper bounds on all dependencies ([`78b6a1d`](https://github.com/KennethEnevoldsen/augmenty/commit/78b6a1dd109e5946b8ba69b3e1215cc6aff328c6))
+
 ## v1.3.4 (2023-05-01)
 ### Fix
 * Handle offset outside "head" annotation scope ([`c02f076`](https://github.com/KennethEnevoldsen/augmenty/commit/c02f076d64ff7e18b5d6a239d2f02a7be966326d))
 * Added fix for issues 170 ([`74aa006`](https://github.com/KennethEnevoldsen/augmenty/commit/74aa00613b6dad7ef004a8f30ab0e8ec3838be94))
 
 ### Documentation
 * Updated docstrings on repeat augmenter ([`f4cf48c`](https://github.com/KennethEnevoldsen/augmenty/commit/f4cf48c1585a592e7e798738f46b02bd5d816878))
```

### Comparing `augmenty-1.3.4/LICENSE` & `augmenty-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/PKG-INFO` & `augmenty-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.4
+Version: 1.3.5
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.4 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.5 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.4/docs/Makefile` & `augmenty-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/_static/favicon.ico` & `augmenty-1.3.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/_static/icon.png` & `augmenty-1.3.5/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/_static/icon_dark.png` & `augmenty-1.3.5/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/adding_an_augmenter.rst` & `augmenty-1.3.5/docs/adding_an_augmenter.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/augmenters_overview.md` & `augmenty-1.3.5/docs/augmenters_overview.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/augmenty.character.rst` & `augmenty-1.3.5/docs/augmenty.character.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/augmenty.doc.rst` & `augmenty-1.3.5/docs/augmenty.doc.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/augmenty.token.rst` & `augmenty-1.3.5/docs/augmenty.token.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/conf.py` & `augmenty-1.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/create_augmenters_table.py` & `augmenty-1.3.5/docs/create_augmenters_table.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/faq.rst` & `augmenty-1.3.5/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/index.rst` & `augmenty-1.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/installation.rst` & `augmenty-1.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/make.bat` & `augmenty-1.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/news.rst` & `augmenty-1.3.5/docs/news.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/docs/tutorials/introduction.ipynb` & `augmenty-1.3.5/docs/tutorials/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/img/icon.png` & `augmenty-1.3.5/img/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/pyproject.toml` & `augmenty-1.3.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "augmenty"
-version = "1.3.4"
+version = "1.3.5"
 description = "An augmentation library based on SpaCy for joint augmentation of text and labels."
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -30,19 +30,19 @@
     "data augmentation",
     "data science",
     "machine learning",
     "deep learning"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "spacy>=3.2.0,<3.6.0",
-    "catalogue>=2.0.4,<2.1.0",
-    "thinc>=8.0.8,<8.2.0",
-    "pydantic>=1.8.2,<1.11.0",
-    "numpy>=1.15.0,<2.0.0"
+    "spacy>=3.2.0",
+    "catalogue>=2.0.4",
+    "thinc>=8.0.8",
+    "pydantic>=1.8.2",
+    "numpy>=1.15.0"
 ]
 
 [project.readme]
 file = "readme.md"
 content-type = "text/markdown"
 
 [project.urls]
@@ -52,38 +52,38 @@
 
 [project.license]
 file = "LICENSE"
 name = "MIT"
 
 
 [project.optional-dependencies]
-da = ["dacy>=2.3.1,<2.4.0"]
-all = ["nltk>=3.6.7,<3.8.0"]
+da = ["dacy>=2.3.1"]
+all = ["nltk>=3.6.7"]
 style = [
     "black==22.12.0",
-    "pre-commit>=2.20.0,<3.1.0",
+    "pre-commit>=2.20.0",
     "ruff==0.0.191",
     "mypy==0.991"
 ]
 tests = [
-    "pytest>=7.1.3,<7.3.0",
-    "pytest-cov>=3.0.0,<3.0.1",
-    "pytest-lazy-fixture>=0.6.3,<0.7.0",
-    "pytest-timeout>=2.1.0,<2.2.0"
+    "pytest>=7.1.3",
+    "pytest-cov>=3.0.0",
+    "pytest-lazy-fixture>=0.6.3",
+    "pytest-timeout>=2.1.0"
 ]
 docs = [
-    "sphinx>=5.3.0,<5.4.0",
-    "furo==2022.12.7",
-    "sphinx-copybutton>=0.5.1,<0.5.2",
-    "sphinxext-opengraph>=0.7.3,<0.7.4",
-    "sphinx_design>=0.3.0,<0.3.1",
-     "myst-nb>=0.6.0,<1.17.0",
+    "sphinx>=5.3.0",
+    "furo>=2022.12.7",
+    "sphinx-copybutton>=0.5.1",
+    "sphinxext-opengraph>=0.7.3",
+    "sphinx_design>=0.3.0",
+    "myst-nb>=0.6.0",
 ]
 tutorials = [
-    "jupyter>=1.0.0,<1.1.0",
+    "jupyter>=1.0.0",
     "faker==13.13.0"
 ]
 
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `augmenty-1.3.4/readme.md` & `augmenty-1.3.5/readme.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/__init__.py` & `augmenty-1.3.5/src/augmenty/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/augment_utilities.py` & `augmenty-1.3.5/src/augmenty/augment_utilities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/character/casing.py` & `augmenty-1.3.5/src/augmenty/character/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/character/replace.py` & `augmenty-1.3.5/src/augmenty/character/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/character/spacing.py` & `augmenty-1.3.5/src/augmenty/character/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/character/swap.py` & `augmenty-1.3.5/src/augmenty/character/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/doc/casing.py` & `augmenty-1.3.5/src/augmenty/doc/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/doc/subset.py` & `augmenty-1.3.5/src/augmenty/doc/subset.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/keyboard.py` & `augmenty-1.3.5/src/augmenty/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/__init__.py` & `augmenty-1.3.5/src/augmenty/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/da/augmenters.py` & `augmenty-1.3.5/src/augmenty/lang/da/augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/da/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/da/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/de/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/de/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/el/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/el/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/en/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/en/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/es/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/es/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/fr/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/fr/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/hu/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/hu/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/it/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/it/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/lt/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/lt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/mk/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/mk/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/nb/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/nb/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/nl/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/nl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/pl/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/pl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/pt/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/pt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/ro/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/ro/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/lang/ru/keyboard.py` & `augmenty-1.3.5/src/augmenty/lang/ru/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/meta.json` & `augmenty-1.3.5/src/augmenty/meta.json`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/span/entities.py` & `augmenty-1.3.5/src/augmenty/span/entities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/__init__.py` & `augmenty-1.3.5/src/augmenty/token/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/casing.py` & `augmenty-1.3.5/src/augmenty/token/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/insert.py` & `augmenty-1.3.5/src/augmenty/token/insert.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/replace.py` & `augmenty-1.3.5/src/augmenty/token/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/spacing.py` & `augmenty-1.3.5/src/augmenty/token/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/static_embedding_util.py` & `augmenty-1.3.5/src/augmenty/token/static_embedding_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/swap.py` & `augmenty-1.3.5/src/augmenty/token/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/token/wordnet_util.py` & `augmenty-1.3.5/src/augmenty/token/wordnet_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty/util.py` & `augmenty-1.3.5/src/augmenty/util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/src/augmenty.egg-info/PKG-INFO` & `augmenty-1.3.5/src/augmenty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.4
+Version: 1.3.5
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.4 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.5 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.4/src/augmenty.egg-info/SOURCES.txt` & `augmenty-1.3.5/src/augmenty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/books.py` & `augmenty-1.3.5/tests/books.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/fixtures.py` & `augmenty-1.3.5/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/lang/test_da.py` & `augmenty-1.3.5/tests/lang/test_da.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/test_all_augmenters.py` & `augmenty-1.3.5/tests/test_all_augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/test_augmentation_utilities.py` & `augmenty-1.3.5/tests/test_augmentation_utilities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/test_character.py` & `augmenty-1.3.5/tests/test_character.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/test_doc.py` & `augmenty-1.3.5/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/test_issue_170.py` & `augmenty-1.3.5/tests/test_issue_170.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/test_spans.py` & `augmenty-1.3.5/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.4/tests/test_token.py` & `augmenty-1.3.5/tests/test_token.py`

 * *Files identical despite different names*

