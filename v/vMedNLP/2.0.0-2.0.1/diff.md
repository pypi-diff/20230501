# Comparing `tmp/vMedNLP-2.0.0-py310-none-any.whl.zip` & `tmp/vMedNLP-2.0.1-py310-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11146 bytes, number of entries: 6
--rw-------  2.0 unx      141 b- defN 23-Apr-28 12:18 vMedNLP/__init__.pyc
--rw-------  2.0 unx    18880 b- defN 23-Apr-28 12:18 vMedNLP/medToolkit.pyc
--rw-------  2.0 unx     8756 b- defN 23-Apr-28 12:18 vMedNLP-2.0.0.dist-info/METADATA
--rw-------  2.0 unx       83 b- defN 23-Apr-28 12:18 vMedNLP-2.0.0.dist-info/WHEEL
--rw-------  2.0 unx        8 b- defN 23-Apr-28 12:18 vMedNLP-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      453 b- defN 23-Apr-28 12:18 vMedNLP-2.0.0.dist-info/RECORD
-6 files, 28321 bytes uncompressed, 10328 bytes compressed:  63.5%
+Zip file size: 11137 bytes, number of entries: 6
+-rw-------  2.0 unx      141 b- defN 23-May-01 10:24 vMedNLP/__init__.pyc
+-rw-------  2.0 unx    18869 b- defN 23-May-01 10:24 vMedNLP/medToolkit.pyc
+-rw-------  2.0 unx     8756 b- defN 23-May-01 10:24 vMedNLP-2.0.1.dist-info/METADATA
+-rw-------  2.0 unx       83 b- defN 23-May-01 10:24 vMedNLP-2.0.1.dist-info/WHEEL
+-rw-------  2.0 unx        8 b- defN 23-May-01 10:24 vMedNLP-2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      453 b- defN 23-May-01 10:24 vMedNLP-2.0.1.dist-info/RECORD
+6 files, 28310 bytes uncompressed, 10319 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vMedNLP/__init__.pyc
 Comment: 
 
 Filename: vMedNLP/medToolkit.pyc
 Comment: 
 
