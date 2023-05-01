# Comparing `tmp/mo_dots-9.368.23092-py2.py3-none-any.whl.zip` & `tmp/mo_dots-9.376.23121-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 25421 bytes, number of entries: 11
+Zip file size: 25457 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat    19983 b- defN 23-Apr-02 13:51 mo_dots/__init__.py
--rw-rw-rw-  2.0 fat    13831 b- defN 23-Apr-02 13:51 mo_dots/datas.py
+-rw-rw-rw-  2.0 fat    14049 b- defN 23-May-01 12:32 mo_dots/datas.py
 -rw-rw-rw-  2.0 fat     9899 b- defN 23-Apr-02 13:51 mo_dots/lists.py
 -rw-rw-rw-  2.0 fat     6670 b- defN 23-Apr-02 13:51 mo_dots/nones.py
 -rw-rw-rw-  2.0 fat     5088 b- defN 23-Apr-02 13:51 mo_dots/objects.py
 -rw-rw-rw-  2.0 fat     1490 b- defN 23-Apr-02 13:51 mo_dots/utils.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-02 13:51 mo_dots-9.368.23092.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4849 b- defN 23-Apr-02 13:51 mo_dots-9.368.23092.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-02 13:51 mo_dots-9.368.23092.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-02 13:51 mo_dots-9.368.23092.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      862 b- defN 23-Apr-02 13:51 mo_dots-9.368.23092.dist-info/RECORD
-11 files, 79515 bytes uncompressed, 23983 bytes compressed:  69.8%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4849 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      862 b- defN 23-May-01 12:32 mo_dots-9.376.23121.dist-info/RECORD
+11 files, 79733 bytes uncompressed, 24019 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mo_dots/objects.py
 Comment: 
 
 Filename: mo_dots/utils.py
 Comment: 
 
-Filename: mo_dots-9.368.23092.dist-info/LICENSE
+Filename: mo_dots-9.376.23121.dist-info/LICENSE
 Comment: 
 
-Filename: mo_dots-9.368.23092.dist-info/METADATA
+Filename: mo_dots-9.376.23121.dist-info/METADATA
 Comment: 
 
-Filename: mo_dots-9.368.23092.dist-info/WHEEL
+Filename: mo_dots-9.376.23121.dist-info/WHEEL
 Comment: 
 
-Filename: mo_dots-9.368.23092.dist-info/top_level.txt
+Filename: mo_dots-9.376.23121.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_dots-9.368.23092.dist-info/RECORD
+Filename: mo_dots-9.376.23121.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_dots/datas.py

```diff
@@ -420,15 +420,25 @@
         yield from _leaves(value, ".")
     else:
         for k, v in _leaves(value, "."):
             yield prefix + k, v
 
 
 def _leaves(value, parent):
-    for k, v in value.items():
+    if isinstance(value, Data):
+        d = _get(value, SLOT)
+        if isinstance(d, dict):
+            items = d.items()
+        else:
+            yield parent, d
+            return
+    else:
+        items = value.items()
+
+    for k, v in items:
         try:
             kk = concat_field(parent, literal_field(k))
             if _get(v, CLASS) in data_types:
                 yield from _leaves(v, kk)
             else:
                 yield kk, to_data(v)
         except Exception as e:
```

## Comparing `mo_dots-9.368.23092.dist-info/LICENSE` & `mo_dots-9.376.23121.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_dots-9.368.23092.dist-info/METADATA` & `mo_dots-9.376.23121.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.368.23092
+Version: 9.376.23121
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

