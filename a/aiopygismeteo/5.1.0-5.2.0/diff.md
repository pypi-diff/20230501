# Comparing `tmp/aiopygismeteo-5.1.0.tar.gz` & `tmp/aiopygismeteo-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopygismeteo-5.1.0.tar", max compression
+gzip compressed data, was "aiopygismeteo-5.2.0.tar", max compression
```

## Comparing `aiopygismeteo-5.1.0.tar` & `aiopygismeteo-5.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-04-16 13:33:16.149443 aiopygismeteo-5.1.0/LICENSE
--rw-r--r--   0        0        0     1479 2023-04-21 20:15:26.923674 aiopygismeteo-5.1.0/README.md
--rw-r--r--   0        0        0      232 2023-04-22 17:46:15.729259 aiopygismeteo-5.1.0/aiopygismeteo/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-22 08:58:30.556323 aiopygismeteo-5.1.0/aiopygismeteo/_current.py
--rw-r--r--   0        0        0     2890 2023-04-22 08:58:38.266323 aiopygismeteo-5.1.0/aiopygismeteo/_gismeteo.py
--rw-r--r--   0        0        0     1464 2023-04-21 20:18:19.323691 aiopygismeteo-5.1.0/aiopygismeteo/_http.py
--rw-r--r--   0        0        0     4003 2023-04-22 17:43:45.689248 aiopygismeteo-5.1.0/aiopygismeteo/_search.py
--rw-r--r--   0        0        0     4722 2023-04-22 17:47:47.299246 aiopygismeteo-5.1.0/aiopygismeteo/_step_n.py
--rw-r--r--   0        0        0        0 2023-04-16 13:33:16.149443 aiopygismeteo-5.1.0/aiopygismeteo/py.typed
--rw-r--r--   0        0        0      322 2023-04-22 18:15:10.209263 aiopygismeteo-5.1.0/aiopygismeteo/types.py
--rw-r--r--   0        0        0     3199 2023-04-22 19:45:20.959236 aiopygismeteo-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 aiopygismeteo-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-16 13:33:16.149443 aiopygismeteo-5.2.0/LICENSE
+-rw-r--r--   0        0        0     1495 2023-04-22 20:08:03.719264 aiopygismeteo-5.2.0/README.md
+-rw-r--r--   0        0        0      232 2023-04-22 17:46:15.729259 aiopygismeteo-5.2.0/aiopygismeteo/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-22 08:58:30.556323 aiopygismeteo-5.2.0/aiopygismeteo/_current.py
+-rw-r--r--   0        0        0     2890 2023-04-22 08:58:38.266323 aiopygismeteo-5.2.0/aiopygismeteo/_gismeteo.py
+-rw-r--r--   0        0        0     1464 2023-04-21 20:18:19.323691 aiopygismeteo-5.2.0/aiopygismeteo/_http.py
+-rw-r--r--   0        0        0     4003 2023-04-22 17:43:45.689248 aiopygismeteo-5.2.0/aiopygismeteo/_search.py
+-rw-r--r--   0        0        0     4722 2023-04-22 17:47:47.299246 aiopygismeteo-5.2.0/aiopygismeteo/_step_n.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:33:16.149443 aiopygismeteo-5.2.0/aiopygismeteo/py.typed
+-rw-r--r--   0        0        0      515 2023-05-01 09:07:45.701133 aiopygismeteo-5.2.0/aiopygismeteo/types.py
+-rw-r--r--   0        0        0     3199 2023-05-01 09:12:02.551139 aiopygismeteo-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 aiopygismeteo-5.2.0/PKG-INFO
```

### Comparing `aiopygismeteo-5.1.0/LICENSE` & `aiopygismeteo-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopygismeteo-5.1.0/README.md` & `aiopygismeteo-5.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Асинхронная обёртка для [Gismeteo API](https://gismeteo.ru/api/).
 
 Синхронная версия [здесь](https://github.com/monosans/pygismeteo).
 
 ## Установка
 
 ```bash
-python -m pip install -U aiopygismeteo
+python -m pip install -U aiopygismeteo pygismeteo-base
 ```
 
 ## Документация
 
 <https://aiopygismeteo.readthedocs.io/>
 
 ## Пример, выводящий температуру в Москве сейчас
```

### Comparing `aiopygismeteo-5.1.0/aiopygismeteo/_current.py` & `aiopygismeteo-5.2.0/aiopygismeteo/_current.py`

 * *Files identical despite different names*

### Comparing `aiopygismeteo-5.1.0/aiopygismeteo/_gismeteo.py` & `aiopygismeteo-5.2.0/aiopygismeteo/_gismeteo.py`

 * *Files identical despite different names*

### Comparing `aiopygismeteo-5.1.0/aiopygismeteo/_http.py` & `aiopygismeteo-5.2.0/aiopygismeteo/_http.py`

 * *Files identical despite different names*

### Comparing `aiopygismeteo-5.1.0/aiopygismeteo/_search.py` & `aiopygismeteo-5.2.0/aiopygismeteo/_search.py`

 * *Files identical despite different names*

### Comparing `aiopygismeteo-5.1.0/aiopygismeteo/_step_n.py` & `aiopygismeteo-5.2.0/aiopygismeteo/_step_n.py`

 * *Files identical despite different names*

### Comparing `aiopygismeteo-5.1.0/pyproject.toml` & `aiopygismeteo-5.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiopygismeteo"
-version = "5.1.0"
+version = "5.2.0"
 description = "Asynchronous wrapper for Gismeteo API"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/aiopygismeteo"
 documentation = "https://aiopygismeteo.readthedocs.io"
 classifiers = [
@@ -36,22 +36,22 @@
 covdefaults = "2.3.0"
 mypy = "1.2.0"
 pre-commit = "2.21.0"
 pydantic = "1.10.7"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.0.0"
-ruff = "0.0.262"
+ruff = "0.0.263"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.2"
-mkdocs-material = "9.1.6"
+mkdocs-material = "9.1.8"
 
 [tool.black]
 target-version = ["py37"]
 skip-magic-trailing-comma = true
 preview = true
 
 [tool.coverage.report]
```

### Comparing `aiopygismeteo-5.1.0/PKG-INFO` & `aiopygismeteo-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopygismeteo
-Version: 5.1.0
+Version: 5.2.0
 Summary: Asynchronous wrapper for Gismeteo API
 Home-page: https://github.com/monosans/aiopygismeteo
 License: MIT
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
@@ -46,15 +46,15 @@
 Асинхронная обёртка для [Gismeteo API](https://gismeteo.ru/api/).
 
 Синхронная версия [здесь](https://github.com/monosans/pygismeteo).
 
 ## Установка
 
 ```bash
-python -m pip install -U aiopygismeteo
+python -m pip install -U aiopygismeteo pygismeteo-base
 ```
 
 ## Документация
 
 <https://aiopygismeteo.readthedocs.io/>
 
 ## Пример, выводящий температуру в Москве сейчас
```