-Filename: vMedNLP-2.0.0.dist-info/METADATA
+Filename: vMedNLP-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: vMedNLP-2.0.0.dist-info/WHEEL
+Filename: vMedNLP-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: vMedNLP-2.0.0.dist-info/top_level.txt
+Filename: vMedNLP-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vMedNLP-2.0.0.dist-info/RECORD
+Filename: vMedNLP-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vMedNLP/medToolkit.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 28 12:17:40 2023 UTC, .py size: 26720 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64b9 4b64 6068 0000  o.......d.Kd`h..
+00000000: 6f0d 0d0a 0000 0000 7d92 4f64 6168 0000  o.......}.Odah..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3802 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c00 6d04 5a04 6d01 5a01  ..d.d.l.m.Z.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 5a06 6400  m.Z...d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6400 6403 6c08 5a08 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6402 6c00 6d04 5a04 6d01 5a01 6d05 5a05  d.l.m.Z.m.Z.m.Z.
@@ -15,32 +15,32 @@
 000000e0: a013 6516 6408 a102 5a17 6508 6a12 a013  ..e.d...Z.e.j...
 000000f0: 6516 6409 a102 5a18 6508 6a12 a013 6516  e.d...Z.e.j...e.
 00000100: 640a a102 5a19 6508 6a12 a013 6516 640b  d...Z.e.j...e.d.
 00000110: a102 5a1a 6508 6a12 a013 6516 640c a102  ..Z.e.j...e.d...
 00000120: 5a1b 6508 6a12 a013 6516 640d a102 5a1c  Z.e.j...e.d...Z.
 00000130: 6508 6a12 a013 6516 640e a102 5a1d 6508  e.j...e.d...Z.e.
 00000140: 6a12 a013 6516 640f a102 5a1e 6508 6a12  j...e.d...Z.e.j.
-00000150: a013 6516 6410 a102 5a1f 6509 a020 6521  ..e.d...Z.e.. e!
-00000160: a101 5a22 6522 a023 6411 a101 0100 6522  ..Z"e".#d.....e"
-00000170: 6a23 6412 6413 6414 6415 9c02 6416 8d02  j#d.d.d.d...d...
-00000180: 0100 6400 6403 6c24 5a24 6400 6403 6c08  ..d.d.l$Z$d.d.l.
-00000190: 5a08 6400 6403 6c25 5a25 6400 6403 6c25  Z.d.d.l%Z%d.d.l%
-000001a0: 5a26 6400 6417 6c27 6d28 5a28 0100 6400  Z&d.d.l'm(Z(..d.
-000001b0: 6403 6c29 5a29 6400 6403 6c09 5a09 6400  d.l)Z)d.d.l.Z.d.
-000001c0: 6418 6c2a 6d2b 5a2b 0100 6400 6419 6c2c  d.l*m+Z+..d.d.l,
-000001d0: 6d2d 5a2d 0100 6400 641a 6c00 6d01 5a01  m-Z-..d.d.l.m.Z.
+00000150: a013 6516 6410 a102 5a1f 6509 a020 6517  ..e.d...Z.e.. e.
+00000160: a101 5a21 6521 a022 6411 a101 0100 6521  ..Z!e!."d.....e!
+00000170: 6a22 6412 6413 6414 6415 9c02 6416 8d02  j"d.d.d.d...d...
+00000180: 0100 6400 6403 6c23 5a23 6400 6403 6c08  ..d.d.l#Z#d.d.l.
+00000190: 5a08 6400 6403 6c24 5a24 6400 6403 6c24  Z.d.d.l$Z$d.d.l$
+000001a0: 5a25 6400 6417 6c26 6d27 5a27 0100 6400  Z%d.d.l&m'Z'..d.
+000001b0: 6403 6c28 5a28 6400 6403 6c09 5a09 6400  d.l(Z(d.d.l.Z.d.
+000001c0: 6418 6c29 6d2a 5a2a 0100 6400 6419 6c2b  d.l)m*Z*..d.d.l+
+000001d0: 6d2c 5a2c 0100 6400 641a 6c00 6d01 5a01  m,Z,..d.d.l.m.Z.
 000001e0: 6d05 5a05 0100 6400 641b 6c00 6d04 5a04  m.Z...d.d.l.m.Z.
-000001f0: 0100 4700 641c 641d 8400 641d 8302 5a2e  ..G.d.d...d...Z.
-00000200: 4700 641e 641f 8400 641f 8302 5a2f 4700  G.d.d...d...Z/G.
-00000210: 6420 6421 8400 6421 8302 5a30 4700 6422  d d!..d!..Z0G.d"
-00000220: 6423 8400 6423 8302 5a31 4700 6424 6425  d#..d#..Z1G.d$d%
-00000230: 8400 6425 8302 5a32 4700 6426 6427 8400  ..d%..Z2G.d&d'..
-00000240: 6427 8302 5a33 4700 6428 6429 8400 6429  d'..Z3G.d(d)..d)
-00000250: 8302 5a34 4700 642a 642b 8400 642b 8302  ..Z4G.d*d+..d+..
-00000260: 5a35 6403 5300 292c e900 0000 0029 03da  Z5d.S.),.....)..
+000001f0: 0100 4700 641c 641d 8400 641d 8302 5a2d  ..G.d.d...d...Z-
+00000200: 4700 641e 641f 8400 641f 8302 5a2e 4700  G.d.d...d...Z.G.
+00000210: 6420 6421 8400 6421 8302 5a2f 4700 6422  d d!..d!..Z/G.d"
+00000220: 6423 8400 6423 8302 5a30 4700 6424 6425  d#..d#..Z0G.d$d%
+00000230: 8400 6425 8302 5a31 4700 6426 6427 8400  ..d%..Z1G.d&d'..
+00000240: 6427 8302 5a32 4700 6428 6429 8400 6429  d'..Z2G.d(d)..d)
+00000250: 8302 5a33 4700 642a 642b 8400 642b 8302  ..Z3G.d*d+..d+..
+00000260: 5a34 6403 5300 292c e900 0000 0029 03da  Z4d.S.),.....)..
 00000270: 0d41 7574 6f54 6f6b 656e 697a 6572 da22  .AutoTokenizer."
 00000280: 4175 746f 4d6f 6465 6c46 6f72 5365 7175  AutoModelForSequ
 00000290: 656e 6365 436c 6173 7369 6669 6361 7469  enceClassificati
 000002a0: 6f6e da1a 5465 7874 436c 6173 7369 6669  on..TextClassifi
 000002b0: 6361 7469 6f6e 5069 7065 6c69 6e65 2903  cationPipeline).
 000002c0: da08 7069 7065 6c69 6e65 7202 0000 00da  ..pipeliner.....
 000002d0: 1f41 7574 6f4d 6f64 656c 466f 7254 6f6b  .AutoModelForTok
@@ -1140,41 +1140,41 @@
 00004730: 696f 6e2e 6465 6964 656e 7469 6679 5f64  ion.deidentify_d
 00004740: 6963 6f6d 4e29 0a72 4a00 0000 724b 0000  icomN).rJ...rK..
 00004750: 0072 4c00 0000 7290 0000 0072 8300 0000  .rL...r....r....
 00004760: 7299 0000 0072 1a00 0000 7247 0000 0072  r....r....rG...r
 00004770: 9a00 0000 729b 0000 0072 1800 0000 7218  ....r....r....r.
 00004780: 0000 0072 1800 0000 7219 0000 0072 8c00  ...r....r....r..
 00004790: 0000 4402 0000 730e 0000 0008 0008 020e  ..D...s.........
-000047a0: 0a08 1408 0908 070c 1572 8c00 0000 2936  .........r....)6
+000047a0: 0a08 1408 0908 070c 1572 8c00 0000 2935  .........r....)5
 000047b0: da0c 7472 616e 7366 6f72 6d65 7273 7202  ..transformersr.
 000047c0: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
 000047d0: 0000 7206 0000 0072 7000 0000 7259 0000  ..r....rp...rY..
 000047e0: 00da 026f 7372 6c00 0000 5a06 7061 6e64  ...osrl...Z.pand
 000047f0: 6173 da02 7064 7207 0000 00da 0873 6369  as..pdr......sci
 00004800: 7370 6163 795a 1573 6369 7370 6163 792e  spacyZ.scispacy.
 00004810: 6162 6272 6576 6961 7469 6f6e 7208 0000  abbreviationr...
 00004820: 005a 1073 6369 7370 6163 792e 6c69 6e6b  .Z.scispacy.link
 00004830: 696e 6772 0900 0000 7239 0000 00da 046a  ingr....r9.....j
 00004840: 6f69 6eda 0764 6972 6e61 6d65 da08 5f5f  oin..dirname..__
 00004850: 6669 6c65 5f5f 5a08 4461 7461 5f64 6972  file__Z.Data_dir
 00004860: 5a0a 7370 6163 7931 5f64 6972 726e 0000  Z.spacy1_dirrn..
 00004870: 0072 2d00 0000 722e 0000 0072 3500 0000  .r-...r....r5...
 00004880: 7276 0000 0072 5b00 0000 728d 0000 0072  rv...r[...r....r
-00004890: 8e00 0000 726d 0000 005a 0973 7061 6379  ....rm...Z.spacy
-000048a0: 5f64 6972 725d 0000 005a 0861 6464 5f70  _dirr]...Z.add_p
-000048b0: 6970 65da 0562 6f74 6f33 da07 7079 6469  ipe..boto3..pydi
-000048c0: 636f 6d5a 0564 6963 6f6d 5a0c 7079 6469  comZ.dicomZ.pydi
-000048d0: 636f 6d2e 6461 7461 720e 0000 005a 0466  com.datar....Z.f
-000048e0: 6974 7ada 1770 7265 7369 6469 6f5f 696d  itz..presidio_im
-000048f0: 6167 655f 7265 6461 6374 6f72 720f 0000  age_redactorr...
-00004900: 00da 1170 7265 7369 6469 6f5f 616e 616c  ...presidio_anal
-00004910: 797a 6572 7210 0000 0072 1200 0000 724d  yzerr....r....rM
-00004920: 0000 0072 6100 0000 7274 0000 0072 7900  ...ra...rt...ry.
-00004930: 0000 727f 0000 0072 8500 0000 728c 0000  ..r....r....r...
-00004940: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00004950: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00004960: 0000 0073 5800 0000 1400 1401 0801 0801  ...sX...........
-00004970: 0801 1402 0801 0801 1402 0803 0c02 0c02  ................
-00004980: 1603 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
-00004990: 0e01 0e01 0a03 0a03 1402 0802 0801 0801  ................
-000049a0: 0803 0c01 0801 0801 0c01 0c01 1001 0c01  ................
-000049b0: 0e04 0e66 0e3c 0e5b 0e4f 0e60 0e2f 1231  ...f.<.[.O.`./.1
+00004890: 8e00 0000 726d 0000 0072 5d00 0000 5a08  ....rm...r]...Z.
+000048a0: 6164 645f 7069 7065 da05 626f 746f 33da  add_pipe..boto3.
+000048b0: 0770 7964 6963 6f6d 5a05 6469 636f 6d5a  .pydicomZ.dicomZ
+000048c0: 0c70 7964 6963 6f6d 2e64 6174 6172 0e00  .pydicom.datar..
+000048d0: 0000 5a04 6669 747a da17 7072 6573 6964  ..Z.fitz..presid
+000048e0: 696f 5f69 6d61 6765 5f72 6564 6163 746f  io_image_redacto
+000048f0: 7272 0f00 0000 da11 7072 6573 6964 696f  rr......presidio
+00004900: 5f61 6e61 6c79 7a65 7272 1000 0000 7212  _analyzerr....r.
+00004910: 0000 0072 4d00 0000 7261 0000 0072 7400  ...rM...ra...rt.
+00004920: 0000 7279 0000 0072 7f00 0000 7285 0000  ..ry...r....r...
+00004930: 0072 8c00 0000 7218 0000 0072 1800 0000  .r....r....r....
+00004940: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
+00004950: 756c 653e 0100 0000 7358 0000 0014 0014  ule>....sX......
+00004960: 0108 0108 0108 0114 0208 0108 0114 0208  ................
+00004970: 030c 020c 0216 030e 010e 010e 010e 010e  ................
+00004980: 010e 010e 010e 010e 010a 030a 0314 0208  ................
+00004990: 0208 0108 0108 030c 0108 0108 010c 010c  ................
+000049a0: 0110 010c 010e 040e 660e 3c0e 5b0e 4f0e  ........f.<.[.O.
+000049b0: 600e 2f12 31                             `./.1
```

## Comparing `vMedNLP-2.0.0.dist-info/METADATA` & `vMedNLP-2.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vMedNLP
-Version: 2.0.0
+Version: 2.0.1
 Summary: Medical NLP Toolkit
 Author: vLife|Virtusa
 Author-email: vlife@virtusa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

