# Comparing `tmp/se_lib-0.25.tar.gz` & `tmp/se_lib-0.26.tar.gz`

## Comparing `se_lib-0.25.tar` & `se_lib-0.26.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.25/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.25/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.25/selib/.DS_Store
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 se_lib-0.25/selib/__init__.py
--rw-r--r--   0        0        0    62384 2020-02-02 00:00:00.000000 se_lib-0.25/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.25/LICENSE
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 se_lib-0.25/README.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 se_lib-0.25/pyproject.toml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 se_lib-0.25/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26/selib/.DS_Store
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 se_lib-0.26/selib/__init__.py
+-rw-r--r--   0        0        0    66120 2020-02-02 00:00:00.000000 se_lib-0.26/selib/selib.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26/LICENSE
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 se_lib-0.26/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 se_lib-0.26/pyproject.toml
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 se_lib-0.26/PKG-INFO
```

### Comparing `se_lib-0.25/.DS_Store` & `se_lib-0.26/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -262,85 +262,85 @@
 00001050: 0069 0074 6d6f 6444 626c 6f62 0000 0008  .i.tmodDblob....
 00001060: 4aeb 5880 64f0 c441 0000 0004 002e 0067  J.X.d..A.......g
 00001070: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
 00001080: 0004 e000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
 00001090: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
 000010a0: 0000 002e ffff ffff ffff 0000 0000 0004  ................
 000010b0: 0064 0069 0073 0074 6277 7370 626c 6f62  .d.i.s.tbwspblob
