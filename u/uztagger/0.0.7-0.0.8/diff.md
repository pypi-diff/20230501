# Comparing `tmp/uztagger-0.0.7-py3-none-any.whl.zip` & `tmp/uztagger-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 351009 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     5566 b- defN 22-Aug-22 06:42 uztagger/__init__.py
+Zip file size: 351008 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     5554 b- defN 23-May-01 12:10 uztagger/__init__.py
 -rw-rw-rw-  2.0 fat  1066063 b- defN 22-Aug-15 06:00 uztagger/lexicon.csv
 -rw-rw-rw-  2.0 fat     1161 b- defN 22-Aug-15 06:00 uztagger/non_affixed_word.csv
 -rw-rw-rw-  2.0 fat    85846 b- defN 22-Aug-16 08:01 uztagger/web-interface-ui.png
--rw-rw-rw-  2.0 fat     1091 b- defN 22-Aug-22 07:39 uztagger-0.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4033 b- defN 22-Aug-22 07:39 uztagger-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-22 07:39 uztagger-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Aug-22 07:39 uztagger-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      720 b- defN 22-Aug-22 07:39 uztagger-0.0.7.dist-info/RECORD
-9 files, 1164581 bytes uncompressed, 349779 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4029 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      720 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/RECORD
+9 files, 1164565 bytes uncompressed, 349778 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: uztagger/non_affixed_word.csv
 Comment: 
 
 Filename: uztagger/web-interface-ui.png
 Comment: 
 
-Filename: uztagger-0.0.7.dist-info/LICENSE
+Filename: uztagger-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: uztagger-0.0.7.dist-info/METADATA
+Filename: uztagger-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: uztagger-0.0.7.dist-info/WHEEL
+Filename: uztagger-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: uztagger-0.0.7.dist-info/top_level.txt
+Filename: uztagger-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: uztagger-0.0.7.dist-info/RECORD
+Filename: uztagger-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uztagger/__init__.py

```diff
@@ -27,15 +27,15 @@
             df_non_aff = pd.read_csv(f)
 
         with open(os.path.join(dirname + "lexicon.csv"), "r", encoding='utf-8') as f:
             df_lexicon = pd.read_csv(f)
 
         df_lexicon = df_lexicon.sort_values(by="stem", key=lambda x: x.str.len())  # sorting to stands a small one at top, after that get first item as a result
 
-        uzmorph = UzMorphAnalyser.UzMorphAnalyser()
+        uzmorph = UzMorphAnalyser()
 
         punctuation = {'.', ',', '!', '?', ':'}  # punctuation list, set pos tag as "PUNC"
         symbol = {'$', '*', '#', '@', '%'}  # symbol list, set pos tag as "SYM"
 
         for token in tokens:
             # 3. check from ready list
             # 3.1 check from punctuation list
@@ -140,11 +140,11 @@
 # Lower case conversion
 # Stop Words removal
 # Stemming
 # Lemmatization
 # Parse tree or Syntax Tree generation
 # POS Tagging
 
-'''text = "Men va G'ulom ba’zan bollar 25-sanada parkka bormoqchimiz."
-obj = Tagger()
-res = obj.pos_tag(text)
-print(res)'''
+# text = "Men va G'ulom ba’zan bollar 25-sanada parkka bormoqchimiz."
+# obj = Tagger()
+# res = obj.pos_tag(text)
+# print(res)
```

## Comparing `uztagger-0.0.7.dist-info/LICENSE` & `uztagger-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uztagger-0.0.7.dist-info/METADATA` & `uztagger-0.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uztagger
-Version: 0.0.7
+Version: 0.0.8
 Summary: uztagger | Uzbek Morphological Part of Speech (POS) Tagging on Python
 Home-page: https://github.com/UlugbekSalaev/uztagger
 Author: Ulugbek Salaev
 Author-email: ulugbek0302@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/uztagger/issues
 Keywords: mophology,uzbek-language,pos tagging,morphological tagging
@@ -29,19 +29,19 @@
 ## About project
 The tool is focused to make tagging sentence with morphological Part of Speech (POS) tagset of Uzbek word based on morphemes. The tool includes list of POS tagset, tagging method.
 
 ## Quick links
 
 - [Github](https://github.com/UlugbekSalaev/uztagger)
 - [PyPI](https://pypi.org/project/uztagger/)
-- [Web-UI](https://nlp.urdu.uz/?menu=postagging)
+- [Web-UI](https://nlp.urdu.uz/?menu=uztagger)
 
 ## Demo
 
-You can use [web interface](http://nlp.urdu.uz/?menu=postagging).
+You can use [web interface](http://nlp.urdu.uz/?menu=uztagger).
 
 ## Features
 
 - Tagging 
 - POS tag list
 - Help function
```

## Comparing `uztagger-0.0.7.dist-info/RECORD` & `uztagger-0.0.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-uztagger/__init__.py,sha256=Vd9GpFz7IiHVcOc3U1yMhkQWheLskvBVqst5ngK_u3w,5566
+uztagger/__init__.py,sha256=iVj5najfigCoRWvE1DMytiLwjAQzv0yLLyh4kQ3uwBc,5554
 uztagger/lexicon.csv,sha256=MkiosgciuDdZeh0MPdTW-Di1FMA8WTRNBrAwQEljj7Y,1066063
 uztagger/non_affixed_word.csv,sha256=iECecb6vWMajPm_L2gxpDJ2_PcnQuXBLNoOjfEFSQls,1161
 uztagger/web-interface-ui.png,sha256=IxLn0GkjC_79JfupXUGGUVc5l2G2-TlDxW4eH9naoA0,85846
-uztagger-0.0.7.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-uztagger-0.0.7.dist-info/METADATA,sha256=8Ls0WzEdOgZ460e9zeVueJdP8C6jgkWurPFgWrJQIc0,4033
-uztagger-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-uztagger-0.0.7.dist-info/top_level.txt,sha256=uaDS85LyY_8T_MoTYuGFvsBD0UwQ90m7jhWirfybf1M,9
-uztagger-0.0.7.dist-info/RECORD,,
+uztagger-0.0.8.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+uztagger-0.0.8.dist-info/METADATA,sha256=15ELScVJ-aoNgupFxtLcGwYNZQLWNFMu7XN3QiII12k,4029
+uztagger-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+uztagger-0.0.8.dist-info/top_level.txt,sha256=uaDS85LyY_8T_MoTYuGFvsBD0UwQ90m7jhWirfybf1M,9
+uztagger-0.0.8.dist-info/RECORD,,
```

