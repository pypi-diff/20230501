# Comparing `tmp/alacorder-80.0.8.tar.gz` & `tmp/alacorder-80.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.0.8.tar", max compression
+gzip compressed data, was "alacorder-80.0.9.tar", max compression
```

## Comparing `alacorder-80.0.8.tar` & `alacorder-80.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.8/LICENSE
--rw-r--r--   0        0        0     6821 2023-04-29 16:14:55.778453 alacorder-80.0.8/README.md
--rw-r--r--   0        0        0      697 2023-04-30 22:11:45.489044 alacorder-80.0.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-30 15:52:56.348120 alacorder-80.0.8/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.8/src/alacorder/__init__.py
--rw-r--r--   0        0        0   214847 2023-04-30 22:11:19.081069 alacorder-80.0.8/src/alacorder/__main__.py
--rw-r--r--   0        0        0   214847 2023-04-30 22:10:51.515736 alacorder-80.0.8/src/alacorder/alac.py
--rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 alacorder-80.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.9/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.0.9/README.md
+-rw-r--r--   0        0        0      697 2023-04-30 22:23:05.387870 alacorder-80.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-30 22:12:00.468048 alacorder-80.0.9/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.9/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   212171 2023-04-30 22:22:57.696267 alacorder-80.0.9/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   212171 2023-04-30 22:22:52.806896 alacorder-80.0.9/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.0.9/PKG-INFO
```

### Comparing `alacorder-80.0.8/LICENSE` & `alacorder-80.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.8/README.md` & `alacorder-80.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -191,237 +191,241 @@
 00000be0: 2020 2020 2020 4372 6561 7465 2062 6c61        Create bla
 00000bf0: 6e6b 2041 4953 202f 2075 6e69 7175 6520  nk AIS / unique 
 00000c00: 7061 6972 696e 6720 7465 6d70 6c61 7465  pairing template
 00000c10: 0a20 2072 656e 616d 6520 2020 2020 2020  .  rename       
 00000c20: 2020 2020 2020 2020 5265 6e61 6d65 2063          Rename c
 00000c30: 6173 6573 2069 6e20 696e 7075 7420 6469  ases in input di
 00000c40: 7265 6374 6f72 7920 746f 2063 6173 6520  rectory to case 
-00000c50: 6e75 6d62 6572 730a 2020 7365 7474 696e  numbers.  settin
-00000c60: 6773 2020 2020 2020 2020 2020 2020 2043  gs             C
+00000c50: 6e75 6d62 6572 730a 2020 7365 6e74 656e  numbers.  senten
+00000c60: 6365 7320 2020 2020 2020 2020 2020 2043  ces            C
 00000c70: 7265 6174 6520 616e 6420 6578 706f 7274  reate and export
