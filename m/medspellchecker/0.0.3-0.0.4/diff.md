# Comparing `tmp/medspellchecker-0.0.3.tar.gz` & `tmp/medspellchecker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspellchecker-0.0.3.tar", last modified: Sat Apr 29 17:52:57 2023, max compression
+gzip compressed data, was "medspellchecker-0.0.4.tar", last modified: Mon May  1 12:21:32 2023, max compression
```

## Comparing `medspellchecker-0.0.3.tar` & `medspellchecker-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.527343 medspellchecker-0.0.3/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    11357 2022-08-03 12:33:44.000000 medspellchecker-0.0.3/LICENSE
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       36 2023-04-29 17:52:50.000000 medspellchecker-0.0.3/MANIFEST.in
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     6333 2023-04-29 17:24:30.000000 medspellchecker-0.0.3/PACKAGE.md
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     7316 2023-04-29 17:52:57.527343 medspellchecker-0.0.3/PKG-INFO
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.519343 medspellchecker-0.0.3/medspellchecker/
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.523342 medspellchecker-0.0.3/medspellchecker/tool/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     8720 2023-03-24 21:02:33.000000 medspellchecker-0.0.3/medspellchecker/tool/abstract_bert_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3080 2023-03-24 21:02:33.000000 medspellchecker-0.0.3/medspellchecker/tool/abstract_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    14945 2022-12-16 21:23:05.000000 medspellchecker-0.0.3/medspellchecker/tool/candidate_generator.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      330 2022-12-14 21:21:48.000000 medspellchecker-0.0.3/medspellchecker/tool/candidate_word.py
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.523342 medspellchecker-0.0.3/medspellchecker/tool/data/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)  4603445 2022-08-03 12:33:45.000000 medspellchecker-0.0.3/medspellchecker/tool/data/processed_lemmatized_all_dict.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      581 2022-12-16 21:23:05.000000 medspellchecker-0.0.3/medspellchecker/tool/distilbert_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4393 2022-12-14 21:21:48.000000 medspellchecker-0.0.3/medspellchecker/tool/edit_distance.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2434 2022-12-14 21:21:48.000000 medspellchecker-0.0.3/medspellchecker/tool/gpu_utils.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    13812 2023-04-22 11:19:05.000000 medspellchecker-0.0.3/medspellchecker/tool/medspellchecker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      169 2023-03-23 20:05:58.000000 medspellchecker-0.0.3/medspellchecker/tool/mistake_type.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4089 2023-04-10 18:03:51.000000 medspellchecker-0.0.3/medspellchecker/tool/pre_post_processor.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      568 2022-12-16 21:23:05.000000 medspellchecker-0.0.3/medspellchecker/tool/roberta_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      569 2022-12-16 23:37:30.000000 medspellchecker-0.0.3/medspellchecker/tool/rubert_tiny2_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      556 2023-03-17 18:40:55.000000 medspellchecker-0.0.3/medspellchecker/tool/rubioberta_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      563 2023-03-17 18:40:55.000000 medspellchecker-0.0.3/medspellchecker/tool/rubioroberta_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      938 2023-04-08 20:00:29.000000 medspellchecker-0.0.3/medspellchecker/tool/word.py
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.523342 medspellchecker-0.0.3/medspellchecker.egg-info/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     7316 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/PKG-INFO
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      963 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        1 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      173 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/requires.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       16 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/top_level.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       38 2023-04-29 17:52:57.527343 medspellchecker-0.0.3/setup.cfg
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2019 2023-04-29 17:50:35.000000 medspellchecker-0.0.3/setup.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-05-01 12:21:32.771818 medspellchecker-0.0.4/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    11357 2022-08-03 12:33:44.000000 medspellchecker-0.0.4/LICENSE
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       36 2023-04-29 17:52:50.000000 medspellchecker-0.0.4/MANIFEST.in
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     6333 2023-04-29 17:24:30.000000 medspellchecker-0.0.4/PACKAGE.md
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     7316 2023-05-01 12:21:32.771818 medspellchecker-0.0.4/PKG-INFO
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-05-01 12:21:32.763818 medspellchecker-0.0.4/medspellchecker/
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-05-01 12:21:32.767818 medspellchecker-0.0.4/medspellchecker/tool/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     8720 2023-03-24 21:02:33.000000 medspellchecker-0.0.4/medspellchecker/tool/abstract_bert_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3080 2023-03-24 21:02:33.000000 medspellchecker-0.0.4/medspellchecker/tool/abstract_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    14945 2022-12-16 21:23:05.000000 medspellchecker-0.0.4/medspellchecker/tool/candidate_generator.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      330 2022-12-14 21:21:48.000000 medspellchecker-0.0.4/medspellchecker/tool/candidate_word.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-05-01 12:21:32.767818 medspellchecker-0.0.4/medspellchecker/tool/data/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)  4603445 2022-08-03 12:33:45.000000 medspellchecker-0.0.4/medspellchecker/tool/data/processed_lemmatized_all_dict.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      581 2022-12-16 21:23:05.000000 medspellchecker-0.0.4/medspellchecker/tool/distilbert_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4393 2022-12-14 21:21:48.000000 medspellchecker-0.0.4/medspellchecker/tool/edit_distance.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2434 2022-12-14 21:21:48.000000 medspellchecker-0.0.4/medspellchecker/tool/gpu_utils.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    13732 2023-05-01 12:20:26.000000 medspellchecker-0.0.4/medspellchecker/tool/medspellchecker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      169 2023-03-23 20:05:58.000000 medspellchecker-0.0.4/medspellchecker/tool/mistake_type.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4089 2023-04-10 18:03:51.000000 medspellchecker-0.0.4/medspellchecker/tool/pre_post_processor.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      568 2022-12-16 21:23:05.000000 medspellchecker-0.0.4/medspellchecker/tool/roberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      569 2022-12-16 23:37:30.000000 medspellchecker-0.0.4/medspellchecker/tool/rubert_tiny2_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      556 2023-03-17 18:40:55.000000 medspellchecker-0.0.4/medspellchecker/tool/rubioberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      563 2023-03-17 18:40:55.000000 medspellchecker-0.0.4/medspellchecker/tool/rubioroberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      938 2023-04-08 20:00:29.000000 medspellchecker-0.0.4/medspellchecker/tool/word.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-05-01 12:21:32.767818 medspellchecker-0.0.4/medspellchecker.egg-info/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     7316 2023-05-01 12:21:32.000000 medspellchecker-0.0.4/medspellchecker.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      963 2023-05-01 12:21:32.000000 medspellchecker-0.0.4/medspellchecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        1 2023-05-01 12:21:32.000000 medspellchecker-0.0.4/medspellchecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      173 2023-05-01 12:21:32.000000 medspellchecker-0.0.4/medspellchecker.egg-info/requires.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       16 2023-05-01 12:21:32.000000 medspellchecker-0.0.4/medspellchecker.egg-info/top_level.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       38 2023-05-01 12:21:32.771818 medspellchecker-0.0.4/setup.cfg
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2004 2023-05-01 12:21:19.000000 medspellchecker-0.0.4/setup.py
```

### Comparing `medspellchecker-0.0.3/LICENSE` & `medspellchecker-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/PACKAGE.md` & `medspellchecker-0.0.4/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/PKG-INFO` & `medspellchecker-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medspellchecker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast and effective spellchecker for Russian medical texts
 Home-page: https://github.com/DmitryPogrebnoy/MedSpellChecker
 Author: Dmitry Pogrebnoy
 Author-email: pogrebnoy.inc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/DmitryPogrebnoy/MedSpellChecker/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/abstract_bert_candidate_ranker.py` & `medspellchecker-0.0.4/medspellchecker/tool/abstract_bert_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/abstract_candidate_ranker.py` & `medspellchecker-0.0.4/medspellchecker/tool/abstract_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/candidate_generator.py` & `medspellchecker-0.0.4/medspellchecker/tool/candidate_generator.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/data/processed_lemmatized_all_dict.txt` & `medspellchecker-0.0.4/medspellchecker/tool/data/processed_lemmatized_all_dict.txt`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/distilbert_candidate_ranker.py` & `medspellchecker-0.0.4/medspellchecker/tool/distilbert_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/edit_distance.py` & `medspellchecker-0.0.4/medspellchecker/tool/edit_distance.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/gpu_utils.py` & `medspellchecker-0.0.4/medspellchecker/tool/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/medspellchecker.py` & `medspellchecker-0.0.4/medspellchecker/tool/medspellchecker.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,15 @@
             best_candidate_word_part_second: str = best_candidate_word_split[1]
 
             restored_first_part: str = self._pre_processor.str_restore_original_form(
                 best_candidate_word_part_first, best_candidate_word_tuple[2])
             restored_second_part: str = self._pre_processor.str_restore_original_form(
                 best_candidate_word_part_second, best_candidate_word_tuple[3])
 
-            # return CandidateWord(f"{restored_first_part} {restored_second_part}", 1), best_candidate_word_tuple[1]
-            return best_candidate_word_tuple[0], best_candidate_word_tuple[1]
+            return CandidateWord(f"{restored_first_part} {restored_second_part}", 1), best_candidate_word_tuple[1]
         else:
             return None
 
     # TODO: Do I need to save the formatting after fixing? -- no for now,
     #  usually formatting is not necessary for ml tasks
     def fix_text(self, text: str) -> str:
         # Remove newlines as the MosesTokenizer fails on newlines.
```

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/pre_post_processor.py` & `medspellchecker-0.0.4/medspellchecker/tool/pre_post_processor.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/roberta_candidate_ranker.py` & `medspellchecker-0.0.4/medspellchecker/tool/roberta_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/rubert_tiny2_candidate_ranker.py` & `medspellchecker-0.0.4/medspellchecker/tool/rubert_tiny2_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/rubioberta_candidate_ranker.py` & `medspellchecker-0.0.4/medspellchecker/tool/rubioberta_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/rubioroberta_candidate_ranker.py` & `medspellchecker-0.0.4/medspellchecker/tool/rubioroberta_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker/tool/word.py` & `medspellchecker-0.0.4/medspellchecker/tool/word.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/medspellchecker.egg-info/PKG-INFO` & `medspellchecker-0.0.4/medspellchecker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medspellchecker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast and effective spellchecker for Russian medical texts
 Home-page: https://github.com/DmitryPogrebnoy/MedSpellChecker
 Author: Dmitry Pogrebnoy
 Author-email: pogrebnoy.inc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/DmitryPogrebnoy/MedSpellChecker/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `medspellchecker-0.0.3/medspellchecker.egg-info/SOURCES.txt` & `medspellchecker-0.0.4/medspellchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.3/setup.py` & `medspellchecker-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pathlib
 
-from setuptools import find_packages, setup
+from setuptools import setup
 
 here = pathlib.Path(__file__).parent.resolve()
 print(here / 'PACKAGE.md')
 # Get the long description from the README file
 long_description = (here / 'PACKAGE.md').read_text(encoding='utf-8')
 
 setup(
     name='medspellchecker',
-    version='0.0.3',
+    version='0.0.4',
     description='Fast and effective spellchecker for Russian medical texts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DmitryPogrebnoy/MedSpellChecker',
     author='Dmitry Pogrebnoy',
     author_email='pogrebnoy.inc@gmail.com',
     license='Apache License 2.0',
```

