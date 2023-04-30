# Comparing `tmp/DinoHash-0.5-py3-none-any.whl.zip` & `tmp/DinoHash-0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3700 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     4709 b- defN 23-Apr-30 21:54 Dino/__init__.py
--rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-30 21:55 DinoHash-0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-30 21:55 DinoHash-0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-30 21:55 DinoHash-0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      365 b- defN 23-Apr-30 21:55 DinoHash-0.5.dist-info/RECORD
-5 files, 5397 bytes uncompressed, 3018 bytes compressed:  44.1%
+Zip file size: 3706 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     4714 b- defN 23-Apr-30 21:58 Dino/__init__.py
+-rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-30 22:01 DinoHash-0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-30 22:01 DinoHash-0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-30 22:01 DinoHash-0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      365 b- defN 23-Apr-30 22:01 DinoHash-0.6.dist-info/RECORD
+5 files, 5402 bytes uncompressed, 3024 bytes compressed:  44.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: Dino/__init__.py
 Comment: 
 
-Filename: DinoHash-0.5.dist-info/METADATA
+Filename: DinoHash-0.6.dist-info/METADATA
 Comment: 
 
-Filename: DinoHash-0.5.dist-info/WHEEL
+Filename: DinoHash-0.6.dist-info/WHEEL
 Comment: 
 
-Filename: DinoHash-0.5.dist-info/top_level.txt
+Filename: DinoHash-0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: DinoHash-0.5.dist-info/RECORD
+Filename: DinoHash-0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Dino/__init__.py

```diff
@@ -1,12 +1,12 @@
 import sys
 
 class Dn(object):
 	def hash(self, argv=None):
-		argf = argv
+		argf = str(argv)
 		dev = 0
 		index = 0
 		for char in [*argf]:
 			index = index + 1
 			dev = int(f"{dev}{ord(char) - 48}") * 65536
 		table = None
```