-00000c80: 2073 6574 7469 6e67 7320 7461 626c 650a   settings table.
-00000c90: 2020 7374 6172 7420 2020 2020 2020 2020    start         
-00000ca0: 2020 2020 2020 204c 6175 6e63 6820 6772         Launch gr
-00000cb0: 6170 6869 6361 6c20 7573 6572 2069 6e74  aphical user int
-00000cc0: 6572 6661 6365 0a20 2074 6162 6c65 2020  erface.  table  
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 4578                Ex
-00000ce0: 706f 7274 2064 6174 6120 7461 626c 6573  port data tables
-00000cf0: 2066 726f 6d20 6172 6368 6976 6520 6f72   from archive or
-00000d00: 2064 6972 6563 746f 7279 0a20 2076 7272   directory.  vrr
-00000d10: 2d70 6169 7273 2020 2020 2020 2020 2020  -pairs          
-00000d20: 2020 4372 6561 7465 2076 6f74 696e 6720    Create voting 
-00000d30: 7269 6768 7473 2073 756d 6d61 7279 2066  rights summary f
-00000d40: 726f 6d20 696e 7075 7420 6361 7365 7320  rom input cases 
-00000d50: 616e 6420 7061 6972 730a 2020 7769 746e  and pairs.  witn
-00000d60: 6573 7365 7320 2020 2020 2020 2020 2020  esses           
-00000d70: 2043 7265 6174 6520 616e 6420 6578 706f   Create and expo
-00000d80: 7274 2077 6974 6e65 7373 6573 2074 6162  rt witnesses tab
-00000d90: 6c65 0a60 6060 0a0a 2323 2046 6574 6368  le.```..## Fetch
-00000da0: 2063 6173 6573 2069 6e20 6275 6c6b 2066   cases in bulk f
-00000db0: 726f 6d20 416c 6163 6f75 7274 2e63 6f6d  rom Alacourt.com
-00000dc0: 200a 0a54 616b 6520 6120 7370 7265 6164   ..Take a spread
-00000dd0: 7368 6565 7420 6f66 206e 616d 6573 2061  sheet of names a
-00000de0: 6e64 2f6f 7220 6f74 6865 7220 7365 6172  nd/or other sear
-00000df0: 6368 2070 6172 616d 6574 6572 7320 616e  ch parameters an
-00000e00: 6420 646f 776e 6c6f 6164 2063 6173 6520  d download case 
-00000e10: 5044 4673 2066 726f 6d20 416c 6163 6f75  PDFs from Alacou
-00000e20: 7274 2069 6e20 6275 6c6b 2e20 446f 776e  rt in bulk. Down
-00000e30: 6c6f 6164 2074 686f 7573 616e 6473 206f  load thousands o
-00000e40: 6620 5044 4673 2069 6e20 6a75 7374 2068  f PDFs in just h
-00000e50: 6f75 7273 2062 7920 6c65 6176 696e 6720  ours by leaving 
-00000e60: 796f 7572 2063 6f6d 7075 7465 7220 756e  your computer un
-00000e70: 6174 7465 6e64 6564 2e20 2847 6f6f 676c  attended. (Googl
-00000e80: 6520 4368 726f 6d65 2069 7320 7265 7175  e Chrome is requ
-00000e90: 6972 6564 2074 6f20 7573 6520 7468 6520  ired to use the 
-00000ea0: 6066 6574 6368 6020 6665 6174 7572 652e  `fetch` feature.
-00000eb0: 290a 0a60 6060 0a55 7361 6765 3a20 7079  )..```.Usage: py
-00000ec0: 7468 6f6e 202d 6d20 616c 6163 6f72 6465  thon -m alacorde
-00000ed0: 7220 6665 7463 6820 5b4f 5054 494f 4e53  r fetch [OPTIONS
-00000ee0: 5d0a 0a20 2046 6574 6368 2063 6173 6573  ]..  Fetch cases
-00000ef0: 2066 726f 6d20 416c 6163 6f75 7274 2e63   from Alacourt.c
-00000f00: 6f6d 0a0a 4f70 7469 6f6e 733a 0a20 202d  om..Options:.  -
-00000f10: 696e 2c20 2d2d 696e 7075 742d 7061 7468  in, --input-path
-00000f20: 2050 4154 4820 2020 2050 6174 6820 746f   PATH    Path to
-00000f30: 2071 7565 7279 2074 6162 6c65 2f73 7072   query table/spr
-00000f40: 6561 6473 6865 6574 2028 2e78 6c73 2c20  eadsheet (.xls, 
-00000f50: 2e78 6c73 7829 0a20 2020 2020 2020 2020  .xlsx).         
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 205b 7265 7175 6972 6564 5d0a 2020     [required].  
-00000f80: 2d6f 7574 2c20 2d2d 6f75 7470 7574 2d70  -out, --output-p
-00000f90: 6174 6820 5041 5448 2020 4465 7369 7265  ath PATH  Desire
-00000fa0: 6420 5044 4620 6f75 7470 7574 2064 6972  d PDF output dir
-00000fb0: 6563 746f 7279 2020 5b72 6571 7569 7265  ectory  [require
-00000fc0: 645d 0a20 202d 632c 202d 2d63 7573 746f  d].  -c, --custo
-00000fd0: 6d65 722d 6964 2054 4558 5420 2020 2043  mer-id TEXT    C
-00000fe0: 7573 746f 6d65 7220 4944 206f 6e20 416c  ustomer ID on Al
-00000ff0: 6163 6f75 7274 2e63 6f6d 2020 5b72 6571  acourt.com  [req
-00001000: 7569 7265 645d 0a20 202d 752c 202d 2d75  uired].  -u, --u
-00001010: 7365 722d 6964 2054 4558 5420 2020 2020  ser-id TEXT     
-00001020: 2020 2055 7365 7220 4944 206f 6e20 416c     User ID on Al
-00001030: 6163 6f75 7274 2e63 6f6d 2020 5b72 6571  acourt.com  [req
-00001040: 7569 7265 645d 0a20 202d 702c 202d 2d70  uired].  -p, --p
-00001050: 6173 7377 6f72 6420 5445 5854 2020 2020  assword TEXT    
-00001060: 2020 2050 6173 7377 6f72 6420 6f6e 2041     Password on A
-00001070: 6c61 636f 7572 742e 636f 6d20 205b 7265  lacourt.com  [re
-00001080: 7175 6972 6564 5d0a 2020 2d6d 6178 2c20  quired].  -max, 
-00001090: 2d2d 6d61 7820 494e 5445 4745 5220 2020  --max INTEGER   
-000010a0: 2020 2020 4d61 7869 6d75 6d20 7175 6572      Maximum quer
-000010b0: 6965 7320 746f 2063 6f6e 6475 6374 206f  ies to conduct o
-000010c0: 6e20 416c 6163 6f75 7274 2e63 6f6d 0a20  n Alacourt.com. 
-000010d0: 202d 736b 6970 2c20 2d2d 736b 6970 2049   -skip, --skip I
-000010e0: 4e54 4547 4552 2020 2020 2053 6b69 7020  NTEGER     Skip 
-000010f0: 656e 7472 6965 7320 6174 2074 6f70 206f  entries at top o
-00001100: 6620 7175 6572 7920 6669 6c65 0a20 202d  f query file.  -
-00001110: 6e2c 202d 2d6e 6f2d 6d61 726b 2020 2020  n, --no-mark    
-00001120: 2020 2020 2020 2020 2044 6f20 6e6f 7420           Do not 
-00001130: 7570 6461 7465 2071 7565 7279 2074 656d  update query tem
-00001140: 706c 6174 6520 6166 7465 7220 636f 6d70  plate after comp
-00001150: 6c65 7469 6f6e 0a20 202d 2d64 6562 7567  letion.  --debug
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2020 2050 7269 6e74 2064 6574 6169 6c65     Print detaile
-00001180: 6420 7275 6e74 696d 6520 696e 666f 726d  d runtime inform
-00001190: 6174 696f 6e20 746f 2063 6f6e 736f 6c65  ation to console
-000011a0: 0a20 202d 682c 202d 2d68 656c 7020 2020  .  -h, --help   
-000011b0: 2020 2020 2020 2020 2020 2020 2053 686f               Sho
-000011c0: 7720 7468 6973 206d 6573 7361 6765 2061  w this message a
-000011d0: 6e64 2065 7869 742e 0a60 6060 0a0a 0a23  nd exit..```...#
-000011e0: 202a 2a57 6f72 6b69 6e67 2077 6974 6820   **Working with 
-000011f0: 6361 7365 2064 6174 6120 696e 2050 7974  case data in Pyt
-00001200: 686f 6e2a 2a0a 0a0a 2323 2320 4f75 7420  hon**...### Out 
-00001210: 6f66 2074 6865 2062 6f78 2c20 416c 6163  of the box, Alac
-00001220: 6f72 6465 7220 6578 706f 7274 7320 746f  order exports to
-00001230: 2060 2e78 6c73 7860 2c20 602e 786c 7360   `.xlsx`, `.xls`
-00001240: 2c20 602e 6373 7660 2c20 602e 6a73 6f6e  , `.csv`, `.json
-00001250: 602c 2061 6e64 2060 2e70 6172 7175 6574  `, and `.parquet
-00001260: 602e 2042 7574 2079 6f75 2063 616e 2075  `. But you can u
-00001270: 7365 2060 706f 6c61 7273 6020 616e 6420  se `polars` and 
-00001280: 6f74 6865 7220 7079 7468 6f6e 206c 6962  other python lib
-00001290: 7261 7269 6573 2074 6f20 6372 6561 7465  raries to create
-000012a0: 2079 6f75 7220 6f77 6e20 6461 7461 2063   your own data c
-000012b0: 6f6c 6c65 6374 696f 6e20 776f 726b 666c  ollection workfl
-000012c0: 6f77 7320 616e 6420 6375 7374 6f6d 697a  ows and customiz
-000012d0: 6520 416c 6163 6f72 6465 7220 6578 706f  e Alacorder expo
-000012e0: 7274 732e 200a 0a2a 2a2a 5468 6520 736e  rts. ..***The sn
-000012f0: 6970 7065 7420 6265 6c6f 7720 7072 696e  ippet below prin
-00001300: 7473 2074 6865 2066 6565 2073 6865 6574  ts the fee sheet
-00001310: 7320 6672 6f6d 2061 2064 6972 6563 746f  s from a directo
-00001320: 7279 206f 6620 6361 7365 2050 4446 7320  ry of case PDFs 
-00001330: 6173 2069 7420 7265 6164 7320 7468 656d  as it reads them
-00001340: 2e2a 2a2a 0a0a 0a60 6060 7079 7468 6f6e  .***...```python
-00001350: 0a66 726f 6d20 616c 6163 6f72 6465 7220  .from alacorder 
-00001360: 696d 706f 7274 2061 6c61 630a 696d 706f  import alac.impo
-00001370: 7274 2070 6f6c 6172 7320 6173 2070 6c0a  rt polars as pl.
-00001380: 0a71 7565 7565 203d 2061 6c61 632e 6765  .queue = alac.ge
-00001390: 745f 7061 7468 7328 222f 5573 6572 732f  t_paths("/Users/
-000013a0: 6372 696d 736f 6e2f 4465 736b 746f 702f  crimson/Desktop/
-000013b0: 5475 7477 696c 6572 2f22 2920 2320 2d3e  Tutwiler/") # ->
-000013c0: 205b 7374 725d 0a0a 726f 7773 203d 205b   [str]..rows = [
-000013d0: 5d0a 0a66 6f72 2069 2c20 7061 7468 2069  ]..for i, path i
-000013e0: 6e20 656e 756d 6572 6174 6528 7175 6575  n enumerate(queu
-000013f0: 6529 3a0a 2020 2020 7465 7874 203d 2061  e):.    text = a
-00001400: 6c61 632e 6578 7472 6163 745f 7465 7874  lac.extract_text
-00001410: 2870 6174 6829 0a20 2020 2063 6e75 6d20  (path).    cnum 
-00001420: 3d20 616c 6163 2e67 6574 4361 7365 4e75  = alac.getCaseNu
-00001430: 6d62 6572 2874 6578 7429 0a20 2020 2063  mber(text).    c
-00001440: 7479 203d 2061 6c61 632e 6765 7443 6f75  ty = alac.getCou
-00001450: 6e74 7928 7465 7874 290a 2020 2020 7462  nty(text).    tb
-00001460: 616c 203d 2061 6c61 632e 6765 7454 6f74  al = alac.getTot
-00001470: 616c 4261 6c61 6e63 6528 7465 7874 290a  alBalance(text).
-00001480: 2020 2020 7074 7220 3d20 616c 6163 2e67      ptr = alac.g
-00001490: 6574 5061 796d 656e 7454 6f52 6573 746f  etPaymentToResto
-000014a0: 7265 2874 6578 7429 2023 2069 2e65 2e20  re(text) # i.e. 
-000014b0: 766f 7469 6e67 2072 6967 6874 730a 2020  voting rights.  
-000014c0: 2020 726f 7773 202b 3d20 5b5b 636e 756d    rows += [[cnum
-000014d0: 2c20 6374 792c 2074 6261 6c2c 2070 7472  , cty, tbal, ptr
-000014e0: 5d5d 0a0a 6361 7365 7320 3d20 706c 2e44  ]]..cases = pl.D
-000014f0: 6174 6146 7261 6d65 2872 6f77 7329 0a0a  ataFrame(rows)..
-00001500: 6361 7365 732e 7772 6974 655f 6578 6365  cases.write_exce
-00001510: 6c28 222f 5573 6572 732f 6372 696d 736f  l("/Users/crimso
-00001520: 6e2f 4465 736b 746f 702f 5475 7477 696c  n/Desktop/Tutwil
-00001530: 6572 2f73 756d 6d61 7279 2e78 6c73 7822  er/summary.xlsx"
-00001540: 290a 0a60 6060 0a0a 2323 2045 7874 656e  )..```..## Exten
-00001550: 6469 6e67 2041 6c61 636f 7264 6572 2077  ding Alacorder w
-00001560: 6974 6820 6070 6f6c 6172 7360 2061 6e64  ith `polars` and
-00001570: 206f 7468 6572 2074 6f6f 6c73 0a0a 416c   other tools..Al
-00001580: 6163 6f72 6465 7220 7275 6e73 206f 6e20  acorder runs on 
-00001590: 5b60 706f 6c61 7273 605d 2868 7474 7073  [`polars`](https
-000015a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
-000015b0: 6c61 2d72 732f 706f 6c61 7273 292c 2061  la-rs/polars), a
-000015c0: 2070 7974 686f 6e20 6c69 6272 6172 7920   python library 
-000015d0: 796f 7520 6361 6e20 7573 6520 746f 2077  you can use to w
-000015e0: 6f72 6b20 7769 7468 2061 6e64 2061 6e61  ork with and ana
-000015f0: 6c79 7a65 2074 6162 756c 6172 2064 6174  lyze tabular dat
-00001600: 612e 2060 706f 6c61 7273 6020 6361 6e20  a. `polars` can 
-00001610: 7265 6164 2066 726f 6d20 616e 6420 7772  read from and wr
-00001620: 6974 6520 746f 2061 6c6c 206d 616a 6f72  ite to all major
-00001630: 2064 6174 6120 7374 6f72 6167 6520 666f   data storage fo
-00001640: 726d 6174 732e 2049 7420 6361 6e20 636f  rmats. It can co
-00001650: 6e6e 6563 7420 746f 2061 2077 6964 6520  nnect to a wide 
-00001660: 7661 7269 6574 7920 6f66 2073 6572 7669  variety of servi
-00001670: 6365 7320 746f 2070 726f 7669 6465 2066  ces to provide f
-00001680: 6f72 2065 6173 7920 696d 706f 7274 2061  or easy import a
-00001690: 6e64 2065 7870 6f72 742e 0a0a 6060 6070  nd export...```p
-000016a0: 7974 686f 6e0a 696d 706f 7274 2070 6f6c  ython.import pol
-000016b0: 6172 7320 6173 2070 6c0a 636f 6e74 656e  ars as pl.conten
-000016c0: 7473 203d 2070 6c2e 7265 6164 5f6a 736f  ts = pl.read_jso
-000016d0: 6e28 222f 7061 7468 2f74 6f2f 6172 6368  n("/path/to/arch
-000016e0: 6976 652e 6a73 6f6e 2229 0a60 6060 0a0a  ive.json").```..
-000016f0: 4966 2079 6f75 2077 6f75 6c64 206c 696b  If you would lik
-00001700: 6520 746f 2076 6973 7561 6c69 7a65 2064  e to visualize d
-00001710: 6174 6120 7769 7468 6f75 7420 6578 706f  ata without expo
-00001720: 7274 696e 6720 746f 2045 7863 656c 206f  rting to Excel o
-00001730: 7220 616e 6f74 6865 7220 666f 726d 6174  r another format
-00001740: 2c20 6372 6561 7465 2061 2060 6a75 7079  , create a `jupy
-00001750: 7465 7220 6e6f 7465 626f 6f6b 6020 616e  ter notebook` an
-00001760: 6420 696e 7374 616c 6c20 746f 6f6c 7320  d install tools 
-00001770: 6c69 6b65 2060 6d61 7470 6c6f 746c 6962  like `matplotlib
-00001780: 602c 2060 7461 6275 6c61 7465 602c 2061  `, `tabulate`, a
-00001790: 6e64 2060 6974 6162 6c65 7360 2074 6f20  nd `itables` to 
-000017a0: 6765 7420 7374 6172 7465 642e 205b 4a75  get started. [Ju
-000017b0: 7079 7465 7220 4e6f 7465 626f 6f6b 5d28  pyter Notebook](
-000017c0: 6874 7470 733a 2f2f 646f 6373 2e6a 7570  https://docs.jup
-000017d0: 7974 6572 2e6f 7267 2f65 6e2f 6c61 7465  yter.org/en/late
-000017e0: 7374 2f73 7461 7274 2f69 6e64 6578 2e68  st/start/index.h
-000017f0: 746d 6c29 2069 7320 6120 5079 7468 6f6e  tml) is a Python
-00001800: 2070 726f 6a65 6374 2079 6f75 2063 616e   project you can
-00001810: 2075 7365 2074 6f20 6372 6561 7465 2069   use to create i
-00001820: 6e74 6572 6163 7469 7665 206e 6f74 6562  nteractive noteb
-00001830: 6f6f 6b73 2066 6f72 2064 6174 6120 616e  ooks for data an
-00001840: 616c 7973 6973 2061 6e64 206f 7468 6572  alysis and other
-00001850: 2070 7572 706f 7365 732e 2049 7420 6361   purposes. It ca
-00001860: 6e20 6265 2069 6e73 7461 6c6c 6564 2075  n be installed u
-00001870: 7369 6e67 2060 7069 7020 696e 7374 616c  sing `pip instal
-00001880: 6c20 6a75 7079 7465 7260 206f 7220 6070  l jupyter` or `p
-00001890: 6970 3320 696e 7374 616c 6c20 6a75 7079  ip3 install jupy
-000018a0: 7465 7260 2061 6e64 206c 6175 6e63 6865  ter` and launche
-000018b0: 6420 7573 696e 6720 606a 7570 7974 6572  d using `jupyter
-000018c0: 206e 6f74 6562 6f6f 6b60 2e20 596f 7572   notebook`. Your
-000018d0: 2064 6576 6963 6520 6d61 7920 616c 7265   device may alre
-000018e0: 6164 7920 6265 2065 7175 6970 7065 6420  ady be equipped 
-000018f0: 746f 2076 6965 7720 602e 6970 796e 6260  to view `.ipynb`
-00001900: 206e 6f74 6562 6f6f 6b73 2e20 0a0a 2323   notebooks. ..##
-00001910: 202a 2a52 6573 6f75 7263 6573 2a2a 0a2a   **Resources**.*
-00001920: 205b 6070 6f6c 6172 7360 2075 7365 7220   [`polars` user 
-00001930: 6775 6964 655d 2868 7474 7073 3a2f 2f70  guide](https://p
-00001940: 6f6c 612d 7273 2e67 6974 6875 622e 696f  ola-rs.github.io
-00001950: 2f70 6f6c 6172 732d 626f 6f6b 2f75 7365  /polars-book/use
-00001960: 722d 6775 6964 652f 696e 6465 782e 6874  r-guide/index.ht
-00001970: 6d6c 290a 2a20 5b72 6567 6578 2063 6865  ml).* [regex che
-00001980: 6174 2073 6865 6574 5d28 6874 7470 733a  at sheet](https:
-00001990: 2f2f 7777 772e 7265 7865 6767 2e63 6f6d  //www.rexegg.com
-000019a0: 2f72 6567 6578 2d71 7569 636b 7374 6172  /regex-quickstar
-000019b0: 742e 6874 6d6c 290a 2a20 5b41 6e61 636f  t.html).* [Anaco
-000019c0: 6e64 6120 2874 7574 6f72 6961 6c73 206f  nda (tutorials o
-000019d0: 6e20 7079 7468 6f6e 2064 6174 6120 616e  n python data an
-000019e0: 616c 7973 6973 295d 2868 7474 7073 3a2f  alysis)](https:/
-000019f0: 2f77 7777 2e61 6e61 636f 6e64 612e 636f  /www.anaconda.co
-00001a00: 6d2f 6f70 656e 2d73 6f75 7263 6529 0a2a  m/open-source).*
-00001a10: 205b 5468 6520 5079 7468 6f6e 2054 7574   [The Python Tut
-00001a20: 6f72 6961 6c5d 2868 7474 7073 3a2f 2f64  orial](https://d
-00001a30: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-00001a40: 2f74 7574 6f72 6961 6c2f 290a 2a20 5b4a  /tutorial/).* [J
-00001a50: 7570 7974 6572 204e 6f74 6562 6f6f 6b20  upyter Notebook 
-00001a60: 696e 7472 6f64 7563 7469 6f6e 5d28 6874  introduction](ht
-00001a70: 7470 733a 2f2f 7265 616c 7079 7468 6f6e  tps://realpython
-00001a80: 2e63 6f6d 2f6a 7570 7974 6572 2d6e 6f74  .com/jupyter-not
-00001a90: 6562 6f6f 6b2d 696e 7472 6f64 7563 7469  ebook-introducti
-00001aa0: 6f6e 2f29 0a                             on/).
+00000c80: 2073 656e 7465 6e63 6573 2074 6162 6c65   sentences table
+00000c90: 0a20 2073 6574 7469 6e67 7320 2020 2020  .  settings     
+00000ca0: 2020 2020 2020 2020 4372 6561 7465 2061          Create a
+00000cb0: 6e64 2065 7870 6f72 7420 7365 7474 696e  nd export settin
+00000cc0: 6773 2074 6162 6c65 0a20 2073 7461 7274  gs table.  start
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 4c61 756e 6368 2067 7261 7068 6963 616c  Launch graphical
+00000cf0: 2075 7365 7220 696e 7465 7266 6163 650a   user interface.
+00000d00: 2020 7672 722d 7061 6972 7320 2020 2020    vrr-pairs     
+00000d10: 2020 2020 2020 2043 7265 6174 6520 766f         Create vo
+00000d20: 7469 6e67 2072 6967 6874 7320 7375 6d6d  ting rights summ
+00000d30: 6172 7920 6672 6f6d 2069 6e70 7574 2063  ary from input c
+00000d40: 6173 6573 2061 6e64 2070 6169 7273 0a20  ases and pairs. 
+00000d50: 2077 6974 6e65 7373 6573 2020 2020 2020   witnesses      
+00000d60: 2020 2020 2020 4372 6561 7465 2061 6e64        Create and
+00000d70: 2065 7870 6f72 7420 7769 746e 6573 7365   export witnesse
+00000d80: 7320 7461 626c 650a 6060 600a 0a23 2320  s table.```..## 
+00000d90: 4665 7463 6820 6361 7365 7320 696e 2062  Fetch cases in b
+00000da0: 756c 6b20 6672 6f6d 2041 6c61 636f 7572  ulk from Alacour
+00000db0: 742e 636f 6d20 0a0a 5461 6b65 2061 2073  t.com ..Take a s
+00000dc0: 7072 6561 6473 6865 6574 206f 6620 6e61  preadsheet of na
+00000dd0: 6d65 7320 616e 642f 6f72 206f 7468 6572  mes and/or other
+00000de0: 2073 6561 7263 6820 7061 7261 6d65 7465   search paramete
+00000df0: 7273 2061 6e64 2064 6f77 6e6c 6f61 6420  rs and download 
+00000e00: 6361 7365 2050 4446 7320 6672 6f6d 2041  case PDFs from A
+00000e10: 6c61 636f 7572 7420 696e 2062 756c 6b2e  lacourt in bulk.
+00000e20: 2044 6f77 6e6c 6f61 6420 7468 6f75 7361   Download thousa
+00000e30: 6e64 7320 6f66 2050 4446 7320 696e 206a  nds of PDFs in j
+00000e40: 7573 7420 686f 7572 7320 6279 206c 6561  ust hours by lea
+00000e50: 7669 6e67 2079 6f75 7220 636f 6d70 7574  ving your comput
+00000e60: 6572 2075 6e61 7474 656e 6465 642e 2028  er unattended. (
+00000e70: 476f 6f67 6c65 2043 6872 6f6d 6520 6973  Google Chrome is
+00000e80: 2072 6571 7569 7265 6420 746f 2075 7365   required to use
+00000e90: 2074 6865 2060 6665 7463 6860 2066 6561   the `fetch` fea
+00000ea0: 7475 7265 2e29 0a0a 6060 600a 5573 6167  ture.)..```.Usag
+00000eb0: 653a 2070 7974 686f 6e20 2d6d 2061 6c61  e: python -m ala
+00000ec0: 636f 7264 6572 2066 6574 6368 205b 4f50  corder fetch [OP
+00000ed0: 5449 4f4e 535d 0a0a 2020 4665 7463 6820  TIONS]..  Fetch 
+00000ee0: 6361 7365 7320 6672 6f6d 2041 6c61 636f  cases from Alaco
+00000ef0: 7572 742e 636f 6d0a 0a4f 7074 696f 6e73  urt.com..Options
+00000f00: 3a0a 2020 2d69 6e2c 202d 2d69 6e70 7574  :.  -in, --input
+00000f10: 2d70 6174 6820 5041 5448 2020 2020 2020  -path PATH      
+00000f20: 5061 7468 2074 6f20 7175 6572 7920 7461  Path to query ta
+00000f30: 626c 652f 7370 7265 6164 7368 6565 7420  ble/spreadsheet 
+00000f40: 282e 786c 732c 202e 786c 7378 290a 2020  (.xls, .xlsx).  
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 2020 2020 2020 2020 2020 2020 5b72 6571              [req
+00000f70: 7569 7265 645d 0a20 202d 6f75 742c 202d  uired].  -out, -
+00000f80: 2d6f 7574 7075 742d 7061 7468 2050 4154  -output-path PAT
+00000f90: 4820 2020 2044 6573 6972 6564 2050 4446  H    Desired PDF
+00000fa0: 206f 7574 7075 7420 6469 7265 6374 6f72   output director
+00000fb0: 7920 205b 7265 7175 6972 6564 5d0a 2020  y  [required].  
+00000fc0: 2d63 7269 6d69 6e61 6c2c 202d 2d63 7269  -criminal, --cri
+00000fd0: 6d69 6e61 6c2d 6f6e 6c79 2020 4f6e 6c79  minal-only  Only
+00000fe0: 2073 6561 7263 6820 6372 696d 696e 616c   search criminal
+00000ff0: 2063 6173 6573 0a20 202d 632c 202d 2d63   cases.  -c, --c
+00001000: 7573 746f 6d65 722d 6964 2054 4558 5420  ustomer-id TEXT 
+00001010: 2020 2020 2043 7573 746f 6d65 7220 4944       Customer ID
+00001020: 206f 6e20 416c 6163 6f75 7274 2e63 6f6d   on Alacourt.com
+00001030: 2020 5b72 6571 7569 7265 645d 0a20 202d    [required].  -
+00001040: 752c 202d 2d75 7365 722d 6964 2054 4558  u, --user-id TEX
+00001050: 5420 2020 2020 2020 2020 2055 7365 7220  T          User 
+00001060: 4944 206f 6e20 416c 6163 6f75 7274 2e63  ID on Alacourt.c
+00001070: 6f6d 2020 5b72 6571 7569 7265 645d 0a20  om  [required]. 
+00001080: 202d 702c 202d 2d70 6173 7377 6f72 6420   -p, --password 
+00001090: 5445 5854 2020 2020 2020 2020 2050 6173  TEXT         Pas
+000010a0: 7377 6f72 6420 6f6e 2041 6c61 636f 7572  sword on Alacour
+000010b0: 742e 636f 6d20 205b 7265 7175 6972 6564  t.com  [required
+000010c0: 5d0a 2020 2d6d 6178 2c20 2d2d 6d61 7820  ].  -max, --max 
+000010d0: 494e 5445 4745 5220 2020 2020 2020 2020  INTEGER         
+000010e0: 4d61 7869 6d75 6d20 7175 6572 6965 7320  Maximum queries 
+000010f0: 746f 2063 6f6e 6475 6374 206f 6e20 416c  to conduct on Al
+00001100: 6163 6f75 7274 2e63 6f6d 0a20 202d 736b  acourt.com.  -sk
+00001110: 6970 2c20 2d2d 736b 6970 2049 4e54 4547  ip, --skip INTEG
+00001120: 4552 2020 2020 2020 2053 6b69 7020 656e  ER       Skip en
+00001130: 7472 6965 7320 6174 2074 6f70 206f 6620  tries at top of 
+00001140: 7175 6572 7920 6669 6c65 0a20 202d 6e2c  query file.  -n,
+00001150: 202d 2d6e 6f2d 6d61 726b 2020 2020 2020   --no-mark      
+00001160: 2020 2020 2020 2020 2044 6f20 6e6f 7420           Do not 
+00001170: 7570 6461 7465 2071 7565 7279 2074 656d  update query tem
+00001180: 706c 6174 6520 6166 7465 7220 636f 6d70  plate after comp
+00001190: 6c65 7469 6f6e 0a20 202d 2d64 6562 7567  letion.  --debug
+000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011b0: 2020 2020 2050 7269 6e74 2064 6574 6169       Print detai
+000011c0: 6c65 6420 7275 6e74 696d 6520 696e 666f  led runtime info
+000011d0: 726d 6174 696f 6e20 746f 2063 6f6e 736f  rmation to conso
+000011e0: 6c65 0a20 202d 682c 202d 2d68 656c 7020  le.  -h, --help 
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2053 686f 7720 7468 6973 206d 6573 7361   Show this messa
+00001210: 6765 2061 6e64 2065 7869 742e 0a60 6060  ge and exit..```
+00001220: 0a0a 0a23 202a 2a57 6f72 6b69 6e67 2077  ...# **Working w
+00001230: 6974 6820 6361 7365 2064 6174 6120 696e  ith case data in
+00001240: 2050 7974 686f 6e2a 2a0a 0a0a 2323 2320   Python**...### 
+00001250: 4f75 7420 6f66 2074 6865 2062 6f78 2c20  Out of the box, 
+00001260: 416c 6163 6f72 6465 7220 6578 706f 7274  Alacorder export
+00001270: 7320 746f 2060 2e78 6c73 7860 2c20 602e  s to `.xlsx`, `.
+00001280: 786c 7360 2c20 602e 6373 7660 2c20 602e  xls`, `.csv`, `.
+00001290: 6a73 6f6e 602c 2061 6e64 2060 2e70 6172  json`, and `.par
+000012a0: 7175 6574 602e 2042 7574 2079 6f75 2063  quet`. But you c
+000012b0: 616e 2075 7365 2060 706f 6c61 7273 6020  an use `polars` 
+000012c0: 616e 6420 6f74 6865 7220 7079 7468 6f6e  and other python
+000012d0: 206c 6962 7261 7269 6573 2074 6f20 6372   libraries to cr
+000012e0: 6561 7465 2079 6f75 7220 6f77 6e20 6461  eate your own da
+000012f0: 7461 2063 6f6c 6c65 6374 696f 6e20 776f  ta collection wo
+00001300: 726b 666c 6f77 7320 616e 6420 6375 7374  rkflows and cust
+00001310: 6f6d 697a 6520 416c 6163 6f72 6465 7220  omize Alacorder 
+00001320: 6578 706f 7274 732e 200a 0a2a 2a2a 5468  exports. ..***Th
+00001330: 6520 736e 6970 7065 7420 6265 6c6f 7720  e snippet below 
+00001340: 7072 696e 7473 2074 6865 2066 6565 2073  prints the fee s
+00001350: 6865 6574 7320 6672 6f6d 2061 2064 6972  heets from a dir
+00001360: 6563 746f 7279 206f 6620 6361 7365 2050  ectory of case P
+00001370: 4446 7320 6173 2069 7420 7265 6164 7320  DFs as it reads 
+00001380: 7468 656d 2e2a 2a2a 0a0a 0a60 6060 7079  them.***...```py
+00001390: 7468 6f6e 0a66 726f 6d20 616c 6163 6f72  thon.from alacor
+000013a0: 6465 7220 696d 706f 7274 2061 6c61 630a  der import alac.
+000013b0: 696d 706f 7274 2070 6f6c 6172 7320 6173  import polars as
+000013c0: 2070 6c0a 0a71 7565 7565 203d 2061 6c61   pl..queue = ala
+000013d0: 632e 6765 745f 7061 7468 7328 222f 5573  c.get_paths("/Us
+000013e0: 6572 732f 6372 696d 736f 6e2f 4465 736b  ers/crimson/Desk
+000013f0: 746f 702f 5475 7477 696c 6572 2f22 2920  top/Tutwiler/") 
+00001400: 2320 2d3e 205b 7374 725d 0a0a 726f 7773  # -> [str]..rows
+00001410: 203d 205b 5d0a 0a66 6f72 2069 2c20 7061   = []..for i, pa
+00001420: 7468 2069 6e20 656e 756d 6572 6174 6528  th in enumerate(
+00001430: 7175 6575 6529 3a0a 2020 2020 7465 7874  queue):.    text
+00001440: 203d 2061 6c61 632e 6578 7472 6163 745f   = alac.extract_
+00001450: 7465 7874 2870 6174 6829 0a20 2020 2063  text(path).    c
+00001460: 6e75 6d20 3d20 616c 6163 2e67 6574 4361  num = alac.getCa
+00001470: 7365 4e75 6d62 6572 2874 6578 7429 0a20  seNumber(text). 
+00001480: 2020 2063 7479 203d 2061 6c61 632e 6765     cty = alac.ge
+00001490: 7443 6f75 6e74 7928 7465 7874 290a 2020  tCounty(text).  
+000014a0: 2020 7462 616c 203d 2061 6c61 632e 6765    tbal = alac.ge
+000014b0: 7454 6f74 616c 4261 6c61 6e63 6528 7465  tTotalBalance(te
+000014c0: 7874 290a 2020 2020 7074 7220 3d20 616c  xt).    ptr = al
+000014d0: 6163 2e67 6574 5061 796d 656e 7454 6f52  ac.getPaymentToR
+000014e0: 6573 746f 7265 2874 6578 7429 2023 2069  estore(text) # i
+000014f0: 2e65 2e20 766f 7469 6e67 2072 6967 6874  .e. voting right
+00001500: 730a 2020 2020 726f 7773 202b 3d20 5b5b  s.    rows += [[
+00001510: 636e 756d 2c20 6374 792c 2074 6261 6c2c  cnum, cty, tbal,
+00001520: 2070 7472 5d5d 0a0a 6361 7365 7320 3d20   ptr]]..cases = 
+00001530: 706c 2e44 6174 6146 7261 6d65 2872 6f77  pl.DataFrame(row
+00001540: 7329 0a0a 6361 7365 732e 7772 6974 655f  s)..cases.write_
+00001550: 6578 6365 6c28 222f 5573 6572 732f 6372  excel("/Users/cr
+00001560: 696d 736f 6e2f 4465 736b 746f 702f 5475  imson/Desktop/Tu
+00001570: 7477 696c 6572 2f73 756d 6d61 7279 2e78  twiler/summary.x
+00001580: 6c73 7822 290a 0a60 6060 0a0a 2323 2045  lsx")..```..## E
+00001590: 7874 656e 6469 6e67 2041 6c61 636f 7264  xtending Alacord
+000015a0: 6572 2077 6974 6820 6070 6f6c 6172 7360  er with `polars`
+000015b0: 2061 6e64 206f 7468 6572 2074 6f6f 6c73   and other tools
+000015c0: 0a0a 416c 6163 6f72 6465 7220 7275 6e73  ..Alacorder runs
+000015d0: 206f 6e20 5b60 706f 6c61 7273 605d 2868   on [`polars`](h
+000015e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000015f0: 6d2f 706f 6c61 2d72 732f 706f 6c61 7273  m/pola-rs/polars
+00001600: 292c 2061 2070 7974 686f 6e20 6c69 6272  ), a python libr
+00001610: 6172 7920 796f 7520 6361 6e20 7573 6520  ary you can use 
+00001620: 746f 2077 6f72 6b20 7769 7468 2061 6e64  to work with and
+00001630: 2061 6e61 6c79 7a65 2074 6162 756c 6172   analyze tabular
+00001640: 2064 6174 612e 2060 706f 6c61 7273 6020   data. `polars` 
+00001650: 6361 6e20 7265 6164 2066 726f 6d20 616e  can read from an
+00001660: 6420 7772 6974 6520 746f 2061 6c6c 206d  d write to all m
+00001670: 616a 6f72 2064 6174 6120 7374 6f72 6167  ajor data storag
+00001680: 6520 666f 726d 6174 732e 2049 7420 6361  e formats. It ca
+00001690: 6e20 636f 6e6e 6563 7420 746f 2061 2077  n connect to a w
+000016a0: 6964 6520 7661 7269 6574 7920 6f66 2073  ide variety of s
+000016b0: 6572 7669 6365 7320 746f 2070 726f 7669  ervices to provi
+000016c0: 6465 2066 6f72 2065 6173 7920 696d 706f  de for easy impo
+000016d0: 7274 2061 6e64 2065 7870 6f72 742e 0a0a  rt and export...
+000016e0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+000016f0: 2070 6f6c 6172 7320 6173 2070 6c0a 636f   polars as pl.co
+00001700: 6e74 656e 7473 203d 2070 6c2e 7265 6164  ntents = pl.read
+00001710: 5f6a 736f 6e28 222f 7061 7468 2f74 6f2f  _json("/path/to/
+00001720: 6172 6368 6976 652e 6a73 6f6e 2229 0a60  archive.json").`
+00001730: 6060 0a0a 4966 2079 6f75 2077 6f75 6c64  ``..If you would
+00001740: 206c 696b 6520 746f 2076 6973 7561 6c69   like to visuali
+00001750: 7a65 2064 6174 6120 7769 7468 6f75 7420  ze data without 
+00001760: 6578 706f 7274 696e 6720 746f 2045 7863  exporting to Exc
+00001770: 656c 206f 7220 616e 6f74 6865 7220 666f  el or another fo
+00001780: 726d 6174 2c20 6372 6561 7465 2061 2060  rmat, create a `
+00001790: 6a75 7079 7465 7220 6e6f 7465 626f 6f6b  jupyter notebook
+000017a0: 6020 616e 6420 696e 7374 616c 6c20 746f  ` and install to
+000017b0: 6f6c 7320 6c69 6b65 2060 6d61 7470 6c6f  ols like `matplo
+000017c0: 746c 6962 602c 2060 7461 6275 6c61 7465  tlib`, `tabulate
+000017d0: 602c 2061 6e64 2060 6974 6162 6c65 7360  `, and `itables`
+000017e0: 2074 6f20 6765 7420 7374 6172 7465 642e   to get started.
+000017f0: 205b 4a75 7079 7465 7220 4e6f 7465 626f   [Jupyter Notebo
+00001800: 6f6b 5d28 6874 7470 733a 2f2f 646f 6373  ok](https://docs
+00001810: 2e6a 7570 7974 6572 2e6f 7267 2f65 6e2f  .jupyter.org/en/
+00001820: 6c61 7465 7374 2f73 7461 7274 2f69 6e64  latest/start/ind
+00001830: 6578 2e68 746d 6c29 2069 7320 6120 5079  ex.html) is a Py
+00001840: 7468 6f6e 2070 726f 6a65 6374 2079 6f75  thon project you
+00001850: 2063 616e 2075 7365 2074 6f20 6372 6561   can use to crea
+00001860: 7465 2069 6e74 6572 6163 7469 7665 206e  te interactive n
+00001870: 6f74 6562 6f6f 6b73 2066 6f72 2064 6174  otebooks for dat
+00001880: 6120 616e 616c 7973 6973 2061 6e64 206f  a analysis and o
+00001890: 7468 6572 2070 7572 706f 7365 732e 2049  ther purposes. I
+000018a0: 7420 6361 6e20 6265 2069 6e73 7461 6c6c  t can be install
+000018b0: 6564 2075 7369 6e67 2060 7069 7020 696e  ed using `pip in
+000018c0: 7374 616c 6c20 6a75 7079 7465 7260 206f  stall jupyter` o
+000018d0: 7220 6070 6970 3320 696e 7374 616c 6c20  r `pip3 install 
+000018e0: 6a75 7079 7465 7260 2061 6e64 206c 6175  jupyter` and lau
+000018f0: 6e63 6865 6420 7573 696e 6720 606a 7570  nched using `jup
+00001900: 7974 6572 206e 6f74 6562 6f6f 6b60 2e20  yter notebook`. 
+00001910: 596f 7572 2064 6576 6963 6520 6d61 7920  Your device may 
+00001920: 616c 7265 6164 7920 6265 2065 7175 6970  already be equip
+00001930: 7065 6420 746f 2076 6965 7720 602e 6970  ped to view `.ip
+00001940: 796e 6260 206e 6f74 6562 6f6f 6b73 2e20  ynb` notebooks. 
+00001950: 0a0a 2323 202a 2a52 6573 6f75 7263 6573  ..## **Resources
+00001960: 2a2a 0a2a 205b 6070 6f6c 6172 7360 2075  **.* [`polars` u
+00001970: 7365 7220 6775 6964 655d 2868 7474 7073  ser guide](https
+00001980: 3a2f 2f70 6f6c 612d 7273 2e67 6974 6875  ://pola-rs.githu
+00001990: 622e 696f 2f70 6f6c 6172 732d 626f 6f6b  b.io/polars-book
+000019a0: 2f75 7365 722d 6775 6964 652f 696e 6465  /user-guide/inde
+000019b0: 782e 6874 6d6c 290a 2a20 5b72 6567 6578  x.html).* [regex
+000019c0: 2063 6865 6174 2073 6865 6574 5d28 6874   cheat sheet](ht
+000019d0: 7470 733a 2f2f 7777 772e 7265 7865 6767  tps://www.rexegg
+000019e0: 2e63 6f6d 2f72 6567 6578 2d71 7569 636b  .com/regex-quick
+000019f0: 7374 6172 742e 6874 6d6c 290a 2a20 5b41  start.html).* [A
+00001a00: 6e61 636f 6e64 6120 2874 7574 6f72 6961  naconda (tutoria
+00001a10: 6c73 206f 6e20 7079 7468 6f6e 2064 6174  ls on python dat
+00001a20: 6120 616e 616c 7973 6973 295d 2868 7474  a analysis)](htt
+00001a30: 7073 3a2f 2f77 7777 2e61 6e61 636f 6e64  ps://www.anacond
+00001a40: 612e 636f 6d2f 6f70 656e 2d73 6f75 7263  a.com/open-sourc
+00001a50: 6529 0a2a 205b 5468 6520 5079 7468 6f6e  e).* [The Python
+00001a60: 2054 7574 6f72 6961 6c5d 2868 7474 7073   Tutorial](https
+00001a70: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00001a80: 7267 2f33 2f74 7574 6f72 6961 6c2f 290a  rg/3/tutorial/).
+00001a90: 2a20 5b4a 7570 7974 6572 204e 6f74 6562  * [Jupyter Noteb
+00001aa0: 6f6f 6b20 696e 7472 6f64 7563 7469 6f6e  ook introduction
+00001ab0: 5d28 6874 7470 733a 2f2f 7265 616c 7079  ](https://realpy
+00001ac0: 7468 6f6e 2e63 6f6d 2f6a 7570 7974 6572  thon.com/jupyter
+00001ad0: 2d6e 6f74 6562 6f6f 6b2d 696e 7472 6f64  -notebook-introd
+00001ae0: 7563 7469 6f6e 2f29 0a                   uction/).
```

### Comparing `alacorder-80.0.8/pyproject.toml` & `alacorder-80.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.0.8"
+version = "80.0.9"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.0.8/src/alacorder/.DS_Store` & `alacorder-80.0.9/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.8/src/alacorder/__init__.py` & `alacorder-80.0.9/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.8/src/alacorder/__main__.py` & `alacorder-80.0.9/src/alacorder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.8"
+version = "80.0.9"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -4465,105 +4465,14 @@
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
         debug=debug,
     )
 
 
-@main.command(name="table", help="Export data tables from archive or directory")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option("--table", "-t", help="Table export selection")
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def cli_table(
-    input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
-):
-    """
-    Write data tables to output path from archive or directory input.
-
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        table (str): Table (all, cases, fees, charges, settings, witnesses, attorneys, case_action_summaries, images)
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] in (".xls", ".xlsx") and not bool(table):
-        table = "all"
-    elif os.path.splitext(output_path)[1] not in (".xls", ".xlsx") and not bool(table):
-        table = click.prompt(
-            "Table export choice (cases, fees, charges, disposition, filing, attorneys, witnesses, images, case-action-summary, settings)"
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table=table,
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
```

### Comparing `alacorder-80.0.8/src/alacorder/alac.py` & `alacorder-80.0.9/src/alacorder/alac.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.8"
+version = "80.0.9"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -4465,105 +4465,14 @@
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
         debug=debug,
     )
 
 
-@main.command(name="table", help="Export data tables from archive or directory")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option("--table", "-t", help="Table export selection")
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def cli_table(
-    input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
-):
-    """
-    Write data tables to output path from archive or directory input.
-
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        table (str): Table (all, cases, fees, charges, settings, witnesses, attorneys, case_action_summaries, images)
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] in (".xls", ".xlsx") and not bool(table):
-        table = "all"
-    elif os.path.splitext(output_path)[1] not in (".xls", ".xlsx") and not bool(table):
-        table = click.prompt(
-            "Table export choice (cases, fees, charges, disposition, filing, attorneys, witnesses, images, case-action-summary, settings)"
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table=table,
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
```

### Comparing `alacorder-80.0.8/PKG-INFO` & `alacorder-80.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.0.8
+Version: 80.0.9
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -75,42 +75,43 @@
   fees                 Create and export fees table
   fetch                Fetch cases from Alacourt.com
   financial-history    Create and export financial history table
   images               Create and export images table
   multi                Export all data tables to .xls/.xlsx
   pair                 Create blank AIS / unique pairing template
   rename               Rename cases in input directory to case numbers
+  sentences            Create and export sentences table
   settings             Create and export settings table
   start                Launch graphical user interface
-  table                Export data tables from archive or directory
   vrr-pairs            Create voting rights summary from input cases and pairs
   witnesses            Create and export witnesses table
 ```
 
 ## Fetch cases in bulk from Alacourt.com 
 
 Take a spreadsheet of names and/or other search parameters and download case PDFs from Alacourt in bulk. Download thousands of PDFs in just hours by leaving your computer unattended. (Google Chrome is required to use the `fetch` feature.)
 
 ```
 Usage: python -m alacorder fetch [OPTIONS]
 
   Fetch cases from Alacourt.com
 
 Options:
-  -in, --input-path PATH    Path to query table/spreadsheet (.xls, .xlsx)
-                            [required]
-  -out, --output-path PATH  Desired PDF output directory  [required]
-  -c, --customer-id TEXT    Customer ID on Alacourt.com  [required]
-  -u, --user-id TEXT        User ID on Alacourt.com  [required]
-  -p, --password TEXT       Password on Alacourt.com  [required]
-  -max, --max INTEGER       Maximum queries to conduct on Alacourt.com
-  -skip, --skip INTEGER     Skip entries at top of query file
-  -n, --no-mark             Do not update query template after completion
-  --debug                   Print detailed runtime information to console
-  -h, --help                Show this message and exit.
+  -in, --input-path PATH      Path to query table/spreadsheet (.xls, .xlsx)
+                              [required]
+  -out, --output-path PATH    Desired PDF output directory  [required]
+  -criminal, --criminal-only  Only search criminal cases
+  -c, --customer-id TEXT      Customer ID on Alacourt.com  [required]
+  -u, --user-id TEXT          User ID on Alacourt.com  [required]
+  -p, --password TEXT         Password on Alacourt.com  [required]
+  -max, --max INTEGER         Maximum queries to conduct on Alacourt.com
+  -skip, --skip INTEGER       Skip entries at top of query file
+  -n, --no-mark               Do not update query template after completion
+  --debug                     Print detailed runtime information to console
+  -h, --help                  Show this message and exit.
 ```
 
 
 # **Working with case data in Python**
 
 
 ### Out of the box, Alacorder exports to `.xlsx`, `.xls`, `.csv`, `.json`, and `.parquet`. But you can use `polars` and other python libraries to create your own data collection workflows and customize Alacorder exports.
```

