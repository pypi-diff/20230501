# Comparing `tmp/numberize-1.0.2.tar.gz` & `tmp/numberize-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\emche\Documents\GitHub\numberize\dist\tmpmdwc9_ml\numberize-1.0.2.tar", last modified: Mon Nov  8 13:18:05 2021, max compression
+gzip compressed data, was "numberize-1.0.3.tar", last modified: Mon May  1 12:13:05 2023, max compression
```

## Comparing `numberize-1.0.2.tar` & `numberize-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2021-11-08 13:18:05.197862 numberize-1.0.2/
--rw-rw-rw-   0        0        0     1073 2021-11-02 14:30:50.000000 numberize-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1268 2021-11-08 13:18:05.196688 numberize-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      630 2021-11-02 14:30:50.000000 numberize-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2021-11-08 13:18:05.078907 numberize-1.0.2/numberize/
--rw-rw-rw-   0        0        0      105 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/__init__.py
--rw-rw-rw-   0        0        0     1646 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/calculators.py
--rw-rw-rw-   0        0        0      169 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/dawgs.py
-drwxrwxrwx   0        0        0        0 2021-11-08 13:18:05.193837 numberize-1.0.2/numberize/dicts/
--rw-rw-rw-   0        0        0       91 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/dicts/__init__.py
--rw-rw-rw-   0        0        0      579 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/dicts/en.py
--rw-rw-rw-   0        0        0     1101 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/dicts/ru.py
--rw-rw-rw-   0        0        0     1085 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/dicts/uk.py
--rw-rw-rw-   0        0        0     2150 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/linguists.py
--rw-rw-rw-   0        0        0      507 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/numberizer.py
--rw-rw-rw-   0        0        0     2339 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/replacers.py
--rw-rw-rw-   0        0        0     2951 2021-11-02 14:30:50.000000 numberize-1.0.2/numberize/tokenizers.py
-drwxrwxrwx   0        0        0        0 2021-11-08 13:18:05.183062 numberize-1.0.2/numberize.egg-info/
--rw-rw-rw-   0        0        0     1268 2021-11-08 13:18:05.000000 numberize-1.0.2/numberize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2021-11-08 13:18:05.000000 numberize-1.0.2/numberize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-08 13:18:05.000000 numberize-1.0.2/numberize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2021-11-08 13:18:05.000000 numberize-1.0.2/numberize.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-11-08 13:18:05.000000 numberize-1.0.2/numberize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-08 13:18:05.197862 numberize-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1026 2021-11-08 13:14:36.000000 numberize-1.0.2/setup.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:13:05.579811 numberize-1.0.3/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1073 2023-05-01 11:12:42.000000 numberize-1.0.3/LICENSE
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1185 2023-05-01 12:13:05.579811 numberize-1.0.3/PKG-INFO
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      630 2023-05-01 11:12:42.000000 numberize-1.0.3/README.md
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:13:05.579811 numberize-1.0.3/numberize/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      105 2023-05-01 11:12:42.000000 numberize-1.0.3/numberize/__init__.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1646 2023-05-01 11:12:42.000000 numberize-1.0.3/numberize/calculators.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:13:05.579811 numberize-1.0.3/numberize/dicts/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       91 2023-05-01 11:12:42.000000 numberize-1.0.3/numberize/dicts/__init__.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      479 2023-05-01 11:51:54.000000 numberize-1.0.3/numberize/dicts/en.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      981 2023-05-01 11:51:54.000000 numberize-1.0.3/numberize/dicts/ru.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      965 2023-05-01 11:51:54.000000 numberize-1.0.3/numberize/dicts/uk.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2150 2023-05-01 11:51:54.000000 numberize-1.0.3/numberize/linguists.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      507 2023-05-01 11:12:42.000000 numberize-1.0.3/numberize/numberizer.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2339 2023-05-01 11:12:42.000000 numberize-1.0.3/numberize/replacers.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2951 2023-05-01 11:12:42.000000 numberize-1.0.3/numberize/tokenizers.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:13:05.579811 numberize-1.0.3/numberize.egg-info/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1185 2023-05-01 12:13:05.000000 numberize-1.0.3/numberize.egg-info/PKG-INFO
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      500 2023-05-01 12:13:05.000000 numberize-1.0.3/numberize.egg-info/SOURCES.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)        1 2023-05-01 12:13:05.000000 numberize-1.0.3/numberize.egg-info/dependency_links.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       40 2023-05-01 12:13:05.000000 numberize-1.0.3/numberize.egg-info/requires.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       10 2023-05-01 12:13:05.000000 numberize-1.0.3/numberize.egg-info/top_level.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       38 2023-05-01 12:13:05.579811 numberize-1.0.3/setup.cfg
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1018 2023-05-01 12:12:18.000000 numberize-1.0.3/setup.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:13:05.579811 numberize-1.0.3/tests/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1005 2023-05-01 11:12:42.000000 numberize-1.0.3/tests/test_calculators.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1482 2023-05-01 11:12:42.000000 numberize-1.0.3/tests/test_linguists.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2536 2023-05-01 11:12:42.000000 numberize-1.0.3/tests/test_numberizer.py
```

### Comparing `numberize-1.0.2/LICENSE` & `numberize-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `numberize-1.0.2/PKG-INFO` & `numberize-1.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-Metadata-Version: 2.1
-Name: numberize
-Version: 1.0.2
-Summary: Replace numerals with numbers
-Home-page: https://github.com/DanATW/numberize.git
-Author: YemchenkoDS
-Author-email: emchenko@dlit.dp.ua
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/DanATW/numberize/issues
-Keywords: text replace numerals words numbers morphology
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Short Info
-Replace numerals with corresponding numbers in the given text.
-Available on [PyPI](https://pypi.org/project/numberize/).
-Consider checking out [Wiki](https://github.com/DanATW/numberize/wiki) for more info.
-## Supported languages
-* Ukrainian
-* Russian
-* English
-## Requirements
-* python 3.6+
-* NLTK Data
-
-## How to install it?
-```pip install numberize```
-
-## How to install requirements?
-After installing this package
-
-```python -m nltk.downloader punkt```
-
-## How to use it?
-```
-import numberize
-numberizer = numberize.Numberizer(lang='ru')    #or 'uk', 'en'
-new_text = numberizer.replace_numerals(old_text)
-   ```
-
-
+Metadata-Version: 2.1
+Name: numberize
+Version: 1.0.3
+Summary: Replace numerals with numbers
+Home-page: https://github.com/DanATW/numberize.git
+Author: YemchenkoDS
+Author-email: emchenko@dlit.dp.ua
+Project-URL: Bug Tracker, https://github.com/DanATW/numberize/issues
+Keywords: text replace numerals words numbers morphology
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Short Info
+Replace numerals with corresponding numbers in the given text.
+Available on [PyPI](https://pypi.org/project/numberize/).
+Consider checking out [Wiki](https://github.com/DanATW/numberize/wiki) for more info.
+## Supported languages
+* Ukrainian
+* Russian
+* English
+## Requirements
+* python 3.6+
+* NLTK Data
+
+## How to install it?
+```pip install numberize```
+
+## How to install requirements?
+After installing this package
+
+```python -m nltk.downloader punkt```
+
+## How to use it?
+```
+import numberize
+numberizer = numberize.Numberizer(lang='ru')    #or 'uk', 'en'
+new_text = numberizer.replace_numerals(old_text)
+   ```
```

