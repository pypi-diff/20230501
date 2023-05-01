# Comparing `tmp/iqmma-0.1.3.1-py3-none-any.whl.zip` & `tmp/iqmma-0.1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 29002 bytes, number of entries: 10
+Zip file size: 29007 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-26 14:17 iqmma/__init__.py
 -rw-r--r--  2.0 unx     1051 b- defN 23-Feb-26 14:17 iqmma/default.ini
--rw-r--r--  2.0 unx    38425 b- defN 23-Apr-25 12:41 iqmma/iqmma.py
+-rw-r--r--  2.0 unx    38525 b- defN 23-May-01 09:17 iqmma/iqmma.py
 -rw-r--r--  2.0 unx    42493 b- defN 23-Apr-25 13:34 iqmma/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    12164 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      771 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/RECORD
-10 files, 106401 bytes uncompressed, 27698 bytes compressed:  74.0%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12164 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      771 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/RECORD
+10 files, 106501 bytes uncompressed, 27703 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: iqmma/iqmma.py
 Comment: 
 
 Filename: iqmma/utils.py
 Comment: 
 
-Filename: iqmma-0.1.3.1.dist-info/LICENSE
+Filename: iqmma-0.1.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: iqmma-0.1.3.1.dist-info/METADATA
+Filename: iqmma-0.1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: iqmma-0.1.3.1.dist-info/WHEEL
+Filename: iqmma-0.1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: iqmma-0.1.3.1.dist-info/entry_points.txt
+Filename: iqmma-0.1.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: iqmma-0.1.3.1.dist-info/top_level.txt
+Filename: iqmma-0.1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: iqmma-0.1.3.1.dist-info/RECORD
+Filename: iqmma-0.1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iqmma/iqmma.py

```diff
@@ -281,15 +281,15 @@
         peptides_dict = {}
         peptides_suf = 'peptides.tsv'
         if args['pept_folder'] :
             if args['pept_folder'] != args['psm_folder'] :
                 if os.path.exists(os.path.normpath(args['pept_folder'])) :
                     dir_name = os.path.abspath(os.path.normpath(args['pept_folder']))
                 else :
-                    logger.critical('path to peptides files folder does not exist')
+                    logger.critical('path to peptides files folder does not exist: {}'.format(os.path.normpath(args['pept_folder'])))
                     return -1
             else :
                 logger.warning('trying to find *%s files in the same directory as PSMs', peptides_suf)
                 dir_name = os.path.dirname(PSMs_full_paths[0])
                 logger.debug(dir_name)
             for sample in samples :
                 i = 0
@@ -307,15 +307,15 @@
         proteins_dict = {}
         proteins_suf = 'proteins.tsv'
         if args['prot_folder'] :
             if args['prot_folder'] != args['psm_folder'] :
                 if os.path.exists(os.path.normpath(args['prot_folder'])) :
                     dir_name = os.path.abspath(os.path.normpath(args['prot_folder']))
                 else :
-                    logger.critical('path to proteins files folder does not exist')
+                    logger.critical('path to proteins files folder does not exist: {}'.format(os.path.normpath(args['pept_folder'])))
                     return -1
             else :
                 logger.warning('Searching *{} files in the same directory as PSMs'.format(proteins_suf))
                 dir_name = os.path.dirname(PSMs_full_paths[0])
             for sample in samples :
                 i = 0
                 for filename in os.listdir(dir_name) :
```

## Comparing `iqmma-0.1.3.1.dist-info/LICENSE` & `iqmma-0.1.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iqmma-0.1.3.1.dist-info/METADATA` & `iqmma-0.1.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqmma
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: A MS1 feature mapping for MS2 spectra identifications.
 Author: Valeriy Postoenko & Leyla Garibova
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
```

