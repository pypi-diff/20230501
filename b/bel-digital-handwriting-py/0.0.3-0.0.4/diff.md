# Comparing `tmp/bel-digital-handwriting-py-0.0.3.tar.gz` & `tmp/bel-digital-handwriting-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bel-digital-handwriting-py-0.0.3.tar", last modified: Mon May  1 08:22:48 2023, max compression
+gzip compressed data, was "bel-digital-handwriting-py-0.0.4.tar", last modified: Mon May  1 08:29:07 2023, max compression
```

## Comparing `bel-digital-handwriting-py-0.0.3.tar` & `bel-digital-handwriting-py-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:22:48.838103 bel-digital-handwriting-py-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:22:48.834103 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/BelDHAnalyser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:22:48.838103 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Models/AnalyzeModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Models/SymbolModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Models/WordSentenceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/WordSentence.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 08:22:48.838103 bel-digital-handwriting-py-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:22:48.838103 bel-digital-handwriting-py-0.0.3/bel_digital_handwriting_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 08:22:48.000000 bel-digital-handwriting-py-0.0.3/bel_digital_handwriting_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 08:22:48.000000 bel-digital-handwriting-py-0.0.3/bel_digital_handwriting_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:22:48.000000 bel-digital-handwriting-py-0.0.3/bel_digital_handwriting_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 08:22:48.000000 bel-digital-handwriting-py-0.0.3/bel_digital_handwriting_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:22:48.838103 bel-digital-handwriting-py-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-01 08:22:27.000000 bel-digital-handwriting-py-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:07.611815 bel-digital-handwriting-py-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:07.527815 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/BelDHAnalyser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:07.531815 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Models/AnalyzeModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Models/SymbolModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Models/WordSentenceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/WordSentence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:07.611815 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/chastica.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  4950968 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/dzeeprymetnik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1360943 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/dzeeprysloue.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 13381977 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/dzeyaslou.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/lychebnik.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 17334871 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/nazounik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/pabochnae_slova.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/predycatiu.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 22399390 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/prymetnik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/prynazounik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   303108 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/prysloue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/vyklichnik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/zaymenik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/slouniki_parsed/zluchnik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 08:29:07.611815 bel-digital-handwriting-py-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:29:07.611815 bel-digital-handwriting-py-0.0.4/bel_digital_handwriting_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 08:29:07.000000 bel-digital-handwriting-py-0.0.4/bel_digital_handwriting_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-01 08:29:07.000000 bel-digital-handwriting-py-0.0.4/bel_digital_handwriting_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:29:07.000000 bel-digital-handwriting-py-0.0.4/bel_digital_handwriting_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 08:29:07.000000 bel-digital-handwriting-py-0.0.4/bel_digital_handwriting_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:29:07.611815 bel-digital-handwriting-py-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-01 08:28:50.000000 bel-digital-handwriting-py-0.0.4/setup.py
```

### Comparing `bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Models/AnalyzeModels.py` & `bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Models/AnalyzeModels.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Models/SymbolModels.py` & `bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Models/SymbolModels.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Models/WordSentenceModels.py` & `bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Models/WordSentenceModels.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/Symbol.py` & `bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/Symbol.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/WordSentence.py` & `bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/WordSentence.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/BelDigitalHandwriting/constants.py` & `bel-digital-handwriting-py-0.0.4/BelDigitalHandwriting/constants.py`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/LICENSE` & `bel-digital-handwriting-py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/PKG-INFO` & `bel-digital-handwriting-py-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bel-digital-handwriting-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Пакет для аналіза беларускіх тэкстаў і вызначэння лічбавага почырку пісьменніка
 Home-page: https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Author: Daniil Kononenko
 License: MIT
 Project-URL: Source, https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bel-digital-handwriting-py-0.0.3/README.md` & `bel-digital-handwriting-py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bel-digital-handwriting-py-0.0.3/bel_digital_handwriting_py.egg-info/PKG-INFO` & `bel-digital-handwriting-py-0.0.4/bel_digital_handwriting_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bel-digital-handwriting-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Пакет для аналіза беларускіх тэкстаў і вызначэння лічбавага почырку пісьменніка
 Home-page: https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Author: Daniil Kononenko
 License: MIT
 Project-URL: Source, https://github.com/Kononenko-Daniil/bel-digital-handwriting-py
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bel-digital-handwriting-py-0.0.3/setup.py` & `bel-digital-handwriting-py-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,13 @@
         'BelDigitalHandwriting': 'BelDigitalHandwriting',
         'BelDigitalHandwriting.Models': 'BelDigitalHandwriting/Models'
     },
     packages=[
         'BelDigitalHandwriting',
         'BelDigitalHandwriting.Models',
     ],
+    package_data={'BelDigitalHandwriting': ['slouniki_parsed/*.txt']},
     license="MIT",
     project_urls={
         "Source": "https://github.com/Kononenko-Daniil/bel-digital-handwriting-py"
     }
 )
```