-000010c0: 0000 00bd 6270 6c69 7374 3030 d601 0203  ....bplist00....
+000010c0: 0000 00be 6270 6c69 7374 3030 d601 0203  ....bplist00....
 000010d0: 0405 0607 0707 070b 075d 5368 6f77 5374  .........]ShowSt
 000010e0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 000010f0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00001100: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00001110: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00001120: 6e64 735b 5368 6f77 5369 6465 6261 7209  nds[ShowSidebar.
-00001130: 0909 095f 101d 7b7b 2d31 3434 302c 202d  ..._..{{-1440, -
-00001140: 3833 377d 2c20 7b31 3338 312c 2032 3138  837}, {1381, 218
-00001150: 327d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  2}}...#/;R_klmno
-00001160: 8f00 0000 0000 0001 0100 0000 0000 0000  ................
-00001170: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-00001180: 9000 0000 0400 6400 6900 7300 7464 7363  ......d.i.s.tdsc
-00001190: 6c62 6f6f 6c01 0000 0004 0064 0069 0073  lbool......d.i.s
-000011a0: 0074 6c67 3153 636f 6d70 0000 0000 0000  .tlg1Scomp......
-000011b0: a5e7 0000 0004 0064 0069 0073 0074 6d6f  .......d.i.s.tmo
-000011c0: 4444 626c 6f62 0000 0008 213b e5ed 61f2  DDblob....!;..a.
-000011d0: c441 0000 0004 0064 0069 0073 0074 6d6f  .A.....d.i.s.tmo
-000011e0: 6444 626c 6f62 0000 0008 213b e5ed 61f2  dDblob....!;..a.
-000011f0: c441 0000 0004 0064 0069 0073 0074 7068  .A.....d.i.s.tph
-00001200: 3153 636f 6d70 0000 0000 0000 c000 0000  1Scomp..........
-00001210: 0004 0064 0069 0073 0074 7653 726e 6c6f  ...d.i.s.tvSrnlo
-00001220: 6e67 0000 0001 0000 0007 004c 0049 0043  ng.........L.I.C
-00001230: 0045 004e 0053 0045 496c 6f63 626c 6f62  .E.N.S.EIlocblob
-00001240: 0000 0010 0000 00af 0000 002e ffff ffff  ................
-00001250: ffff 0000 0000 000e 0070 0079 0070 0072  .........p.y.p.r
-00001260: 006f 006a 0065 0063 0074 002e 0074 006f  .o.j.e.c.t...t.o
-00001270: 006d 006c 496c 6f63 626c 6f62 0000 0010  .m.lIlocblob....
-00001280: 0000 011d 0000 002e ffff ffff ffff 0000  ................
-00001290: 0000 0009 0052 0045 0041 0044 004d 0045  .....R.E.A.D.M.E
-000012a0: 002e 006d 0064 496c 6f63 626c 6f62 0000  ...m.dIlocblob..
-000012b0: 0010 0000 01f9 0000 002e ffff ffff ffff  ................
-000012c0: 0000 0000 0005 0073 0065 006c 0069 0062  .......s.e.l.i.b
-000012d0: 496c 6f63 626c 6f62 0000 0010 0000 0267  Ilocblob.......g
-000012e0: 0000 002e ffff ffff ffff 0000 0000 0005  ................
-000012f0: 0073 0065 006c 0069 0062 6277 7370 626c  .s.e.l.i.bbwspbl
-00001300: 6f62 0000 00bd 6270 6c69 7374 3030 d601  ob....bplist00..
-00001310: 0203 0405 0607 0709 070b 075d 5368 6f77  ...........]Show
-00001320: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-00001330: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00001340: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00001350: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00001360: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001370: 7209 0908 095f 101d 7b7b 2d31 3431 372c  r...._..{{-1417,
-00001380: 202d 3133 387d 2c20 7b31 3430 342c 2031   -138}, {1404, 1
-00001390: 3931 367d 7d09 0815 232f 3b52 5f6b 6c6d  916}}...#/;R_klm
-000013a0: 6e6f 8f00 0000 0000 0001 0100 0000 0000  no..............
-000013b0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
-000013c0: 0000 9000 0000 0500 7300 6500 6c00 6900  ........s.e.l.i.
-000013d0: 6264 7363 6c62 6f6f 6c01 0000 0005 0073  bdsclbool......s
-000013e0: 0065 006c 0069 0062 6c67 3153 636f 6d70  .e.l.i.blg1Scomp
-000013f0: 0000 0000 0000 f955 0000 0005 0073 0065  .......U.....s.e
-00001400: 006c 0069 0062 6d6f 4444 626c 6f62 0000  .l.i.bmoDDblob..
-00001410: 0008 e7af bd52 62f0 c441 0000 0005 0073  .....Rb..A.....s
-00001420: 0065 006c 0069 0062 6d6f 6444 626c 6f62  .e.l.i.bmodDblob
-00001430: 0000 0008 e7af bd52 62f0 c441 0000 0005  .......Rb..A....
-00001440: 0073 0065 006c 0069 0062 7068 3153 636f  .s.e.l.i.bph1Sco
-00001450: 6d70 0000 0000 0001 2000 0000 0005 0073  mp...... ......s
-00001460: 0065 006c 0069 0062 7653 726e 6c6f 6e67  .e.l.i.bvSrnlong
-00001470: 0000 0001 0000 0005 0074 0065 0073 0074  .........t.e.s.t
-00001480: 0073 496c 6f63 626c 6f62 0000 0010 0000  .sIlocblob......
-00001490: 02d5 0000 002e ffff ffff ffff 0000 0000  ................
-000014a0: 0005 0074 0065 0073 0074 0073 6473 636c  ...t.e.s.t.sdscl
-000014b0: 626f 6f6c 0100 0000 0500 7400 6500 7300  bool......t.e.s.
-000014c0: 7400 736c 6731 5363 6f6d 7000 0000 0000  t.slg1Scomp.....
-000014d0: 0000 0000 0000 0500 7400 6500 7300 7400  ........t.e.s.t.
-000014e0: 736d 6f44 4462 6c6f 6200 0000 08ef 3e9a  smoDDblob.....>.
-000014f0: 4d87 e2c4 4100 0000 0500 7400 6500 7300  M...A.....t.e.s.
-00001500: 7400 736d 6f64 4462 6c6f 6200 0000 08ef  t.smodDblob.....
-00001510: 3e9a 4d87 e2c4 4100 0000 0500 7400 6500  >.M...A.....t.e.
-00001520: 7300 7400 7370 6831 5363 6f6d 7000 0000  s.t.sph1Scomp...
+00001130: 0909 095f 101e 7b7b 2d31 3434 302c 202d  ..._..{{-1440, -
+00001140: 3132 3136 7d2c 207b 3133 3831 2c20 3231  1216}, {1381, 21
+00001150: 3832 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  82}}...#/;R_klmn
+00001160: 6f90 0000 0000 0000 0101 0000 0000 0000  o...............
+00001170: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00001180: 0091 0000 0004 0064 0069 0073 0074 6473  .......d.i.s.tds
+00001190: 636c 626f 6f6c 0100 0000 0400 6400 6900  clbool......d.i.
+000011a0: 7300 746c 6731 5363 6f6d 7000 0000 0000  s.tlg1Scomp.....
+000011b0: 00a5 e700 0000 0400 6400 6900 7300 746d  ........d.i.s.tm
+000011c0: 6f44 4462 6c6f 6200 0000 0821 3be5 ed61  oDDblob....!;..a
+000011d0: f2c4 4100 0000 0400 6400 6900 7300 746d  ..A.....d.i.s.tm
+000011e0: 6f64 4462 6c6f 6200 0000 0821 3be5 ed61  odDblob....!;..a
+000011f0: f2c4 4100 0000 0400 6400 6900 7300 7470  ..A.....d.i.s.tp
+00001200: 6831 5363 6f6d 7000 0000 0000 00c0 0000  h1Scomp.........
+00001210: 0000 0400 6400 6900 7300 7476 5372 6e6c  ....d.i.s.tvSrnl
+00001220: 6f6e 6700 0000 0100 0000 0700 4c00 4900  ong.........L.I.
+00001230: 4300 4500 4e00 5300 4549 6c6f 6362 6c6f  C.E.N.S.EIlocblo
+00001240: 6200 0000 1000 0000 af00 0000 2eff ffff  b...............
+00001250: ffff ff00 0000 0000 0e00 7000 7900 7000  ..........p.y.p.
+00001260: 7200 6f00 6a00 6500 6300 7400 2e00 7400  r.o.j.e.c.t...t.
+00001270: 6f00 6d00 6c49 6c6f 6362 6c6f 6200 0000  o.m.lIlocblob...
+00001280: 1000 0001 1d00 0000 2eff ffff ffff ff00  ................
+00001290: 0000 0000 0900 5200 4500 4100 4400 4d00  ......R.E.A.D.M.
+000012a0: 4500 2e00 6d00 6449 6c6f 6362 6c6f 6200  E...m.dIlocblob.
+000012b0: 0000 1000 0001 f900 0000 2eff ffff ffff  ................
+000012c0: ff00 0000 0000 0500 7300 6500 6c00 6900  ........s.e.l.i.
+000012d0: 6249 6c6f 6362 6c6f 6200 0000 1000 0002  bIlocblob.......
+000012e0: 6700 0000 2eff ffff ffff ff00 0000 0000  g...............
+000012f0: 0500 7300 6500 6c00 6900 6262 7773 7062  ..s.e.l.i.bbwspb
+00001300: 6c6f 6200 0000 bd62 706c 6973 7430 30d6  lob....bplist00.
+00001310: 0102 0304 0506 0707 0907 0b07 5d53 686f  ............]Sho
+00001320: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
+00001330: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
+00001340: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
+00001350: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
+00001360: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
+00001370: 6172 0909 0809 5f10 1d7b 7b2d 3134 3137  ar...._..{{-1417
+00001380: 2c20 2d31 3338 7d2c 207b 3134 3034 2c20  , -138}, {1404, 
+00001390: 3139 3136 7d7d 0908 1523 2f3b 525f 6b6c  1916}}...#/;R_kl
+000013a0: 6d6e 6f8f 0000 0000 0000 0101 0000 0000  mno.............
+000013b0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+000013c0: 0000 0090 0000 0005 0073 0065 006c 0069  .........s.e.l.i
+000013d0: 0062 6473 636c 626f 6f6c 0100 0000 0500  .bdsclbool......
+000013e0: 7300 6500 6c00 6900 626c 6731 5363 6f6d  s.e.l.i.blg1Scom
+000013f0: 7000 0000 0000 00f9 5500 0000 0500 7300  p.......U.....s.
+00001400: 6500 6c00 6900 626d 6f44 4462 6c6f 6200  e.l.i.bmoDDblob.
+00001410: 0000 08e7 afbd 5262 f0c4 4100 0000 0500  ......Rb..A.....
+00001420: 7300 6500 6c00 6900 626d 6f64 4462 6c6f  s.e.l.i.bmodDblo
+00001430: 6200 0000 08e7 afbd 5262 f0c4 4100 0000  b.......Rb..A...
+00001440: 0500 7300 6500 6c00 6900 6270 6831 5363  ..s.e.l.i.bph1Sc
+00001450: 6f6d 7000 0000 0000 0120 0000 0000 0500  omp...... ......
+00001460: 7300 6500 6c00 6900 6276 5372 6e6c 6f6e  s.e.l.i.bvSrnlon
+00001470: 6700 0000 0100 0000 0500 7400 6500 7300  g.........t.e.s.
+00001480: 7400 7349 6c6f 6362 6c6f 6200 0000 1000  t.sIlocblob.....
+00001490: 0002 d500 0000 2eff ffff ffff ff00 0000  ................
+000014a0: 0000 0500 7400 6500 7300 7400 7364 7363  ....t.e.s.t.sdsc
+000014b0: 6c62 6f6f 6c01 0000 0005 0074 0065 0073  lbool......t.e.s
+000014c0: 0074 0073 6c67 3153 636f 6d70 0000 0000  .t.slg1Scomp....
+000014d0: 0000 0000 0000 0005 0074 0065 0073 0074  .........t.e.s.t
+000014e0: 0073 6d6f 4444 626c 6f62 0000 0008 ef3e  .smoDDblob.....>
+000014f0: 9a4d 87e2 c441 0000 0005 0074 0065 0073  .M...A.....t.e.s
+00001500: 0074 0073 6d6f 6444 626c 6f62 0000 0008  .t.smodDblob....
+00001510: ef3e 9a4d 87e2 c441 0000 0005 0074 0065  .>.M...A.....t.e
+00001520: 0073 0074 0073 7068 3153 636f 6d70 0000  .s.t.sph1Scomp..
 00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,18 +457,18 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0000 7300  .....@........s.