### Comparing `numberize-1.0.2/README.md` & `numberize-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `numberize-1.0.2/numberize/calculators.py` & `numberize-1.0.3/numberize/calculators.py`

 * *Files identical despite different names*

### Comparing `numberize-1.0.2/numberize/linguists.py` & `numberize-1.0.3/numberize/linguists.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import Optional
 
 import pymorphy2
 
-import numberize.dawgs as dawgs
+import numberize.dicts as dicts
 
 
 class Linguist(ABC):
     @staticmethod
     @abstractmethod
     def get_number(token: str) -> Optional[int]:
         """
@@ -22,37 +22,37 @@
     @staticmethod
     def get_number(token: str) -> Optional[int]:
         token = token.lower()
         if '-' in token:
             parts = token.split('-')
             if len(parts) != 2:
                 return
-            left = dawgs.en_nums.get(parts[0])
+            left = dicts.en.nums.get(parts[0])
             if not left or left < 20 or left > 90:
                 return
-            right = dawgs.en_nums.get(parts[1])
+            right = dicts.en.nums.get(parts[1])
             if not right or right > 9 or right < 1:
                 return
             return left + right
-        return dawgs.en_nums.get(token)
+        return dicts.en.nums.get(token)
 
 
 class RuLinguist(Linguist):
     def __init__(self, morph: 'pymorphy2.MorphAnalyzer'):
         """
         :param morph: MorphAnalyzer to normalize words
         """
         self.analyzer = morph
 
     def get_number(self, token: str) -> Optional[int]:
         token = token.lower()
         if token[-1] == '.' and len(token) > 3:
             token = token[:-1]
         for form in self.analyzer.normal_forms(token):
-            number = dawgs.ru_nums.get(form)
+            number = dicts.ru.nums.get(form)
             if number:
                 return number
 
 
 class UkLinguist(Linguist):
     def __init__(self, morph: 'pymorphy2.MorphAnalyzer'):
         """
