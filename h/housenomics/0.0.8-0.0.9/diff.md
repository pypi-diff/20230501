# Comparing `tmp/housenomics-0.0.8.tar.gz` & `tmp/housenomics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "housenomics-0.0.8.tar", max compression
+gzip compressed data, was "housenomics-0.0.9.tar", max compression
```

## Comparing `housenomics-0.0.8.tar` & `housenomics-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,15 @@
--rw-r--r--   0        0        0     1211 2022-08-12 18:05:08.000000 housenomics-0.0.8/LICENSE
--rw-r--r--   0        0        0     1042 2023-02-15 08:55:50.735345 housenomics-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      670 2023-02-09 17:59:03.622478 housenomics-0.0.8/src/toolbox/database.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 housenomics-0.0.8/setup.py
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 housenomics-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1211 2022-08-12 18:05:08.000000 housenomics-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1099 2023-02-15 08:57:15.746494 housenomics-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-12 18:05:08.000000 housenomics-0.0.9/src/housenomics/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-14 20:48:08.000000 housenomics-0.0.9/src/housenomics/application/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-04 09:42:37.647818 housenomics-0.0.9/src/housenomics/application/import_transactions.py
+-rw-r--r--   0        0        0      281 2023-02-15 08:44:00.551860 housenomics-0.0.9/src/housenomics/application/list_transactions.py
+-rw-r--r--   0        0        0     1287 2023-02-14 21:53:36.272822 housenomics-0.0.9/src/housenomics/application/views/transactions.py
+-rw-r--r--   0        0        0     1736 2023-02-04 09:42:37.648096 housenomics-0.0.9/src/housenomics/infrastructure/cgd_csv_file.py
+-rw-r--r--   0        0        0      201 2023-02-04 09:42:37.648242 housenomics-0.0.9/src/housenomics/infrastructure/transactions.py
+-rw-r--r--   0        0        0      386 2023-02-14 21:21:41.435788 housenomics-0.0.9/src/housenomics/transaction.py
+-rw-r--r--   0        0        0        0 2023-02-04 09:42:37.648453 housenomics-0.0.9/src/housenomics/ui/cli/__init__.py
+-rw-r--r--   0        0        0     2907 2023-02-15 08:57:01.254278 housenomics-0.0.9/src/housenomics/ui/cli/main.py
+-rw-r--r--   0        0        0      670 2023-02-09 17:59:03.622478 housenomics-0.0.9/src/toolbox/database.py
+-rw-r--r--   0        0        0     1291 1970-01-01 00:00:00.000000 housenomics-0.0.9/setup.py
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 housenomics-0.0.9/PKG-INFO
```

### Comparing `housenomics-0.0.8/LICENSE` & `housenomics-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `housenomics-0.0.8/pyproject.toml` & `housenomics-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "housenomics"
-version = "0.0.8"
+version = "0.0.9"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
-packages = [{include = "toolbox", from = "src"}]
+packages = [
+    { include = "toolbox", from = "src" },
+    { include = "housenomics", from = "src" }
+]
 
 [tool.poetry.scripts]
 housenomics = "housenomics.ui.cli.main:app"
 
 [tool.poetry.dependencies]
 python = "3.11.1"
 rich = "^13.3.1"
 typer = "^0.7.0"
 pendulum = "^2.1.2"
 sqlalchemy = "^2.0.3"
 
 [tool.poetry.dev-dependencies]
-bandit = {extras = ["toml"], version = "^1.7.4"}
+bandit = { extras = ["toml"], version = "^1.7.4" }
 behave = "^1.2.6"
 black = "^23.1.0"
 coverage = "^7.1.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.0.0"
 pre-commit = "^3.0.4"
```

### Comparing `housenomics-0.0.8/src/toolbox/database.py` & `housenomics-0.0.9/src/toolbox/database.py`

 * *Files identical despite different names*