-00001d00: 7400 736d 6f64 4462 6c6f 6200 0000 08ef  t.smodDblob.....
-00001d10: 3e9a 4d87 e2c4 4100 0000 0500 7400 6500  >.M...A.....t.e.
-00001d20: 7300 7400 7370 6831 5363 6f6d 7000 0000  s.t.sph1Scomp...
+00001cf0: 0000 0000 0140 0000 0000 0000 0065 0073  .....@.......e.s
+00001d00: 0074 0073 6d6f 6444 626c 6f62 0000 0008  .t.smodDblob....
+00001d10: ef3e 9a4d 87e2 c441 0000 0005 0074 0065  .>.M...A.....t.e
+00001d20: 0073 0074 0073 7068 3153 636f 6d70 0000  .s.t.sph1Scomp..
 00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `se_lib-0.25/selib/.DS_Store` & `se_lib-0.26/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.25/selib/selib.py` & `se_lib-0.26/selib/selib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-se-lib Version .24
+se-lib Version .26
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
@@ -1368,19 +1368,20 @@
                 continue
     if verbose: print(f'***{css=}') # rm
     ft = copy
     return(css)
 
 # system dynamics simulation functions
 
-def init_model(start, stop, dt):
+def init_sd_model(start, stop, dt):
   """
   Instantiates a system dynamics model for simulation
   """
-  global xmile_header, model, model_specs
+  global xmile_header, model, model_specs, model_dict, model_type
+  model_type = "continuous"
   xmile_header = f"""<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
     <xmile version="1.0" xmlns="http://docs.oasis-open.org/xmile/ns/XMILE/v1.0">
         <header>
             <vendor>Ray Madachy</vendor>
             <name>Battle Simulator</name>
             <options>
                 <uses_outputs/>
@@ -1392,14 +1393,15 @@
         <sim_specs>
                 <stop>{stop}</stop>
                 <start>{start}</start>
                 <dt>{dt}</dt>
         </sim_specs>"""
   model = ""
   build_model()
+  model_dict={'stocks': {}, 'flows': {}, 'auxiliaries': {}}
 
 def build_model():
   global xmile_string
   xmile_closing = """
     </xmile>
     """
   model_string = """
@@ -1436,58 +1438,66 @@
                 <stock name="{name}">
                     <doc>{name}</doc>
                     {inflow_string}
                     {outflow_string}
                     <eqn>{initial}</eqn>
                 </stock>"""
   build_model()
+  model_dict['stocks'][name]={'inflows': inflows, 'outflows': outflows}
   
-def add_auxiliary(name, equation):
+def add_auxiliary(name, equation, inputs=[]):
   """
   Adds auxiliary equation or constant to the model
 
   Parameters
   ----------
   name: str
     The name of the auxiliary 
   equation: str
     Equation for the auxiliary using other named model variables
+  inputs: list
+    Optional list of variable input names used to draw model diagram 
   """
   if "random()" in str(equation): equation = convert_random_to_xmile(equation) 
   if "random.uniform(" in str(equation): equation = convert_random_to_xmile(equation)
   if "RANDOM" in str(equation): equation = equation.replace("RANDOM", '(GET_TIME_VALUE(0,0,0) + .00001) / (GET_TIME_VALUE(0,0,0) + .00001) * RANDOM')
   global model
   model += f"""
                 <aux name="{name}">
                     <doc>{name}</doc>
                     <eqn>{equation}</eqn>
                 </aux>"""
   build_model()
+  model_dict['auxiliaries'][name]={'equation': equation, 'inputs': inputs}
     
-def add_flow(name, equation):
-    """
-    Adds a flow to the model
-
-    Parameters
-    ----------
-    name: str
-      The name of the flow 
-    equation: str
-      Equation for the flow using other named model variables
-    """
-    if "random()" in str(equation): equation = convert_random_to_xmile(equation) 
-    if "random.uniform(" in str(equation): equation = convert_random_to_xmile(equation)
-    if "RANDOM" in str(equation): equation = equation.replace("RANDOM", '(GET_TIME_VALUE(0,0,0) + .00001) / (GET_TIME_VALUE(0,0,0) + .00001) * RANDOM')
-    global model
-    model += f"""
-                <flow name="{name}">
-                    <doc>{name}</doc>
-                    <eqn>{equation}</eqn>
-                </flow>"""
-    build_model()
+def add_flow(name, equation, inputs=[]):
+	"""
+	Adds a flow to the model
+
+	Parameters
+	----------
+	name: str
+	  The name of the flow 
+	equation: str
+	  Equation for the flow using other named model variables
+	inputs: list
+	  Optional list of variable input names used to draw model diagram 
+	"""
+	if "random()" in str(equation): equation = convert_random_to_xmile(equation) 
+	if "random.uniform(" in str(equation): equation = convert_random_to_xmile(equation)
+	if "RANDOM" in str(equation): equation = equation.replace("RANDOM", '(GET_TIME_VALUE(0,0,0) + .00001) / (GET_TIME_VALUE(0,0,0) + .00001) * RANDOM')
+	global model
+	model += f"""
+				<flow name="{name}">
+					<doc>{name}</doc>
+					<eqn>{equation}</eqn>
+				</flow>"""
+	build_model()
+	model_dict['flows'][name]={'equation': equation, 'inputs': inputs}
+	
 
 def convert_random_to_xmile(equation):
   equation = equation.replace("random(", "RANDOM_0_1(")
   equation = equation.replace("random.uniform(", "RANDOM_UNIFORM(")
   return(equation)
 
 
@@ -1539,15 +1549,15 @@
     Pandas dataframe containing run outputs for each variable each timestep
     """
     import pysd
     global output
     global model
     model = pysd.read_xmile('./test.xmile')
     output = model.run(progress=False)
-    return (output)
+    return (output, model_dict)
     
 def set_logical_run_time(condition):
     """
     Enables a run time to be measured based on a logical condition for when the simulation should be run (like a while statement).  The logical end time will be available from the 'get_logical_end_time()' function in lieu of the fixed end time for a simulation. 
     """
     add_flow("time_flow", 'if_then_else('+str(condition)+', 1, 0)')
     #add_flow("time_flow", 'if_then_else(not '+str(condition)+', 1, 0)')
@@ -1562,8 +1572,76 @@
     ----------
     logical_end_time: float
         end time when the 'set_logical_run_time()'' condition expires
     """
     return (get_final_value("logical_end_time"))  
     
 def get_final_value(variable):
-    return (output[variable][model['FINAL TIME']]) 
+    return (output[variable][model['FINAL TIME']]) 
+	
+	
+	
+def draw_sd_model(filename=None, format='svg'):
+    system_dynamics_dict = model_dict
+    graph = graphviz.Digraph(engine='dot', filename=filename, format=format)
+    graph.attr(rankdir='LR', size='10,8', splines='spline',)
+    graph.attr('node', fontname="arial", fontcolor='blue', color='invis', fontsize='10')
+    #graph.attr('edge',  minlen='1')
+    
+    
+    with graph.subgraph(name='cluster_flowchain') as c:
+        # Add stocks as boxes
+        for stock_name in system_dynamics_dict['stocks']:
+            graph.node(stock_name, shape='box', color='blue', )
+        
+        # Add flows as circles
+        for flow_name in system_dynamics_dict['flows']:
+            graph.node(flow_name, shape='circle', color='blue', width='.2', fixedsize="true" , label=f"\n\n{flow_name}")
+        
+    # Add auxiliaries as circles
+    for aux_name in system_dynamics_dict['auxiliaries']:
+        graph.node(aux_name, shape='circle', color='blue', width='.2', fixedsize="true", label=f"\n\n{aux_name}")
+    
+    # Add edges from inflows to stocks
+    for stock_name, stock_dict in system_dynamics_dict['stocks'].items():
+        for inflow_name in stock_dict['inflows']:
+            graph.edge(inflow_name, stock_name, color="blue:blue", arrowhead="onormal")
+            if inflow_name not in stock_dict['outflows']:
+                graph.node(f'{inflow_name}_source', width=".01", fontsize='14', fixedsize="true", label="✽")
+                graph.edge(f'{inflow_name}_source', inflow_name, tailclip="true", color="blue:blue", arrowhead="none")
+    
+    # Add edges from stocks to outflows
+    for stock_name, stock_dict in system_dynamics_dict['stocks'].items():
+        for outflow_name in stock_dict['outflows']:
+            graph.edge(stock_name, outflow_name, color="blue:blue", arrowhead="none")
+            if outflow_name not in stock_dict['inflows']:
+                graph.node(f'{outflow_name}_sink', width=".01", fontsize='14', fixedsize="true", label="✽")
+                graph.edge(outflow_name, f'{outflow_name}_sink', headclip="true", color="blue:blue", arrowhead="onormal")
+
+    # Add edges from variable inputs to flows
+    for flow_name, flow_dict in system_dynamics_dict['flows'].items():
+        for input_name in flow_dict['inputs']:
+            graph.edge(input_name, flow_name, color="red", arrowhead="normal", constraint='false')
+ 
+           
+    # Add edges from variable inputs to auxiliaries
+    for aux_name, aux_dict in system_dynamics_dict['auxiliaries'].items():
+        for input_name in aux_dict['inputs']:
+            graph.edge(input_name, aux_name, color="red", arrowhead="normal", constraint='false')
+    
+    if filename is not None:
+        graph.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
+    return graph
+	
+	
+def draw_model_diagram(filename=None, format="svg"):
+    """
+    Draw a model diagram. 
+    
+    Returns
+    -------
+    g : diagram object view
+        Save the diagram to a file, and open the rendered result in its default viewing application. se-lib calls the Graphviz API for this.
+    """
+    filename = filename
+    format = format
+    if model_type == "continuous": return(draw_sd_model(filename, format))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `se_lib-0.25/LICENSE` & `se_lib-0.26/LICENSE`

 * *Files identical despite different names*