@@ -61,10 +61,10 @@
         self.analyzer = morph
 
     def get_number(self, token: str) -> Optional[int]:
         token = token.lower()
         if token[-1] == '.' and len(token) > 3:  # TokTokTokenizer sometimes
             token = token[:-1]              # doesn't tokenize points "тисяча."
         for form in self.analyzer.normal_forms(token):
-            number = dawgs.uk_nums.get(form)
+            number = dicts.uk.nums.get(form)
             if number:
                 return number
```

### Comparing `numberize-1.0.2/numberize/replacers.py` & `numberize-1.0.3/numberize/replacers.py`

 * *Files identical despite different names*

### Comparing `numberize-1.0.2/numberize/tokenizers.py` & `numberize-1.0.3/numberize/tokenizers.py`

 * *Files identical despite different names*

### Comparing `numberize-1.0.2/numberize.egg-info/PKG-INFO` & `numberize-1.0.3/numberize.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-Metadata-Version: 2.1
-Name: numberize
-Version: 1.0.2
-Summary: Replace numerals with numbers
-Home-page: https://github.com/DanATW/numberize.git
-Author: YemchenkoDS
-Author-email: emchenko@dlit.dp.ua
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/DanATW/numberize/issues
-Keywords: text replace numerals words numbers morphology
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Short Info
-Replace numerals with corresponding numbers in the given text.
-Available on [PyPI](https://pypi.org/project/numberize/).
-Consider checking out [Wiki](https://github.com/DanATW/numberize/wiki) for more info.
-## Supported languages
-* Ukrainian
-* Russian
-* English
-## Requirements
-* python 3.6+
-* NLTK Data
-
-## How to install it?
-```pip install numberize```
-
-## How to install requirements?
-After installing this package
-
-```python -m nltk.downloader punkt```
-
-## How to use it?
-```
-import numberize
-numberizer = numberize.Numberizer(lang='ru')    #or 'uk', 'en'
-new_text = numberizer.replace_numerals(old_text)
-   ```
-
-
+Metadata-Version: 2.1
+Name: numberize
+Version: 1.0.3
+Summary: Replace numerals with numbers
+Home-page: https://github.com/DanATW/numberize.git
+Author: YemchenkoDS
+Author-email: emchenko@dlit.dp.ua
+Project-URL: Bug Tracker, https://github.com/DanATW/numberize/issues
+Keywords: text replace numerals words numbers morphology
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Short Info
+Replace numerals with corresponding numbers in the given text.
+Available on [PyPI](https://pypi.org/project/numberize/).
+Consider checking out [Wiki](https://github.com/DanATW/numberize/wiki) for more info.
+## Supported languages
+* Ukrainian
+* Russian
+* English
+## Requirements
+* python 3.6+
+* NLTK Data
+
+## How to install it?
+```pip install numberize```
+
+## How to install requirements?
+After installing this package
+
+```python -m nltk.downloader punkt```
+
+## How to use it?
+```
+import numberize
+numberizer = numberize.Numberizer(lang='ru')    #or 'uk', 'en'
+new_text = numberizer.replace_numerals(old_text)
+   ```
```

### Comparing `numberize-1.0.2/setup.py` & `numberize-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="numberize",
-    version="1.0.2",
+    version="1.0.3",
     author="YemchenkoDS",
     author_email="emchenko@dlit.dp.ua",
     description="Replace numerals with numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanATW/numberize.git",
     project_urls={
@@ -22,12 +22,12 @@
     ],
     keywords='text replace numerals words numbers morphology',
     packages=[
         'numberize',
         'numberize.dicts'
     ],
     python_requires=">=3.6",
-    install_requires=['pymorphy2[fast]', 'pymorphy2-dicts-uk', 'nltk', 'DAWG'],
+    install_requires=['pymorphy2[fast]', 'pymorphy2-dicts-uk', 'nltk'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest==6.2.4'],
     test_suite='tests'
 )
```

