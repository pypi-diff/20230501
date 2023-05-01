# Comparing `tmp/pygismeteo-5.1.0.tar.gz` & `tmp/pygismeteo-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygismeteo-5.1.0.tar", max compression
+gzip compressed data, was "pygismeteo-5.2.0.tar", max compression
```

## Comparing `pygismeteo-5.1.0.tar` & `pygismeteo-5.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-04-19 14:48:31.640689 pygismeteo-5.1.0/LICENSE
--rw-r--r--   0        0        0     1330 2023-04-21 20:07:41.333689 pygismeteo-5.1.0/README.md
--rw-r--r--   0        0        0      209 2023-04-21 20:30:00.863662 pygismeteo-5.1.0/pygismeteo/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-22 09:03:37.506335 pygismeteo-5.1.0/pygismeteo/_current.py
--rw-r--r--   0        0        0     2818 2023-04-22 09:02:08.356344 pygismeteo-5.1.0/pygismeteo/_gismeteo.py
--rw-r--r--   0        0        0     1288 2023-04-21 20:13:03.143666 pygismeteo-5.1.0/pygismeteo/_http.py
--rw-r--r--   0        0        0     3921 2023-04-22 17:44:22.569254 pygismeteo-5.1.0/pygismeteo/_search.py
--rw-r--r--   0        0        0     4632 2023-04-22 17:48:05.969246 pygismeteo-5.1.0/pygismeteo/_step_n.py
--rw-r--r--   0        0        0        0 2023-04-19 14:48:31.650689 pygismeteo-5.1.0/pygismeteo/py.typed
--rw-r--r--   0        0        0      322 2023-04-22 18:14:51.489227 pygismeteo-5.1.0/pygismeteo/types.py
--rw-r--r--   0        0        0     3132 2023-04-22 19:45:13.249235 pygismeteo-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 pygismeteo-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-19 14:48:31.640689 pygismeteo-5.2.0/LICENSE
+-rw-r--r--   0        0        0     1346 2023-04-22 20:07:51.349263 pygismeteo-5.2.0/README.md
+-rw-r--r--   0        0        0      209 2023-04-21 20:30:00.863662 pygismeteo-5.2.0/pygismeteo/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-22 09:03:37.506335 pygismeteo-5.2.0/pygismeteo/_current.py
+-rw-r--r--   0        0        0     2818 2023-04-22 09:02:08.356344 pygismeteo-5.2.0/pygismeteo/_gismeteo.py
+-rw-r--r--   0        0        0     1288 2023-04-21 20:13:03.143666 pygismeteo-5.2.0/pygismeteo/_http.py
+-rw-r--r--   0        0        0     3921 2023-04-22 17:44:22.569254 pygismeteo-5.2.0/pygismeteo/_search.py
+-rw-r--r--   0        0        0     4632 2023-04-22 17:48:05.969246 pygismeteo-5.2.0/pygismeteo/_step_n.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:48:31.650689 pygismeteo-5.2.0/pygismeteo/py.typed
+-rw-r--r--   0        0        0      515 2023-05-01 09:10:15.371131 pygismeteo-5.2.0/pygismeteo/types.py
+-rw-r--r--   0        0        0     3130 2023-05-01 09:12:01.881139 pygismeteo-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 pygismeteo-5.2.0/PKG-INFO
```

### Comparing `pygismeteo-5.1.0/LICENSE` & `pygismeteo-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygismeteo-5.1.0/README.md` & `pygismeteo-5.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Обёртка для [Gismeteo API](https://gismeteo.ru/api/).
 
 Асинхронная версия [здесь](https://github.com/monosans/aiopygismeteo).
 
 ## Установка
 
 ```bash
-python -m pip install -U pygismeteo
+python -m pip install -U pygismeteo pygismeteo-base
 ```
 
 ## Документация
 
 <https://pygismeteo.readthedocs.io/>
 
 ## Пример, выводящий температуру в Москве сейчас
```

### Comparing `pygismeteo-5.1.0/pygismeteo/_current.py` & `pygismeteo-5.2.0/pygismeteo/_current.py`

 * *Files identical despite different names*

### Comparing `pygismeteo-5.1.0/pygismeteo/_gismeteo.py` & `pygismeteo-5.2.0/pygismeteo/_gismeteo.py`

 * *Files identical despite different names*

### Comparing `pygismeteo-5.1.0/pygismeteo/_http.py` & `pygismeteo-5.2.0/pygismeteo/_http.py`

 * *Files identical despite different names*

### Comparing `pygismeteo-5.1.0/pygismeteo/_search.py` & `pygismeteo-5.2.0/pygismeteo/_search.py`

 * *Files identical despite different names*

### Comparing `pygismeteo-5.1.0/pygismeteo/_step_n.py` & `pygismeteo-5.2.0/pygismeteo/_step_n.py`

 * *Files identical despite different names*

### Comparing `pygismeteo-5.1.0/pyproject.toml` & `pygismeteo-5.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygismeteo"
-version = "5.1.0"
+version = "5.2.0"
 description = "Wrapper for Gismeteo API"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/pygismeteo"
 documentation = "https://pygismeteo.readthedocs.io"
 classifiers = [
@@ -34,23 +34,23 @@
 black = "23.3.0"
 covdefaults = "2.3.0"
 mypy = "1.2.0"
 pre-commit = "2.21.0"
 pydantic = "1.10.7"
 pytest = "7.3.1"
 pytest-cov = "4.0.0"
-ruff = "0.0.262"
-types-requests = "2.28.11.17"
+ruff = "0.0.263"
+types-requests = "2.29.0.0"
 
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

### Comparing `pygismeteo-5.1.0/PKG-INFO` & `pygismeteo-5.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygismeteo
-Version: 5.1.0
+Version: 5.2.0
 Summary: Wrapper for Gismeteo API
 Home-page: https://github.com/monosans/pygismeteo
 License: MIT
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
@@ -45,15 +45,15 @@
 Обёртка для [Gismeteo API](https://gismeteo.ru/api/).
 
 Асинхронная версия [здесь](https://github.com/monosans/aiopygismeteo).
 
 ## Установка
 
 ```bash
-python -m pip install -U pygismeteo
+python -m pip install -U pygismeteo pygismeteo-base
 ```
 
 ## Документация
 
 <https://pygismeteo.readthedocs.io/>
 
 ## Пример, выводящий температуру в Москве сейчас
```

