# Comparing `tmp/bel-digital-handwriting-py-0.0.1.tar.gz` & `tmp/bel-digital-handwriting-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bel-digital-handwriting-py-0.0.1.tar", last modified: Mon May  1 07:49:53 2023, max compression
+gzip compressed data, was "bel-digital-handwriting-py-0.0.2.tar", last modified: Mon May  1 08:13:43 2023, max compression
```

## Comparing `bel-digital-handwriting-py-0.0.1.tar` & `bel-digital-handwriting-py-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:49:53.979227 bel-digital-handwriting-py-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:49:53.975227 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/BelDHAnalyser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:49:53.975227 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Models/AnalyzeModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Models/SymbolModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Models/WordSentenceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/WordSentence.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-01 07:49:42.000000 bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 07:49:43.000000 bel-digital-handwriting-py-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 07:49:53.979227 bel-digital-handwriting-py-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-01 07:49:43.000000 bel-digital-handwriting-py-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:49:53.979227 bel-digital-handwriting-py-0.0.1/bel_digital_handwriting_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 07:49:53.000000 bel-digital-handwriting-py-0.0.1/bel_digital_handwriting_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 07:49:53.000000 bel-digital-handwriting-py-0.0.1/bel_digital_handwriting_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:49:53.000000 bel-digital-handwriting-py-0.0.1/bel_digital_handwriting_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 07:49:53.000000 bel-digital-handwriting-py-0.0.1/bel_digital_handwriting_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:49:53.979227 bel-digital-handwriting-py-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-01 07:49:43.000000 bel-digital-handwriting-py-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:13:43.073612 bel-digital-handwriting-py-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:13:43.073612 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/BelDHAnalyser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:13:43.073612 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Models/AnalyzeModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Models/SymbolModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Models/WordSentenceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/WordSentence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 08:13:43.073612 bel-digital-handwriting-py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:13:43.073612 bel-digital-handwriting-py-0.0.2/bel_digital_handwriting_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 08:13:43.000000 bel-digital-handwriting-py-0.0.2/bel_digital_handwriting_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 08:13:43.000000 bel-digital-handwriting-py-0.0.2/bel_digital_handwriting_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:13:43.000000 bel-digital-handwriting-py-0.0.2/bel_digital_handwriting_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 08:13:43.000000 bel-digital-handwriting-py-0.0.2/bel_digital_handwriting_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:13:43.073612 bel-digital-handwriting-py-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-01 08:13:29.000000 bel-digital-handwriting-py-0.0.2/setup.py
```

### Comparing `bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Models/AnalyzeModels.py` & `bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Models/AnalyzeModels.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Models/SymbolModels.py` & `bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Models/SymbolModels.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Models/WordSentenceModels.py` & `bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Models/WordSentenceModels.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/Symbol.py` & `bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/Symbol.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/WordSentence.py` & `bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/WordSentence.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/BelDigitalHandwriting/constants.py` & `bel-digital-handwriting-py-0.0.2/BelDigitalHandwriting/constants.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/LICENSE` & `bel-digital-handwriting-py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/PKG-INFO` & `bel-digital-handwriting-py-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bel-digital-handwriting-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Пакет для аналіза беларускіх тэкстаў і вызначэння лічбавага почырку пісьменніка
 Home-page: https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Author: Daniil Kononenko
 License: MIT
 Project-URL: Source, https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bel-digital-handwriting-py-0.0.1/README.md` & `bel-digital-handwriting-py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/bel_digital_handwriting_py.egg-info/PKG-INFO` & `bel-digital-handwriting-py-0.0.2/bel_digital_handwriting_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bel-digital-handwriting-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Пакет для аналіза беларускіх тэкстаў і вызначэння лічбавага почырку пісьменніка
 Home-page: https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Author: Daniil Kononenko
 License: MIT
 Project-URL: Source, https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bel-digital-handwriting-py-0.0.1/bel_digital_handwriting_py.egg-info/SOURCES.txt` & `bel-digital-handwriting-py-0.0.2/bel_digital_handwriting_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.1/setup.py` & `bel-digital-handwriting-py-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,16 @@
     long_description_content_type='text/markdown',
     url='https://github.com/Kononenko-Daniil/bel-digital-handwriting-py',
     author='Daniil Kononenko',
     package_dir={
         'BelDigitalHandwriting': 'BelDigitalHandwriting',
         'BelDigitalHandwriting.Models': 'BelDigitalHandwriting/Models'
     },
-    packages=['BelDigitalHandwriting', 'BelDigitalHandwriting.Models'],
+    packages=[
+        'BelDigitalHandwriting',
+        'BelDigitalHandwriting.Models',
+    ],
     license="MIT",
     project_urls={
         "Source": "https://github.com/Kononenko-Daniil/bel-digital-handwriting-py"
     }
 )
```

